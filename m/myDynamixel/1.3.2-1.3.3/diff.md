# Comparing `tmp/myDynamixel-1.3.2-py3-none-any.whl.zip` & `tmp/myDynamixel-1.3.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3920 bytes, number of entries: 6
+Zip file size: 4120 bytes, number of entries: 6
 -rw-rw-rw-  2.0 fat       37 b- defN 22-Dec-12 06:36 myDynamixel/__init__.py
--rw-rw-rw-  2.0 fat    13012 b- defN 23-Jun-05 08:59 myDynamixel/myDynamixel.py
--rw-rw-rw-  2.0 fat      258 b- defN 23-Jun-05 09:09 myDynamixel-1.3.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-05 09:09 myDynamixel-1.3.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-Jun-05 09:09 myDynamixel-1.3.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      475 b- defN 23-Jun-05 09:09 myDynamixel-1.3.2.dist-info/RECORD
-6 files, 13886 bytes uncompressed, 3056 bytes compressed:  78.0%
+-rw-rw-rw-  2.0 fat    13859 b- defN 23-Aug-01 10:03 myDynamixel/myDynamixel.py
+-rw-rw-rw-  2.0 fat      258 b- defN 23-Aug-01 10:04 myDynamixel-1.3.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-01 10:04 myDynamixel-1.3.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Aug-01 10:04 myDynamixel-1.3.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      475 b- defN 23-Aug-01 10:04 myDynamixel-1.3.3.dist-info/RECORD
+6 files, 14733 bytes uncompressed, 3256 bytes compressed:  77.9%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: myDynamixel/__init__.py
 Comment: 
 
 Filename: myDynamixel/myDynamixel.py
 Comment: 
 
-Filename: myDynamixel-1.3.2.dist-info/METADATA
+Filename: myDynamixel-1.3.3.dist-info/METADATA
 Comment: 
 
-Filename: myDynamixel-1.3.2.dist-info/WHEEL
+Filename: myDynamixel-1.3.3.dist-info/WHEEL
 Comment: 
 
-Filename: myDynamixel-1.3.2.dist-info/top_level.txt
+Filename: myDynamixel-1.3.3.dist-info/top_level.txt
 Comment: 
 
-Filename: myDynamixel-1.3.2.dist-info/RECORD
+Filename: myDynamixel-1.3.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## myDynamixel/myDynamixel.py

```diff
@@ -1,8 +1,8 @@
-# ver 1.3.2
+# ver 1.3.3
 
 import numpy as np
 from dynamixel_sdk import *
 
 class Dxlfunc:
     class Adrress:
         ModelNumber         = 0
@@ -92,14 +92,34 @@
         XH540_V150 = 1150
         XM540_W270 = 1120
         XH540_W270 = 1100
         XH540_V270 = 1140
         XW540_T140 = 1180
         XW540_T260 = 1170
 
+    class br_list:
+        br9600 = 9600
+        br19200 = 19200
+        br38400 = 38400
+        br57600 = 57600
+        br115200 = 115200
+        br230400 = 230400
+        br460800 = 460800
+        br500000 = 500000
+        br576000 = 576000
+        br921600 = 921600
+        br1000000 = 1000000
+        br1152000 = 1152000
+        br2000000 = 2000000
+        br2500000 = 2500000
+        br3000000 = 3000000
+        br3500000 = 3500000
+        br4000000 = 4000000
+        br4500000 = 4500000
+
     class __initErrorCode:
         USB_disconnect = -3000
         PowerSource_disconnect = -3001
 
     class DXL_Error(Exception):
         pass
 
@@ -134,18 +154,24 @@
                                  self.Adrress.VelocityTrajectory, self.Adrress.PositionTrajectory]
 
     def init(self, com, baudrate=57600):
         self._portHandler = PortHandler(com)
         baudrates = [9600, 57600, 115200, 1000000, 2000000, 3000000, 4000000]
         try:
             if self._portHandler.openPort():
-                self._portHandler.setBaudRate(baudrate)
+                if baudrate in baudrates:
+                    self._portHandler.setBaudRate(baudrate)
+                elif baudrate == self.br_list.br4500000:
+                    self._portHandler.baudrate = baudrate
+                    self._portHandler.setupPort(baudrate)
                 self.IDs = [i for i in range(10) if self._packetHandler.read1ByteTxRx(self._portHandler, i, self.Adrress.ID)[1] == 0]
                 if len(self.IDs) == 0:
-                    for br in baudrates:
+                    for br in list(self.br_list.__dict__.values()):
+                        if type(br) != int:
+                            continue
                         self._portHandler.setBaudRate(br)
                         self.IDs = [i for i in range(10) if self._packetHandler.read1ByteTxRx(self._portHandler, i, self.Adrress.ID)[1] == 0]
                         if len(self.IDs) > 0:
                             raise self.DXL_Error("Argument baud rate is different from baud rate set in motor")
                 if len(self.IDs) > 0:
                     return len(self.IDs)
                 else:
```

