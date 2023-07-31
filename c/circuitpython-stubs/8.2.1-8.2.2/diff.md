# Comparing `tmp/circuitpython-stubs-8.2.1.tar.gz` & `tmp/circuitpython-stubs-8.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-stubs-8.2.1.tar", last modified: Tue Jul 25 16:37:31 2023, max compression
+gzip compressed data, was "circuitpython-stubs-8.2.2.tar", last modified: Mon Jul 31 22:21:15 2023, max compression
```

## Comparing `circuitpython-stubs-8.2.1.tar` & `circuitpython-stubs-8.2.2.tar`

### file list

```diff
@@ -1,232 +1,232 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.534528 circuitpython-stubs-8.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-25 16:37:21.000000 circuitpython-stubs-8.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-25 16:37:31.530528 circuitpython-stubs-8.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-25 16:37:21.000000 circuitpython-stubs-8.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.510528 circuitpython-stubs-8.2.1/_bleio/
--rw-r--r--   0 runner    (1001) docker     (123)    31094 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/_bleio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.510528 circuitpython-stubs-8.2.1/_eve/
--rw-r--r--   0 runner    (1001) docker     (123)    20379 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/_eve/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.510528 circuitpython-stubs-8.2.1/_pew/
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/_pew/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.510528 circuitpython-stubs-8.2.1/_pixelmap/
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/_pixelmap/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.510528 circuitpython-stubs-8.2.1/_stage/
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/_stage/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.510528 circuitpython-stubs-8.2.1/adafruit_bus_device/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/adafruit_bus_device/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.510528 circuitpython-stubs-8.2.1/adafruit_bus_device/i2c_device/
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/adafruit_bus_device/i2c_device/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.510528 circuitpython-stubs-8.2.1/adafruit_bus_device/spi_device/
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/adafruit_bus_device/spi_device/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.510528 circuitpython-stubs-8.2.1/adafruit_pixelbuf/
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/adafruit_pixelbuf/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.510528 circuitpython-stubs-8.2.1/aesio/
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/aesio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.510528 circuitpython-stubs-8.2.1/alarm/
--rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/alarm/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.510528 circuitpython-stubs-8.2.1/alarm/pin/
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/alarm/pin/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.510528 circuitpython-stubs-8.2.1/alarm/time/
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/alarm/time/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.510528 circuitpython-stubs-8.2.1/alarm/touch/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/alarm/touch/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.510528 circuitpython-stubs-8.2.1/analogbufio/
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/analogbufio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.510528 circuitpython-stubs-8.2.1/analogio/
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/analogio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.510528 circuitpython-stubs-8.2.1/atexit/
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/atexit/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.510528 circuitpython-stubs-8.2.1/audiobusio/
--rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/audiobusio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.510528 circuitpython-stubs-8.2.1/audiocore/
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/audiocore/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.510528 circuitpython-stubs-8.2.1/audioio/
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/audioio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.514528 circuitpython-stubs-8.2.1/audiomixer/
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/audiomixer/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.514528 circuitpython-stubs-8.2.1/audiomp3/
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/audiomp3/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.514528 circuitpython-stubs-8.2.1/audiopwmio/
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/audiopwmio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.514528 circuitpython-stubs-8.2.1/bitbangio/
--rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/bitbangio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.514528 circuitpython-stubs-8.2.1/bitmaptools/
--rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/bitmaptools/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.514528 circuitpython-stubs-8.2.1/bitops/
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/bitops/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.514528 circuitpython-stubs-8.2.1/board/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/board/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.514528 circuitpython-stubs-8.2.1/busio/
--rw-r--r--   0 runner    (1001) docker     (123)    20590 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/busio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.514528 circuitpython-stubs-8.2.1/camera/
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/camera/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.514528 circuitpython-stubs-8.2.1/canio/
--rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/canio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.530528 circuitpython-stubs-8.2.1/circuitpython_stubs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-25 16:37:30.000000 circuitpython-stubs-8.2.1/circuitpython_stubs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-07-25 16:37:31.000000 circuitpython-stubs-8.2.1/circuitpython_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 16:37:30.000000 circuitpython-stubs-8.2.1/circuitpython_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 16:37:30.000000 circuitpython-stubs-8.2.1/circuitpython_stubs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-25 16:37:30.000000 circuitpython-stubs-8.2.1/circuitpython_stubs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.514528 circuitpython-stubs-8.2.1/countio/
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/countio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.514528 circuitpython-stubs-8.2.1/cyw43/
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-25 16:37:21.000000 circuitpython-stubs-8.2.1/cyw43/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.514528 circuitpython-stubs-8.2.1/digitalio/
--rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/digitalio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.514528 circuitpython-stubs-8.2.1/displayio/
--rw-r--r--   0 runner    (1001) docker     (123)    40379 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/displayio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.514528 circuitpython-stubs-8.2.1/dualbank/
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/dualbank/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.514528 circuitpython-stubs-8.2.1/espcamera/
--rw-r--r--   0 runner    (1001) docker     (123)    11830 2023-07-25 16:37:21.000000 circuitpython-stubs-8.2.1/espcamera/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.514528 circuitpython-stubs-8.2.1/espidf/
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-07-25 16:37:21.000000 circuitpython-stubs-8.2.1/espidf/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.514528 circuitpython-stubs-8.2.1/espnow/
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-07-25 16:37:21.000000 circuitpython-stubs-8.2.1/espnow/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.514528 circuitpython-stubs-8.2.1/espulp/
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-07-25 16:37:21.000000 circuitpython-stubs-8.2.1/espulp/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.514528 circuitpython-stubs-8.2.1/floppyio/
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/floppyio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.514528 circuitpython-stubs-8.2.1/fontio/
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/fontio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/framebufferio/
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/framebufferio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/frequencyio/
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/frequencyio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/getpass/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/getpass/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/gifio/
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/gifio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/gnss/
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/gnss/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/hashlib/
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/hashlib/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/i2ctarget/
--rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/i2ctarget/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/imagecapture/
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/imagecapture/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/ipaddress/
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/ipaddress/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/is31fl3741/
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/is31fl3741/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/keypad/
--rw-r--r--   0 runner    (1001) docker     (123)    13945 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/keypad/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/math/
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/math/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/mdns/
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/mdns/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/memorymap/
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/memorymap/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/memorymonitor/
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/memorymonitor/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/microcontroller/
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/microcontroller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/msgpack/
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/msgpack/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/neopixel_write/
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/neopixel_write/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/nvm/
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/nvm/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/onewireio/
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/onewireio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/os/
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/os/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/paralleldisplay/
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/paralleldisplay/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/picodvi/
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-07-25 16:37:21.000000 circuitpython-stubs-8.2.1/picodvi/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.522528 circuitpython-stubs-8.2.1/ps2io/
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/ps2io/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.522528 circuitpython-stubs-8.2.1/pulseio/
--rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/pulseio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.522528 circuitpython-stubs-8.2.1/pwmio/
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/pwmio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.522528 circuitpython-stubs-8.2.1/qrio/
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/qrio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.522528 circuitpython-stubs-8.2.1/rainbowio/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/rainbowio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.522528 circuitpython-stubs-8.2.1/random/
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/random/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.522528 circuitpython-stubs-8.2.1/rgbmatrix/
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/rgbmatrix/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.522528 circuitpython-stubs-8.2.1/rotaryio/
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/rotaryio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.522528 circuitpython-stubs-8.2.1/rp2pio/
--rw-r--r--   0 runner    (1001) docker     (123)    16742 2023-07-25 16:37:21.000000 circuitpython-stubs-8.2.1/rp2pio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.522528 circuitpython-stubs-8.2.1/rtc/
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/rtc/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.522528 circuitpython-stubs-8.2.1/samd/
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/samd/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.522528 circuitpython-stubs-8.2.1/sdcardio/
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/sdcardio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.522528 circuitpython-stubs-8.2.1/sdioio/
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/sdioio/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 16:37:31.534528 circuitpython-stubs-8.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-25 16:37:21.000000 circuitpython-stubs-8.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.522528 circuitpython-stubs-8.2.1/sharpdisplay/
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/sharpdisplay/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.522528 circuitpython-stubs-8.2.1/socketpool/
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/socketpool/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.522528 circuitpython-stubs-8.2.1/ssl/
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/ssl/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.522528 circuitpython-stubs-8.2.1/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/storage/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.522528 circuitpython-stubs-8.2.1/struct/
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/struct/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.522528 circuitpython-stubs-8.2.1/supervisor/
--rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/supervisor/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.522528 circuitpython-stubs-8.2.1/synthio/
--rw-r--r--   0 runner    (1001) docker     (123)    22728 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/synthio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.522528 circuitpython-stubs-8.2.1/terminalio/
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/terminalio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.526528 circuitpython-stubs-8.2.1/time/
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/time/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.526528 circuitpython-stubs-8.2.1/touchio/
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/touchio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.526528 circuitpython-stubs-8.2.1/traceback/
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/traceback/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.526528 circuitpython-stubs-8.2.1/uheap/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/uheap/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.526528 circuitpython-stubs-8.2.1/ulab/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/ulab/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.526528 circuitpython-stubs-8.2.1/ulab/numpy/
--rw-r--r--   0 runner    (1001) docker     (123)    15556 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/ulab/numpy/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.526528 circuitpython-stubs-8.2.1/ulab/numpy/carray/
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/ulab/numpy/carray/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.526528 circuitpython-stubs-8.2.1/ulab/numpy/fft/
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/ulab/numpy/fft/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.526528 circuitpython-stubs-8.2.1/ulab/numpy/linalg/
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/ulab/numpy/linalg/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.526528 circuitpython-stubs-8.2.1/ulab/scipy/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/ulab/scipy/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.526528 circuitpython-stubs-8.2.1/ulab/scipy/linalg/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/ulab/scipy/linalg/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.526528 circuitpython-stubs-8.2.1/ulab/scipy/optimize/
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/ulab/scipy/optimize/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.526528 circuitpython-stubs-8.2.1/ulab/user/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/ulab/user/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.526528 circuitpython-stubs-8.2.1/ulab/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/ulab/utils/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.526528 circuitpython-stubs-8.2.1/usb/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/usb/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.526528 circuitpython-stubs-8.2.1/usb/core/
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/usb/core/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.526528 circuitpython-stubs-8.2.1/usb_cdc/
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/usb_cdc/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.526528 circuitpython-stubs-8.2.1/usb_hid/
--rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/usb_hid/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.526528 circuitpython-stubs-8.2.1/usb_host/
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/usb_host/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.526528 circuitpython-stubs-8.2.1/usb_midi/
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/usb_midi/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.526528 circuitpython-stubs-8.2.1/ustack/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/ustack/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.526528 circuitpython-stubs-8.2.1/vectorio/
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/vectorio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.530528 circuitpython-stubs-8.2.1/watchdog/
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/watchdog/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.530528 circuitpython-stubs-8.2.1/wifi/
--rw-r--r--   0 runner    (1001) docker     (123)    11022 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/wifi/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.530528 circuitpython-stubs-8.2.1/zlib/
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/zlib/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.547826 circuitpython-stubs-8.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-31 22:21:05.000000 circuitpython-stubs-8.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-31 22:21:15.547826 circuitpython-stubs-8.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-31 22:21:05.000000 circuitpython-stubs-8.2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.523826 circuitpython-stubs-8.2.2/_bleio/
+-rw-r--r--   0 runner    (1001) docker     (123)    31094 2023-07-31 22:21:01.000000 circuitpython-stubs-8.2.2/_bleio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.523826 circuitpython-stubs-8.2.2/_eve/
+-rw-r--r--   0 runner    (1001) docker     (123)    20379 2023-07-31 22:21:02.000000 circuitpython-stubs-8.2.2/_eve/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.523826 circuitpython-stubs-8.2.2/_pew/
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-31 22:21:02.000000 circuitpython-stubs-8.2.2/_pew/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.523826 circuitpython-stubs-8.2.2/_pixelmap/
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-31 22:21:02.000000 circuitpython-stubs-8.2.2/_pixelmap/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.523826 circuitpython-stubs-8.2.2/_stage/
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-07-31 22:21:02.000000 circuitpython-stubs-8.2.2/_stage/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.523826 circuitpython-stubs-8.2.2/adafruit_bus_device/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-31 22:21:02.000000 circuitpython-stubs-8.2.2/adafruit_bus_device/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.523826 circuitpython-stubs-8.2.2/adafruit_bus_device/i2c_device/
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-07-31 22:21:02.000000 circuitpython-stubs-8.2.2/adafruit_bus_device/i2c_device/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.523826 circuitpython-stubs-8.2.2/adafruit_bus_device/spi_device/
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-31 22:21:02.000000 circuitpython-stubs-8.2.2/adafruit_bus_device/spi_device/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.523826 circuitpython-stubs-8.2.2/adafruit_pixelbuf/
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-07-31 22:21:02.000000 circuitpython-stubs-8.2.2/adafruit_pixelbuf/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.523826 circuitpython-stubs-8.2.2/aesio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-31 22:21:02.000000 circuitpython-stubs-8.2.2/aesio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.523826 circuitpython-stubs-8.2.2/alarm/
+-rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-07-31 22:21:02.000000 circuitpython-stubs-8.2.2/alarm/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.523826 circuitpython-stubs-8.2.2/alarm/pin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-31 22:21:02.000000 circuitpython-stubs-8.2.2/alarm/pin/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.523826 circuitpython-stubs-8.2.2/alarm/time/
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-31 22:21:02.000000 circuitpython-stubs-8.2.2/alarm/time/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.523826 circuitpython-stubs-8.2.2/alarm/touch/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-31 22:21:02.000000 circuitpython-stubs-8.2.2/alarm/touch/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.523826 circuitpython-stubs-8.2.2/analogbufio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-07-31 22:21:02.000000 circuitpython-stubs-8.2.2/analogbufio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.523826 circuitpython-stubs-8.2.2/analogio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-07-31 22:21:02.000000 circuitpython-stubs-8.2.2/analogio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.523826 circuitpython-stubs-8.2.2/atexit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-31 22:21:02.000000 circuitpython-stubs-8.2.2/atexit/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.523826 circuitpython-stubs-8.2.2/audiobusio/
+-rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-07-31 22:21:02.000000 circuitpython-stubs-8.2.2/audiobusio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.527826 circuitpython-stubs-8.2.2/audiocore/
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-07-31 22:21:02.000000 circuitpython-stubs-8.2.2/audiocore/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.527826 circuitpython-stubs-8.2.2/audioio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-07-31 22:21:02.000000 circuitpython-stubs-8.2.2/audioio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.527826 circuitpython-stubs-8.2.2/audiomixer/
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-07-31 22:21:02.000000 circuitpython-stubs-8.2.2/audiomixer/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.527826 circuitpython-stubs-8.2.2/audiomp3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-07-31 22:21:02.000000 circuitpython-stubs-8.2.2/audiomp3/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.527826 circuitpython-stubs-8.2.2/audiopwmio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-07-31 22:21:02.000000 circuitpython-stubs-8.2.2/audiopwmio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.527826 circuitpython-stubs-8.2.2/bitbangio/
+-rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-07-31 22:21:02.000000 circuitpython-stubs-8.2.2/bitbangio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.527826 circuitpython-stubs-8.2.2/bitmaptools/
+-rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-07-31 22:21:02.000000 circuitpython-stubs-8.2.2/bitmaptools/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.527826 circuitpython-stubs-8.2.2/bitops/
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-31 22:21:02.000000 circuitpython-stubs-8.2.2/bitops/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.527826 circuitpython-stubs-8.2.2/board/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-31 22:21:02.000000 circuitpython-stubs-8.2.2/board/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.527826 circuitpython-stubs-8.2.2/busio/
+-rw-r--r--   0 runner    (1001) docker     (123)    20590 2023-07-31 22:21:02.000000 circuitpython-stubs-8.2.2/busio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.527826 circuitpython-stubs-8.2.2/camera/
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-31 22:21:02.000000 circuitpython-stubs-8.2.2/camera/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.527826 circuitpython-stubs-8.2.2/canio/
+-rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-07-31 22:21:02.000000 circuitpython-stubs-8.2.2/canio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.543826 circuitpython-stubs-8.2.2/circuitpython_stubs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-31 22:21:14.000000 circuitpython-stubs-8.2.2/circuitpython_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-07-31 22:21:15.000000 circuitpython-stubs-8.2.2/circuitpython_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 22:21:14.000000 circuitpython-stubs-8.2.2/circuitpython_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 22:21:14.000000 circuitpython-stubs-8.2.2/circuitpython_stubs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-31 22:21:14.000000 circuitpython-stubs-8.2.2/circuitpython_stubs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.527826 circuitpython-stubs-8.2.2/countio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-07-31 22:21:02.000000 circuitpython-stubs-8.2.2/countio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.527826 circuitpython-stubs-8.2.2/cyw43/
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-31 22:21:05.000000 circuitpython-stubs-8.2.2/cyw43/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.527826 circuitpython-stubs-8.2.2/digitalio/
+-rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-07-31 22:21:02.000000 circuitpython-stubs-8.2.2/digitalio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.527826 circuitpython-stubs-8.2.2/displayio/
+-rw-r--r--   0 runner    (1001) docker     (123)    40379 2023-07-31 22:21:02.000000 circuitpython-stubs-8.2.2/displayio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.527826 circuitpython-stubs-8.2.2/dualbank/
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-31 22:21:02.000000 circuitpython-stubs-8.2.2/dualbank/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.527826 circuitpython-stubs-8.2.2/espcamera/
+-rw-r--r--   0 runner    (1001) docker     (123)    11830 2023-07-31 22:21:05.000000 circuitpython-stubs-8.2.2/espcamera/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.527826 circuitpython-stubs-8.2.2/espidf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-07-31 22:21:05.000000 circuitpython-stubs-8.2.2/espidf/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.527826 circuitpython-stubs-8.2.2/espnow/
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-07-31 22:21:05.000000 circuitpython-stubs-8.2.2/espnow/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.531826 circuitpython-stubs-8.2.2/espulp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-07-31 22:21:05.000000 circuitpython-stubs-8.2.2/espulp/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.531826 circuitpython-stubs-8.2.2/floppyio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-31 22:21:02.000000 circuitpython-stubs-8.2.2/floppyio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.531826 circuitpython-stubs-8.2.2/fontio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-07-31 22:21:02.000000 circuitpython-stubs-8.2.2/fontio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.531826 circuitpython-stubs-8.2.2/framebufferio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-07-31 22:21:02.000000 circuitpython-stubs-8.2.2/framebufferio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.531826 circuitpython-stubs-8.2.2/frequencyio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-07-31 22:21:02.000000 circuitpython-stubs-8.2.2/frequencyio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.531826 circuitpython-stubs-8.2.2/getpass/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-31 22:21:02.000000 circuitpython-stubs-8.2.2/getpass/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.531826 circuitpython-stubs-8.2.2/gifio/
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-07-31 22:21:02.000000 circuitpython-stubs-8.2.2/gifio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.531826 circuitpython-stubs-8.2.2/gnss/
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-31 22:21:02.000000 circuitpython-stubs-8.2.2/gnss/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.531826 circuitpython-stubs-8.2.2/hashlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/hashlib/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.531826 circuitpython-stubs-8.2.2/i2ctarget/
+-rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/i2ctarget/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.531826 circuitpython-stubs-8.2.2/imagecapture/
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/imagecapture/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.531826 circuitpython-stubs-8.2.2/ipaddress/
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/ipaddress/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.531826 circuitpython-stubs-8.2.2/is31fl3741/
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/is31fl3741/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.531826 circuitpython-stubs-8.2.2/keypad/
+-rw-r--r--   0 runner    (1001) docker     (123)    13945 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/keypad/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.531826 circuitpython-stubs-8.2.2/math/
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/math/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.531826 circuitpython-stubs-8.2.2/mdns/
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/mdns/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.531826 circuitpython-stubs-8.2.2/memorymap/
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/memorymap/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.531826 circuitpython-stubs-8.2.2/memorymonitor/
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/memorymonitor/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.531826 circuitpython-stubs-8.2.2/microcontroller/
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/microcontroller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.531826 circuitpython-stubs-8.2.2/msgpack/
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/msgpack/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.531826 circuitpython-stubs-8.2.2/neopixel_write/
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/neopixel_write/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.531826 circuitpython-stubs-8.2.2/nvm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/nvm/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.531826 circuitpython-stubs-8.2.2/onewireio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/onewireio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.535826 circuitpython-stubs-8.2.2/os/
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/os/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.535826 circuitpython-stubs-8.2.2/paralleldisplay/
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/paralleldisplay/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.535826 circuitpython-stubs-8.2.2/picodvi/
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-07-31 22:21:05.000000 circuitpython-stubs-8.2.2/picodvi/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.535826 circuitpython-stubs-8.2.2/ps2io/
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/ps2io/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.535826 circuitpython-stubs-8.2.2/pulseio/
+-rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/pulseio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.535826 circuitpython-stubs-8.2.2/pwmio/
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/pwmio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.535826 circuitpython-stubs-8.2.2/qrio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/qrio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.535826 circuitpython-stubs-8.2.2/rainbowio/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/rainbowio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.535826 circuitpython-stubs-8.2.2/random/
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/random/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.535826 circuitpython-stubs-8.2.2/rgbmatrix/
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/rgbmatrix/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.535826 circuitpython-stubs-8.2.2/rotaryio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/rotaryio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.535826 circuitpython-stubs-8.2.2/rp2pio/
+-rw-r--r--   0 runner    (1001) docker     (123)    16742 2023-07-31 22:21:05.000000 circuitpython-stubs-8.2.2/rp2pio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.535826 circuitpython-stubs-8.2.2/rtc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/rtc/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.535826 circuitpython-stubs-8.2.2/samd/
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-31 22:21:04.000000 circuitpython-stubs-8.2.2/samd/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.535826 circuitpython-stubs-8.2.2/sdcardio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/sdcardio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.535826 circuitpython-stubs-8.2.2/sdioio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/sdioio/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 22:21:15.547826 circuitpython-stubs-8.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-31 22:21:05.000000 circuitpython-stubs-8.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.535826 circuitpython-stubs-8.2.2/sharpdisplay/
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/sharpdisplay/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.535826 circuitpython-stubs-8.2.2/socketpool/
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/socketpool/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.535826 circuitpython-stubs-8.2.2/ssl/
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/ssl/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.535826 circuitpython-stubs-8.2.2/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/storage/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.535826 circuitpython-stubs-8.2.2/struct/
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/struct/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.539826 circuitpython-stubs-8.2.2/supervisor/
+-rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/supervisor/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.539826 circuitpython-stubs-8.2.2/synthio/
+-rw-r--r--   0 runner    (1001) docker     (123)    22728 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/synthio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.539826 circuitpython-stubs-8.2.2/terminalio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/terminalio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.539826 circuitpython-stubs-8.2.2/time/
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/time/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.539826 circuitpython-stubs-8.2.2/touchio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/touchio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.539826 circuitpython-stubs-8.2.2/traceback/
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/traceback/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.539826 circuitpython-stubs-8.2.2/uheap/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/uheap/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.539826 circuitpython-stubs-8.2.2/ulab/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-31 22:21:04.000000 circuitpython-stubs-8.2.2/ulab/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.539826 circuitpython-stubs-8.2.2/ulab/numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)    15556 2023-07-31 22:21:04.000000 circuitpython-stubs-8.2.2/ulab/numpy/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.539826 circuitpython-stubs-8.2.2/ulab/numpy/carray/
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-31 22:21:04.000000 circuitpython-stubs-8.2.2/ulab/numpy/carray/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.539826 circuitpython-stubs-8.2.2/ulab/numpy/fft/
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-31 22:21:04.000000 circuitpython-stubs-8.2.2/ulab/numpy/fft/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.539826 circuitpython-stubs-8.2.2/ulab/numpy/linalg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-07-31 22:21:04.000000 circuitpython-stubs-8.2.2/ulab/numpy/linalg/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.539826 circuitpython-stubs-8.2.2/ulab/scipy/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-31 22:21:04.000000 circuitpython-stubs-8.2.2/ulab/scipy/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.539826 circuitpython-stubs-8.2.2/ulab/scipy/linalg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-31 22:21:04.000000 circuitpython-stubs-8.2.2/ulab/scipy/linalg/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.539826 circuitpython-stubs-8.2.2/ulab/scipy/optimize/
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-31 22:21:04.000000 circuitpython-stubs-8.2.2/ulab/scipy/optimize/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.539826 circuitpython-stubs-8.2.2/ulab/user/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-31 22:21:04.000000 circuitpython-stubs-8.2.2/ulab/user/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.539826 circuitpython-stubs-8.2.2/ulab/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-31 22:21:04.000000 circuitpython-stubs-8.2.2/ulab/utils/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.539826 circuitpython-stubs-8.2.2/usb/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/usb/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.539826 circuitpython-stubs-8.2.2/usb/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/usb/core/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.543826 circuitpython-stubs-8.2.2/usb_cdc/
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/usb_cdc/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.543826 circuitpython-stubs-8.2.2/usb_hid/
+-rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/usb_hid/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.543826 circuitpython-stubs-8.2.2/usb_host/
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/usb_host/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.543826 circuitpython-stubs-8.2.2/usb_midi/
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/usb_midi/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.543826 circuitpython-stubs-8.2.2/ustack/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-31 22:21:03.000000 circuitpython-stubs-8.2.2/ustack/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.543826 circuitpython-stubs-8.2.2/vectorio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-07-31 22:21:04.000000 circuitpython-stubs-8.2.2/vectorio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.543826 circuitpython-stubs-8.2.2/watchdog/
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-07-31 22:21:04.000000 circuitpython-stubs-8.2.2/watchdog/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.543826 circuitpython-stubs-8.2.2/wifi/
+-rw-r--r--   0 runner    (1001) docker     (123)    11022 2023-07-31 22:21:04.000000 circuitpython-stubs-8.2.2/wifi/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:21:15.543826 circuitpython-stubs-8.2.2/zlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-31 22:21:04.000000 circuitpython-stubs-8.2.2/zlib/__init__.pyi
```

### Comparing `circuitpython-stubs-8.2.1/README.rst` & `circuitpython-stubs-8.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/_bleio/__init__.pyi` & `circuitpython-stubs-8.2.2/_bleio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/_eve/__init__.pyi` & `circuitpython-stubs-8.2.2/_eve/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/_pew/__init__.pyi` & `circuitpython-stubs-8.2.2/_pew/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/_pixelmap/__init__.pyi` & `circuitpython-stubs-8.2.2/_pixelmap/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/_stage/__init__.pyi` & `circuitpython-stubs-8.2.2/_stage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/adafruit_bus_device/i2c_device/__init__.pyi` & `circuitpython-stubs-8.2.2/adafruit_bus_device/i2c_device/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/adafruit_bus_device/spi_device/__init__.pyi` & `circuitpython-stubs-8.2.2/adafruit_bus_device/spi_device/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/adafruit_pixelbuf/__init__.pyi` & `circuitpython-stubs-8.2.2/adafruit_pixelbuf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/aesio/__init__.pyi` & `circuitpython-stubs-8.2.2/aesio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/alarm/__init__.pyi` & `circuitpython-stubs-8.2.2/alarm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/alarm/pin/__init__.pyi` & `circuitpython-stubs-8.2.2/alarm/pin/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/alarm/time/__init__.pyi` & `circuitpython-stubs-8.2.2/alarm/time/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/alarm/touch/__init__.pyi` & `circuitpython-stubs-8.2.2/alarm/touch/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/analogbufio/__init__.pyi` & `circuitpython-stubs-8.2.2/analogbufio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/analogio/__init__.pyi` & `circuitpython-stubs-8.2.2/analogio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/atexit/__init__.pyi` & `circuitpython-stubs-8.2.2/atexit/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/audiobusio/__init__.pyi` & `circuitpython-stubs-8.2.2/audiobusio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/audiocore/__init__.pyi` & `circuitpython-stubs-8.2.2/audiocore/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/audioio/__init__.pyi` & `circuitpython-stubs-8.2.2/audioio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/audiomixer/__init__.pyi` & `circuitpython-stubs-8.2.2/audiomixer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/audiomp3/__init__.pyi` & `circuitpython-stubs-8.2.2/audiomp3/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/audiopwmio/__init__.pyi` & `circuitpython-stubs-8.2.2/audiopwmio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/bitbangio/__init__.pyi` & `circuitpython-stubs-8.2.2/bitbangio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/bitmaptools/__init__.pyi` & `circuitpython-stubs-8.2.2/bitmaptools/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/bitops/__init__.pyi` & `circuitpython-stubs-8.2.2/bitops/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/board/__init__.pyi` & `circuitpython-stubs-8.2.2/board/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/busio/__init__.pyi` & `circuitpython-stubs-8.2.2/busio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/camera/__init__.pyi` & `circuitpython-stubs-8.2.2/camera/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/canio/__init__.pyi` & `circuitpython-stubs-8.2.2/canio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/circuitpython_stubs.egg-info/SOURCES.txt` & `circuitpython-stubs-8.2.2/circuitpython_stubs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/circuitpython_stubs.egg-info/top_level.txt` & `circuitpython-stubs-8.2.2/circuitpython_stubs.egg-info/top_level.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/countio/__init__.pyi` & `circuitpython-stubs-8.2.2/countio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/cyw43/__init__.pyi` & `circuitpython-stubs-8.2.2/cyw43/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/digitalio/__init__.pyi` & `circuitpython-stubs-8.2.2/digitalio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/displayio/__init__.pyi` & `circuitpython-stubs-8.2.2/displayio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/dualbank/__init__.pyi` & `circuitpython-stubs-8.2.2/dualbank/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/espcamera/__init__.pyi` & `circuitpython-stubs-8.2.2/espcamera/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/espidf/__init__.pyi` & `circuitpython-stubs-8.2.2/espidf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/espnow/__init__.pyi` & `circuitpython-stubs-8.2.2/espnow/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/espulp/__init__.pyi` & `circuitpython-stubs-8.2.2/espulp/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/floppyio/__init__.pyi` & `circuitpython-stubs-8.2.2/floppyio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/fontio/__init__.pyi` & `circuitpython-stubs-8.2.2/fontio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/framebufferio/__init__.pyi` & `circuitpython-stubs-8.2.2/framebufferio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/frequencyio/__init__.pyi` & `circuitpython-stubs-8.2.2/frequencyio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/getpass/__init__.pyi` & `circuitpython-stubs-8.2.2/getpass/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/gifio/__init__.pyi` & `circuitpython-stubs-8.2.2/gifio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/gnss/__init__.pyi` & `circuitpython-stubs-8.2.2/gnss/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/hashlib/__init__.pyi` & `circuitpython-stubs-8.2.2/hashlib/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/i2ctarget/__init__.pyi` & `circuitpython-stubs-8.2.2/i2ctarget/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/imagecapture/__init__.pyi` & `circuitpython-stubs-8.2.2/imagecapture/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/ipaddress/__init__.pyi` & `circuitpython-stubs-8.2.2/ipaddress/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/is31fl3741/__init__.pyi` & `circuitpython-stubs-8.2.2/is31fl3741/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/keypad/__init__.pyi` & `circuitpython-stubs-8.2.2/keypad/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/math/__init__.pyi` & `circuitpython-stubs-8.2.2/math/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/mdns/__init__.pyi` & `circuitpython-stubs-8.2.2/mdns/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/memorymap/__init__.pyi` & `circuitpython-stubs-8.2.2/memorymap/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/memorymonitor/__init__.pyi` & `circuitpython-stubs-8.2.2/memorymonitor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/microcontroller/__init__.pyi` & `circuitpython-stubs-8.2.2/microcontroller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/msgpack/__init__.pyi` & `circuitpython-stubs-8.2.2/msgpack/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/neopixel_write/__init__.pyi` & `circuitpython-stubs-8.2.2/neopixel_write/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/nvm/__init__.pyi` & `circuitpython-stubs-8.2.2/nvm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/onewireio/__init__.pyi` & `circuitpython-stubs-8.2.2/onewireio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/os/__init__.pyi` & `circuitpython-stubs-8.2.2/os/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/paralleldisplay/__init__.pyi` & `circuitpython-stubs-8.2.2/paralleldisplay/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/picodvi/__init__.pyi` & `circuitpython-stubs-8.2.2/picodvi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/ps2io/__init__.pyi` & `circuitpython-stubs-8.2.2/ps2io/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/pulseio/__init__.pyi` & `circuitpython-stubs-8.2.2/pulseio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/pwmio/__init__.pyi` & `circuitpython-stubs-8.2.2/pwmio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/qrio/__init__.pyi` & `circuitpython-stubs-8.2.2/qrio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/random/__init__.pyi` & `circuitpython-stubs-8.2.2/random/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/rgbmatrix/__init__.pyi` & `circuitpython-stubs-8.2.2/rgbmatrix/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/rotaryio/__init__.pyi` & `circuitpython-stubs-8.2.2/rotaryio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/rp2pio/__init__.pyi` & `circuitpython-stubs-8.2.2/rp2pio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/rtc/__init__.pyi` & `circuitpython-stubs-8.2.2/rtc/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/samd/__init__.pyi` & `circuitpython-stubs-8.2.2/samd/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/sdcardio/__init__.pyi` & `circuitpython-stubs-8.2.2/sdcardio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/sdioio/__init__.pyi` & `circuitpython-stubs-8.2.2/sdioio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/setup.py` & `circuitpython-stubs-8.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/sharpdisplay/__init__.pyi` & `circuitpython-stubs-8.2.2/sharpdisplay/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/socketpool/__init__.pyi` & `circuitpython-stubs-8.2.2/socketpool/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/ssl/__init__.pyi` & `circuitpython-stubs-8.2.2/ssl/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/storage/__init__.pyi` & `circuitpython-stubs-8.2.2/storage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/struct/__init__.pyi` & `circuitpython-stubs-8.2.2/struct/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/supervisor/__init__.pyi` & `circuitpython-stubs-8.2.2/supervisor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/synthio/__init__.pyi` & `circuitpython-stubs-8.2.2/synthio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/terminalio/__init__.pyi` & `circuitpython-stubs-8.2.2/terminalio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/time/__init__.pyi` & `circuitpython-stubs-8.2.2/time/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/touchio/__init__.pyi` & `circuitpython-stubs-8.2.2/touchio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/traceback/__init__.pyi` & `circuitpython-stubs-8.2.2/traceback/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/ulab/__init__.pyi` & `circuitpython-stubs-8.2.2/ulab/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/ulab/numpy/__init__.pyi` & `circuitpython-stubs-8.2.2/ulab/numpy/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/ulab/numpy/carray/__init__.pyi` & `circuitpython-stubs-8.2.2/ulab/numpy/carray/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/ulab/numpy/fft/__init__.pyi` & `circuitpython-stubs-8.2.2/ulab/numpy/fft/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/ulab/numpy/linalg/__init__.pyi` & `circuitpython-stubs-8.2.2/ulab/numpy/linalg/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/ulab/scipy/linalg/__init__.pyi` & `circuitpython-stubs-8.2.2/ulab/scipy/linalg/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/ulab/scipy/optimize/__init__.pyi` & `circuitpython-stubs-8.2.2/ulab/scipy/optimize/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/usb/core/__init__.pyi` & `circuitpython-stubs-8.2.2/usb/core/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/usb_cdc/__init__.pyi` & `circuitpython-stubs-8.2.2/usb_cdc/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/usb_hid/__init__.pyi` & `circuitpython-stubs-8.2.2/usb_hid/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/usb_host/__init__.pyi` & `circuitpython-stubs-8.2.2/usb_host/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/usb_midi/__init__.pyi` & `circuitpython-stubs-8.2.2/usb_midi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/vectorio/__init__.pyi` & `circuitpython-stubs-8.2.2/vectorio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/watchdog/__init__.pyi` & `circuitpython-stubs-8.2.2/watchdog/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/wifi/__init__.pyi` & `circuitpython-stubs-8.2.2/wifi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.1/zlib/__init__.pyi` & `circuitpython-stubs-8.2.2/zlib/__init__.pyi`

 * *Files identical despite different names*

