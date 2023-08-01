# Comparing `tmp/micrOSDevToolKit-1.21.0.tar.gz` & `tmp/micrOSDevToolKit-1.21.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/micrOSDevToolKit-1.21.0.tar", last modified: Wed Jul 26 14:54:48 2023, max compression
+gzip compressed data, was "dist/micrOSDevToolKit-1.21.1.tar", last modified: Tue Aug  1 20:08:06 2023, max compression
```

## Comparing `micrOSDevToolKit-1.21.0.tar` & `micrOSDevToolKit-1.21.1.tar`

### file list

```diff
@@ -1,253 +1,255 @@
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 14:54:48.773724 micrOSDevToolKit-1.21.0/
--rw-r--r--   0 bnm        (501) staff       (20)      333 2023-07-18 21:54:39.000000 micrOSDevToolKit-1.21.0/MANIFEST.in
--rw-r--r--   0 bnm        (501) staff       (20)    54579 2023-07-26 14:54:48.773220 micrOSDevToolKit-1.21.0/PKG-INFO
--rw-r--r--   0 bnm        (501) staff       (20)    45024 2023-07-05 20:30:41.000000 micrOSDevToolKit-1.21.0/README.md
--rwxr-xr-x   0 bnm        (501) staff       (20)     8984 2023-07-05 20:33:26.000000 micrOSDevToolKit-1.21.0/devToolKit.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 14:54:48.404457 micrOSDevToolKit-1.21.0/env/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.0/env/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 14:54:48.409750 micrOSDevToolKit-1.21.0/media/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.21.0/media/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)    42752 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.0/media/dnd.png
--rw-r--r--   0 bnm        (501) staff       (20)   482208 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.21.0/media/logo.png
--rw-r--r--   0 bnm        (501) staff       (20)    24854 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.0/media/logo_mini.png
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 14:54:48.413297 micrOSDevToolKit-1.21.0/micrOS/
--rw-r--r--   0 bnm        (501) staff       (20)     1312 2023-07-13 18:57:05.000000 micrOSDevToolKit-1.21.0/micrOS/SchedulerUT.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.0/micrOS/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 14:54:48.466565 micrOSDevToolKit-1.21.0/micrOS/micropython/
--rw-r--r--   0 bnm        (501) staff       (20)  1560976 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.0/micrOS/micropython/esp32-20220618-v1.19.1.bin
--rw-r--r--   0 bnm        (501) staff       (20)  1230192 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.0/micrOS/micropython/esp32s2-20220618-v1.19.1.bin
--rw-r--r--   0 bnm        (501) staff       (20)  1446848 2023-06-14 11:15:48.000000 micrOSDevToolKit-1.21.0/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin
--rw-r--r--   0 bnm        (501) staff       (20)  1400832 2023-05-11 08:44:05.000000 micrOSDevToolKit-1.21.0/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2
--rw-r--r--   0 bnm        (501) staff       (20)  1519248 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.0/micrOS/micropython/tinypico-20220618-v1.19.1.bin
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 14:54:48.538825 micrOSDevToolKit-1.21.0/micrOS/source/
--rw-r--r--   0 bnm        (501) staff       (20)     6148 2023-02-01 11:41:53.000000 micrOSDevToolKit-1.21.0/micrOS/source/.DS_Store
--rw-r--r--   0 bnm        (501) staff       (20)     6198 2023-07-17 14:02:35.000000 micrOSDevToolKit-1.21.0/micrOS/source/Common.py
--rw-r--r--   0 bnm        (501) staff       (20)     8423 2023-07-17 14:17:45.000000 micrOSDevToolKit-1.21.0/micrOS/source/ConfigHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)     6331 2023-07-17 14:19:18.000000 micrOSDevToolKit-1.21.0/micrOS/source/Debug.py
--rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-07-17 14:24:13.000000 micrOSDevToolKit-1.21.0/micrOS/source/Hooks.py
--rw-r--r--   0 bnm        (501) staff       (20)     6844 2023-07-22 08:28:00.000000 micrOSDevToolKit-1.21.0/micrOS/source/InterConnect.py
--rw-r--r--   0 bnm        (501) staff       (20)    11569 2023-07-26 14:03:06.000000 micrOSDevToolKit-1.21.0/micrOS/source/InterpreterShell.py
--rw-r--r--   0 bnm        (501) staff       (20)     7470 2023-07-20 09:51:20.000000 micrOSDevToolKit-1.21.0/micrOS/source/InterruptHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)     2358 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_L298N_DCmotor.py
--rw-r--r--   0 bnm        (501) staff       (20)     1774 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_L9110_DCmotor.py
--rw-r--r--   0 bnm        (501) staff       (20)    10011 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_VL53L0X.py
--rw-r--r--   0 bnm        (501) staff       (20)    12710 2023-07-15 21:14:31.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_bme280.py
--rw-r--r--   0 bnm        (501) staff       (20)     8364 2023-06-26 10:58:53.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_buzzer.py
--rw-r--r--   0 bnm        (501) staff       (20)     1647 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_catgame.py
--rw-r--r--   0 bnm        (501) staff       (20)    14014 2023-03-13 19:15:23.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_cct.py
--rw-r--r--   0 bnm        (501) staff       (20)     5149 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_co2.py
--rw-r--r--   0 bnm        (501) staff       (20)     1952 2023-07-18 21:04:59.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_demo.py
--rw-r--r--   0 bnm        (501) staff       (20)     2149 2023-07-15 21:11:36.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_dht11.py
--rw-r--r--   0 bnm        (501) staff       (20)     2149 2023-07-15 19:50:30.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_dht22.py
--rw-r--r--   0 bnm        (501) staff       (20)     8137 2023-03-13 17:50:37.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_dimmer.py
--rw-r--r--   0 bnm        (501) staff       (20)     2433 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_distance.py
--rw-r--r--   0 bnm        (501) staff       (20)     1532 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_ds18.py
--rw-r--r--   0 bnm        (501) staff       (20)     1470 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)     4106 2022-12-29 20:58:04.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_genIO.py
--rw-r--r--   0 bnm        (501) staff       (20)     1015 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_i2c.py
--rw-r--r--   0 bnm        (501) staff       (20)     1608 2023-03-09 18:56:28.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_intercon.py
--rw-r--r--   0 bnm        (501) staff       (20)     1618 2023-07-06 20:03:50.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_light_sensor.py
--rw-r--r--   0 bnm        (501) staff       (20)     2890 2023-07-18 20:07:19.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_lmpacman.py
--rw-r--r--   0 bnm        (501) staff       (20)    10473 2022-12-30 23:37:13.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_neoeffects.py
--rw-r--r--   0 bnm        (501) staff       (20)    13027 2023-03-13 17:52:36.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_neopixel.py
--rw-r--r--   0 bnm        (501) staff       (20)     6745 2023-06-26 12:47:51.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_oled.py
--rw-r--r--   0 bnm        (501) staff       (20)     9649 2023-06-26 12:52:45.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_oled_sh1106.py
--rw-r--r--   0 bnm        (501) staff       (20)    19328 2023-07-26 14:42:47.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_oled_ui.py
--rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-01-21 00:34:37.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_pet_feeder.py
--rw-r--r--   0 bnm        (501) staff       (20)     1279 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_ph_sensor.py
--rw-r--r--   0 bnm        (501) staff       (20)     8081 2023-03-08 10:25:44.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_presence.py
--rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-01-21 19:25:04.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_rencoder.py
--rw-r--r--   0 bnm        (501) staff       (20)    11895 2023-03-13 17:53:56.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_rgb.py
--rw-r--r--   0 bnm        (501) staff       (20)     9383 2023-03-07 15:19:00.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_roboarm.py
--rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-02-01 13:23:22.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_robustness.py
--rw-r--r--   0 bnm        (501) staff       (20)     3427 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_servo.py
--rw-r--r--   0 bnm        (501) staff       (20)     4228 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_stepper.py
--rw-r--r--   0 bnm        (501) staff       (20)     7567 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_switch.py
--rw-r--r--   0 bnm        (501) staff       (20)     6374 2023-07-17 18:21:37.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_system.py
--rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-03-19 11:48:09.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_telegram.py
--rw-r--r--   0 bnm        (501) staff       (20)     2947 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_tinyrgb.py
--rw-r--r--   0 bnm        (501) staff       (20)     2183 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.0/micrOS/source/LP_esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-06-26 12:00:43.000000 micrOSDevToolKit-1.21.0/micrOS/source/LP_esp32s2.py
--rw-r--r--   0 bnm        (501) staff       (20)     2104 2023-06-14 17:40:43.000000 micrOSDevToolKit-1.21.0/micrOS/source/LP_esp32s3.py
--rw-r--r--   0 bnm        (501) staff       (20)       99 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.0/micrOS/source/LP_rp2.py
--rw-r--r--   0 bnm        (501) staff       (20)     2200 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.0/micrOS/source/LP_tinypico.py
--rw-r--r--   0 bnm        (501) staff       (20)     5742 2023-06-14 13:29:12.000000 micrOSDevToolKit-1.21.0/micrOS/source/LogicalPins.py
--rw-r--r--   0 bnm        (501) staff       (20)     9579 2023-07-17 14:33:44.000000 micrOSDevToolKit-1.21.0/micrOS/source/Network.py
--rw-r--r--   0 bnm        (501) staff       (20)     9189 2023-07-15 18:23:05.000000 micrOSDevToolKit-1.21.0/micrOS/source/Notify.py
--rw-r--r--   0 bnm        (501) staff       (20)     7744 2023-07-09 11:44:18.000000 micrOSDevToolKit-1.21.0/micrOS/source/Scheduler.py
--rw-r--r--   0 bnm        (501) staff       (20)    11566 2023-07-15 19:57:59.000000 micrOSDevToolKit-1.21.0/micrOS/source/SocketServer.py
--rw-r--r--   0 bnm        (501) staff       (20)    19349 2023-07-26 13:44:08.000000 micrOSDevToolKit-1.21.0/micrOS/source/TaskManager.py
--rw-r--r--   0 bnm        (501) staff       (20)     6254 2023-07-15 20:34:18.000000 micrOSDevToolKit-1.21.0/micrOS/source/Time.py
--rw-r--r--   0 bnm        (501) staff       (20)      981 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.0/micrOS/source/TinyPLed.py
--rw-r--r--   0 bnm        (501) staff       (20)      440 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.0/micrOS/source/main.py
--rw-r--r--   0 bnm        (501) staff       (20)     2657 2023-07-17 14:37:17.000000 micrOSDevToolKit-1.21.0/micrOS/source/micrOS.py
--rw-r--r--   0 bnm        (501) staff       (20)     4678 2023-07-17 14:34:26.000000 micrOSDevToolKit-1.21.0/micrOS/source/micrOSloader.py
--rw-r--r--   0 bnm        (501) staff       (20)      183 2023-03-09 19:11:59.000000 micrOSDevToolKit-1.21.0/micrOS/source/reset.py
--rw-r--r--   0 bnm        (501) staff       (20)     4926 2023-07-17 14:41:23.000000 micrOSDevToolKit-1.21.0/micrOS/source/urequests.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 14:54:48.544057 micrOSDevToolKit-1.21.0/micrOSDevToolKit.egg-info/
--rw-r--r--   0 bnm        (501) staff       (20)    54579 2023-07-26 14:54:48.000000 micrOSDevToolKit-1.21.0/micrOSDevToolKit.egg-info/PKG-INFO
--rw-r--r--   0 bnm        (501) staff       (20)     8866 2023-07-26 14:54:48.000000 micrOSDevToolKit-1.21.0/micrOSDevToolKit.egg-info/SOURCES.txt
--rw-r--r--   0 bnm        (501) staff       (20)        1 2023-07-26 14:54:48.000000 micrOSDevToolKit-1.21.0/micrOSDevToolKit.egg-info/dependency_links.txt
--rw-r--r--   0 bnm        (501) staff       (20)      149 2023-07-26 14:54:48.000000 micrOSDevToolKit-1.21.0/micrOSDevToolKit.egg-info/requires.txt
--rw-r--r--   0 bnm        (501) staff       (20)       25 2023-07-26 14:54:48.000000 micrOSDevToolKit-1.21.0/micrOSDevToolKit.egg-info/top_level.txt
--rw-r--r--   0 bnm        (501) staff       (20)       38 2023-07-26 14:54:48.773872 micrOSDevToolKit-1.21.0/setup.cfg
--rw-r--r--   0 bnm        (501) staff       (20)     1282 2023-07-26 14:51:46.000000 micrOSDevToolKit-1.21.0/setup.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 14:54:48.554680 micrOSDevToolKit-1.21.0/toolkit/
--rw-r--r--   0 bnm        (501) staff       (20)     8377 2023-01-04 20:19:38.000000 micrOSDevToolKit-1.21.0/toolkit/DevEnvCompile.py
--rw-r--r--   0 bnm        (501) staff       (20)    24453 2023-07-15 18:35:28.000000 micrOSDevToolKit-1.21.0/toolkit/DevEnvOTA.py
--rw-r--r--   0 bnm        (501) staff       (20)    31441 2023-07-12 17:35:49.000000 micrOSDevToolKit-1.21.0/toolkit/DevEnvUSB.py
--rw-r--r--   0 bnm        (501) staff       (20)    12307 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.0/toolkit/Gateway.py
--rw-r--r--   0 bnm        (501) staff       (20)    11615 2023-07-17 15:49:40.000000 micrOSDevToolKit-1.21.0/toolkit/MicrOSDevEnv.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.0/toolkit/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 14:54:48.572579 micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/
--rw-r--r--   0 bnm        (501) staff       (20)      747 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/AirQualityBME280.py
--rw-r--r--   0 bnm        (501) staff       (20)      749 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/AirQualityDHT22_CO2.py
--rw-r--r--   0 bnm        (501) staff       (20)     1278 2023-01-14 18:12:52.000000 micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/CCTDemo.py
--rw-r--r--   0 bnm        (501) staff       (20)     3798 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/CCTTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     1487 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/CatGame.py
--rw-r--r--   0 bnm        (501) staff       (20)      937 2023-01-16 18:30:18.000000 micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/Dimmer.py
--rw-r--r--   0 bnm        (501) staff       (20)      542 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/GetVersion.py
--rw-r--r--   0 bnm        (501) staff       (20)      407 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/MicrophoneTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     2409 2023-01-14 15:33:34.000000 micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/NeoEffectsDemo.py
--rw-r--r--   0 bnm        (501) staff       (20)     3938 2023-01-05 18:02:55.000000 micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/NeopixelTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     3920 2023-01-05 18:11:07.000000 micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/RGBTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     2084 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/RoboArm.py
--rw-r--r--   0 bnm        (501) staff       (20)     2782 2023-01-05 18:10:36.000000 micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/SED_test.py
--rw-r--r--   0 bnm        (501) staff       (20)    17600 2023-07-19 10:50:53.000000 micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/SystemTest.py
--rw-r--r--   0 bnm        (501) staff       (20)      760 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/Template_app.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)     3901 2023-03-08 10:26:06.000000 micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/_micPlotting.py
--rw-r--r--   0 bnm        (501) staff       (20)     3380 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/uLightDemo.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 14:54:48.579360 micrOSDevToolKit-1.21.0/toolkit/lib/
--rw-r--r--   0 bnm        (501) staff       (20)    18734 2023-02-07 20:49:31.000000 micrOSDevToolKit-1.21.0/toolkit/lib/LocalMachine.py
--rw-r--r--   0 bnm        (501) staff       (20)     5421 2023-07-05 11:31:18.000000 micrOSDevToolKit-1.21.0/toolkit/lib/SearchDevices.py
--rw-r--r--   0 bnm        (501) staff       (20)     6222 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.0/toolkit/lib/SerialDriverHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)      847 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.0/toolkit/lib/TerminalColors.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.0/toolkit/lib/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)    16808 2023-03-15 15:54:40.000000 micrOSDevToolKit-1.21.0/toolkit/lib/micrOSClient.py
--rw-r--r--   0 bnm        (501) staff       (20)    52184 2023-07-01 21:55:14.000000 micrOSDevToolKit-1.21.0/toolkit/micrOSdashboard.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 14:54:48.597853 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/
--rw-r--r--   0 bnm        (501) staff       (20)     2071 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/LP_darwin.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 14:54:48.648074 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/
--rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      473 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/dotstar.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      483 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/dotstar.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/esp32.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/esp32.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/framebuf.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/framebuf.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     6832 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     7029 2023-07-04 17:16:29.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1124 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1340 2023-03-17 15:56:36.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     2985 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     2991 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/onewire.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/onewire.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1063 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      362 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/simgc.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      471 2023-02-01 12:53:53.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/simgc.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     4799 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     5397 2023-07-15 16:13:28.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/tinypico.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/tinypico.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      976 2022-12-14 21:38:13.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1355 2023-06-27 16:26:11.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1583 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1583 2023-06-27 12:57:10.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      254 2022-12-03 14:47:41.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/webrepl.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      254 2023-01-01 15:36:25.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/webrepl.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)       95 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/dotstar.py
--rw-r--r--   0 bnm        (501) staff       (20)      193 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/ds18x20.py
--rw-r--r--   0 bnm        (501) staff       (20)       71 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)       47 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/framebuf.py
--rw-r--r--   0 bnm        (501) staff       (20)     4430 2023-07-01 22:39:14.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/machine.py
--rw-r--r--   0 bnm        (501) staff       (20)      909 2023-03-17 15:56:08.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/micropython.py
--rw-r--r--   0 bnm        (501) staff       (20)      567 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/neopixel.py
--rw-r--r--   0 bnm        (501) staff       (20)     2490 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/network.py
--rw-r--r--   0 bnm        (501) staff       (20)      109 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/ntptime.py
--rw-r--r--   0 bnm        (501) staff       (20)       77 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/onewire.py
--rw-r--r--   0 bnm        (501) staff       (20)      943 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/sim_console.py
--rw-r--r--   0 bnm        (501) staff       (20)      140 2023-02-01 12:53:17.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/simgc.py
--rw-r--r--   0 bnm        (501) staff       (20)     6545 2023-07-15 16:13:22.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/simulator.py
--rw-r--r--   0 bnm        (501) staff       (20)      156 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/tinypico.py
--rw-r--r--   0 bnm        (501) staff       (20)      528 2023-06-27 16:23:56.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/uasyncio.py
--rw-r--r--   0 bnm        (501) staff       (20)      942 2023-06-27 12:56:02.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/utime.py
--rw-r--r--   0 bnm        (501) staff       (20)       37 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/webrepl.py
--rwxr-xr-x   0 bnm        (501) staff       (20)    16970 2023-07-19 10:36:50.000000 micrOSDevToolKit-1.21.0/toolkit/socketClient.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 14:54:48.649109 micrOSDevToolKit-1.21.0/toolkit/user_data/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2023-07-18 21:50:53.000000 micrOSDevToolKit-1.21.0/toolkit/user_data/.include
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 14:54:48.649626 micrOSDevToolKit-1.21.0/toolkit/user_data/node_config_archive/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2023-07-18 21:53:27.000000 micrOSDevToolKit-1.21.0/toolkit/user_data/node_config_archive/.include
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 14:54:48.650416 micrOSDevToolKit-1.21.0/toolkit/workspace/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 14:54:48.771650 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/
--rw-r--r--   0 bnm        (501) staff       (20)     1791 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/Common.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2996 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/ConfigHandler.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1927 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/Debug.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      759 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/Hooks.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2085 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/InterConnect.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     4174 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/InterpreterShell.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2145 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/InterruptHandler.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      869 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1774 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_L9110_DCmotor.py
--rw-r--r--   0 bnm        (501) staff       (20)    10011 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_VL53L0X.py
--rw-r--r--   0 bnm        (501) staff       (20)     4280 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_bme280.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2604 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_buzzer.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1647 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_catgame.py
--rw-r--r--   0 bnm        (501) staff       (20)     3836 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_cct.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1359 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_co2.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1952 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_demo.py
--rw-r--r--   0 bnm        (501) staff       (20)      793 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_dht11.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      793 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_dht22.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2353 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_dimmer.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2433 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_distance.py
--rw-r--r--   0 bnm        (501) staff       (20)      522 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_ds18.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1470 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)     1364 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_genIO.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1015 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_i2c.py
--rw-r--r--   0 bnm        (501) staff       (20)      616 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_intercon.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      512 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_light_sensor.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1477 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_lmpacman.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2865 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_neoeffects.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3650 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_neopixel.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_oled.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3203 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_oled_sh1106.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     6191 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_oled_ui.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_pet_feeder.py
--rw-r--r--   0 bnm        (501) staff       (20)     1279 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_ph_sensor.py
--rw-r--r--   0 bnm        (501) staff       (20)     2558 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_presence.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_rencoder.py
--rw-r--r--   0 bnm        (501) staff       (20)     3508 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_rgb.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2946 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_roboarm.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_robustness.py
--rw-r--r--   0 bnm        (501) staff       (20)     1143 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_servo.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1471 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_stepper.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2167 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_switch.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2754 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_system.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      872 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_telegram.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1001 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_tinyrgb.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      550 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LP_esp32.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      563 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LP_esp32s2.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      553 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LP_esp32s3.mpy
--rw-r--r--   0 bnm        (501) staff       (20)       54 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LP_rp2.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      491 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LP_tinypico.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1348 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LogicalPins.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3400 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/Network.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2900 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/Notify.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1903 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/Scheduler.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3763 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/SocketServer.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     5718 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/TaskManager.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2727 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/Time.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      434 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/TinyPLed.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      440 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/main.py
--rw-r--r--   0 bnm        (501) staff       (20)     1186 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/micrOS.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1730 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/micrOSloader.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      198 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/reset.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1451 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/urequests.mpy
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-01 20:08:06.723503 micrOSDevToolKit-1.21.1/
+-rw-r--r--   0 bnm        (501) staff       (20)      333 2023-07-18 21:54:39.000000 micrOSDevToolKit-1.21.1/MANIFEST.in
+-rw-r--r--   0 bnm        (501) staff       (20)    54579 2023-08-01 20:08:06.722123 micrOSDevToolKit-1.21.1/PKG-INFO
+-rw-r--r--   0 bnm        (501) staff       (20)    45024 2023-07-05 20:30:41.000000 micrOSDevToolKit-1.21.1/README.md
+-rwxr-xr-x   0 bnm        (501) staff       (20)     8984 2023-07-05 20:33:26.000000 micrOSDevToolKit-1.21.1/devToolKit.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-01 20:08:06.315578 micrOSDevToolKit-1.21.1/env/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.1/env/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-01 20:08:06.329491 micrOSDevToolKit-1.21.1/media/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.21.1/media/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)    42752 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.1/media/dnd.png
+-rw-r--r--   0 bnm        (501) staff       (20)   482208 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.21.1/media/logo.png
+-rw-r--r--   0 bnm        (501) staff       (20)    24854 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.1/media/logo_mini.png
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-01 20:08:06.332517 micrOSDevToolKit-1.21.1/micrOS/
+-rw-r--r--   0 bnm        (501) staff       (20)     1312 2023-07-13 18:57:05.000000 micrOSDevToolKit-1.21.1/micrOS/SchedulerUT.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.1/micrOS/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-01 20:08:06.379010 micrOSDevToolKit-1.21.1/micrOS/micropython/
+-rw-r--r--   0 bnm        (501) staff       (20)  1560976 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.1/micrOS/micropython/esp32-20220618-v1.19.1.bin
+-rw-r--r--   0 bnm        (501) staff       (20)  1230192 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.1/micrOS/micropython/esp32s2-20220618-v1.19.1.bin
+-rw-r--r--   0 bnm        (501) staff       (20)  1446848 2023-06-14 11:15:48.000000 micrOSDevToolKit-1.21.1/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin
+-rw-r--r--   0 bnm        (501) staff       (20)  1400832 2023-05-11 08:44:05.000000 micrOSDevToolKit-1.21.1/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2
+-rw-r--r--   0 bnm        (501) staff       (20)  1519248 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.1/micrOS/micropython/tinypico-20220618-v1.19.1.bin
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-01 20:08:06.490203 micrOSDevToolKit-1.21.1/micrOS/source/
+-rw-r--r--   0 bnm        (501) staff       (20)     6148 2023-02-01 11:41:53.000000 micrOSDevToolKit-1.21.1/micrOS/source/.DS_Store
+-rw-r--r--   0 bnm        (501) staff       (20)     6205 2023-08-01 19:27:35.000000 micrOSDevToolKit-1.21.1/micrOS/source/Common.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8423 2023-07-17 14:17:45.000000 micrOSDevToolKit-1.21.1/micrOS/source/ConfigHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6443 2023-08-01 19:27:35.000000 micrOSDevToolKit-1.21.1/micrOS/source/Debug.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-07-17 14:24:13.000000 micrOSDevToolKit-1.21.1/micrOS/source/Hooks.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6844 2023-07-22 08:28:00.000000 micrOSDevToolKit-1.21.1/micrOS/source/InterConnect.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11569 2023-08-01 19:32:01.000000 micrOSDevToolKit-1.21.1/micrOS/source/InterpreterShell.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7470 2023-07-20 09:51:20.000000 micrOSDevToolKit-1.21.1/micrOS/source/InterruptHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2358 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_L298N_DCmotor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1774 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_L9110_DCmotor.py
+-rw-r--r--   0 bnm        (501) staff       (20)    10011 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_VL53L0X.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3786 2023-08-01 19:30:57.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_aht10.py
+-rw-r--r--   0 bnm        (501) staff       (20)    12710 2023-07-15 21:14:31.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_bme280.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8364 2023-06-26 10:58:53.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_buzzer.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1647 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_catgame.py
+-rw-r--r--   0 bnm        (501) staff       (20)    14014 2023-03-13 19:15:23.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_cct.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5149 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_co2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1952 2023-07-18 21:04:59.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_demo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2149 2023-07-15 21:11:36.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_dht11.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2149 2023-07-15 19:50:30.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_dht22.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8137 2023-03-13 17:50:37.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_dimmer.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2433 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_distance.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1532 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_ds18.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1470 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4106 2022-12-29 20:58:04.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_genIO.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1015 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_i2c.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1608 2023-03-09 18:56:28.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_intercon.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1618 2023-07-06 20:03:50.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_light_sensor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2890 2023-07-18 20:07:19.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_lmpacman.py
+-rw-r--r--   0 bnm        (501) staff       (20)    10473 2022-12-30 23:37:13.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_neoeffects.py
+-rw-r--r--   0 bnm        (501) staff       (20)    13027 2023-03-13 17:52:36.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_neopixel.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6745 2023-06-26 12:47:51.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_oled.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9649 2023-06-26 12:52:45.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_oled_sh1106.py
+-rw-r--r--   0 bnm        (501) staff       (20)    19328 2023-07-26 14:42:47.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_oled_ui.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-01-21 00:34:37.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_pet_feeder.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1279 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_ph_sensor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8081 2023-03-08 10:25:44.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_presence.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-01-21 19:25:04.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_rencoder.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11895 2023-03-13 17:53:56.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_rgb.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9383 2023-03-07 15:19:00.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_roboarm.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-02-01 13:23:22.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_robustness.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3427 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_servo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4228 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_stepper.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7567 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_switch.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6374 2023-07-17 18:21:37.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_system.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-03-19 11:48:09.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_telegram.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2947 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.1/micrOS/source/LM_tinyrgb.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2183 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.1/micrOS/source/LP_esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-06-26 12:00:43.000000 micrOSDevToolKit-1.21.1/micrOS/source/LP_esp32s2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2104 2023-06-14 17:40:43.000000 micrOSDevToolKit-1.21.1/micrOS/source/LP_esp32s3.py
+-rw-r--r--   0 bnm        (501) staff       (20)       99 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.1/micrOS/source/LP_rp2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2200 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.1/micrOS/source/LP_tinypico.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5742 2023-06-14 13:29:12.000000 micrOSDevToolKit-1.21.1/micrOS/source/LogicalPins.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9579 2023-07-17 14:33:44.000000 micrOSDevToolKit-1.21.1/micrOS/source/Network.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9189 2023-07-15 18:23:05.000000 micrOSDevToolKit-1.21.1/micrOS/source/Notify.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7744 2023-07-09 11:44:18.000000 micrOSDevToolKit-1.21.1/micrOS/source/Scheduler.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11566 2023-07-29 10:25:26.000000 micrOSDevToolKit-1.21.1/micrOS/source/SocketServer.py
+-rw-r--r--   0 bnm        (501) staff       (20)    19349 2023-07-29 10:13:31.000000 micrOSDevToolKit-1.21.1/micrOS/source/TaskManager.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6254 2023-07-15 20:34:18.000000 micrOSDevToolKit-1.21.1/micrOS/source/Time.py
+-rw-r--r--   0 bnm        (501) staff       (20)      981 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.1/micrOS/source/TinyPLed.py
+-rw-r--r--   0 bnm        (501) staff       (20)      440 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.1/micrOS/source/main.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2657 2023-07-17 14:37:17.000000 micrOSDevToolKit-1.21.1/micrOS/source/micrOS.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4678 2023-07-17 14:34:26.000000 micrOSDevToolKit-1.21.1/micrOS/source/micrOSloader.py
+-rw-r--r--   0 bnm        (501) staff       (20)      183 2023-03-09 19:11:59.000000 micrOSDevToolKit-1.21.1/micrOS/source/reset.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4926 2023-07-17 14:41:23.000000 micrOSDevToolKit-1.21.1/micrOS/source/urequests.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-01 20:08:06.493405 micrOSDevToolKit-1.21.1/micrOSDevToolKit.egg-info/
+-rw-r--r--   0 bnm        (501) staff       (20)    54579 2023-08-01 20:08:06.000000 micrOSDevToolKit-1.21.1/micrOSDevToolKit.egg-info/PKG-INFO
+-rw-r--r--   0 bnm        (501) staff       (20)     8935 2023-08-01 20:08:06.000000 micrOSDevToolKit-1.21.1/micrOSDevToolKit.egg-info/SOURCES.txt
+-rw-r--r--   0 bnm        (501) staff       (20)        1 2023-08-01 20:08:06.000000 micrOSDevToolKit-1.21.1/micrOSDevToolKit.egg-info/dependency_links.txt
+-rw-r--r--   0 bnm        (501) staff       (20)      149 2023-08-01 20:08:06.000000 micrOSDevToolKit-1.21.1/micrOSDevToolKit.egg-info/requires.txt
+-rw-r--r--   0 bnm        (501) staff       (20)       25 2023-08-01 20:08:06.000000 micrOSDevToolKit-1.21.1/micrOSDevToolKit.egg-info/top_level.txt
+-rw-r--r--   0 bnm        (501) staff       (20)       38 2023-08-01 20:08:06.724174 micrOSDevToolKit-1.21.1/setup.cfg
+-rw-r--r--   0 bnm        (501) staff       (20)     1282 2023-08-01 19:35:09.000000 micrOSDevToolKit-1.21.1/setup.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-01 20:08:06.501959 micrOSDevToolKit-1.21.1/toolkit/
+-rw-r--r--   0 bnm        (501) staff       (20)     8377 2023-01-04 20:19:38.000000 micrOSDevToolKit-1.21.1/toolkit/DevEnvCompile.py
+-rw-r--r--   0 bnm        (501) staff       (20)    24453 2023-07-15 18:35:28.000000 micrOSDevToolKit-1.21.1/toolkit/DevEnvOTA.py
+-rw-r--r--   0 bnm        (501) staff       (20)    31441 2023-07-12 17:35:49.000000 micrOSDevToolKit-1.21.1/toolkit/DevEnvUSB.py
+-rw-r--r--   0 bnm        (501) staff       (20)    12307 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.1/toolkit/Gateway.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11615 2023-07-17 15:49:40.000000 micrOSDevToolKit-1.21.1/toolkit/MicrOSDevEnv.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.1/toolkit/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-01 20:08:06.520929 micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/
+-rw-r--r--   0 bnm        (501) staff       (20)      747 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/AirQualityBME280.py
+-rw-r--r--   0 bnm        (501) staff       (20)      749 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/AirQualityDHT22_CO2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1278 2023-01-14 18:12:52.000000 micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/CCTDemo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3798 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/CCTTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1487 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/CatGame.py
+-rw-r--r--   0 bnm        (501) staff       (20)      937 2023-01-16 18:30:18.000000 micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/Dimmer.py
+-rw-r--r--   0 bnm        (501) staff       (20)      542 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/GetVersion.py
+-rw-r--r--   0 bnm        (501) staff       (20)      407 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/MicrophoneTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2409 2023-01-14 15:33:34.000000 micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/NeoEffectsDemo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3938 2023-01-05 18:02:55.000000 micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/NeopixelTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3920 2023-01-05 18:11:07.000000 micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/RGBTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2084 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/RoboArm.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2782 2023-01-05 18:10:36.000000 micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/SED_test.py
+-rw-r--r--   0 bnm        (501) staff       (20)    17600 2023-07-19 10:50:53.000000 micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/SystemTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)      760 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/Template_app.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3901 2023-03-08 10:26:06.000000 micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/_micPlotting.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3380 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/uLightDemo.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-01 20:08:06.527045 micrOSDevToolKit-1.21.1/toolkit/lib/
+-rw-r--r--   0 bnm        (501) staff       (20)    18734 2023-02-07 20:49:31.000000 micrOSDevToolKit-1.21.1/toolkit/lib/LocalMachine.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5421 2023-07-05 11:31:18.000000 micrOSDevToolKit-1.21.1/toolkit/lib/SearchDevices.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6222 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.1/toolkit/lib/SerialDriverHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)      847 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.1/toolkit/lib/TerminalColors.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.1/toolkit/lib/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)    16808 2023-03-15 15:54:40.000000 micrOSDevToolKit-1.21.1/toolkit/lib/micrOSClient.py
+-rw-r--r--   0 bnm        (501) staff       (20)    52184 2023-07-01 21:55:14.000000 micrOSDevToolKit-1.21.1/toolkit/micrOSdashboard.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-01 20:08:06.541894 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/
+-rw-r--r--   0 bnm        (501) staff       (20)     2071 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/LP_darwin.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-01 20:08:06.603010 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/
+-rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      473 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/dotstar.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      483 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/dotstar.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/esp32.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/esp32.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/framebuf.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/framebuf.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     6832 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     7029 2023-07-04 17:16:29.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1124 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1340 2023-03-17 15:56:36.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     2985 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     2991 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/onewire.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/onewire.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1063 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      362 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/simgc.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      471 2023-02-01 12:53:53.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/simgc.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     4799 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     5415 2023-08-01 19:28:24.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/tinypico.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/tinypico.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      976 2022-12-14 21:38:13.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1355 2023-06-27 16:26:11.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1583 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1583 2023-06-27 12:57:10.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      254 2022-12-03 14:47:41.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/webrepl.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      254 2023-01-01 15:36:25.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/webrepl.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)       95 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/dotstar.py
+-rw-r--r--   0 bnm        (501) staff       (20)      193 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/ds18x20.py
+-rw-r--r--   0 bnm        (501) staff       (20)       71 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)       47 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/framebuf.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4430 2023-07-01 22:39:14.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/machine.py
+-rw-r--r--   0 bnm        (501) staff       (20)      909 2023-03-17 15:56:08.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/micropython.py
+-rw-r--r--   0 bnm        (501) staff       (20)      567 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/neopixel.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2490 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/network.py
+-rw-r--r--   0 bnm        (501) staff       (20)      109 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/ntptime.py
+-rw-r--r--   0 bnm        (501) staff       (20)       77 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/onewire.py
+-rw-r--r--   0 bnm        (501) staff       (20)      943 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/sim_console.py
+-rw-r--r--   0 bnm        (501) staff       (20)      140 2023-02-01 12:53:17.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/simgc.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6584 2023-08-01 19:27:35.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/simulator.py
+-rw-r--r--   0 bnm        (501) staff       (20)      156 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/tinypico.py
+-rw-r--r--   0 bnm        (501) staff       (20)      528 2023-06-27 16:23:56.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/uasyncio.py
+-rw-r--r--   0 bnm        (501) staff       (20)      942 2023-06-27 12:56:02.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/utime.py
+-rw-r--r--   0 bnm        (501) staff       (20)       37 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.1/toolkit/simulator_lib/webrepl.py
+-rwxr-xr-x   0 bnm        (501) staff       (20)    16970 2023-07-19 10:36:50.000000 micrOSDevToolKit-1.21.1/toolkit/socketClient.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-01 20:08:06.605101 micrOSDevToolKit-1.21.1/toolkit/user_data/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2023-07-18 21:50:53.000000 micrOSDevToolKit-1.21.1/toolkit/user_data/.include
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-01 20:08:06.605965 micrOSDevToolKit-1.21.1/toolkit/user_data/node_config_archive/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2023-07-18 21:53:27.000000 micrOSDevToolKit-1.21.1/toolkit/user_data/node_config_archive/.include
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-01 20:08:06.606344 micrOSDevToolKit-1.21.1/toolkit/workspace/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-01 20:08:06.719150 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/
+-rw-r--r--   0 bnm        (501) staff       (20)     1791 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/Common.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2996 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/ConfigHandler.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1990 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/Debug.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      759 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/Hooks.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2085 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/InterConnect.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     4174 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/InterpreterShell.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2145 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/InterruptHandler.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      869 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1774 2023-08-01 19:46:43.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_L9110_DCmotor.py
+-rw-r--r--   0 bnm        (501) staff       (20)    10011 2023-08-01 19:46:43.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_VL53L0X.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1297 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_aht10.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     4280 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_bme280.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2604 2023-08-01 19:46:43.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_buzzer.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1647 2023-08-01 19:46:43.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_catgame.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3836 2023-08-01 19:46:43.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_cct.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1359 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_co2.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1952 2023-08-01 19:46:43.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_demo.py
+-rw-r--r--   0 bnm        (501) staff       (20)      793 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_dht11.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      793 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_dht22.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2353 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_dimmer.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2433 2023-08-01 19:46:43.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_distance.py
+-rw-r--r--   0 bnm        (501) staff       (20)      522 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_ds18.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1470 2023-08-01 19:46:43.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1364 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_genIO.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1015 2023-08-01 19:46:43.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_i2c.py
+-rw-r--r--   0 bnm        (501) staff       (20)      616 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_intercon.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      512 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_light_sensor.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1477 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_lmpacman.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2865 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_neoeffects.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3650 2023-08-01 19:46:43.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_neopixel.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_oled.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3203 2023-08-01 19:46:43.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_oled_sh1106.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     6191 2023-08-01 19:46:43.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_oled_ui.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-08-01 19:46:43.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_pet_feeder.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1279 2023-08-01 19:46:43.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_ph_sensor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2558 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_presence.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-08-01 19:46:43.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_rencoder.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3508 2023-08-01 19:46:43.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_rgb.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2946 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_roboarm.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-08-01 19:46:43.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_robustness.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1143 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_servo.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1471 2023-08-01 19:46:43.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_stepper.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2167 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_switch.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2754 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_system.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      872 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_telegram.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1001 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_tinyrgb.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      550 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LP_esp32.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      563 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LP_esp32s2.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      553 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LP_esp32s3.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)       54 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LP_rp2.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      491 2023-08-01 19:46:43.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LP_tinypico.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1348 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LogicalPins.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3400 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/Network.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2900 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/Notify.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1903 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/Scheduler.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3763 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/SocketServer.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     5718 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/TaskManager.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2727 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/Time.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      434 2023-08-01 19:46:43.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/TinyPLed.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      440 2023-08-01 19:46:43.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/main.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1186 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/micrOS.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1730 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/micrOSloader.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      198 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/reset.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1451 2023-08-01 19:46:42.000000 micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/urequests.mpy
```

### Comparing `micrOSDevToolKit-1.21.0/PKG-INFO` & `micrOSDevToolKit-1.21.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micrOSDevToolKit
-Version: 1.21.0
+Version: 1.21.1
 Summary: Development and deployment environment for micrOS, the diy micropython automation OS (IoT)
 Home-page: https://github.com/BxNxM/micrOS
 Author: Marcell Ban
 Author-email: miros.framework@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/BxNxM/micrOS/issues
 Project-URL: GitHub Discussions, https://github.com/BxNxM/micrOS/discussions
```

### Comparing `micrOSDevToolKit-1.21.0/README.md` & `micrOSDevToolKit-1.21.1/README.md`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/devToolKit.py` & `micrOSDevToolKit-1.21.1/devToolKit.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/media/dnd.png` & `micrOSDevToolKit-1.21.1/media/dnd.png`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/media/logo.png` & `micrOSDevToolKit-1.21.1/media/logo.png`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/media/logo_mini.png` & `micrOSDevToolKit-1.21.1/media/logo_mini.png`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/SchedulerUT.py` & `micrOSDevToolKit-1.21.1/micrOS/SchedulerUT.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/micropython/esp32-20220618-v1.19.1.bin` & `micrOSDevToolKit-1.21.1/micrOS/micropython/esp32-20220618-v1.19.1.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/micropython/esp32s2-20220618-v1.19.1.bin` & `micrOSDevToolKit-1.21.1/micrOS/micropython/esp32s2-20220618-v1.19.1.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin` & `micrOSDevToolKit-1.21.1/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2` & `micrOSDevToolKit-1.21.1/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/micropython/tinypico-20220618-v1.19.1.bin` & `micrOSDevToolKit-1.21.1/micrOS/micropython/tinypico-20220618-v1.19.1.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/.DS_Store` & `micrOSDevToolKit-1.21.1/micrOS/source/.DS_Store`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/Common.py` & `micrOSDevToolKit-1.21.1/micrOS/source/Common.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 def transition(from_val, to_val, step_ms, interval_sec):
     """
     [LM] Single Generator for color/value transition:
     :param from_val: from value - start from
     :param to_val: to value - target value
     :param step_ms: step to reach to_val - timirq_seq
-    :param interval_sec: full intervals
+    :param interval_sec: time of full interval
     """
     if interval_sec > 0:
         step_cnt = round((interval_sec*1000)/step_ms)
         delta = abs((from_val-to_val)/step_cnt)
         direc = -1 if from_val > to_val else 1
         for cnt in range(0, step_cnt+1):
             yield round(from_val + (cnt * delta) * direc)
```

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/ConfigHandler.py` & `micrOSDevToolKit-1.21.1/micrOS/source/ConfigHandler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/Debug.py` & `micrOSDevToolKit-1.21.1/micrOS/source/Debug.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,18 +96,21 @@
         except Exception as e:
             errlog_add(f"debug led step error: {e}")
             return False
 
 
 def console_write(msg):
     if DebugCfg.DEBUG:
-        analog = DebugCfg.step()
-        print(msg)
-        if analog:
-            DebugCfg.step()
+        try:
+            analog = DebugCfg.step()
+            print(msg)
+            if analog:
+                DebugCfg.step()
+        except Exception as e:
+            errlog_add(f"[ERR] console_write: {e}")
 
 #############################################
 #        LOGGING WITH DATA ROTATION         #
 #############################################
 
 
 def logger(data, f_name, limit):
```

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/Hooks.py` & `micrOSDevToolKit-1.21.1/micrOS/source/Hooks.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/InterConnect.py` & `micrOSDevToolKit-1.21.1/micrOS/source/InterConnect.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/InterpreterShell.py` & `micrOSDevToolKit-1.21.1/micrOS/source/InterpreterShell.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 #################################################################
 #                  SHELL Interpreter FUNCTIONS                  #
 #################################################################
 
 class Shell:
-    MICROS_VERSION = '1.21.0-0'
+    MICROS_VERSION = '1.21.0-1'
 
     def __init__(self, msg_obj=None):
         """
         comm_obj - communication object - send messages back
                  - comm_obj.reply('msg')
         """
         self.msg_obj = msg_obj
```

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/InterruptHandler.py` & `micrOSDevToolKit-1.21.1/micrOS/source/InterruptHandler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/LM_L298N_DCmotor.py` & `micrOSDevToolKit-1.21.1/micrOS/source/LM_L298N_DCmotor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/LM_L9110_DCmotor.py` & `micrOSDevToolKit-1.21.1/micrOS/source/LM_L9110_DCmotor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/LM_VL53L0X.py` & `micrOSDevToolKit-1.21.1/micrOS/source/LM_VL53L0X.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/LM_bme280.py` & `micrOSDevToolKit-1.21.1/micrOS/source/LM_bme280.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/LM_buzzer.py` & `micrOSDevToolKit-1.21.1/micrOS/source/LM_buzzer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/LM_catgame.py` & `micrOSDevToolKit-1.21.1/micrOS/source/LM_catgame.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/LM_cct.py` & `micrOSDevToolKit-1.21.1/micrOS/source/LM_cct.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/LM_co2.py` & `micrOSDevToolKit-1.21.1/micrOS/source/LM_co2.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/LM_demo.py` & `micrOSDevToolKit-1.21.1/micrOS/source/LM_demo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/LM_dht11.py` & `micrOSDevToolKit-1.21.1/micrOS/source/LM_dht11.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/LM_dht22.py` & `micrOSDevToolKit-1.21.1/micrOS/source/LM_dht22.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/LM_dimmer.py` & `micrOSDevToolKit-1.21.1/micrOS/source/LM_dimmer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/LM_distance.py` & `micrOSDevToolKit-1.21.1/micrOS/source/LM_distance.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/LM_ds18.py` & `micrOSDevToolKit-1.21.1/micrOS/source/LM_ds18.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/LM_esp32.py` & `micrOSDevToolKit-1.21.1/micrOS/source/LM_esp32.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/LM_genIO.py` & `micrOSDevToolKit-1.21.1/micrOS/source/LM_genIO.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/LM_i2c.py` & `micrOSDevToolKit-1.21.1/micrOS/source/LM_i2c.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/LM_intercon.py` & `micrOSDevToolKit-1.21.1/micrOS/source/LM_intercon.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/LM_light_sensor.py` & `micrOSDevToolKit-1.21.1/micrOS/source/LM_light_sensor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/LM_lmpacman.py` & `micrOSDevToolKit-1.21.1/micrOS/source/LM_lmpacman.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/LM_neoeffects.py` & `micrOSDevToolKit-1.21.1/micrOS/source/LM_neoeffects.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/LM_neopixel.py` & `micrOSDevToolKit-1.21.1/micrOS/source/LM_neopixel.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/LM_oled.py` & `micrOSDevToolKit-1.21.1/micrOS/source/LM_oled.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/LM_oled_sh1106.py` & `micrOSDevToolKit-1.21.1/micrOS/source/LM_oled_sh1106.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/LM_oled_ui.py` & `micrOSDevToolKit-1.21.1/micrOS/source/LM_oled_ui.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/LM_pet_feeder.py` & `micrOSDevToolKit-1.21.1/micrOS/source/LM_pet_feeder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/LM_ph_sensor.py` & `micrOSDevToolKit-1.21.1/micrOS/source/LM_ph_sensor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/LM_presence.py` & `micrOSDevToolKit-1.21.1/micrOS/source/LM_presence.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/LM_rencoder.py` & `micrOSDevToolKit-1.21.1/micrOS/source/LM_rencoder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/LM_rgb.py` & `micrOSDevToolKit-1.21.1/micrOS/source/LM_rgb.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/LM_roboarm.py` & `micrOSDevToolKit-1.21.1/micrOS/source/LM_roboarm.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/LM_robustness.py` & `micrOSDevToolKit-1.21.1/micrOS/source/LM_robustness.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/LM_servo.py` & `micrOSDevToolKit-1.21.1/micrOS/source/LM_servo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/LM_stepper.py` & `micrOSDevToolKit-1.21.1/micrOS/source/LM_stepper.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/LM_switch.py` & `micrOSDevToolKit-1.21.1/micrOS/source/LM_switch.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/LM_system.py` & `micrOSDevToolKit-1.21.1/micrOS/source/LM_system.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/LM_telegram.py` & `micrOSDevToolKit-1.21.1/micrOS/source/LM_telegram.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/LM_tinyrgb.py` & `micrOSDevToolKit-1.21.1/micrOS/source/LM_tinyrgb.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/LP_esp32.py` & `micrOSDevToolKit-1.21.1/micrOS/source/LP_esp32.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/LP_esp32s2.py` & `micrOSDevToolKit-1.21.1/micrOS/source/LP_esp32s2.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/LP_esp32s3.py` & `micrOSDevToolKit-1.21.1/micrOS/source/LP_esp32s3.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/LP_tinypico.py` & `micrOSDevToolKit-1.21.1/micrOS/source/LP_tinypico.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/LogicalPins.py` & `micrOSDevToolKit-1.21.1/micrOS/source/LogicalPins.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/Network.py` & `micrOSDevToolKit-1.21.1/micrOS/source/Network.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/Notify.py` & `micrOSDevToolKit-1.21.1/micrOS/source/Notify.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/Scheduler.py` & `micrOSDevToolKit-1.21.1/micrOS/source/Scheduler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/SocketServer.py` & `micrOSDevToolKit-1.21.1/micrOS/source/SocketServer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/TaskManager.py` & `micrOSDevToolKit-1.21.1/micrOS/source/TaskManager.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/Time.py` & `micrOSDevToolKit-1.21.1/micrOS/source/Time.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/TinyPLed.py` & `micrOSDevToolKit-1.21.1/micrOS/source/TinyPLed.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/micrOS.py` & `micrOSDevToolKit-1.21.1/micrOS/source/micrOS.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/micrOSloader.py` & `micrOSDevToolKit-1.21.1/micrOS/source/micrOSloader.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOS/source/urequests.py` & `micrOSDevToolKit-1.21.1/micrOS/source/urequests.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/micrOSDevToolKit.egg-info/PKG-INFO` & `micrOSDevToolKit-1.21.1/micrOSDevToolKit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micrOSDevToolKit
-Version: 1.21.0
+Version: 1.21.1
 Summary: Development and deployment environment for micrOS, the diy micropython automation OS (IoT)
 Home-page: https://github.com/BxNxM/micrOS
 Author: Marcell Ban
 Author-email: miros.framework@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/BxNxM/micrOS/issues
 Project-URL: GitHub Discussions, https://github.com/BxNxM/micrOS/discussions
```

### Comparing `micrOSDevToolKit-1.21.0/micrOSDevToolKit.egg-info/SOURCES.txt` & `micrOSDevToolKit-1.21.1/micrOSDevToolKit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 micrOS/source/Hooks.py
 micrOS/source/InterConnect.py
 micrOS/source/InterpreterShell.py
 micrOS/source/InterruptHandler.py
 micrOS/source/LM_L298N_DCmotor.py
 micrOS/source/LM_L9110_DCmotor.py
 micrOS/source/LM_VL53L0X.py
+micrOS/source/LM_aht10.py
 micrOS/source/LM_bme280.py
 micrOS/source/LM_buzzer.py
 micrOS/source/LM_catgame.py
 micrOS/source/LM_cct.py
 micrOS/source/LM_co2.py
 micrOS/source/LM_demo.py
 micrOS/source/LM_dht11.py
@@ -176,14 +177,15 @@
 toolkit/workspace/precompiled/Hooks.mpy
 toolkit/workspace/precompiled/InterConnect.mpy
 toolkit/workspace/precompiled/InterpreterShell.mpy
 toolkit/workspace/precompiled/InterruptHandler.mpy
 toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy
 toolkit/workspace/precompiled/LM_L9110_DCmotor.py
 toolkit/workspace/precompiled/LM_VL53L0X.py
+toolkit/workspace/precompiled/LM_aht10.mpy
 toolkit/workspace/precompiled/LM_bme280.mpy
 toolkit/workspace/precompiled/LM_buzzer.mpy
 toolkit/workspace/precompiled/LM_catgame.py
 toolkit/workspace/precompiled/LM_cct.mpy
 toolkit/workspace/precompiled/LM_co2.mpy
 toolkit/workspace/precompiled/LM_demo.py
 toolkit/workspace/precompiled/LM_dht11.mpy
```

### Comparing `micrOSDevToolKit-1.21.0/setup.py` & `micrOSDevToolKit-1.21.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # https://towardsdatascience.com/create-your-custom-python-package-that-you-can-pip-install-from-your-git-repository-f90465867893
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='micrOSDevToolKit',
-    version='1.21.0',
+    version='1.21.1',
     author='Marcell Ban',
     author_email='miros.framework@gmail.com',
     description='Development and deployment environment for micrOS, the diy micropython automation OS (IoT)',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/BxNxM/micrOS',
     project_urls={
```

### Comparing `micrOSDevToolKit-1.21.0/toolkit/DevEnvCompile.py` & `micrOSDevToolKit-1.21.1/toolkit/DevEnvCompile.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/DevEnvOTA.py` & `micrOSDevToolKit-1.21.1/toolkit/DevEnvOTA.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/DevEnvUSB.py` & `micrOSDevToolKit-1.21.1/toolkit/DevEnvUSB.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/Gateway.py` & `micrOSDevToolKit-1.21.1/toolkit/Gateway.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/MicrOSDevEnv.py` & `micrOSDevToolKit-1.21.1/toolkit/MicrOSDevEnv.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/AirQualityBME280.py` & `micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/AirQualityBME280.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/AirQualityDHT22_CO2.py` & `micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/AirQualityDHT22_CO2.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/CCTDemo.py` & `micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/CCTDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/CCTTest.py` & `micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/CCTTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/CatGame.py` & `micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/CatGame.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/Dimmer.py` & `micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/Dimmer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/GetVersion.py` & `micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/GetVersion.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/NeoEffectsDemo.py` & `micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/NeoEffectsDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/NeopixelTest.py` & `micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/NeopixelTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/RGBTest.py` & `micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/RGBTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/RoboArm.py` & `micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/RoboArm.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/SED_test.py` & `micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/SED_test.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/SystemTest.py` & `micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/SystemTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/Template_app.py` & `micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/Template_app.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/_micPlotting.py` & `micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/_micPlotting.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/uLightDemo.py` & `micrOSDevToolKit-1.21.1/toolkit/dashboard_apps/uLightDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/lib/LocalMachine.py` & `micrOSDevToolKit-1.21.1/toolkit/lib/LocalMachine.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/lib/SearchDevices.py` & `micrOSDevToolKit-1.21.1/toolkit/lib/SearchDevices.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/lib/SerialDriverHandler.py` & `micrOSDevToolKit-1.21.1/toolkit/lib/SerialDriverHandler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/lib/TerminalColors.py` & `micrOSDevToolKit-1.21.1/toolkit/lib/TerminalColors.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/lib/micrOSClient.py` & `micrOSDevToolKit-1.21.1/toolkit/lib/micrOSClient.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/micrOSdashboard.py` & `micrOSDevToolKit-1.21.1/toolkit/micrOSdashboard.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/LP_darwin.py` & `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/LP_darwin.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc` & `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc` & `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc` & `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc` & `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc` & `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc` & `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc` & `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc` & `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc` & `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc` & `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc` & `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc` & `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc` & `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc` & `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc` & `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc` & `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sat Jul 15 16:13:22 2023 UTC, .py size: 6545 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 a2c5 b264 9119 0000  a..........d....
+00000000: 610d 0d0a 0000 0000 a75c c964 b819 0000  a........\.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 d600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6501 6a05 a006 6507 a101  d.l.Z.e.j...e...
 00000060: 5a08 6501 6a05 a009 6508 6402 a102 5a0a  Z.e.j...e.d...Z.
 00000070: 6500 6a05 a00b 6400 650a a102 0100 6500  e.j...d.e.....e.
@@ -15,324 +15,325 @@
 000000e0: 6408 8301 0100 6503 a014 6409 a101 0100  d.....e...d.....
 000000f0: 6512 a015 a100 0100 6510 a016 a100 0100  e.......e.......
 00000100: 6401 5300 290a e900 0000 004e 7a16 2e2e  d.S.)......Nz...
 00000110: 2f77 6f72 6b73 7061 6365 2f73 696d 756c  /workspace/simul
 00000120: 6174 6f72 7a06 2e2e 2f6c 6962 2901 da07  atorz.../lib)...
 00000130: 636f 6e73 6f6c 6563 0000 0000 0000 0000  consolec........
 00000140: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
-00000150: 7356 0000 0065 005a 0164 005a 0267 005a  sV...e.Z.d.Z.g.Z
-00000160: 0364 1364 0264 0384 015a 0464 0464 0584  .d.d.d...Z.d.d..
-00000170: 005a 0564 0664 0784 005a 0664 0864 0984  .Z.d.d...Z.d.d..
-00000180: 005a 0764 0a64 0b84 005a 0865 0964 0c64  .Z.d.d...Z.e.d.d
-00000190: 0d84 0083 015a 0a64 0e64 0f84 005a 0b64  .....Z.d.d...Z.d
-000001a0: 1064 1184 005a 0c64 1253 0029 14da 086d  .d...Z.d.S.)...m
-000001b0: 6963 724f 5349 4d46 6302 0000 0000 0000  icrOSIMFc.......
-000001c0: 0000 0000 0002 0000 0005 0000 0043 0000  .............C..
-000001d0: 0073 5600 0000 7c01 7214 7400 6401 8301  .sV...|.r.t.d...
-000001e0: 0100 6402 7c00 5f01 6e3e 7400 6403 a002  ..d.|._.n>t.d...
-000001f0: 7403 a004 a100 a101 8301 0100 7400 6404  t...........t.d.
-00000200: 8301 0100 7403 6a05 7c00 6a06 6405 8d01  ....t.j.|.j.d...
-00000210: 7c00 5f07 6400 7c00 5f08 7409 6a0a a00b  |._.d.|._.t.j...
-00000220: 7c00 6a07 a101 0100 6400 5300 2906 4e7a  |.j.....d.S.).Nz
-00000230: 2a5b 6d69 6372 4f53 494d 5d20 4372 6561  *[micrOSIM] Crea
-00000240: 7465 206d 6963 724f 5320 4c4d 2064 6f63  te micrOS LM doc
-00000250: 2028 656e 7620 7072 6f63 2929 024e 4e7a   (env proc)).NNz
-00000260: 235b 6d69 6372 4f53 494d 5d20 494e 464f  #[micrOSIM] INFO
-00000270: 3a20 4e75 6d62 6572 206f 6620 6370 7520  : Number of cpu 
-00000280: 3a20 7b7d 7a2d 5b6d 6963 724f 5349 4d5d  : {}z-[micrOSIM]
-00000290: 2043 7265 6174 6520 6d69 6372 4f53 2073   Create micrOS s
-000002a0: 696d 756c 6174 6f72 2070 726f 6365 7373  imulator process
-000002b0: 2e2e 2ea9 01da 0674 6172 6765 7429 0c72  .......target).r
-000002c0: 0200 0000 da0a 646f 635f 6f75 7470 7574  ......doc_output
-000002d0: da06 666f 726d 6174 da0f 6d75 6c74 6970  ..format..multip
-000002e0: 726f 6365 7373 696e 67da 0963 7075 5f63  rocessing..cpu_c
-000002f0: 6f75 6e74 da07 5072 6f63 6573 73da 116d  ount..Process..m
-00000300: 6963 724f 535f 7369 6d5f 776f 726b 6572  icrOS_sim_worker
-00000310: da07 7072 6f63 6573 73da 0370 6964 7203  ..process..pidr.
-00000320: 0000 00da 1053 494d 5f50 524f 4345 5353  .....SIM_PROCESS
-00000330: 5f4c 4953 54da 0661 7070 656e 6429 02da  _LIST..append)..
-00000340: 0473 656c 66da 0b64 6f63 5f72 6573 6f6c  .self..doc_resol
-00000350: 7665 a900 7212 0000 00fa 3b2f 5573 6572  ve..r.....;/User
-00000360: 732f 626e 6d2f 6d69 6372 4f53 2f6d 6963  s/bnm/micrOS/mic
-00000370: 724f 532f 746f 6f6c 6b69 742f 7369 6d75  rOS/toolkit/simu
-00000380: 6c61 746f 725f 6c69 622f 7369 6d75 6c61  lator_lib/simula
-00000390: 746f 722e 7079 da08 5f5f 696e 6974 5f5f  tor.py..__init__
-000003a0: 1300 0000 7310 0000 0000 0104 0108 0208  ....s...........
-000003b0: 0212 0108 0110 0106 017a 116d 6963 724f  .........z.micrO
-000003c0: 5349 4d2e 5f5f 696e 6974 5f5f 6301 0000  SIM.__init__c...
-000003d0: 0000 0000 0000 0000 0003 0000 0004 0000  ................
-000003e0: 0003 0000 0073 6000 0000 7400 a001 a100  .....s`...t.....
-000003f0: 7d01 7c01 a002 7403 a101 0100 7404 6401  }.|...t.....t.d.
-00000400: a005 7403 a101 8301 0100 7406 a006 a100  ..t.......t.....
-00000410: 8900 8700 6601 6402 6403 8408 7d02 7407  ....f.d.d...}.t.
-00000420: a008 7c02 a101 0100 7409 a00a a100 0100  ..|.....t.......
-00000430: 7404 6404 a005 7403 a101 8301 0100 7c01  t.d...t.......|.
-00000440: a00b a100 0100 6400 5300 2905 4e7a 255b  ......d.S.).Nz%[
-00000450: 6d69 6372 4f53 494d 5d20 5374 6172 7420  micrOSIM] Start 
-00000460: 6d69 6372 4f53 206c 6f61 6465 7220 696e  micrOS loader in
-00000470: 3a20 7b7d 6303 0000 0000 0000 0000 0000  : {}c...........
-00000480: 0007 0000 000e 0000 0013 0000 0073 9000  .............s..
-00000490: 0000 6401 a000 7401 a001 a100 8800 1800  ..d...t.........
-000004a0: a101 7d03 7401 a001 a100 8900 7c00 6a02  ..}.t.......|.j.
-000004b0: 6a03 7d04 7c00 6a04 7d05 7c00 6a02 6a05  j.}.|.j.}.|.j.j.
-000004c0: 7d06 6402 7c04 7600 728c 7c06 6403 6b03  }.d.|.v.r.|.d.k.
-000004d0: 728c 7406 6404 9b00 6405 7c03 9b00 6406  r.t.d...d.|...d.
-000004e0: 7c01 9b00 6407 7c05 9b00 6408 6409 a007  |...d.|...d.d...
-000004f0: 7c04 a008 6409 a101 640a 6400 8502 1900  |...d...d.d.....
-00000500: a101 9b00 640b 7c06 9b00 640c 7c02 7282  ....d.|...d.|.r.
-00000510: 7c02 6e02 640d 9b00 9d0d 8301 0100 6400  |.n.d.........d.
-00000520: 5300 290e 4e7a 067b 3a2e 3265 7d7a 0a73  S.).Nz.{:.2e}z.s
-00000530: 696d 756c 6174 6f72 2f5a 0969 646c 655f  imulator/Z.idle_
-00000540: 7461 736b 7a32 2020 2020 2020 2020 2020  taskz2          
+00000150: 7358 0000 0065 005a 0164 005a 0267 005a  sX...e.Z.d.Z.g.Z
+00000160: 0364 1364 0264 0384 015a 0464 1464 0464  .d.d.d...Z.d.d.d
+00000170: 0584 015a 0564 0664 0784 005a 0664 0864  ...Z.d.d...Z.d.d
+00000180: 0984 005a 0764 0a64 0b84 005a 0865 0964  ...Z.d.d...Z.e.d
+00000190: 0c64 0d84 0083 015a 0a64 0e64 0f84 005a  .d.....Z.d.d...Z
+000001a0: 0b64 1064 1184 005a 0c64 1253 0029 15da  .d.d...Z.d.S.)..
+000001b0: 086d 6963 724f 5349 4d46 6302 0000 0000  .micrOSIMFc.....
+000001c0: 0000 0000 0000 0002 0000 0005 0000 0043  ...............C
+000001d0: 0000 0073 5600 0000 7c01 7214 7400 6401  ...sV...|.r.t.d.
+000001e0: 8301 0100 6402 7c00 5f01 6e3e 7400 6403  ....d.|._.n>t.d.
+000001f0: a002 7403 a004 a100 a101 8301 0100 7400  ..t...........t.
+00000200: 6404 8301 0100 7403 6a05 7c00 6a06 6405  d.....t.j.|.j.d.
+00000210: 8d01 7c00 5f07 6400 7c00 5f08 7409 6a0a  ..|._.d.|._.t.j.
+00000220: a00b 7c00 6a07 a101 0100 6400 5300 2906  ..|.j.....d.S.).
+00000230: 4e7a 2a5b 6d69 6372 4f53 494d 5d20 4372  Nz*[micrOSIM] Cr
+00000240: 6561 7465 206d 6963 724f 5320 4c4d 2064  eate micrOS LM d
+00000250: 6f63 2028 656e 7620 7072 6f63 2929 024e  oc (env proc)).N
+00000260: 4e7a 235b 6d69 6372 4f53 494d 5d20 494e  Nz#[micrOSIM] IN
+00000270: 464f 3a20 4e75 6d62 6572 206f 6620 6370  FO: Number of cp
+00000280: 7520 3a20 7b7d 7a2d 5b6d 6963 724f 5349  u : {}z-[micrOSI
+00000290: 4d5d 2043 7265 6174 6520 6d69 6372 4f53  M] Create micrOS
+000002a0: 2073 696d 756c 6174 6f72 2070 726f 6365   simulator proce
+000002b0: 7373 2e2e 2ea9 01da 0674 6172 6765 7429  ss.......target)
+000002c0: 0c72 0200 0000 da0a 646f 635f 6f75 7470  .r......doc_outp
+000002d0: 7574 da06 666f 726d 6174 da0f 6d75 6c74  ut..format..mult
+000002e0: 6970 726f 6365 7373 696e 67da 0963 7075  iprocessing..cpu
+000002f0: 5f63 6f75 6e74 da07 5072 6f63 6573 73da  _count..Process.
+00000300: 116d 6963 724f 535f 7369 6d5f 776f 726b  .micrOS_sim_work
+00000310: 6572 da07 7072 6f63 6573 73da 0370 6964  er..process..pid
+00000320: 7203 0000 00da 1053 494d 5f50 524f 4345  r......SIM_PROCE
+00000330: 5353 5f4c 4953 54da 0661 7070 656e 6429  SS_LIST..append)
+00000340: 02da 0473 656c 66da 0b64 6f63 5f72 6573  ...self..doc_res
+00000350: 6f6c 7665 a900 7212 0000 00fa 3b2f 5573  olve..r.....;/Us
+00000360: 6572 732f 626e 6d2f 6d69 6372 4f53 2f6d  ers/bnm/micrOS/m
+00000370: 6963 724f 532f 746f 6f6c 6b69 742f 7369  icrOS/toolkit/si
+00000380: 6d75 6c61 746f 725f 6c69 622f 7369 6d75  mulator_lib/simu
+00000390: 6c61 746f 722e 7079 da08 5f5f 696e 6974  lator.py..__init
+000003a0: 5f5f 1300 0000 7310 0000 0000 0104 0108  __....s.........
+000003b0: 0208 0212 0108 0110 0106 017a 116d 6963  ...........z.mic
+000003c0: 724f 5349 4d2e 5f5f 696e 6974 5f5f 6302  rOSIM.__init__c.
+000003d0: 0000 0000 0000 0000 0000 0004 0000 0004  ................
+000003e0: 0000 0003 0000 0073 6400 0000 7400 a001  .......sd...t...
+000003f0: a100 7d02 7c02 a002 7403 a101 0100 7404  ..}.|...t.....t.
+00000400: 6401 a005 7403 a101 8301 0100 7406 a006  d...t.......t...
+00000410: a100 8900 8700 6601 6402 6403 8408 7d03  ......f.d.d...}.
+00000420: 7c01 7242 7407 a008 7c03 a101 0100 7409  |.rBt...|.....t.
+00000430: a00a a100 0100 7404 6404 a005 7403 a101  ......t.d...t...
+00000440: 8301 0100 7c02 a00b a100 0100 6400 5300  ....|.......d.S.
+00000450: 2905 4e7a 255b 6d69 6372 4f53 494d 5d20  ).Nz%[micrOSIM] 
+00000460: 5374 6172 7420 6d69 6372 4f53 206c 6f61  Start micrOS loa
+00000470: 6465 7220 696e 3a20 7b7d 6303 0000 0000  der in: {}c.....
+00000480: 0000 0000 0000 0007 0000 000e 0000 0013  ................
+00000490: 0000 0073 9000 0000 6401 a000 7401 a001  ...s....d...t...
+000004a0: a100 8800 1800 a101 7d03 7401 a001 a100  ........}.t.....
+000004b0: 8900 7c00 6a02 6a03 7d04 7c00 6a04 7d05  ..|.j.j.}.|.j.}.
+000004c0: 7c00 6a02 6a05 7d06 6402 7c04 7600 728c  |.j.j.}.d.|.v.r.
+000004d0: 7c06 6403 6b03 728c 7406 6404 9b00 6405  |.d.k.r.t.d...d.
+000004e0: 7c03 9b00 6406 7c01 9b00 6407 7c05 9b00  |...d.|...d.|...
+000004f0: 6408 6409 a007 7c04 a008 6409 a101 640a  d.d...|...d...d.
+00000500: 6400 8502 1900 a101 9b00 640b 7c06 9b00  d.........d.|...
+00000510: 640c 7c02 7282 7c02 6e02 640d 9b00 9d0d  d.|.r.|.n.d.....
+00000520: 8301 0100 6400 5300 290e 4e7a 067b 3a2e  ....d.S.).Nz.{:.
+00000530: 3265 7d7a 0a73 696d 756c 6174 6f72 2f5a  2e}z.simulator/Z
+00000540: 0969 646c 655f 7461 736b 7a32 2020 2020  .idle_taskz2    
 00000550: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000570: 2020 2020 2020 2020 7a08 5b74 7261 6365          z.[trace
-00000580: 5d5b 7a03 735d 5b7a 025d 207a 023a 20fa  ][z.s][z.] z.: .
-00000590: 012f e9ff ffff ffda 012e fa01 20da 0029  ./.......... ..)
-000005a0: 0972 0700 0000 da04 7469 6d65 da06 665f  .r......time..f_
-000005b0: 636f 6465 da0b 636f 5f66 696c 656e 616d  code..co_filenam
-000005c0: 65da 0866 5f6c 696e 656e 6fda 0763 6f5f  e..f_lineno..co_
-000005d0: 6e61 6d65 da05 7072 696e 74da 046a 6f69  name..print..joi
-000005e0: 6eda 0573 706c 6974 2907 da05 6672 616d  n..split)...fram
-000005f0: 65da 0565 7665 6e74 da03 6172 67da 0c65  e..event..arg..e
-00000600: 6c61 7073 6564 5f74 696d 65da 0466 696c  lapsed_time..fil
-00000610: 65da 046c 696e 65da 0463 6f64 65a9 015a  e..line..code..Z
-00000620: 0670 7265 765f 7472 1200 0000 7213 0000  .prev_tr....r...
-00000630: 00da 0a74 7261 6365 5f66 756e 6325 0000  ...trace_func%..
-00000640: 0073 0e00 0000 0002 1201 0801 0801 0601  .s..............
-00000650: 0801 1001 7a2e 6d69 6372 4f53 494d 2e6d  ....z.micrOSIM.m
-00000660: 6963 724f 535f 7369 6d5f 776f 726b 6572  icrOS_sim_worker
-00000670: 2e3c 6c6f 6361 6c73 3e2e 7472 6163 655f  .<locals>.trace_
-00000680: 6675 6e63 7a1b 5b6d 6963 724f 5349 4d5d  funcz.[micrOSIM]
-00000690: 2053 746f 7020 6d69 6372 4f53 2028 7b7d   Stop micrOS ({}
-000006a0: 2929 0cda 0c4c 6f63 616c 4d61 6368 696e  ))...LocalMachin
-000006b0: 65da 0e53 696d 706c 6550 6f70 5075 7368  e..SimplePopPush
-000006c0: 64da 0570 7573 6864 da08 5349 4d5f 5041  d..pushd..SIM_PA
-000006d0: 5448 7202 0000 0072 0700 0000 721a 0000  THr....r....r...
-000006e0: 00da 0373 7973 da08 7365 7474 7261 6365  ...sys..settrace
-000006f0: da0c 6d69 6372 4f53 6c6f 6164 6572 da04  ..micrOSloader..
-00000700: 6d61 696e da04 706f 7064 2903 7210 0000  main..popd).r...
-00000710: 005a 0873 696d 5f70 6174 6872 2a00 0000  .Z.sim_pathr*...
-00000720: 7212 0000 0072 2900 0000 7213 0000 0072  r....r)...r....r
-00000730: 0b00 0000 1f00 0000 7312 0000 0000 0108  ........s.......
-00000740: 010a 010e 0108 020c 0b0a 0108 020e 017a  ...............z
-00000750: 1a6d 6963 724f 5349 4d2e 6d69 6372 4f53  .micrOSIM.micrOS
-00000760: 5f73 696d 5f77 6f72 6b65 7263 0100 0000  _sim_workerc....
-00000770: 0000 0000 0000 0000 0200 0000 0a00 0000  ................
-00000780: 4300 0000 7340 0000 007a 0e7c 006a 00a0  C...s@...z.|.j..
-00000790: 01a1 0001 0057 006e 2c04 0074 0279 3a01  .....W.n,..t.y:.
-000007a0: 007d 0101 007a 1474 037c 0183 0101 0057  .}...z.t.|.....W
-000007b0: 0059 0064 007d 017e 016e 0a64 007d 017e  .Y.d.}.~.n.d.}.~
-000007c0: 0130 0030 0064 0053 0029 014e 2904 720c  .0.0.d.S.).N).r.
-000007d0: 0000 0072 2000 0000 da09 4578 6365 7074  ...r .....Except
-000007e0: 696f 6e72 0200 0000 2902 7210 0000 00da  ionr....).r.....
-000007f0: 0165 7212 0000 0072 1200 0000 7213 0000  .er....r....r...
-00000800: 00da 0c77 6169 745f 7072 6f63 6573 7336  ...wait_process6
-00000810: 0000 0073 0800 0000 0001 0201 0e01 0e01  ...s............
-00000820: 7a15 6d69 6372 4f53 494d 2e77 6169 745f  z.micrOSIM.wait_
-00000830: 7072 6f63 6573 7363 0100 0000 0000 0000  processc........
-00000840: 0000 0000 0100 0000 0400 0000 4300 0000  ............C...
-00000850: 7330 0000 0074 0064 0183 0101 007c 006a  s0...t.d.....|.j
-00000860: 01a0 02a1 0001 007c 006a 016a 037c 005f  .......|.j.j.|._
-00000870: 0374 0064 02a0 047c 006a 03a1 0183 0101  .t.d...|.j......
-00000880: 0064 0053 0029 034e 7a29 5b6d 6963 724f  .d.S.).Nz)[micrO
-00000890: 5349 4d5d 2053 7461 7274 206d 6963 724f  SIM] Start micrO
-000008a0: 5320 7369 6d75 6c61 746f 7220 7072 6f63  S simulator proc
-000008b0: 6573 737a 295b 6d69 6372 4f53 494d 5d20  essz)[micrOSIM] 
-000008c0: 6d69 6372 4f53 2070 726f 6365 7373 2077  micrOS process w
-000008d0: 6173 2073 7461 7274 6564 3a20 7b7d 2905  as started: {}).
-000008e0: 7202 0000 0072 0c00 0000 da05 7374 6172  r....r......star
-000008f0: 7472 0d00 0000 7207 0000 00a9 0172 1000  tr....r......r..
-00000900: 0000 7212 0000 0072 1200 0000 7213 0000  ..r....r....r...
-00000910: 0072 3700 0000 3c00 0000 7308 0000 0000  .r7...<...s.....
-00000920: 0108 010a 010a 017a 0e6d 6963 724f 5349  .......z.micrOSI
-00000930: 4d2e 7374 6172 7463 0100 0000 0000 0000  M.startc........
-00000940: 0000 0000 0100 0000 0400 0000 4300 0000  ............C...
-00000950: 7358 0000 007c 006a 00a0 01a1 0072 3a7c  sX...|.j.....r:|
-00000960: 006a 00a0 02a1 0001 007c 006a 00a0 01a1  .j.......|.j....
-00000970: 0072 3a74 0364 01a0 047c 006a 05a1 0183  .r:t.d...|.j....
-00000980: 0101 0074 06a0 0764 02a1 0101 0071 147c  ...t...d.....q.|
-00000990: 006a 00a0 08a1 0001 0074 0364 03a0 047c  .j.......t.d...|
-000009a0: 006a 05a1 0183 0101 0064 0053 0029 044e  .j.......d.S.).N
-000009b0: 7a28 5b6d 6963 724f 5349 4d5d 2057 6169  z([micrOSIM] Wai
-000009c0: 7420 7072 6f63 6573 7320 746f 2074 6572  t process to ter
-000009d0: 6d69 6e61 7465 3a20 7b7d e901 0000 007a  minate: {}.....z
-000009e0: 205b 6d69 6372 4f53 494d 5d20 5072 6f63   [micrOSIM] Proc
-000009f0: 2077 6173 2066 696e 6973 6865 643a 207b   was finished: {
-00000a00: 7d29 0972 0c00 0000 da08 6973 5f61 6c69  }).r......is_ali
-00000a10: 7665 da09 7465 726d 696e 6174 6572 0200  ve..terminater..
-00000a20: 0000 7207 0000 0072 0d00 0000 721a 0000  ..r....r....r...
-00000a30: 00da 0573 6c65 6570 da05 636c 6f73 6572  ...sleep..closer
-00000a40: 3800 0000 7212 0000 0072 1200 0000 7213  8...r....r....r.
-00000a50: 0000 0072 3b00 0000 4200 0000 730e 0000  ...r;...B...s...
-00000a60: 0000 010a 010a 010a 0110 010c 010a 017a  ...............z
-00000a70: 126d 6963 724f 5349 4d2e 7465 726d 696e  .micrOSIM.termin
-00000a80: 6174 6563 0000 0000 0000 0000 0000 0000  atec............
-00000a90: 0500 0000 0b00 0000 4300 0000 73be 0000  ........C...s...
-00000aa0: 0074 006a 017d 0074 027c 0083 017d 0174  .t.j.}.t.|...}.t
-00000ab0: 037c 0083 0144 005d 9c5c 027d 027d 037a  .|...D.].\.}.}.z
-00000ac0: 447c 03a0 04a1 0072 587c 03a0 05a1 0001  D|.....rX|......
-00000ad0: 007c 03a0 04a1 0072 5874 0664 01a0 077c  .|.....rXt.d...|
-00000ae0: 0264 0217 007c 01a1 0283 0101 0074 08a0  .d...|.......t..
-00000af0: 0964 02a1 0101 0071 307c 03a0 0aa1 0001  .d.....q0|......
-00000b00: 0057 006e 3a04 0074 0b79 9c01 007d 0401  .W.n:..t.y...}..
-00000b10: 007a 2274 0664 03a0 077c 0264 0217 007c  .z"t.d...|.d...|
-00000b20: 017c 04a1 0383 0101 0057 0059 0064 007d  .|.......W.Y.d.}
-00000b30: 047e 046e 0a64 007d 047e 0430 0030 0074  .~.n.d.}.~.0.0.t
-00000b40: 0664 04a0 077c 0264 0217 007c 01a1 0283  .d...|.d...|....
-00000b50: 0101 0071 1667 0074 005f 0164 0053 0029  ...q.g.t._.d.S.)
-00000b60: 054e 7a2b 5b6d 6963 724f 5349 4d5d 2057  .Nz+[micrOSIM] W
-00000b70: 6169 7420 7072 6f63 6573 7320 746f 2074  ait process to t
-00000b80: 6572 6d69 6e61 7465 3a20 7b7d 2f7b 7d72  erminate: {}/{}r
-00000b90: 3900 0000 7a2a 5b6d 6963 724f 5349 4d5d  9...z*[micrOSIM]
-00000ba0: 2050 726f 6320 616c 7265 6164 7920 7374   Proc already st
-00000bb0: 6f70 7065 643a 207b 7d2f 7b7d 3a20 7b7d  opped: {}/{}: {}
-00000bc0: 7a23 5b6d 6963 724f 5349 4d5d 2050 726f  z#[micrOSIM] Pro
-00000bd0: 6320 7761 7320 6669 6e69 7368 6564 3a20  c was finished: 
-00000be0: 7b7d 2f7b 7d29 0c72 0300 0000 720e 0000  {}/{}).r....r...
-00000bf0: 00da 036c 656e da09 656e 756d 6572 6174  ...len..enumerat
-00000c00: 6572 3a00 0000 723b 0000 0072 0200 0000  er:...r;...r....
-00000c10: 7207 0000 0072 1a00 0000 723c 0000 0072  r....r....r<...r
-00000c20: 3d00 0000 7234 0000 0029 055a 0970 726f  =...r4...).Z.pro
-00000c30: 635f 6c69 7374 5a08 7072 6f63 5f6c 656e  c_listZ.proc_len
-00000c40: da01 69da 0470 726f 6372 3500 0000 7212  ..i..procr5...r.
-00000c50: 0000 0072 1200 0000 7213 0000 00da 0873  ...r....r......s
-00000c60: 746f 705f 616c 6c4b 0000 0073 1c00 0000  top_allK...s....
-00000c70: 0002 0601 0801 1001 0201 0801 0801 0801  ................
-00000c80: 1401 0c01 0c01 0e01 2c01 1601 7a11 6d69  ........,...z.mi
-00000c90: 6372 4f53 494d 2e73 746f 705f 616c 6c63  crOSIM.stop_allc
-00000ca0: 0200 0000 0000 0000 0000 0000 0c00 0000  ................
-00000cb0: 0c00 0000 4300 0000 73e6 0100 0074 00a0  ....C...s....t..
-00000cc0: 017c 01a1 017d 0274 02a0 03a1 007d 037c  .|...}.t.....}.|
-00000cd0: 03a0 0474 05a1 0101 007c 01a0 06a1 0044  ...t.....|.....D
-00000ce0: 0090 015d a85c 027d 047d 057c 017c 0419  ...].\.}.}.|.|..
-00000cf0: 0064 0119 007d 0664 027c 069b 0064 037c  .d...}.d.|...d.|
-00000d00: 049b 0064 049d 057c 027c 0419 0064 013c  ...d...|.|...d.<
-00000d10: 007c 0544 0090 015d 727d 0774 077c 017c  .|.D...]r}.t.|.|
-00000d20: 0419 007c 0719 0074 0883 0273 7271 5874  ...|...t...srqXt
-00000d30: 0964 057c 049b 0064 067c 079b 0064 079d  .d.|...d.|...d..
-00000d40: 0583 0101 007a 9474 0a64 087c 049b 009d  .....z.t.d.|....
-00000d50: 0283 0101 0074 0b64 097c 049b 0064 067c  .....t.d.|...d.|
-00000d60: 079b 0064 079d 0583 017d 087c 0764 0a6b  ...d.....}.|.d.k
-00000d70: 0290 0172 1a74 0964 0b7c 049b 0064 0c9d  ...r.t.d.|...d..
-00000d80: 0383 0101 007a 3874 0b64 097c 049b 0064  .....z8t.d.|...d
-00000d90: 0c9d 0383 017d 097c 0964 0d75 0172 fe64  .....}.|.d.u.r.d
-00000da0: 0ea0 0c74 087c 0983 01a0 0da1 00a1 017d  ...t.|.........}
-00000db0: 0964 0f7c 099b 009d 027d 0957 006e 1001  .d.|.....}.W.n..
-00000dc0: 0001 0001 0064 107d 0959 006e 0230 007c  .....d.}.Y.n.0.|
-00000dd0: 087c 0937 007d 0857 006e 2e04 0074 0e90  .|.7.}.W.n...t..
-00000de0: 0179 4a01 007d 0a01 007a 1474 0f7c 0a83  .yJ..}...z.t.|..
-00000df0: 017d 0857 0059 0064 0d7d 0a7e 0a6e 0a64  .}.W.Y.d.}.~.n.d
-00000e00: 0d7d 0a7e 0a30 0030 007c 087c 017c 0419  .}.~.0.0.|.|.|..
-00000e10: 007c 0719 0064 113c 007c 0864 0d75 0090  .|...d.<.|.d.u..
-00000e20: 0172 6a64 126e 167c 08a0 10a1 00a0 1164  .rjd.n.|.......d
-00000e30: 1364 14a1 02a0 1164 1564 16a1 027c 027c  .d.....d.d...|.|
-00000e40: 0419 007c 0719 0064 113c 007c 027c 0419  ...|...d.<.|.|..
-00000e50: 007c 0719 00a0 1264 1764 0da1 027d 0b7c  .|.....d.d...}.|
-00000e60: 0b64 0d75 0172 5874 137c 0ba0 10a1 0083  .d.u.rXt.|......
-00000e70: 0164 186b 0272 587c 027c 0419 007c 0719  .d.k.rX|.|...|..
-00000e80: 00a0 1464 17a1 0101 0071 5871 247c 03a0  ...d.....qXq$|..
-00000e90: 15a1 0001 007c 017c 0266 027c 005f 1664  .....|.|.f.|._.d
-00000ea0: 0d53 0029 197a bd0a 2020 2020 2020 2020  .S.).z..        
-00000eb0: 436f 6c6c 6563 7420 6675 6e63 7469 6f6e  Collect function
-00000ec0: 2064 6f63 2073 7472 696e 6773 2061 6e64   doc strings and
-00000ed0: 206d 6f64 756c 6520 6c6f 6769 6361 6c20   module logical 
-00000ee0: 7069 6e73 2028 7069 6e20 6d61 7029 0a20  pins (pin map). 
-00000ef0: 2020 2020 2020 2043 7265 6174 6520 3220         Create 2 
-00000f00: 6469 6374 2073 7472 7563 7475 7265 7320  dict structures 
-00000f10: 6164 6469 6e67 2064 6f63 7374 7269 6e67  adding docstring
-00000f20: 0a20 2020 2020 2020 202d 2068 746d 6c20  .        - html 
-00000f30: 6861 636b 2073 7472 7563 7475 7265 0a20  hack structure. 
-00000f40: 2020 2020 2020 202d 206a 736f 6e20 7261         - json ra
-00000f50: 7720 7374 7275 6374 7572 650a 2020 2020  w structure.    
-00000f60: 2020 2020 da03 696d 677a 0a3c 696d 6720      ..imgz.<img 
-00000f70: 7372 633d 227a 0722 2061 6c74 3d22 7a0d  src="z." alt="z.
-00000f80: 2220 6865 6967 6874 3d31 3530 3e7a 1f5b  " height=150>z.[
-00000f90: 6d69 6372 4f53 494d 5d5b 4578 7472 6163  micrOSIM][Extrac
-00000fa0: 7420 646f 632d 7374 725d 204c 4d5f 7217  t doc-str] LM_r.
-00000fb0: 0000 007a 082e 5f5f 646f 635f 5f7a 0a69  ...z..__doc__z.i
-00000fc0: 6d70 6f72 7420 4c4d 5fda 034c 4d5f 5a06  mport LM_..LM_Z.
-00000fd0: 7069 6e6d 6170 7a26 5b6d 6963 724f 5349  pinmapz&[micrOSI
-00000fe0: 4d5d 5b45 7874 7261 6374 2070 696e 206d  M][Extract pin m
-00000ff0: 6170 2074 6f6b 656e 735d 204c 4d5f 7a09  ap tokens] LM_z.
-00001000: 2e70 696e 6d61 7028 294e 7a02 2c20 7a0a  .pinmap()Nz., z.
-00001010: 0a70 696e 206d 6170 3a20 7219 0000 00da  .pin map: r.....
-00001020: 0364 6f63 7a17 4e6f 2064 6f63 2073 7472  .docz.No doc str
-00001030: 696e 6720 6176 6169 6c61 626c 65da 010a  ing available...
-00001040: 7a05 3c62 723e 0a72 1800 0000 7a06 266e  z.<br>.r....z.&n
-00001050: 6273 703b 7a08 7061 7261 6d28 7329 7201  bsp;z.param(s)r.
-00001060: 0000 0029 17da 0463 6f70 79da 0864 6565  ...)...copy..dee
-00001070: 7063 6f70 7972 2b00 0000 722c 0000 0072  pcopyr+...r,...r
-00001080: 2d00 0000 722e 0000 00da 0569 7465 6d73  -...r......items
-00001090: da0a 6973 696e 7374 616e 6365 da04 6469  ..isinstance..di
-000010a0: 6374 7202 0000 00da 0465 7865 63da 0465  ctr......exec..e
-000010b0: 7661 6c72 2000 0000 da04 6b65 7973 7234  valr .....keysr4
-000010c0: 0000 00da 0373 7472 da05 7374 7269 70da  .....str..strip.
-000010d0: 0772 6570 6c61 6365 da03 6765 7472 3e00  .replace..getr>.
-000010e0: 0000 da03 706f 7072 3300 0000 7206 0000  ....popr3...r...
-000010f0: 0029 0c72 1000 0000 da09 7374 7275 6374  .).r......struct
-00001100: 7572 655a 1173 7472 7563 7475 7265 5f74  ureZ.structure_t
-00001110: 6f5f 6874 6d6c 7233 0000 00da 036d 6f64  o_htmlr3.....mod
-00001120: 5a09 6675 6e63 5f64 6963 745a 0769 6d67  Z.func_dictZ.img
-00001130: 5f75 726c da04 6675 6e63 5a07 646f 635f  _url..funcZ.doc_
-00001140: 7374 725a 0a6d 6f64 5f70 696e 6d61 7072  strZ.mod_pinmapr
-00001150: 3500 0000 5a0a 7061 7261 6d5f 6365 6c6c  5...Z.param_cell
-00001160: 7212 0000 0072 1200 0000 7213 0000 00da  r....r....r.....
-00001170: 0f5f 6c6d 5f64 6f63 5f73 7472 696e 6773  ._lm_doc_strings
-00001180: 5c00 0000 7348 0000 0000 070a 0308 010a  \...sH..........
-00001190: 0312 020c 011a 020a 0212 0102 0316 0102  ................
-000011a0: 020e 0116 020a 0210 0102 0110 0108 0112  ................
-000011b0: 010e 0106 010a 020c 0110 011e 0210 0116  ................
-000011c0: 0104 ff04 0104 ff10 0314 0118 0116 0308  ................
-000011d0: 017a 186d 6963 724f 5349 4d2e 5f6c 6d5f  .z.micrOSIM._lm_
-000011e0: 646f 635f 7374 7269 6e67 7363 0200 0000  doc_stringsc....
-000011f0: 0000 0000 0000 0000 0400 0000 0a00 0000  ................
-00001200: 4300 0000 7366 0000 007a 2e74 006a 017c  C...sf...z.t.j.|
-00001210: 00a0 027c 01a1 0164 018d 017d 027c 02a0  ...|...d...}.|..
-00001220: 03a1 0072 2874 04a0 0564 02a1 0101 0071  ...r(t...d.....q
-00001230: 147c 006a 0657 0053 0004 0074 0779 6001  .|.j.W.S...t.y`.
-00001240: 007d 0301 007a 1a74 0864 03a0 097c 03a1  .}...z.t.d...|..
-00001250: 0183 0101 0057 0059 0064 007d 037e 036e  .....W.Y.d.}.~.n
-00001260: 0a64 007d 037e 0330 0030 0064 0053 0029  .d.}.~.0.0.d.S.)
-00001270: 044e 7204 0000 0067 9a99 9999 9999 b93f  .Nr....g.......?
-00001280: 7a42 5b6d 6963 724f 5349 4d5d 5b44 4f43  zB[micrOSIM][DOC
-00001290: 2045 5252 5d20 446f 6320 6765 6e65 7261   ERR] Doc genera
-000012a0: 7469 6f6e 2065 7272 6f72 3a20 6765 6e5f  tion error: gen_
-000012b0: 6c6d 5f64 6f63 5f6a 736f 6e5f 6874 6d6c  lm_doc_json_html
-000012c0: 3a20 7b7d 290a 7208 0000 0072 0a00 0000  : {}).r....r....
-000012d0: 7257 0000 0072 3a00 0000 721a 0000 0072  rW...r:...r....r
-000012e0: 3c00 0000 7206 0000 0072 3400 0000 7202  <...r....r4...r.
-000012f0: 0000 0072 0700 0000 2904 7210 0000 0072  ...r....).r....r
-00001300: 5400 0000 7241 0000 0072 3500 0000 7212  T...rA...r5...r.
-00001310: 0000 0072 1200 0000 7213 0000 00da 1467  ...r....r......g
-00001320: 656e 5f6c 6d5f 646f 635f 6a73 6f6e 5f68  en_lm_doc_json_h
-00001330: 746d 6c96 0000 0073 1000 0000 0001 0201  tml....s........
-00001340: 1201 0801 0c01 0801 0e01 2401 7a1d 6d69  ..........$.z.mi
-00001350: 6372 4f53 494d 2e67 656e 5f6c 6d5f 646f  crOSIM.gen_lm_do
-00001360: 635f 6a73 6f6e 5f68 746d 6c4e 2901 4629  c_json_htmlN).F)
-00001370: 0dda 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-00001380: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-00001390: 616d 655f 5f72 0e00 0000 7214 0000 0072  ame__r....r....r
-000013a0: 0b00 0000 7236 0000 0072 3700 0000 723b  ....r6...r7...r;
-000013b0: 0000 00da 0c73 7461 7469 636d 6574 686f  .....staticmetho
-000013c0: 6472 4200 0000 7257 0000 0072 5800 0000  drB...rW...rX...
-000013d0: 7212 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
-000013e0: 1300 0000 7203 0000 0010 0000 0073 1400  ....r........s..
-000013f0: 0000 0801 0402 0a0c 0817 0806 0806 0809  ................
-00001400: 0201 0a10 083a 7203 0000 00da 085f 5f6d  .....:r......__m
-00001410: 6169 6e5f 5f7a 1c54 6573 7420 6d6f 6465  ain__z.Test mode
-00001420: 202d 2053 746f 7020 6166 7465 7220 3320   - Stop after 3 
-00001430: 7365 63e9 0300 0000 2917 722f 0000 00da  sec.....).r/....
-00001440: 026f 7372 0800 0000 721a 0000 0072 4700  .osr....r....rG.
-00001450: 0000 da04 7061 7468 da07 6469 726e 616d  ....path..dirnam
-00001460: 65da 085f 5f66 696c 655f 5fda 064d 5950  e..__file__..MYP
-00001470: 4154 4872 2000 0000 722e 0000 00da 0669  ATHr ...r......i
-00001480: 6e73 6572 745a 0b73 696d 5f63 6f6e 736f  nsertZ.sim_conso
-00001490: 6c65 7202 0000 0072 3100 0000 722b 0000  ler....r1...r+..
-000014a0: 0072 0300 0000 7259 0000 00da 0373 696d  .r....rY.....sim
-000014b0: 7237 0000 0072 3c00 0000 723b 0000 0072  r7...r<...r;...r
-000014c0: 4200 0000 7212 0000 0072 1200 0000 7212  B...r....r....r.
-000014d0: 0000 0072 1300 0000 da08 3c6d 6f64 756c  ...r......<modul
-000014e0: 653e 0100 0000 732a 0000 0008 0108 0108  e>....s*........
-000014f0: 0108 0108 020c 010e 010e 0118 010c 0108  ................
-00001500: 0108 030e 7f00 1208 0106 0108 0108 0108  ................
-00001510: 010a 0108 01                             .....
+00000570: 2020 2020 2020 2020 2020 2020 2020 7a08                z.
+00000580: 5b74 7261 6365 5d5b 7a03 735d 5b7a 025d  [trace][z.s][z.]
+00000590: 207a 023a 20fa 012f e9ff ffff ffda 012e   z.: ../........
+000005a0: fa01 20da 0029 0972 0700 0000 da04 7469  .. ..).r......ti
+000005b0: 6d65 da06 665f 636f 6465 da0b 636f 5f66  me..f_code..co_f
+000005c0: 696c 656e 616d 65da 0866 5f6c 696e 656e  ilename..f_linen
+000005d0: 6fda 0763 6f5f 6e61 6d65 da05 7072 696e  o..co_name..prin
+000005e0: 74da 046a 6f69 6eda 0573 706c 6974 2907  t..join..split).
+000005f0: da05 6672 616d 65da 0565 7665 6e74 da03  ..frame..event..
+00000600: 6172 67da 0c65 6c61 7073 6564 5f74 696d  arg..elapsed_tim
+00000610: 65da 0466 696c 65da 046c 696e 65da 0463  e..file..line..c
+00000620: 6f64 65a9 015a 0670 7265 765f 7472 1200  ode..Z.prev_tr..
+00000630: 0000 7213 0000 00da 0a74 7261 6365 5f66  ..r......trace_f
+00000640: 756e 6325 0000 0073 0e00 0000 0002 1201  unc%...s........
+00000650: 0801 0801 0601 0801 1001 7a2e 6d69 6372  ..........z.micr
+00000660: 4f53 494d 2e6d 6963 724f 535f 7369 6d5f  OSIM.micrOS_sim_
+00000670: 776f 726b 6572 2e3c 6c6f 6361 6c73 3e2e  worker.<locals>.
+00000680: 7472 6163 655f 6675 6e63 7a1b 5b6d 6963  trace_funcz.[mic
+00000690: 724f 5349 4d5d 2053 746f 7020 6d69 6372  rOSIM] Stop micr
+000006a0: 4f53 2028 7b7d 2929 0cda 0c4c 6f63 616c  OS ({}))...Local
+000006b0: 4d61 6368 696e 65da 0e53 696d 706c 6550  Machine..SimpleP
+000006c0: 6f70 5075 7368 64da 0570 7573 6864 da08  opPushd..pushd..
+000006d0: 5349 4d5f 5041 5448 7202 0000 0072 0700  SIM_PATHr....r..
+000006e0: 0000 721a 0000 00da 0373 7973 da08 7365  ..r......sys..se
+000006f0: 7474 7261 6365 da0c 6d69 6372 4f53 6c6f  ttrace..micrOSlo
+00000700: 6164 6572 da04 6d61 696e da04 706f 7064  ader..main..popd
+00000710: 2904 7210 0000 00da 0574 7261 6365 5a08  ).r......traceZ.
+00000720: 7369 6d5f 7061 7468 722a 0000 0072 1200  sim_pathr*...r..
+00000730: 0000 7229 0000 0072 1300 0000 720b 0000  ..r)...r....r...
+00000740: 001f 0000 0073 1400 0000 0001 0801 0a01  .....s..........
+00000750: 0e01 0802 0c0a 0402 0a01 0802 0e01 7a1a  ..............z.
+00000760: 6d69 6372 4f53 494d 2e6d 6963 724f 535f  micrOSIM.micrOS_
+00000770: 7369 6d5f 776f 726b 6572 6301 0000 0000  sim_workerc.....
+00000780: 0000 0000 0000 0002 0000 000a 0000 0043  ...............C
+00000790: 0000 0073 4000 0000 7a0e 7c00 6a00 a001  ...s@...z.|.j...
+000007a0: a100 0100 5700 6e2c 0400 7402 793a 0100  ....W.n,..t.y:..
+000007b0: 7d01 0100 7a14 7403 7c01 8301 0100 5700  }...z.t.|.....W.
+000007c0: 5900 6400 7d01 7e01 6e0a 6400 7d01 7e01  Y.d.}.~.n.d.}.~.
+000007d0: 3000 3000 6400 5300 2901 4e29 0472 0c00  0.0.d.S.).N).r..
+000007e0: 0000 7220 0000 00da 0945 7863 6570 7469  ..r .....Excepti
+000007f0: 6f6e 7202 0000 0029 0272 1000 0000 da01  onr....).r......
+00000800: 6572 1200 0000 7212 0000 0072 1300 0000  er....r....r....
+00000810: da0c 7761 6974 5f70 726f 6365 7373 3700  ..wait_process7.
+00000820: 0000 7308 0000 0000 0102 010e 010e 017a  ..s............z
+00000830: 156d 6963 724f 5349 4d2e 7761 6974 5f70  .micrOSIM.wait_p
+00000840: 726f 6365 7373 6301 0000 0000 0000 0000  rocessc.........
+00000850: 0000 0001 0000 0004 0000 0043 0000 0073  ...........C...s
+00000860: 3000 0000 7400 6401 8301 0100 7c00 6a01  0...t.d.....|.j.
+00000870: a002 a100 0100 7c00 6a01 6a03 7c00 5f03  ......|.j.j.|._.
+00000880: 7400 6402 a004 7c00 6a03 a101 8301 0100  t.d...|.j.......
+00000890: 6400 5300 2903 4e7a 295b 6d69 6372 4f53  d.S.).Nz)[micrOS
+000008a0: 494d 5d20 5374 6172 7420 6d69 6372 4f53  IM] Start micrOS
+000008b0: 2073 696d 756c 6174 6f72 2070 726f 6365   simulator proce
+000008c0: 7373 7a29 5b6d 6963 724f 5349 4d5d 206d  ssz)[micrOSIM] m
+000008d0: 6963 724f 5320 7072 6f63 6573 7320 7761  icrOS process wa
+000008e0: 7320 7374 6172 7465 643a 207b 7d29 0572  s started: {}).r
+000008f0: 0200 0000 720c 0000 00da 0573 7461 7274  ....r......start
+00000900: 720d 0000 0072 0700 0000 a901 7210 0000  r....r......r...
+00000910: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
+00000920: 7238 0000 003d 0000 0073 0800 0000 0001  r8...=...s......
+00000930: 0801 0a01 0a01 7a0e 6d69 6372 4f53 494d  ......z.micrOSIM
+00000940: 2e73 7461 7274 6301 0000 0000 0000 0000  .startc.........
+00000950: 0000 0001 0000 0004 0000 0043 0000 0073  ...........C...s
+00000960: 5800 0000 7c00 6a00 a001 a100 723a 7c00  X...|.j.....r:|.
+00000970: 6a00 a002 a100 0100 7c00 6a00 a001 a100  j.......|.j.....
+00000980: 723a 7403 6401 a004 7c00 6a05 a101 8301  r:t.d...|.j.....
+00000990: 0100 7406 a007 6402 a101 0100 7114 7c00  ..t...d.....q.|.
+000009a0: 6a00 a008 a100 0100 7403 6403 a004 7c00  j.......t.d...|.
+000009b0: 6a05 a101 8301 0100 6400 5300 2904 4e7a  j.......d.S.).Nz
+000009c0: 285b 6d69 6372 4f53 494d 5d20 5761 6974  ([micrOSIM] Wait
+000009d0: 2070 726f 6365 7373 2074 6f20 7465 726d   process to term
+000009e0: 696e 6174 653a 207b 7de9 0100 0000 7a20  inate: {}.....z 
+000009f0: 5b6d 6963 724f 5349 4d5d 2050 726f 6320  [micrOSIM] Proc 
+00000a00: 7761 7320 6669 6e69 7368 6564 3a20 7b7d  was finished: {}
+00000a10: 2909 720c 0000 00da 0869 735f 616c 6976  ).r......is_aliv
+00000a20: 65da 0974 6572 6d69 6e61 7465 7202 0000  e..terminater...
+00000a30: 0072 0700 0000 720d 0000 0072 1a00 0000  .r....r....r....
+00000a40: da05 736c 6565 70da 0563 6c6f 7365 7239  ..sleep..closer9
+00000a50: 0000 0072 1200 0000 7212 0000 0072 1300  ...r....r....r..
+00000a60: 0000 723c 0000 0043 0000 0073 0e00 0000  ..r<...C...s....
+00000a70: 0001 0a01 0a01 0a01 1001 0c01 0a01 7a12  ..............z.
+00000a80: 6d69 6372 4f53 494d 2e74 6572 6d69 6e61  micrOSIM.termina
+00000a90: 7465 6300 0000 0000 0000 0000 0000 0005  tec.............
+00000aa0: 0000 000b 0000 0043 0000 0073 be00 0000  .......C...s....
+00000ab0: 7400 6a01 7d00 7402 7c00 8301 7d01 7403  t.j.}.t.|...}.t.
+00000ac0: 7c00 8301 4400 5d9c 5c02 7d02 7d03 7a44  |...D.].\.}.}.zD
+00000ad0: 7c03 a004 a100 7258 7c03 a005 a100 0100  |.....rX|.......
+00000ae0: 7c03 a004 a100 7258 7406 6401 a007 7c02  |.....rXt.d...|.
+00000af0: 6402 1700 7c01 a102 8301 0100 7408 a009  d...|.......t...
+00000b00: 6402 a101 0100 7130 7c03 a00a a100 0100  d.....q0|.......
+00000b10: 5700 6e3a 0400 740b 799c 0100 7d04 0100  W.n:..t.y...}...
+00000b20: 7a22 7406 6403 a007 7c02 6402 1700 7c01  z"t.d...|.d...|.
+00000b30: 7c04 a103 8301 0100 5700 5900 6400 7d04  |.......W.Y.d.}.
+00000b40: 7e04 6e0a 6400 7d04 7e04 3000 3000 7406  ~.n.d.}.~.0.0.t.
+00000b50: 6404 a007 7c02 6402 1700 7c01 a102 8301  d...|.d...|.....
+00000b60: 0100 7116 6700 7400 5f01 6400 5300 2905  ..q.g.t._.d.S.).
+00000b70: 4e7a 2b5b 6d69 6372 4f53 494d 5d20 5761  Nz+[micrOSIM] Wa
+00000b80: 6974 2070 726f 6365 7373 2074 6f20 7465  it process to te
+00000b90: 726d 696e 6174 653a 207b 7d2f 7b7d 723a  rminate: {}/{}r:
+00000ba0: 0000 007a 2a5b 6d69 6372 4f53 494d 5d20  ...z*[micrOSIM] 
+00000bb0: 5072 6f63 2061 6c72 6561 6479 2073 746f  Proc already sto
+00000bc0: 7070 6564 3a20 7b7d 2f7b 7d3a 207b 7d7a  pped: {}/{}: {}z
+00000bd0: 235b 6d69 6372 4f53 494d 5d20 5072 6f63  #[micrOSIM] Proc
+00000be0: 2077 6173 2066 696e 6973 6865 643a 207b   was finished: {
+00000bf0: 7d2f 7b7d 290c 7203 0000 0072 0e00 0000  }/{}).r....r....
+00000c00: da03 6c65 6eda 0965 6e75 6d65 7261 7465  ..len..enumerate
+00000c10: 723b 0000 0072 3c00 0000 7202 0000 0072  r;...r<...r....r
+00000c20: 0700 0000 721a 0000 0072 3d00 0000 723e  ....r....r=...r>
+00000c30: 0000 0072 3500 0000 2905 5a09 7072 6f63  ...r5...).Z.proc
+00000c40: 5f6c 6973 745a 0870 726f 635f 6c65 6eda  _listZ.proc_len.
+00000c50: 0169 da04 7072 6f63 7236 0000 0072 1200  .i..procr6...r..
+00000c60: 0000 7212 0000 0072 1300 0000 da08 7374  ..r....r......st
+00000c70: 6f70 5f61 6c6c 4c00 0000 731c 0000 0000  op_allL...s.....
+00000c80: 0206 0108 0110 0102 0108 0108 0108 0114  ................
+00000c90: 010c 010c 010e 012c 0116 017a 116d 6963  .......,...z.mic
+00000ca0: 724f 5349 4d2e 7374 6f70 5f61 6c6c 6302  rOSIM.stop_allc.
+00000cb0: 0000 0000 0000 0000 0000 000c 0000 000c  ................
+00000cc0: 0000 0043 0000 0073 e601 0000 7400 a001  ...C...s....t...
+00000cd0: 7c01 a101 7d02 7402 a003 a100 7d03 7c03  |...}.t.....}.|.
+00000ce0: a004 7405 a101 0100 7c01 a006 a100 4400  ..t.....|.....D.
+00000cf0: 9001 5da8 5c02 7d04 7d05 7c01 7c04 1900  ..].\.}.}.|.|...
+00000d00: 6401 1900 7d06 6402 7c06 9b00 6403 7c04  d...}.d.|...d.|.
+00000d10: 9b00 6404 9d05 7c02 7c04 1900 6401 3c00  ..d...|.|...d.<.
+00000d20: 7c05 4400 9001 5d72 7d07 7407 7c01 7c04  |.D...]r}.t.|.|.
+00000d30: 1900 7c07 1900 7408 8302 7372 7158 7409  ..|...t...srqXt.
+00000d40: 6405 7c04 9b00 6406 7c07 9b00 6407 9d05  d.|...d.|...d...
+00000d50: 8301 0100 7a94 740a 6408 7c04 9b00 9d02  ....z.t.d.|.....
+00000d60: 8301 0100 740b 6409 7c04 9b00 6406 7c07  ....t.d.|...d.|.
+00000d70: 9b00 6407 9d05 8301 7d08 7c07 640a 6b02  ..d.....}.|.d.k.
+00000d80: 9001 721a 7409 640b 7c04 9b00 640c 9d03  ..r.t.d.|...d...
+00000d90: 8301 0100 7a38 740b 6409 7c04 9b00 640c  ....z8t.d.|...d.
+00000da0: 9d03 8301 7d09 7c09 640d 7501 72fe 640e  ....}.|.d.u.r.d.
+00000db0: a00c 7408 7c09 8301 a00d a100 a101 7d09  ..t.|.........}.
+00000dc0: 640f 7c09 9b00 9d02 7d09 5700 6e10 0100  d.|.....}.W.n...
+00000dd0: 0100 0100 6410 7d09 5900 6e02 3000 7c08  ....d.}.Y.n.0.|.
+00000de0: 7c09 3700 7d08 5700 6e2e 0400 740e 9001  |.7.}.W.n...t...
+00000df0: 794a 0100 7d0a 0100 7a14 740f 7c0a 8301  yJ..}...z.t.|...
+00000e00: 7d08 5700 5900 640d 7d0a 7e0a 6e0a 640d  }.W.Y.d.}.~.n.d.
+00000e10: 7d0a 7e0a 3000 3000 7c08 7c01 7c04 1900  }.~.0.0.|.|.|...
+00000e20: 7c07 1900 6411 3c00 7c08 640d 7500 9001  |...d.<.|.d.u...
+00000e30: 726a 6412 6e16 7c08 a010 a100 a011 6413  rjd.n.|.......d.
+00000e40: 6414 a102 a011 6415 6416 a102 7c02 7c04  d.....d.d...|.|.
+00000e50: 1900 7c07 1900 6411 3c00 7c02 7c04 1900  ..|...d.<.|.|...
+00000e60: 7c07 1900 a012 6417 640d a102 7d0b 7c0b  |.....d.d...}.|.
+00000e70: 640d 7501 7258 7413 7c0b a010 a100 8301  d.u.rXt.|.......
+00000e80: 6418 6b02 7258 7c02 7c04 1900 7c07 1900  d.k.rX|.|...|...
+00000e90: a014 6417 a101 0100 7158 7124 7c03 a015  ..d.....qXq$|...
+00000ea0: a100 0100 7c01 7c02 6602 7c00 5f16 640d  ....|.|.f.|._.d.
+00000eb0: 5300 2919 7abd 0a20 2020 2020 2020 2043  S.).z..        C
+00000ec0: 6f6c 6c65 6374 2066 756e 6374 696f 6e20  ollect function 
+00000ed0: 646f 6320 7374 7269 6e67 7320 616e 6420  doc strings and 
+00000ee0: 6d6f 6475 6c65 206c 6f67 6963 616c 2070  module logical p
+00000ef0: 696e 7320 2870 696e 206d 6170 290a 2020  ins (pin map).  
+00000f00: 2020 2020 2020 4372 6561 7465 2032 2064        Create 2 d
+00000f10: 6963 7420 7374 7275 6374 7572 6573 2061  ict structures a
+00000f20: 6464 696e 6720 646f 6373 7472 696e 670a  dding docstring.
+00000f30: 2020 2020 2020 2020 2d20 6874 6d6c 2068          - html h
+00000f40: 6163 6b20 7374 7275 6374 7572 650a 2020  ack structure.  
+00000f50: 2020 2020 2020 2d20 6a73 6f6e 2072 6177        - json raw
+00000f60: 2073 7472 7563 7475 7265 0a20 2020 2020   structure.     
+00000f70: 2020 20da 0369 6d67 7a0a 3c69 6d67 2073     ..imgz.<img s
+00000f80: 7263 3d22 7a07 2220 616c 743d 227a 0d22  rc="z." alt="z."
+00000f90: 2068 6569 6768 743d 3135 303e 7a1f 5b6d   height=150>z.[m
+00000fa0: 6963 724f 5349 4d5d 5b45 7874 7261 6374  icrOSIM][Extract
+00000fb0: 2064 6f63 2d73 7472 5d20 4c4d 5f72 1700   doc-str] LM_r..
+00000fc0: 0000 7a08 2e5f 5f64 6f63 5f5f 7a0a 696d  ..z..__doc__z.im
+00000fd0: 706f 7274 204c 4d5f da03 4c4d 5f5a 0670  port LM_..LM_Z.p
+00000fe0: 696e 6d61 707a 265b 6d69 6372 4f53 494d  inmapz&[micrOSIM
+00000ff0: 5d5b 4578 7472 6163 7420 7069 6e20 6d61  ][Extract pin ma
+00001000: 7020 746f 6b65 6e73 5d20 4c4d 5f7a 092e  p tokens] LM_z..
+00001010: 7069 6e6d 6170 2829 4e7a 022c 207a 0a0a  pinmap()Nz., z..
+00001020: 7069 6e20 6d61 703a 2072 1900 0000 da03  pin map: r......
+00001030: 646f 637a 174e 6f20 646f 6320 7374 7269  docz.No doc stri
+00001040: 6e67 2061 7661 696c 6162 6c65 da01 0a7a  ng available...z
+00001050: 053c 6272 3e0a 7218 0000 007a 0626 6e62  .<br>.r....z.&nb
+00001060: 7370 3b7a 0870 6172 616d 2873 2972 0100  sp;z.param(s)r..
+00001070: 0000 2917 da04 636f 7079 da08 6465 6570  ..)...copy..deep
+00001080: 636f 7079 722b 0000 0072 2c00 0000 722d  copyr+...r,...r-
+00001090: 0000 0072 2e00 0000 da05 6974 656d 73da  ...r......items.
+000010a0: 0a69 7369 6e73 7461 6e63 65da 0464 6963  .isinstance..dic
+000010b0: 7472 0200 0000 da04 6578 6563 da04 6576  tr......exec..ev
+000010c0: 616c 7220 0000 00da 046b 6579 7372 3500  alr .....keysr5.
+000010d0: 0000 da03 7374 72da 0573 7472 6970 da07  ....str..strip..
+000010e0: 7265 706c 6163 65da 0367 6574 723f 0000  replace..getr?..
+000010f0: 00da 0370 6f70 7233 0000 0072 0600 0000  ...popr3...r....
+00001100: 290c 7210 0000 00da 0973 7472 7563 7475  ).r......structu
+00001110: 7265 5a11 7374 7275 6374 7572 655f 746f  reZ.structure_to
+00001120: 5f68 746d 6c72 3300 0000 da03 6d6f 645a  _htmlr3.....modZ
+00001130: 0966 756e 635f 6469 6374 5a07 696d 675f  .func_dictZ.img_
+00001140: 7572 6cda 0466 756e 635a 0764 6f63 5f73  url..funcZ.doc_s
+00001150: 7472 5a0a 6d6f 645f 7069 6e6d 6170 7236  trZ.mod_pinmapr6
+00001160: 0000 005a 0a70 6172 616d 5f63 656c 6c72  ...Z.param_cellr
+00001170: 1200 0000 7212 0000 0072 1300 0000 da0f  ....r....r......
+00001180: 5f6c 6d5f 646f 635f 7374 7269 6e67 735d  _lm_doc_strings]
+00001190: 0000 0073 4800 0000 0007 0a03 0801 0a03  ...sH...........
+000011a0: 1202 0c01 1a02 0a02 1201 0203 1601 0202  ................
+000011b0: 0e01 1602 0a02 1001 0201 1001 0801 1201  ................
+000011c0: 0e01 0601 0a02 0c01 1001 1e02 1001 1601  ................
+000011d0: 04ff 0401 04ff 1003 1401 1801 1603 0801  ................
+000011e0: 7a18 6d69 6372 4f53 494d 2e5f 6c6d 5f64  z.micrOSIM._lm_d
+000011f0: 6f63 5f73 7472 696e 6773 6302 0000 0000  oc_stringsc.....
+00001200: 0000 0000 0000 0004 0000 000a 0000 0043  ...............C
+00001210: 0000 0073 6600 0000 7a2e 7400 6a01 7c00  ...sf...z.t.j.|.
+00001220: a002 7c01 a101 6401 8d01 7d02 7c02 a003  ..|...d...}.|...
+00001230: a100 7228 7404 a005 6402 a101 0100 7114  ..r(t...d.....q.
+00001240: 7c00 6a06 5700 5300 0400 7407 7960 0100  |.j.W.S...t.y`..
+00001250: 7d03 0100 7a1a 7408 6403 a009 7c03 a101  }...z.t.d...|...
+00001260: 8301 0100 5700 5900 6400 7d03 7e03 6e0a  ....W.Y.d.}.~.n.
+00001270: 6400 7d03 7e03 3000 3000 6400 5300 2904  d.}.~.0.0.d.S.).
+00001280: 4e72 0400 0000 679a 9999 9999 99b9 3f7a  Nr....g.......?z
+00001290: 425b 6d69 6372 4f53 494d 5d5b 444f 4320  B[micrOSIM][DOC 
+000012a0: 4552 525d 2044 6f63 2067 656e 6572 6174  ERR] Doc generat
+000012b0: 696f 6e20 6572 726f 723a 2067 656e 5f6c  ion error: gen_l
+000012c0: 6d5f 646f 635f 6a73 6f6e 5f68 746d 6c3a  m_doc_json_html:
+000012d0: 207b 7d29 0a72 0800 0000 720a 0000 0072   {}).r....r....r
+000012e0: 5800 0000 723b 0000 0072 1a00 0000 723d  X...r;...r....r=
+000012f0: 0000 0072 0600 0000 7235 0000 0072 0200  ...r....r5...r..
+00001300: 0000 7207 0000 0029 0472 1000 0000 7255  ..r....).r....rU
+00001310: 0000 0072 4200 0000 7236 0000 0072 1200  ...rB...r6...r..
+00001320: 0000 7212 0000 0072 1300 0000 da14 6765  ..r....r......ge
+00001330: 6e5f 6c6d 5f64 6f63 5f6a 736f 6e5f 6874  n_lm_doc_json_ht
+00001340: 6d6c 9700 0000 7310 0000 0000 0102 0112  ml....s.........
+00001350: 0108 010c 0108 010e 0124 017a 1d6d 6963  .........$.z.mic
+00001360: 724f 5349 4d2e 6765 6e5f 6c6d 5f64 6f63  rOSIM.gen_lm_doc
+00001370: 5f6a 736f 6e5f 6874 6d6c 4e29 0146 2901  _json_htmlN).F).
+00001380: 4629 0dda 085f 5f6e 616d 655f 5fda 0a5f  F)...__name__.._
+00001390: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+000013a0: 6c6e 616d 655f 5f72 0e00 0000 7214 0000  lname__r....r...
+000013b0: 0072 0b00 0000 7237 0000 0072 3800 0000  .r....r7...r8...
+000013c0: 723c 0000 00da 0c73 7461 7469 636d 6574  r<.....staticmet
+000013d0: 686f 6472 4300 0000 7258 0000 0072 5900  hodrC...rX...rY.
+000013e0: 0000 7212 0000 0072 1200 0000 7212 0000  ..r....r....r...
+000013f0: 0072 1300 0000 7203 0000 0010 0000 0073  .r....r........s
+00001400: 1400 0000 0801 0402 0a0c 0a18 0806 0806  ................
+00001410: 0809 0201 0a10 083a 7203 0000 00da 085f  .......:r......_
+00001420: 5f6d 6169 6e5f 5f7a 1c54 6573 7420 6d6f  _main__z.Test mo
+00001430: 6465 202d 2053 746f 7020 6166 7465 7220  de - Stop after 
+00001440: 3320 7365 63e9 0300 0000 2917 722f 0000  3 sec.....).r/..
+00001450: 00da 026f 7372 0800 0000 721a 0000 0072  ...osr....r....r
+00001460: 4800 0000 da04 7061 7468 da07 6469 726e  H.....path..dirn
+00001470: 616d 65da 085f 5f66 696c 655f 5fda 064d  ame..__file__..M
+00001480: 5950 4154 4872 2000 0000 722e 0000 00da  YPATHr ...r.....
+00001490: 0669 6e73 6572 745a 0b73 696d 5f63 6f6e  .insertZ.sim_con
+000014a0: 736f 6c65 7202 0000 0072 3100 0000 722b  soler....r1...r+
+000014b0: 0000 0072 0300 0000 725a 0000 00da 0373  ...r....rZ.....s
+000014c0: 696d 7238 0000 0072 3d00 0000 723c 0000  imr8...r=...r<..
+000014d0: 0072 4300 0000 7212 0000 0072 1200 0000  .rC...r....r....
+000014e0: 7212 0000 0072 1300 0000 da08 3c6d 6f64  r....r......<mod
+000014f0: 756c 653e 0100 0000 732a 0000 0008 0108  ule>....s*......
+00001500: 0108 0108 0108 020c 010e 010e 0118 010c  ................
+00001510: 0108 0108 030e 7f00 1308 0106 0108 0108  ................
+00001520: 0108 010a 0108 01                        .......
```

### Comparing `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc` & `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc` & `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc` & `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc` & `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/machine.py` & `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/machine.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/micropython.py` & `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/micropython.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/neopixel.py` & `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/neopixel.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/network.py` & `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/network.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/sim_console.py` & `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/sim_console.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/simulator.py` & `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         else:
             console("[micrOSIM] INFO: Number of cpu : {}".format(multiprocessing.cpu_count()))
             console("[micrOSIM] Create micrOS simulator process...")
             self.process = multiprocessing.Process(target=self.micrOS_sim_worker)
             self.pid = None
             micrOSIM.SIM_PROCESS_LIST.append(self.process)
 
-    def micrOS_sim_worker(self):
+    def micrOS_sim_worker(self, trace=False):
         sim_path = LocalMachine.SimplePopPushd()
         sim_path.pushd(SIM_PATH)
         console("[micrOSIM] Start micrOS loader in: {}".format(SIM_PATH))
         prev_t = time.time()
 
         def trace_func(frame, event, arg):
             nonlocal prev_t
@@ -40,16 +40,17 @@
             prev_t = time.time()
             file = frame.f_code.co_filename
             line = frame.f_lineno
             code = frame.f_code.co_name
             if 'simulator/' in file and code != 'idle_task':
                 print(f"{' '*50}[trace][{elapsed_time}s][{event}] {line}: {'/'.join(file.split('/')[-1:])}.{code} {arg if arg else ''}")
 
-        # Trace handling - DEBUG
-        sys.settrace(trace_func)
+        if trace:
+            # Trace handling - DEBUG
+            sys.settrace(trace_func)
         micrOSloader.main()
 
         console("[micrOSIM] Stop micrOS ({})".format(SIM_PATH))
         sim_path.popd()
 
     def wait_process(self):
         try:
```

### Comparing `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/uasyncio.py` & `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/uasyncio.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/utime.py` & `micrOSDevToolKit-1.21.1/toolkit/simulator_lib/utime.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/socketClient.py` & `micrOSDevToolKit-1.21.1/toolkit/socketClient.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/Common.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/Common.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/ConfigHandler.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/ConfigHandler.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/Debug.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/Debug.mpy`

 * *Files 10% similar despite different names*

```diff
@@ -1,121 +1,125 @@
-00000000: 4d06 001f 5208 1044 6562 7567 2e70 7900  M...R..Debug.py.
+00000000: 4d06 001f 5209 1044 6562 7567 2e70 7900  M...R..Debug.py.
 00000010: 0f04 6f73 0012 6c6f 6361 6c74 696d 6500  ..os..localtime.
 00000020: 0874 696d 6500 0650 696e 000e 6d61 6368  .time..Pin..mach
 00000030: 696e 6500 104e 656f 5069 7865 6c00 106e  ine..NeoPixel..n
 00000040: 656f 7069 7865 6c00 1870 6879 7369 6361  eopixel..physica
 00000050: 6c5f 7069 6e00 1670 696e 6d61 705f 6475  l_pin..pinmap_du
 00000060: 6d70 001e 6465 7465 6374 5f70 6c61 7466  mp..detect_platf
 00000070: 6f72 6d00 164c 6f67 6963 616c 5069 6e73  orm..LogicalPins
 00000080: 0010 5469 6e79 504c 6564 0010 4465 6275  ..TinyPLed..Debu
 00000090: 6743 6667 001a 636f 6e73 6f6c 655f 7772  gCfg..console_wr
-000000a0: 6974 6500 0a44 4542 5547 0082 2b0c 6c6f  ite..DEBUG..+.lo
-000000b0: 6767 6572 0004 722b 0004 612b 000e 6c6f  gger..r+..a+..lo
-000000c0: 675f 6765 7400 0272 0081 7f82 310a 5b45  g_get..r....1.[E
-000000d0: 5252 5d00 1465 7272 6c6f 675f 6164 6400  RR]..errlog_add.
-000000e0: 0e65 7272 2e6c 6f67 000a 6c69 6d69 7400  .err.log..limit.
-000000f0: 1465 7272 6c6f 675f 6765 7400 1865 7272  .errlog_get..err
-00000100: 6c6f 675f 636c 6561 6e00 0e6c 6973 7464  log_clean..listd
-00000110: 6972 0081 2982 0112 696e 6974 5f70 6c65  ir..)...init_ple
+000000a0: 6974 6500 0a44 4542 5547 0082 2b81 290c  ite..DEBUG..+.).
+000000b0: 6c6f 6767 6572 0004 722b 0004 612b 000e  logger..r+..a+..
+000000c0: 6c6f 675f 6765 7400 0272 0081 7f82 310a  log_get..r....1.
+000000d0: 5b45 5252 5d00 1465 7272 6c6f 675f 6164  [ERR]..errlog_ad
+000000e0: 6400 0e65 7272 2e6c 6f67 000a 6c69 6d69  d..err.log..limi
+000000f0: 7400 1465 7272 6c6f 675f 6765 7400 1865  t..errlog_get..e
+00000100: 7272 6c6f 675f 636c 6561 6e00 0e6c 6973  rrlog_clean..lis
+00000110: 7464 6972 0082 0112 696e 6974 5f70 6c65  tdir....init_ple
 00000120: 6400 1074 696e 7970 6963 6f00 185f 696e  d..tinypico.._in
 00000130: 6974 5f61 7061 3130 3200 0e62 7569 6c74  it_apa102..built
 00000140: 696e 000e 6573 7033 3273 3300 185f 696e  in..esp32s3.._in
 00000150: 6974 5f77 7332 3831 3200 185f 696e 6974  it_ws2812.._init
 00000160: 5f73 696d 706c 6500 064f 5554 0010 504c  _simple..OUT..PL
 00000170: 4544 5f4f 424a 0016 696e 6974 5f41 5041  ED_OBJ..init_APA
 00000180: 3130 3200 185f 7374 6570 5f77 7332 3831  102.._step_ws281
 00000190: 3200 124e 454f 5f57 4845 454c 0033 8249  2..NEO_WHEEL.3.I
 000001a0: 8245 0e5f 6c6f 6767 6572 0002 2e00 8151  .E._logger.....Q
 000001b0: 022d 0002 3a00 0c7b 7d20 7b7d 0a00 1272  .-..:..{} {}...r
 000001c0: 6561 646c 696e 6573 0079 0873 6565 6b00  eadlines.y.seek.
 000001d0: 0314 3c6c 6973 7463 6f6d 703e 0081 1f08  ..<listcomp>....
 000001e0: 2e6c 6f67 001a 5f5f 636f 6c6f 725f 7768  .log..__color_wh
 000001f0: 6565 6c00 2f2d 3582 2906 6d73 6700 8177  eel./-5.).msg..w
-00000200: 0864 6174 6100 0c66 5f6e 616d 6500 0c6d  .data..f_name..m
-00000210: 7367 6f62 6a00 816d 8143 490a 5f64 6174  sgobj..m.CI._dat
+00000200: 4908 6461 7461 000c 665f 6e61 6d65 000c  I.data..f_name..
+00000210: 6d73 676f 626a 0081 6d81 430a 5f64 6174  msgobj..m.C._dat
 00000220: 6100 0e5f 665f 6e61 6d65 000c 5f6c 696d  a.._f_name.._lim
 00000230: 6974 000c 665f 6d6f 6465 0081 570b 822f  it..f_mode..W../
-00000240: 050b 2044 656c 6574 653a 207b 7d00 0518  .. Delete: {}...
-00000250: 6465 6275 6720 6c65 6420 7374 6570 2065  debug led step e
-00000260: 7272 6f72 3a20 7b7d 000a 0307 0231 3007  rror: {}.....10.
-00000270: 0130 0701 300a 0307 0135 0701 3507 0130  .0..0....5..5..0
-00000280: 0a03 0701 3007 0231 3007 0130 0a03 0701  ....0..10..0....
-00000290: 3007 0135 0701 350a 0307 0130 0701 3007  0..5..5....0..0.
-000002a0: 0231 300a 0307 0135 0701 3007 0135 8a3c  .10....5..0..5.<
-000002b0: 1c30 0126 2c2c 4c22 5b46 4249 8608 894e  .0.&,,L"[FBI...N
-000002c0: 840c 842f 881c 8409 8807 8051 1b02 1602  .../.......Q....
-000002d0: 8010 032a 011b 041c 0316 0359 8010 052a  ...*.......Y...*
-000002e0: 011b 061c 0516 0559 8010 072a 011b 081c  .......Y...*....
-000002f0: 0716 0759 481a 8010 0910 0a10 0b2a 031b  ...YH........*..
-00000300: 0c1c 0916 091c 0a16 0a1c 0b16 0b59 4a07  .............YJ.
-00000310: 5951 160b 4a01 5d48 0880 511b 0d16 0d4a  YQ..J.]H..Q....J
-00000320: 0759 5116 0d4a 015d 5432 0010 0e34 0216  .YQ..J.]T2...4..
-00000330: 0e32 0116 0f32 0216 1251 2a01 5333 0316  .2...2...Q*.S3..
-00000340: 1532 0416 1a51 2a01 5333 0516 1d51 2a01  .2...Q*.S3...Q*.
-00000350: 5333 0616 1e51 6307 852c 0820 0e88 1723  S3...Qc..,. ...#
-00000360: 2343 8812 6840 6840 6840 880f 113f 1640  #C..h@h@h@...?.@
-00000370: 100e 1641 5216 1051 162a 5116 2d11 4232  ...AR..Q.*Q.-.B2
-00000380: 0034 0116 2211 4232 0134 0116 2811 4232  .4..".B2.4..(.B2
-00000390: 0234 0116 2411 4232 0334 0116 2711 4232  .4..$.B2.4..'.B2
-000003a0: 0434 0116 2c11 4232 0534 0116 1151 6306  .4..,.B2.4...Qc.
-000003b0: 8540 1016 2280 1e46 2225 4d29 2e46 6912  .@.."..F"%M).Fi.
-000003c0: 0b51 de44 4251 6312 0b34 00c0 b010 23d9  .Q.DBQc..4....#.
-000003d0: 4450 120d 51de d344 4912 0e14 2436 0059  DP..Q..DI...$6.Y
-000003e0: 4266 120a 1025 3401 1025 5551 ded3 4458  Bf...%4..%UQ..DX
-000003f0: b010 26d9 4449 120e 1427 3600 5942 4712  ..&.DI...'6.YBG.
-00000400: 0e14 2836 0059 4240 5163 8148 1006 2880  ..(6.YB@Qc.H..(.
-00000410: 3012 0512 0910 2534 0112 0513 2934 0212  0.....%4....)4..
-00000420: 0e18 2a51 6381 0808 0624 8035 120d 142b  ..*Qc....$.5...+
-00000430: 3600 120e 182a 5163 8168 1808 2780 392b  6....*Qc.h..'.9+
-00000440: 1205 1209 1025 3401 3401 c012 07b0 8134  .....%4.4......4
-00000450: 0212 0e18 2a51 6383 2c18 102c 803e 8308  ....*Qc.,..,.>..
-00000460: 2827 2e32 00c0 120e 132d 51de 4447 b034  ('.2.....-Q.DG.4
-00000470: 0012 0e18 2d12 0e13 2d14 2e36 0012 0e13  ....-...-..6....
-00000480: 2a80 5612 0e13 2a14 2f36 0059 5163 0182  *.V...*./6.YQc..
-00000490: 4080 4012 3e80 3f20 2424 2424 2423 0267  @.@.>.? $$$$$#.g
-000004a0: 5923 0367 5923 0467 5923 0567 5923 0667  Y#.gY#.gY#.gY#.g
-000004b0: 5923 0767 5942 2651 6388 28b8 0220 1180  Y#.gYB&Qc.(.. ..
-000004c0: 4d60 4022 4c32 224c 2722 4e27 4d2c 484e  M`@"L2"L'"N'M,HN
-000004d0: 1249 120e 132a 1205 3402 4454 120e 132a  .I...*..4.DT...*
-000004e0: 1430 120e 132a 1430 3600 d336 0159 5263  .0...*.06..6.YRc
-000004f0: 1249 120e 132a 1207 3402 4449 120e 142c  .I...*..4.DI...,
-00000500: 3600 5950 6312 0d51 de43 5112 0e13 2a51  6.YPc..Q.CQ...*Q
-00000510: de43 4912 0d14 1136 0059 5063 4a20 5712  .CI....6.YPcJ W.
-00000520: 4adf 4459 c049 0f12 1a23 0114 20b0 3601  J.DY.I...#.. .6.
-00000530: 3401 5950 6351 51c0 2800 5d4a 015d 5163  4.YPcQQ.(.]J.]Qc
-00000540: 8248 1910 0f43 8065 2627 2623 120e 1310  .H...C.e&'&#....
-00000550: 4457 120e 1411 3600 c112 44b0 3401 59b1  DW....6...D.4.Y.
-00000560: 4447 120e 1411 3600 5951 6383 74db 021e  DG....6.YQc.t...
-00000570: 1245 461c 8071 800a 8818 424a 424c 2810  .EF..q....BJBL(.
-00000580: 132a 0153 3300 c348 09b3 b0b1 b234 0359  .*.S3..H.....4.Y
-00000590: 4a17 5948 0bb3 b0b1 b210 1434 0459 4a06  J.YH.......4.YJ.
-000005a0: 5950 634a 015d 4a01 5d52 6301 8a14 fc05  YPcJ.]J.]Rc.....
-000005b0: 2831 4b4c 4d4e 807c 4a29 5d29 494a 2627  (1KLMN.|J)])IJ&'
-000005c0: 4725 284a 48b2 9ed8 4443 9e42 41b2 c232  G%(JH...DC.BA..2
-000005d0: 0012 0334 0034 01c4 1032 1433 b480 832e  ...4.4...2.3....
-000005e0: 0255 3601 1034 f210 3514 33b4 8386 2e02  .U6..4..5.3.....
-000005f0: 5536 01f2 c512 48b1 b334 0247 4fc6 1036  U6....H..4.GO..6
-00000600: 1420 b5b0 3602 c032 01b6 1437 3600 3401  . ..6..2...76.4.
-00000610: c712 4fb7 3401 c8b7 1438 b036 0159 b614  ..O.4....8.6.Y..
-00000620: 3980 3601 59b8 b2db 4452 b7b2 d151 2e02  9.6.Y...DR...Q..
-00000630: 55c7 103a 1433 b736 01c9 4248 103a 1433  U..:.3.6..BH.:.3
-00000640: b736 01c9 b614 2fb9 3601 5951 5c5d 5163  .6..../.6.YQ\]Qc
-00000650: 0281 3841 083b 5080 7e2b 00b0 5f4b 0ac1  ..8A.;P.~+.._K..
-00000660: 1251 b134 012f 1442 3463 8178 4108 3b50  .Q.4./.B4c.xA.;P
-00000670: 8084 2b00 b05f 4b12 c110 34b1 dd44 3710  ..+.._K...4..D7.
-00000680: 32b1 dd44 31b1 2f14 422c 6386 30ca 0324  2..D1./.B,c.0..$
-00000690: 1546 4780 a060 2022 222a 2a42 4d25 4825  .FG..` ""**BM%H%
-000006a0: 5323 80c2 4847 1248 b010 1634 0247 3ac3  S#..HG.H...4.G:.
-000006b0: b314 1736 0014 1836 00c4 4269 b210 19b4  ...6...6..Bi....
-000006c0: dd44 4381 4241 80e5 c2b1 51de 4448 120f  .DC.BA....Q.DH..
-000006d0: b434 0159 4245 b1b4 3401 59b3 1417 3600  .4.YBE..4.Y...6.
-000006e0: 1418 3600 c4b4 4314 515c 5d4a 0459 4a01  ..6...C.Q\]J.YJ.
-000006f0: 5db2 6381 3831 0e1a 4580 bc60 2023 101b  ].c.81..E..` #..
-00000700: c112 12b0 b110 1c85 3482 0263 8128 a901  ........4..c.(..
-00000710: 0c1d 4780 c523 4710 1bc1 1215 b1b0 3402  ..G..#G.......4.
-00000720: c2b2 6384 1cd1 0114 1e47 80cc 2b25 2825  ..c......G..+%(%
-00000730: 4825 3200 1202 141f 3600 3401 c1b1 5f4b  H%2.....6.4..._K
-00000740: 25c2 2300 1420 b236 01c3 b051 de44 4812  %.#.. .6...Q.DH.
-00000750: 0fb3 3401 5942 45b0 b334 0159 1202 1421  ..4.YBE..4.Y...!
-00000760: b236 0159 4219 5163 0181 6049 083b 5080  .6.YB.Qc..`I.;P.
-00000770: cc2b 00b0 5f4b 0fc1 b114 3c10 3d36 0144  .+.._K....<.=6.D
-00000780: 34b1 2f14 422f 63                        4./.B/c
+00000240: 0517 5b45 5252 5d20 636f 6e73 6f6c 655f  ..[ERR] console_
+00000250: 7772 6974 653a 207b 7d00 050b 2044 656c  write: {}... Del
+00000260: 6574 653a 207b 7d00 0518 6465 6275 6720  ete: {}...debug 
+00000270: 6c65 6420 7374 6570 2065 7272 6f72 3a20  led step error: 
+00000280: 7b7d 000a 0307 0231 3007 0130 0701 300a  {}.....10..0..0.
+00000290: 0307 0135 0701 3507 0130 0a03 0701 3007  ...5..5..0....0.
+000002a0: 0231 3007 0130 0a03 0701 3007 0135 0701  .10..0....0..5..
+000002b0: 350a 0307 0130 0701 3007 0231 300a 0307  5....0..0..10...
+000002c0: 0135 0701 3007 0135 8a3c 1c30 0126 2c2c  .5..0..5.<.0.&,,
+000002d0: 4c22 5b46 4249 8608 894e 840f 842f 881c  L"[FBI...N.../..
+000002e0: 8409 8807 8051 1b02 1602 8010 032a 011b  .....Q.......*..
+000002f0: 041c 0316 0359 8010 052a 011b 061c 0516  .....Y...*......
+00000300: 0559 8010 072a 011b 081c 0716 0759 481a  .Y...*.......YH.
+00000310: 8010 0910 0a10 0b2a 031b 0c1c 0916 091c  .......*........
+00000320: 0a16 0a1c 0b16 0b59 4a07 5951 160b 4a01  .......YJ.YQ..J.
+00000330: 5d48 0880 511b 0d16 0d4a 0759 5116 0d4a  ]H..Q....J.YQ..J
+00000340: 015d 5432 0010 0e34 0216 0e32 0116 0f32  .]T2...4...2...2
+00000350: 0216 1351 2a01 5333 0316 1632 0416 1b51  ...Q*.S3...2...Q
+00000360: 2a01 5333 0516 1e51 2a01 5333 0616 1f51  *.S3...Q*.S3...Q
+00000370: 6307 852c 0820 0e88 1723 2343 8812 6840  c..,. ...##C..h@
+00000380: 6840 6840 880f 113f 1640 100e 1641 5216  h@h@...?.@...AR.
+00000390: 1051 162a 5116 2d11 4232 0034 0116 2211  .Q.*Q.-.B2.4..".
+000003a0: 4232 0134 0116 2811 4232 0234 0116 2411  B2.4..(.B2.4..$.
+000003b0: 4232 0334 0116 2711 4232 0434 0116 2c11  B2.4..'.B2.4..,.
+000003c0: 4232 0534 0116 1151 6306 8540 1016 2280  B2.4...Qc..@..".
+000003d0: 1e46 2225 4d29 2e46 6912 0b51 de44 4251  .F"%M).Fi..Q.DBQ
+000003e0: 6312 0b34 00c0 b010 23d9 4450 120d 51de  c..4....#.DP..Q.
+000003f0: d344 4912 0e14 2436 0059 4266 120a 1025  .DI...$6.YBf...%
+00000400: 3401 1025 5551 ded3 4458 b010 26d9 4449  4..%UQ..DX..&.DI
+00000410: 120e 1427 3600 5942 4712 0e14 2836 0059  ...'6.YBG...(6.Y
+00000420: 4240 5163 8148 1006 2880 3012 0512 0910  B@Qc.H..(.0.....
+00000430: 2534 0112 0513 2934 0212 0e18 2a51 6381  %4....)4....*Qc.
+00000440: 0808 0624 8035 120d 142b 3600 120e 182a  ...$.5...+6....*
+00000450: 5163 8168 1808 2780 392b 1205 1209 1025  Qc.h..'.9+.....%
+00000460: 3401 3401 c012 07b0 8134 0212 0e18 2a51  4.4......4....*Q
+00000470: 6383 2c18 102c 803e 8308 2827 2e32 00c0  c.,..,.>..('.2..
+00000480: 120e 132d 51de 4447 b034 0012 0e18 2d12  ...-Q.DG.4....-.
+00000490: 0e13 2d14 2e36 0012 0e13 2a80 5612 0e13  ..-..6....*.V...
+000004a0: 2a14 2f36 0059 5163 0182 4080 4012 3e80  *./6.YQc..@.@.>.
+000004b0: 3f20 2424 2424 2423 0367 5923 0467 5923  ? $$$$$#.gY#.gY#
+000004c0: 0567 5923 0667 5923 0767 5923 0867 5942  .gY#.gY#.gY#.gYB
+000004d0: 2651 6388 28b8 0220 1180 4d60 4022 4c32  &Qc.(.. ..M`@"L2
+000004e0: 224c 2722 4e27 4d2c 484e 124a 120e 132a  "L'"N'M,HN.J...*
+000004f0: 1205 3402 4454 120e 132a 1430 120e 132a  ..4.DT...*.0...*
+00000500: 1430 3600 d336 0159 5263 124a 120e 132a  .06..6.YRc.J...*
+00000510: 1207 3402 4449 120e 142c 3600 5950 6312  ..4.DI...,6.YPc.
+00000520: 0d51 de43 5112 0e13 2a51 de43 4912 0d14  .Q.CQ...*Q.CI...
+00000530: 1136 0059 5063 4a20 5712 45df 4459 c049  .6.YPcJ W.E.DY.I
+00000540: 0f12 1b23 0214 12b0 3601 3401 5950 6351  ...#....6.4.YPcQ
+00000550: 51c0 2800 5d4a 015d 5163 8470 c902 140f  Q.(.]J.]Qc.p....
+00000560: 4380 6526 2227 2623 5212 0e13 1044 7948  C.e&"'&#R....DyH
+00000570: 1912 0e14 1136 00c1 1244 b034 0159 b144  .....6...D.4.Y.D
+00000580: 4712 0e14 1136 0059 4a1e 5712 45df 4457  G....6.YJ.W.E.DW
+00000590: c249 0d12 1b23 0014 12b2 3601 3401 5951  .I...#....6.4.YQ
+000005a0: 51c2 2802 5d4a 015d 5163 8374 db02 1e13  Q.(.]J.]Qc.t....
+000005b0: 4647 1d80 7480 0a88 1842 4a42 4c28 1014  FG..t....BJBL(..
+000005c0: 2a01 5333 00c3 4809 b3b0 b1b2 3403 594a  *.S3..H.....4.YJ
+000005d0: 1759 480b b3b0 b1b2 1015 3404 594a 0659  .YH.......4.YJ.Y
+000005e0: 5063 4a01 5d4a 015d 5263 018a 14fc 0528  PcJ.]J.]Rc.....(
+000005f0: 314b 4c4d 4e80 7f4a 295d 2949 4a26 2747  1KLMN..J)])IJ&'G
+00000600: 2528 4a48 b29e d844 439e 4241 b2c2 3200  %(JH...DC.BA..2.
+00000610: 1203 3400 3401 c410 3214 33b4 8083 2e02  ..4.4...2.3.....
+00000620: 5536 0110 34f2 1035 1433 b483 862e 0255  U6..4..5.3.....U
+00000630: 3601 f2c5 1249 b1b3 3402 474f c610 3614  6....I..4.GO..6.
+00000640: 12b5 b036 02c0 3201 b614 3736 0034 01c7  ...6..2...76.4..
+00000650: 124f b734 01c8 b714 38b0 3601 59b6 1439  .O.4....8.6.Y..9
+00000660: 8036 0159 b8b2 db44 52b7 b2d1 512e 0255  .6.Y...DR...Q..U
+00000670: c710 3a14 33b7 3601 c942 4810 3a14 33b7  ..:.3.6..BH.:.3.
+00000680: 3601 c9b6 142f b936 0159 515c 5d51 6302  6..../.6.YQ\]Qc.
+00000690: 8138 4108 3b50 8081 2b00 b05f 4b0a c112  .8A.;P..+.._K...
+000006a0: 51b1 3401 2f14 4234 6381 7841 083b 5080  Q.4./.B4c.xA.;P.
+000006b0: 872b 00b0 5f4b 12c1 1034 b1dd 4437 1032  .+.._K...4..D7.2
+000006c0: b1dd 4431 b12f 1442 2c63 8630 ca03 2416  ..D1./.B,c.0..$.
+000006d0: 4748 80a3 6020 2222 2a2a 424d 2548 2553  GH..` ""**BM%H%S
+000006e0: 2380 c248 4712 49b0 1017 3402 473a c3b3  #..HG.I...4.G:..
+000006f0: 1418 3600 1419 3600 c442 69b2 101a b4dd  ..6...6..Bi.....
+00000700: 4443 8142 4180 e5c2 b151 de44 4812 0fb4  DC.BA....Q.DH...
+00000710: 3401 5942 45b1 b434 0159 b314 1836 0014  4.YBE..4.Y...6..
+00000720: 1936 00c4 b443 1451 5c5d 4a04 594a 015d  .6...C.Q\]J.YJ.]
+00000730: b263 8138 310e 1b46 80bf 6020 2310 1cc1  .c.81..F..` #...
+00000740: 1213 b0b1 101d 8534 8202 6381 28a9 010c  .......4..c.(...
+00000750: 1e48 80c8 2347 101c c112 16b1 b034 02c2  .H..#G.......4..
+00000760: b263 841c d101 141f 4880 cf2b 2528 2548  .c......H..+%(%H
+00000770: 2532 0012 0214 2036 0034 01c1 b15f 4b25  %2.... 6.4..._K%
+00000780: c223 0114 12b2 3601 c3b0 51de 4448 120f  .#....6...Q.DH..
+00000790: b334 0159 4245 b0b3 3401 5912 0214 21b2  .4.YBE..4.Y...!.
+000007a0: 3601 5942 1951 6301 8160 4908 3b50 80cf  6.YB.Qc..`I.;P..
+000007b0: 2b00 b05f 4b0f c1b1 143c 103d 3601 4434  +.._K....<.=6.D4
+000007c0: b12f 1442 2f63                           ./.B/c
```

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/Hooks.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/Hooks.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/InterConnect.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/InterConnect.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/InterpreterShell.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/InterpreterShell.mpy`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 00000040: 6366 6770 7574 001a 436f 6e66 6967 4861  cfgput..ConfigHa
 00000050: 6e64 6c65 7200 1865 7865 635f 6c6d 5f63  ndler..exec_lm_c
 00000060: 6f72 6500 1654 6173 6b4d 616e 6167 6572  ore..TaskManager
 00000070: 001a 636f 6e73 6f6c 655f 7772 6974 6500  ..console_write.
 00000080: 1465 7272 6c6f 675f 6164 6400 0a44 6562  .errlog_add..Deb
 00000090: 7567 000a 7265 7365 7400 1473 6f66 745f  ug..reset..soft_
 000000a0: 7265 7365 7400 0e6d 6163 6869 6e65 000a  reset..machine..
-000000b0: 5368 656c 6c00 1031 2e32 312e 302d 3000  Shell..1.21.0-0.
+000000b0: 5368 656c 6c00 1031 2e32 312e 302d 3100  Shell..1.21.0-1.
 000000c0: 230e 6d73 675f 6f62 6a00 0c64 6576 6669  #.msg_obj..devfi
 000000d0: 6400 105f 5f64 6576 6669 6400 0861 7574  d..__devfid..aut
 000000e0: 6800 165f 5f61 7574 685f 6d6f 6465 000a  h..__auth_mode..
 000000f0: 6877 7569 6400 0e5f 5f68 7775 6964 0012  hwuid..__hwuid..
 00000100: 5f5f 6175 7468 5f6f 6b00 165f 5f63 6f6e  __auth_ok..__con
 00000110: 665f 6d6f 6465 000e 7665 7273 696f 6e00  f_mode..version.
 00000120: 1c4d 4943 524f 535f 5645 5253 494f 4e00  .MICROS_VERSION.
```

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/InterruptHandler.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/InterruptHandler.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_L9110_DCmotor.py` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_L9110_DCmotor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_VL53L0X.py` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_VL53L0X.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_bme280.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_bme280.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_buzzer.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_buzzer.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_catgame.py` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_catgame.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_cct.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_cct.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_co2.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_co2.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_demo.py` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_demo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_dht11.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_dht11.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_dht22.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_dht22.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_dimmer.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_dimmer.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_distance.py` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_distance.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_ds18.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_ds18.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_esp32.py` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_esp32.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_genIO.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_genIO.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_i2c.py` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_i2c.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_intercon.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_intercon.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_light_sensor.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_light_sensor.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_lmpacman.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_lmpacman.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_neoeffects.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_neoeffects.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_neopixel.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_neopixel.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_oled.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_oled.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_oled_sh1106.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_oled_sh1106.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_oled_ui.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_oled_ui.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_pet_feeder.py` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_pet_feeder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_ph_sensor.py` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_ph_sensor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_presence.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_presence.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_rencoder.py` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_rencoder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_rgb.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_rgb.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_roboarm.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_roboarm.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_robustness.py` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_robustness.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_servo.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_servo.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_stepper.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_stepper.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_switch.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_switch.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_system.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_system.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_telegram.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_telegram.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_tinyrgb.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LM_tinyrgb.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LP_esp32.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LP_esp32.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LP_esp32s2.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LP_esp32s2.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LP_esp32s3.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LP_esp32s3.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LogicalPins.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/LogicalPins.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/Network.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/Network.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/Notify.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/Notify.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/Scheduler.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/Scheduler.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/SocketServer.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/SocketServer.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/TaskManager.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/TaskManager.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/Time.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/Time.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/micrOS.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/micrOS.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/micrOSloader.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/micrOSloader.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/urequests.mpy` & `micrOSDevToolKit-1.21.1/toolkit/workspace/precompiled/urequests.mpy`

 * *Files identical despite different names*

