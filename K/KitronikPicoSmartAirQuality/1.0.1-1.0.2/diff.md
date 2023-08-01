# Comparing `tmp/KitronikPicoSmartAirQuality-1.0.1.tar.gz` & `tmp/KitronikPicoSmartAirQuality-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KitronikPicoSmartAirQuality-1.0.1.tar", last modified: Mon Jun 19 07:37:42 2023, max compression
+gzip compressed data, was "KitronikPicoSmartAirQuality-1.0.2.tar", last modified: Tue Aug  1 09:46:09 2023, max compression
```

## Comparing `KitronikPicoSmartAirQuality-1.0.1.tar` & `KitronikPicoSmartAirQuality-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2023-06-19 07:37:42.494702 KitronikPicoSmartAirQuality-1.0.1/
-drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2023-06-19 07:37:42.494702 KitronikPicoSmartAirQuality-1.0.1/KitronikPicoSmartAirQuality.egg-info/
--rw-r--r--   0 jack      (1000) jack      (1000)    12991 2023-06-19 07:37:42.000000 KitronikPicoSmartAirQuality-1.0.1/KitronikPicoSmartAirQuality.egg-info/PKG-INFO
--rw-r--r--   0 jack      (1000) jack      (1000)      280 2023-06-19 07:37:42.000000 KitronikPicoSmartAirQuality-1.0.1/KitronikPicoSmartAirQuality.egg-info/SOURCES.txt
--rw-r--r--   0 jack      (1000) jack      (1000)        1 2023-06-19 07:37:42.000000 KitronikPicoSmartAirQuality-1.0.1/KitronikPicoSmartAirQuality.egg-info/dependency_links.txt
--rw-r--r--   0 jack      (1000) jack      (1000)       15 2023-06-19 07:37:42.000000 KitronikPicoSmartAirQuality-1.0.1/KitronikPicoSmartAirQuality.egg-info/top_level.txt
--rw-r--r--   0 jack      (1000) jack      (1000)      382 2023-06-19 07:35:42.000000 KitronikPicoSmartAirQuality-1.0.1/KitronikPicoSmartAirQualityWheelSetup.py
--rw-r--r--   0 jack      (1000) jack      (1000)     1070 2023-06-19 07:34:18.000000 KitronikPicoSmartAirQuality-1.0.1/LICENSE
--rw-r--r--   0 jack      (1000) jack      (1000)    12991 2023-06-19 07:37:42.494702 KitronikPicoSmartAirQuality-1.0.1/PKG-INFO
--rw-r--r--   0 jack      (1000) jack      (1000)    55785 2023-06-19 07:34:18.000000 KitronikPicoSmartAirQuality-1.0.1/PicoAirQuality.py
--rw-r--r--   0 jack      (1000) jack      (1000)    12800 2023-06-19 07:34:18.000000 KitronikPicoSmartAirQuality-1.0.1/README.md
--rw-r--r--   0 jack      (1000) jack      (1000)       38 2023-06-19 07:37:42.494702 KitronikPicoSmartAirQuality-1.0.1/setup.cfg
+drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2023-08-01 09:46:09.793500 KitronikPicoSmartAirQuality-1.0.2/
+drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2023-08-01 09:46:09.793500 KitronikPicoSmartAirQuality-1.0.2/KitronikPicoSmartAirQuality.egg-info/
+-rw-r--r--   0 jack      (1000) jack      (1000)    13252 2023-08-01 09:46:09.000000 KitronikPicoSmartAirQuality-1.0.2/KitronikPicoSmartAirQuality.egg-info/PKG-INFO
+-rw-r--r--   0 jack      (1000) jack      (1000)      253 2023-08-01 09:46:09.000000 KitronikPicoSmartAirQuality-1.0.2/KitronikPicoSmartAirQuality.egg-info/SOURCES.txt
+-rw-r--r--   0 jack      (1000) jack      (1000)        1 2023-08-01 09:46:09.000000 KitronikPicoSmartAirQuality-1.0.2/KitronikPicoSmartAirQuality.egg-info/dependency_links.txt
+-rw-r--r--   0 jack      (1000) jack      (1000)       15 2023-08-01 09:46:09.000000 KitronikPicoSmartAirQuality-1.0.2/KitronikPicoSmartAirQuality.egg-info/top_level.txt
+-rw-r--r--   0 jack      (1000) jack      (1000)     1070 2023-08-01 09:39:35.000000 KitronikPicoSmartAirQuality-1.0.2/LICENSE
+-rw-r--r--   0 jack      (1000) jack      (1000)    13252 2023-08-01 09:46:09.793500 KitronikPicoSmartAirQuality-1.0.2/PKG-INFO
+-rw-r--r--   0 jack      (1000) jack      (1000)    56044 2023-08-01 09:39:35.000000 KitronikPicoSmartAirQuality-1.0.2/PicoAirQuality.py
+-rw-r--r--   0 jack      (1000) jack      (1000)    12955 2023-08-01 09:39:35.000000 KitronikPicoSmartAirQuality-1.0.2/README.md
+-rw-r--r--   0 jack      (1000) jack      (1000)      525 2023-08-01 09:45:03.000000 KitronikPicoSmartAirQuality-1.0.2/WheelSetup.py
+-rw-r--r--   0 jack      (1000) jack      (1000)       38 2023-08-01 09:46:09.793500 KitronikPicoSmartAirQuality-1.0.2/setup.cfg
```

### Comparing `KitronikPicoSmartAirQuality-1.0.1/KitronikPicoSmartAirQuality.egg-info/PKG-INFO` & `KitronikPicoSmartAirQuality-1.0.2/KitronikPicoSmartAirQuality.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: KitronikPicoSmartAirQuality
-Version: 1.0.1
+Version: 1.0.2
 Summary: Kitronik Air Quality Datalogging Board for Pico
+Keywords: micropython,package
+Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Other Languages: [FRANCAIS](README_FR.md)
 
 # Kitronik-Pico-Smart-Air-Quality-Board-MicroPython
 
@@ -248,23 +250,30 @@
 ## KitronikOutputControl
 ### Servo:
 The servo PWM (20ms repeat, on period capped between 500 and 2500us) is driven using the Pico PIO.  
 To register a servo ready to be used:  
 ```python
  output.registerServo()
 ```
+
 This process sets the PIO PWM active on the servo pin (**Note:** The servo is registered by default).  
 To control the movement of a servo, turning it to a set angle (or controlling the speed/direction of a continuous rotation servo):  
 ```python
 output.servoToPosition(degrees)
 ```
+
+To control the movement of the servo we can also set it using radians from 0 to 3.1416 (Pi to four digits).
+``` python
+output.servoToRadians(radians)
+```
+
 If the pin is needed for another purpose it can be 'deregistered' which sets the PIO to inactive:  
- ```python
+```python
 output.deregisterServo()
- ```
+```
 
 ### High-Power Outputs:
 The high-power outputs on the board are controlled via two pins on the Pico: GP3 and GP15.  
 The control of these outputs is very simple, either setting them to be **ON** or **OFF**:  
 ```python
 output.highPowerOn(pin)
 output.highPowerOff(pin)
```

### Comparing `KitronikPicoSmartAirQuality-1.0.1/LICENSE` & `KitronikPicoSmartAirQuality-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `KitronikPicoSmartAirQuality-1.0.1/PKG-INFO` & `KitronikPicoSmartAirQuality-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: KitronikPicoSmartAirQuality
-Version: 1.0.1
+Version: 1.0.2
 Summary: Kitronik Air Quality Datalogging Board for Pico
+Keywords: micropython,package
+Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Other Languages: [FRANCAIS](README_FR.md)
 
 # Kitronik-Pico-Smart-Air-Quality-Board-MicroPython
 
@@ -248,23 +250,30 @@
 ## KitronikOutputControl
 ### Servo:
 The servo PWM (20ms repeat, on period capped between 500 and 2500us) is driven using the Pico PIO.  
 To register a servo ready to be used:  
 ```python
  output.registerServo()
 ```
+
 This process sets the PIO PWM active on the servo pin (**Note:** The servo is registered by default).  
 To control the movement of a servo, turning it to a set angle (or controlling the speed/direction of a continuous rotation servo):  
 ```python
 output.servoToPosition(degrees)
 ```
+
+To control the movement of the servo we can also set it using radians from 0 to 3.1416 (Pi to four digits).
+``` python
+output.servoToRadians(radians)
+```
+
 If the pin is needed for another purpose it can be 'deregistered' which sets the PIO to inactive:  
- ```python
+```python
 output.deregisterServo()
- ```
+```
 
 ### High-Power Outputs:
 The high-power outputs on the board are controlled via two pins on the Pico: GP3 and GP15.  
 The control of these outputs is very simple, either setting them to be **ON** or **OFF**:  
 ```python
 output.highPowerOn(pin)
 output.highPowerOff(pin)
```

### Comparing `KitronikPicoSmartAirQuality-1.0.1/PicoAirQuality.py` & `KitronikPicoSmartAirQuality-1.0.2/PicoAirQuality.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
         # 1us is freq of 1000000
         # Servo pulses range from 500 to 2500us and overall pulse train is 20000us repeat.
         # Servo is on GP2
         self.maxServoPulse = 2500
         self.minServoPulse = 500
         self.pulseTrain = 20000
         self.degreesToUS = 2000/180
+        self.piEstimate = 3.1416
 
         # Create and start the servo statemachine
         for i in range(8): # StateMachine range from 0 to 7
             if usedSM[i]:
                 continue # Ignore this index if already used
             try:
                 self.servo.append(StateMachine(i, self._servo_pwm, freq=2000000, sideset_base=Pin(2)))
@@ -96,14 +97,20 @@
     # 0degrees->180 degrees is 0->2000us, plus offset of 500uS
     # 1 degree ~ 11uS.
     # This function does the sum then calls goToPeriod to actually poke the PIO 
     def servoToPosition(self, degrees):
         pulseLength = int(degrees*self.degreesToUS + 500)
         self.servoToPeriod(pulseLength)
     
+    # Takes the angle in radians to move the servo to.
+    # 0 radians to 3.1416
+    def servoToRadians(self, radians):
+        period = int((radians / self.piEstimate) * 2000) + 500
+        self.servoToPeriod(period)
+    
     def servoToPeriod(self, period):
         if(period < 500):
             period = 500
         if(period >2500):
             period =2500
         self.servo[0].put(period)
 
@@ -724,15 +731,15 @@
         self.hRead = self.hRead // 1000
 
     # Gas sensor heater target temperature to target resistance calculation
     # 'ambientTemp' is reading from Temperature sensor in degC (could be averaged over a day when there is enough data?)
     # 'targetTemp' is the desired temperature of the hot plate in degC (in range 200 to 400)
     # Note: Heating duration also needs to be specified for each heating step in 'gas_wait' registers
     def intConvertGasTargetTemp(self, ambientTemp, targetTemp):
-        var1 = ((ambientTemp * self.PAR_G3) // 1000) << 8    # Divide by 1000 as we have ambientTemp in pre-degC format (i.e. 2500 rather than 25.00 degC)
+        var1 = int((ambientTemp * self.PAR_G3) // 1000) << 8    # Divide by 1000 as we have ambientTemp in pre-degC format (i.e. 2500 rather than 25.00 degC)
         var2 = (self.PAR_G1 + 784) * (((((self.PAR_G2 + 154009) * targetTemp * 5) // 100) + 3276800) // 10)
         var3 = var1 + (var2 >> 1)
         var4 = (var3 // (self.RES_HEAT_RANGE + 4))
         var5 = (131 * self.RES_HEAT_VAL) + 65536                 # Target heater resistance in Ohms
         resHeatX100 = (((var4 // var5) - 250) * 34)
         resHeat = ((resHeatX100 + 50) // 100)
```

### Comparing `KitronikPicoSmartAirQuality-1.0.1/README.md` & `KitronikPicoSmartAirQuality-1.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -241,23 +241,30 @@
 ## KitronikOutputControl
 ### Servo:
 The servo PWM (20ms repeat, on period capped between 500 and 2500us) is driven using the Pico PIO.  
 To register a servo ready to be used:  
 ```python
  output.registerServo()
 ```
+
 This process sets the PIO PWM active on the servo pin (**Note:** The servo is registered by default).  
 To control the movement of a servo, turning it to a set angle (or controlling the speed/direction of a continuous rotation servo):  
 ```python
 output.servoToPosition(degrees)
 ```
+
+To control the movement of the servo we can also set it using radians from 0 to 3.1416 (Pi to four digits).
+``` python
+output.servoToRadians(radians)
+```
+
 If the pin is needed for another purpose it can be 'deregistered' which sets the PIO to inactive:  
- ```python
+```python
 output.deregisterServo()
- ```
+```
 
 ### High-Power Outputs:
 The high-power outputs on the board are controlled via two pins on the Pico: GP3 and GP15.  
 The control of these outputs is very simple, either setting them to be **ON** or **OFF**:  
 ```python
 output.highPowerOn(pin)
 output.highPowerOff(pin)
```

