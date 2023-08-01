# Comparing `tmp/hpl_rv_ros-1.0.0-py3-none-any.whl.zip` & `tmp/hpl_rv_ros-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 11301 bytes, number of entries: 14
+Zip file size: 11458 bytes, number of entries: 14
 -rw-rw-rw-  2.0 fat      662 b- defN 23-Jul-19 08:36 hplrv_ros/__init__.py
 -rw-rw-rw-  2.0 fat      865 b- defN 23-Jul-19 08:36 hplrv_ros/__main__.py
 -rw-rw-rw-  2.0 fat     5047 b- defN 23-Aug-01 09:28 hplrv_ros/cli.py
 -rw-rw-rw-  2.0 fat     1699 b- defN 23-Aug-01 09:29 hplrv_ros/common.py
 -rw-rw-rw-  2.0 fat     1550 b- defN 23-Aug-01 09:27 hplrv_ros/rclpy.py
 -rw-rw-rw-  2.0 fat     1550 b- defN 23-Aug-01 09:26 hplrv_ros/rospy.py
--rw-rw-rw-  2.0 fat     3062 b- defN 23-Aug-01 09:45 hplrv_ros/templates/rclpy.py.jinja
--rw-rw-rw-  2.0 fat     2457 b- defN 23-Aug-01 08:24 hplrv_ros/templates/rospy.py.jinja
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Aug-01 10:17 hpl_rv_ros-1.0.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     5970 b- defN 23-Aug-01 10:17 hpl_rv_ros-1.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-01 10:17 hpl_rv_ros-1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       50 b- defN 23-Aug-01 10:17 hpl_rv_ros-1.0.0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       10 b- defN 23-Aug-01 10:17 hpl_rv_ros-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1134 b- defN 23-Aug-01 10:17 hpl_rv_ros-1.0.0.dist-info/RECORD
-14 files, 25239 bytes uncompressed, 9419 bytes compressed:  62.7%
+-rw-rw-rw-  2.0 fat     3357 b- defN 23-Aug-01 13:38 hplrv_ros/templates/rclpy.py.jinja
+-rw-rw-rw-  2.0 fat     2645 b- defN 23-Aug-01 13:37 hplrv_ros/templates/rospy.py.jinja
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Aug-01 13:43 hpl_rv_ros-1.0.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     5970 b- defN 23-Aug-01 13:43 hpl_rv_ros-1.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-01 13:43 hpl_rv_ros-1.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       50 b- defN 23-Aug-01 13:43 hpl_rv_ros-1.0.1.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Aug-01 13:43 hpl_rv_ros-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1134 b- defN 23-Aug-01 13:43 hpl_rv_ros-1.0.1.dist-info/RECORD
+14 files, 25722 bytes uncompressed, 9576 bytes compressed:  62.8%
```

## zipnote {}

```diff
@@ -18,26 +18,26 @@
 
 Filename: hplrv_ros/templates/rclpy.py.jinja
 Comment: 
 
 Filename: hplrv_ros/templates/rospy.py.jinja
 Comment: 
 
-Filename: hpl_rv_ros-1.0.0.dist-info/LICENSE
+Filename: hpl_rv_ros-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: hpl_rv_ros-1.0.0.dist-info/METADATA
+Filename: hpl_rv_ros-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: hpl_rv_ros-1.0.0.dist-info/WHEEL
+Filename: hpl_rv_ros-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: hpl_rv_ros-1.0.0.dist-info/entry_points.txt
+Filename: hpl_rv_ros-1.0.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: hpl_rv_ros-1.0.0.dist-info/top_level.txt
+Filename: hpl_rv_ros-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: hpl_rv_ros-1.0.0.dist-info/RECORD
+Filename: hpl_rv_ros-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hplrv_ros/templates/rclpy.py.jinja

```diff
@@ -22,14 +22,17 @@
 {% endfor %}
 
 
 class HplMonitorNode(Node):
     def __init__(self):
         super().__init__('hplrv_monitor')
         self.monitor = HplMonitorManager(success_cb=self._on_success, failure_cb=self._on_failure)
+        self.monitor.live_server.host = '127.0.0.1'
+        self.monitor.live_server.port = 4242
+        self._thread = None
         self.timer = self.create_timer(0.01, self.on_timer)
         latching_qos = QoSProfile(
             depth=1,
             durability=DurabilityPolicy.TRANSIENT_LOCAL,
             history=HistoryPolicy.KEEP_LAST,
         )
         self.pubs = {}
@@ -47,20 +50,24 @@
                 self.on_msg_{{ topic|replace('/', '_') }},
                 10,
             ),
         {% endfor %}
         ]
 
     def on_launch(self):
+        self._thread = self.monitor.live_server.start_thread()
         t = self.get_clock().now()
         self.monitor.launch(t)
 
     def on_shutdown(self):
         t = self.get_clock().now()
         self.monitor.shutdown(t)
+        assert self._thread is not None
+        self._thread.join(10.0)
+        self._thread = None
 
     def on_timer(self):
         t = self.get_clock().now()
         self.monitor.on_timer(t)
     {# -#}
 {% for topic in topics %}
```

## hplrv_ros/templates/rospy.py.jinja

```diff
@@ -17,14 +17,16 @@
 import {{ rospkg }}.msg as {{ rospkg }}
 {% endfor %}
 
 
 class HplMonitorNode:
     def __init__(self):
         self.monitor = HplMonitorManager(success_cb=self._on_success, failure_cb=self._on_failure)
+        self.monitor.live_server.host = '127.0.0.1'
+        self.monitor.live_server.port = 4242
         self.pubs = {}
         for i in range(len(self.monitor.monitors)):
             mon = self.monitor.monitors[i]
             cls = type(mon).__name__
             assert cls not in self.pubs
             self.pubs[cls] = rospy.Publisher(f'~p{i}/verdict',
                 std_msgs.Bool, queue_size=1, latch=True)
@@ -33,25 +35,27 @@
         {% for topic, typename in topics.items() %}
             rospy.Subscriber('{{ topic }}', {{ typename|replace('/', '.') }},
                 self.on_msg_{{ topic|replace('/', '_') }}),
         {% endfor %}
         ]
 
     def run(self):
+        thread = self.monitor.live_server.start_thread()
         t = rospy.get_time()
         self.monitor.launch(t)
         rate = rospy.Rate(100) # 100hz
         try:
             while not rospy.is_shutdown():
                 t = rospy.get_time()
                 self.monitor.on_timer(t)
                 rate.sleep()
         except rospy.ROSInterruptException:
             t = rospy.get_time()
             self.monitor.shutdown(t)
+            thread.join(10.0)
     {# -#}
 {% for topic in topics %}
 
     {% set cbname = 'on_msg_' ~ topic.replace('/', '_') %}
     def {{ cbname }}(self, msg):
         t = rospy.get_time()
         self.monitor.{{ cbname }}(msg, t)
```

## Comparing `hpl_rv_ros-1.0.0.dist-info/LICENSE` & `hpl_rv_ros-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `hpl_rv_ros-1.0.0.dist-info/METADATA` & `hpl_rv_ros-1.0.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpl-rv-ros
-Version: 1.0.0
+Version: 1.0.1
 Summary: Runtime Verification tools for ROS systems
 Home-page: https://github.com/HAROS-framework/hpl-rv-ros
 Author: André Santos
 Author-email: haros.framework@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/HAROS-framework/hpl-rv-ros/
 Project-URL: Tracker, https://github.com/HAROS-framework/hpl-rv-ros/issues
```

## Comparing `hpl_rv_ros-1.0.0.dist-info/RECORD` & `hpl_rv_ros-1.0.1.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 hplrv_ros/__init__.py,sha256=0QvjTC35kEG_eai19GzApYwpOpTUbzKPugnFBXB2JTw,662
 hplrv_ros/__main__.py,sha256=Vi58xVcaVJjKCirJrpSgjpddTQ4Vlk07Dv_ktGaqW1Q,865
 hplrv_ros/cli.py,sha256=qlvkejQ2gtTx3vW28ktJCpfj7a_uKD6bT3QBaa-GZp0,5047
 hplrv_ros/common.py,sha256=toj4Sq-r_WuBTKuzBTw_41-TRFcD5NbpSEnwAbwIhr8,1699
 hplrv_ros/rclpy.py,sha256=s-neWg0sMf1ZvmVbLfCKOHYUaPyu6bOi4jUfAgrIGdQ,1550
 hplrv_ros/rospy.py,sha256=xq0cYuJGexiLZYrLlZGxt24Zemp5x301hYAq2r6gfUI,1550
-hplrv_ros/templates/rclpy.py.jinja,sha256=sEEexJTu-ZlzBWNP3cO5h9xe2_9NULVRTOOyuKCNRbo,3062
-hplrv_ros/templates/rospy.py.jinja,sha256=1rZxqX2Igb1ElMXtdIYbl9TvVyb0Qg_uozbhbtu2u40,2457
-hpl_rv_ros-1.0.0.dist-info/LICENSE,sha256=SmN5t61DpK1f9yysci-wag1YZg9pl9_xTege637Cxeg,1091
-hpl_rv_ros-1.0.0.dist-info/METADATA,sha256=9Jd0RSbVoDqnVxbG_CNhgOPRiIvuNZjxGTft5vz670I,5970
-hpl_rv_ros-1.0.0.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-hpl_rv_ros-1.0.0.dist-info/entry_points.txt,sha256=Ihz_I9WUrzitBvSB-GzXrBRFMM7IXaGZG-eHoJLS6UY,50
-hpl_rv_ros-1.0.0.dist-info/top_level.txt,sha256=Ff-Am09wUkQGcfg3VCE8Anb_LMRkpD_EW5qM3MAF7Ec,10
-hpl_rv_ros-1.0.0.dist-info/RECORD,,
+hplrv_ros/templates/rclpy.py.jinja,sha256=QPn4331nzA1iih5-Kn2-UCzP38TnfiNfo9zk81nAZjw,3357
+hplrv_ros/templates/rospy.py.jinja,sha256=rUlth-6Z1mlCWiIS8KG-d4tKzKx7A5jXs8kMkNEr1-M,2645
+hpl_rv_ros-1.0.1.dist-info/LICENSE,sha256=SmN5t61DpK1f9yysci-wag1YZg9pl9_xTege637Cxeg,1091
+hpl_rv_ros-1.0.1.dist-info/METADATA,sha256=y5kXrXrKnz5q-oVh0dDe2ZEmoXvfRne8iSjRPWgfmeA,5970
+hpl_rv_ros-1.0.1.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+hpl_rv_ros-1.0.1.dist-info/entry_points.txt,sha256=Ihz_I9WUrzitBvSB-GzXrBRFMM7IXaGZG-eHoJLS6UY,50
+hpl_rv_ros-1.0.1.dist-info/top_level.txt,sha256=Ff-Am09wUkQGcfg3VCE8Anb_LMRkpD_EW5qM3MAF7Ec,10
+hpl_rv_ros-1.0.1.dist-info/RECORD,,
```

