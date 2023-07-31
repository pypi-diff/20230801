# Comparing `tmp/py4AxisStage-0.0.2-py3-none-any.whl.zip` & `tmp/py4AxisStage-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2371 bytes, number of entries: 6
+Zip file size: 2389 bytes, number of entries: 6
 -rw-rw-rw-  2.0 fat       39 b- defN 23-Jul-24 02:03 py4AxisStage/__init__.py
--rw-rw-rw-  2.0 fat     2015 b- defN 23-Jul-24 02:37 py4AxisStage/py4AxisStage.py
--rw-rw-rw-  2.0 fat      191 b- defN 23-Jul-24 02:39 py4AxisStage-0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-24 02:39 py4AxisStage-0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 23-Jul-24 02:39 py4AxisStage-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      481 b- defN 23-Jul-24 02:39 py4AxisStage-0.0.2.dist-info/RECORD
-6 files, 2831 bytes uncompressed, 1493 bytes compressed:  47.3%
+-rw-rw-rw-  2.0 fat     2070 b- defN 23-Jul-31 22:34 py4AxisStage/py4AxisStage.py
+-rw-rw-rw-  2.0 fat      191 b- defN 23-Jul-31 22:35 py4AxisStage-0.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-31 22:35 py4AxisStage-0.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 23-Jul-31 22:35 py4AxisStage-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      481 b- defN 23-Jul-31 22:35 py4AxisStage-0.0.3.dist-info/RECORD
+6 files, 2886 bytes uncompressed, 1511 bytes compressed:  47.6%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: py4AxisStage/__init__.py
 Comment: 
 
 Filename: py4AxisStage/py4AxisStage.py
 Comment: 
 
-Filename: py4AxisStage-0.0.2.dist-info/METADATA
+Filename: py4AxisStage-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: py4AxisStage-0.0.2.dist-info/WHEEL
+Filename: py4AxisStage-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: py4AxisStage-0.0.2.dist-info/top_level.txt
+Filename: py4AxisStage-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: py4AxisStage-0.0.2.dist-info/RECORD
+Filename: py4AxisStage-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## py4AxisStage/py4AxisStage.py

```diff
@@ -1,8 +1,8 @@
-# v0.0.2
+# v0.0.3
 
 from socket import socket, AF_INET, SOCK_DGRAM
 from threading import Thread
 import json
 import subprocess
 
 class py4AxisStage:
@@ -32,16 +32,18 @@
             exit()
         self._th_monitor_pos = Thread(target=self._get_position, daemon=True)
         self._th_monitor_pos.start()
         self.position = {}
         while len(self.position) == 0:
             pass
     def _get_position(self):
-        msg_recv, _ = self._s_recv.recvfrom(2048)
-        self.position = json.loads(msg_recv.decode().replace('\x00', ''))
+        while True:
+            msg_recv, _ = self._s_recv.recvfrom(2048)
+            self.position = json.loads(msg_recv.decode().replace('\x00', ''))
+            del msg_recv
     def send_command(self, axis, speed, distance, coord):  # logファイルと同じ形式でデータ送信（No.は不要）：[軸，速度，移動量]
         msg = '{ax},{co},{sp},{dist}'.format(ax=axis, sp=speed, dist=distance, co=coord)
         self._s_send.sendto(msg.encode(), (self._socket_setting.address, self._socket_setting.port_send))
     def stop(self):
         msg = 'stop'
         self._s_send.sendto(msg.encode(), (self._socket_setting.address, self._socket_setting.port_send))
     def exit(self):
```

