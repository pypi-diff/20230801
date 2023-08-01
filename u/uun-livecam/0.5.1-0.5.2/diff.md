# Comparing `tmp/uun-livecam-0.5.1.tar.gz` & `tmp/uun-livecam-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uun-livecam-0.5.1.tar", last modified: Thu Jan 26 11:42:48 2023, max compression
+gzip compressed data, was "uun-livecam-0.5.2.tar", last modified: Tue Aug  1 10:27:32 2023, max compression
```

## Comparing `uun-livecam-0.5.1.tar` & `uun-livecam-0.5.2.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwx------   0 hello     (1000) hello     (1000)        0 2023-01-26 11:42:48.219462 uun-livecam-0.5.1/
--rw-------   0 hello     (1000) hello     (1000)     1075 2023-01-22 14:44:04.000000 uun-livecam-0.5.1/LICENSE.md
--rw-------   0 hello     (1000) hello     (1000)      172 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/MANIFEST.in
--rw-------   0 hello     (1000) hello     (1000)      462 2023-01-26 11:42:48.219462 uun-livecam-0.5.1/PKG-INFO
-drwx------   0 hello     (1000) hello     (1000)        0 2023-01-26 11:42:48.209462 uun-livecam-0.5.1/bin/
--rwx------   0 hello     (1000) hello     (1000)     1818 2023-01-26 11:41:31.000000 uun-livecam-0.5.1/bin/uun-livecam
--rwx------   0 hello     (1000) hello     (1000)      610 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/bin/uun-livecam-install
--rw-------   0 hello     (1000) hello     (1000)       38 2023-01-26 11:42:48.219462 uun-livecam-0.5.1/setup.cfg
--rw-------   0 hello     (1000) hello     (1000)     1264 2023-01-26 11:41:07.000000 uun-livecam-0.5.1/setup.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-01-26 11:42:48.209462 uun-livecam-0.5.1/uun_livecam/
--rw-------   0 hello     (1000) hello     (1000)        0 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/uun_livecam/__init__.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-01-26 11:42:48.209462 uun-livecam-0.5.1/uun_livecam/data/
-drwx------   0 hello     (1000) hello     (1000)        0 2023-01-26 11:42:48.212795 uun-livecam-0.5.1/uun_livecam/data/camera-manual/
--rw-------   0 hello     (1000) hello     (1000)        0 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/uun_livecam/data/camera-manual/__init__.py
--rw-------   0 hello     (1000) hello     (1000)     1078 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/uun_livecam/data/camera-manual/get-info.py
--rwx------   0 hello     (1000) hello     (1000)     3038 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/uun_livecam/data/camera-manual/main.py
--rw-------   0 hello     (1000) hello     (1000)      212 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/uun_livecam/data/camera-manual/positions.json
--rw-------   0 hello     (1000) hello     (1000)     5536 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/uun_livecam/data/camera-manual/ptz-continuous.py
--rw-------   0 hello     (1000) hello     (1000)     6194 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/uun_livecam/data/camera-manual/ptz.py
--rw-------   0 hello     (1000) hello     (1000)     1415 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/uun_livecam/data/camera-manual/snapshot.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-01-26 11:42:48.212795 uun-livecam-0.5.1/uun_livecam/data/camera-manual/snapshots/
--rw-------   0 hello     (1000) hello     (1000)        0 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/uun_livecam/data/camera-manual/snapshots/.gitkeeper
-drwx------   0 hello     (1000) hello     (1000)        0 2023-01-26 11:42:48.216128 uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/
--rw-------   0 hello     (1000) hello     (1000)    38072 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/accesscontrol.wsdl
--rw-------   0 hello     (1000) hello     (1000)    57255 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/actionengine.wsdl
--rw-------   0 hello     (1000) hello     (1000)     7263 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/addressing
--rw-------   0 hello     (1000) hello     (1000)    79284 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/advancedsecurity.wsdl
--rw-------   0 hello     (1000) hello     (1000)    24131 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/analytics.wsdl
--rw-------   0 hello     (1000) hello     (1000)    31976 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/analyticsdevice.wsdl
--rw-------   0 hello     (1000) hello     (1000)    23286 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/b-2.xsd
--rw-------   0 hello     (1000) hello     (1000)     5100 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/bf-2.xsd
--rw-------   0 hello     (1000) hello     (1000)    20498 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/bw-2.wsdl
--rw-------   0 hello     (1000) hello     (1000)    60231 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/deviceio.wsdl
--rw-------   0 hello     (1000) hello     (1000)   163209 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/devicemgmt.wsdl
--rw-------   0 hello     (1000) hello     (1000)    24593 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/display.wsdl
--rw-------   0 hello     (1000) hello     (1000)    53648 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/doorcontrol.wsdl
--rw-------   0 hello     (1000) hello     (1000)     6249 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/envelope
--rw-------   0 hello     (1000) hello     (1000)    37688 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/events.wsdl
--rw-------   0 hello     (1000) hello     (1000)    17998 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/imaging.wsdl
--rw-------   0 hello     (1000) hello     (1000)      511 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/include
--rw-------   0 hello     (1000) hello     (1000)   174812 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/media.wsdl
--rw-------   0 hello     (1000) hello     (1000)   363349 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/onvif.xsd
--rw-------   0 hello     (1000) hello     (1000)    54058 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/ptz.wsdl
--rw-------   0 hello     (1000) hello     (1000)     3660 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/r-2.xsd
--rw-------   0 hello     (1000) hello     (1000)    17214 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/receiver.wsdl
--rw-------   0 hello     (1000) hello     (1000)    40704 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/recording.wsdl
--rw-------   0 hello     (1000) hello     (1000)     5596 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/remotediscovery.wsdl
--rw-------   0 hello     (1000) hello     (1000)    10581 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/replay.wsdl
--rw-------   0 hello     (1000) hello     (1000)     3727 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/rw-2.wsdl
--rw-------   0 hello     (1000) hello     (1000)    43139 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/search.wsdl
--rw-------   0 hello     (1000) hello     (1000)     8960 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/t-1.xsd
--rw-------   0 hello     (1000) hello     (1000)     3738 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/types.xsd
--rw-------   0 hello     (1000) hello     (1000)     5849 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/ws-addr.xsd
--rw-------   0 hello     (1000) hello     (1000)    10455 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/ws-discovery.xsd
--rw-------   0 hello     (1000) hello     (1000)     8836 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/xml.xsd
--rw-------   0 hello     (1000) hello     (1000)     1639 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/xmlmime
--rw-------   0 hello     (1000) hello     (1000)     1690 2022-10-16 10:02:59.000000 uun-livecam-0.5.1/uun_livecam/data/sample-config.json
--rwx------   0 hello     (1000) hello     (1000)       63 2022-10-16 10:03:00.000000 uun-livecam-0.5.1/uun_livecam/data/start.sh
--rw-------   0 hello     (1000) hello     (1000)      285 2022-10-16 10:03:00.000000 uun-livecam-0.5.1/uun_livecam/data/systemd.service
-drwx------   0 hello     (1000) hello     (1000)        0 2023-01-26 11:42:48.216128 uun-livecam-0.5.1/uun_livecam/modules/
--rw-------   0 hello     (1000) hello     (1000)     4092 2022-10-16 10:03:00.000000 uun-livecam-0.5.1/uun_livecam/modules/SnapCam.py
--rw-------   0 hello     (1000) hello     (1000)     1294 2022-10-16 10:03:00.000000 uun-livecam-0.5.1/uun_livecam/modules/__init__.py
--rw-------   0 hello     (1000) hello     (1000)    11240 2022-10-16 10:03:00.000000 uun-livecam-0.5.1/uun_livecam/onvif.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-01-26 11:42:48.219462 uun-livecam-0.5.1/uun_livecam/wsdl/
--rw-------   0 hello     (1000) hello     (1000)    38072 2022-10-16 10:03:00.000000 uun-livecam-0.5.1/uun_livecam/wsdl/accesscontrol.wsdl
--rw-------   0 hello     (1000) hello     (1000)    57255 2022-10-16 10:03:00.000000 uun-livecam-0.5.1/uun_livecam/wsdl/actionengine.wsdl
--rw-------   0 hello     (1000) hello     (1000)     7263 2022-10-16 10:03:00.000000 uun-livecam-0.5.1/uun_livecam/wsdl/addressing
--rw-------   0 hello     (1000) hello     (1000)    79284 2022-10-16 10:03:00.000000 uun-livecam-0.5.1/uun_livecam/wsdl/advancedsecurity.wsdl
--rw-------   0 hello     (1000) hello     (1000)    24131 2022-10-16 10:03:00.000000 uun-livecam-0.5.1/uun_livecam/wsdl/analytics.wsdl
--rw-------   0 hello     (1000) hello     (1000)    31976 2022-10-16 10:03:00.000000 uun-livecam-0.5.1/uun_livecam/wsdl/analyticsdevice.wsdl
--rw-------   0 hello     (1000) hello     (1000)    23286 2022-10-16 10:03:00.000000 uun-livecam-0.5.1/uun_livecam/wsdl/b-2.xsd
--rw-------   0 hello     (1000) hello     (1000)     5100 2022-10-16 10:03:00.000000 uun-livecam-0.5.1/uun_livecam/wsdl/bf-2.xsd
--rw-------   0 hello     (1000) hello     (1000)    20498 2022-10-16 10:03:00.000000 uun-livecam-0.5.1/uun_livecam/wsdl/bw-2.wsdl
--rw-------   0 hello     (1000) hello     (1000)    60231 2022-10-16 10:03:00.000000 uun-livecam-0.5.1/uun_livecam/wsdl/deviceio.wsdl
--rw-------   0 hello     (1000) hello     (1000)   163209 2022-10-16 10:03:00.000000 uun-livecam-0.5.1/uun_livecam/wsdl/devicemgmt.wsdl
--rw-------   0 hello     (1000) hello     (1000)    24593 2022-10-16 10:03:00.000000 uun-livecam-0.5.1/uun_livecam/wsdl/display.wsdl
--rw-------   0 hello     (1000) hello     (1000)    53648 2022-10-16 10:03:00.000000 uun-livecam-0.5.1/uun_livecam/wsdl/doorcontrol.wsdl
--rw-------   0 hello     (1000) hello     (1000)     6249 2022-10-16 10:03:00.000000 uun-livecam-0.5.1/uun_livecam/wsdl/envelope
--rw-------   0 hello     (1000) hello     (1000)    37688 2022-10-16 10:03:00.000000 uun-livecam-0.5.1/uun_livecam/wsdl/events.wsdl
--rw-------   0 hello     (1000) hello     (1000)    17998 2022-10-16 10:03:00.000000 uun-livecam-0.5.1/uun_livecam/wsdl/imaging.wsdl
--rw-------   0 hello     (1000) hello     (1000)      511 2022-10-16 10:03:00.000000 uun-livecam-0.5.1/uun_livecam/wsdl/include
--rw-------   0 hello     (1000) hello     (1000)   174812 2022-10-16 10:03:00.000000 uun-livecam-0.5.1/uun_livecam/wsdl/media.wsdl
--rw-------   0 hello     (1000) hello     (1000)   363349 2022-10-16 10:03:00.000000 uun-livecam-0.5.1/uun_livecam/wsdl/onvif.xsd
--rw-------   0 hello     (1000) hello     (1000)    54058 2022-10-16 10:03:00.000000 uun-livecam-0.5.1/uun_livecam/wsdl/ptz.wsdl
--rw-------   0 hello     (1000) hello     (1000)     3660 2022-10-16 10:03:00.000000 uun-livecam-0.5.1/uun_livecam/wsdl/r-2.xsd
--rw-------   0 hello     (1000) hello     (1000)    17214 2022-10-16 10:03:00.000000 uun-livecam-0.5.1/uun_livecam/wsdl/receiver.wsdl
--rw-------   0 hello     (1000) hello     (1000)    40704 2022-10-16 10:03:00.000000 uun-livecam-0.5.1/uun_livecam/wsdl/recording.wsdl
--rw-------   0 hello     (1000) hello     (1000)     5596 2022-10-16 10:03:00.000000 uun-livecam-0.5.1/uun_livecam/wsdl/remotediscovery.wsdl
--rw-------   0 hello     (1000) hello     (1000)    10581 2022-10-16 10:03:00.000000 uun-livecam-0.5.1/uun_livecam/wsdl/replay.wsdl
--rw-------   0 hello     (1000) hello     (1000)     3727 2022-10-16 10:03:00.000000 uun-livecam-0.5.1/uun_livecam/wsdl/rw-2.wsdl
--rw-------   0 hello     (1000) hello     (1000)    43139 2022-10-16 10:03:00.000000 uun-livecam-0.5.1/uun_livecam/wsdl/search.wsdl
--rw-------   0 hello     (1000) hello     (1000)     8960 2022-10-16 10:03:00.000000 uun-livecam-0.5.1/uun_livecam/wsdl/t-1.xsd
--rw-------   0 hello     (1000) hello     (1000)     3738 2022-10-16 10:03:00.000000 uun-livecam-0.5.1/uun_livecam/wsdl/types.xsd
--rw-------   0 hello     (1000) hello     (1000)     5849 2022-10-16 10:03:00.000000 uun-livecam-0.5.1/uun_livecam/wsdl/ws-addr.xsd
--rw-------   0 hello     (1000) hello     (1000)    10455 2022-10-16 10:03:00.000000 uun-livecam-0.5.1/uun_livecam/wsdl/ws-discovery.xsd
--rw-------   0 hello     (1000) hello     (1000)     8836 2022-10-16 10:03:00.000000 uun-livecam-0.5.1/uun_livecam/wsdl/xml.xsd
--rw-------   0 hello     (1000) hello     (1000)     1639 2022-10-16 10:03:00.000000 uun-livecam-0.5.1/uun_livecam/wsdl/xmlmime
-drwx------   0 hello     (1000) hello     (1000)        0 2023-01-26 11:42:48.209462 uun-livecam-0.5.1/uun_livecam.egg-info/
--rw-------   0 hello     (1000) hello     (1000)      462 2023-01-26 11:42:48.000000 uun-livecam-0.5.1/uun_livecam.egg-info/PKG-INFO
--rw-------   0 hello     (1000) hello     (1000)     3390 2023-01-26 11:42:48.000000 uun-livecam-0.5.1/uun_livecam.egg-info/SOURCES.txt
--rw-------   0 hello     (1000) hello     (1000)        1 2023-01-26 11:42:48.000000 uun-livecam-0.5.1/uun_livecam.egg-info/dependency_links.txt
--rw-------   0 hello     (1000) hello     (1000)       26 2023-01-26 11:42:48.000000 uun-livecam-0.5.1/uun_livecam.egg-info/requires.txt
--rw-------   0 hello     (1000) hello     (1000)       12 2023-01-26 11:42:48.000000 uun-livecam-0.5.1/uun_livecam.egg-info/top_level.txt
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 10:27:32.391278 uun-livecam-0.5.2/
+-rw-------   0 hello     (1000) hello     (1000)     1075 2023-01-22 14:44:04.000000 uun-livecam-0.5.2/LICENSE.md
+-rw-------   0 hello     (1000) hello     (1000)      172 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/MANIFEST.in
+-rw-------   0 hello     (1000) hello     (1000)      462 2023-08-01 10:27:32.391278 uun-livecam-0.5.2/PKG-INFO
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 10:27:32.367945 uun-livecam-0.5.2/bin/
+-rwx------   0 hello     (1000) hello     (1000)     2443 2023-08-01 10:24:41.000000 uun-livecam-0.5.2/bin/uun-livecam
+-rwx------   0 hello     (1000) hello     (1000)      610 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/bin/uun-livecam-install
+-rw-------   0 hello     (1000) hello     (1000)       38 2023-08-01 10:27:32.391278 uun-livecam-0.5.2/setup.cfg
+-rw-------   0 hello     (1000) hello     (1000)     1264 2023-08-01 10:13:49.000000 uun-livecam-0.5.2/setup.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 10:27:32.367945 uun-livecam-0.5.2/uun_livecam/
+-rw-------   0 hello     (1000) hello     (1000)        0 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/uun_livecam/__init__.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 10:27:32.367945 uun-livecam-0.5.2/uun_livecam/data/
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 10:27:32.367945 uun-livecam-0.5.2/uun_livecam/data/camera-manual/
+-rw-------   0 hello     (1000) hello     (1000)        0 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/uun_livecam/data/camera-manual/__init__.py
+-rw-------   0 hello     (1000) hello     (1000)     1078 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/uun_livecam/data/camera-manual/get-info.py
+-rwx------   0 hello     (1000) hello     (1000)     3038 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/uun_livecam/data/camera-manual/main.py
+-rw-------   0 hello     (1000) hello     (1000)      212 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/uun_livecam/data/camera-manual/positions.json
+-rw-------   0 hello     (1000) hello     (1000)     5536 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/uun_livecam/data/camera-manual/ptz-continuous.py
+-rw-------   0 hello     (1000) hello     (1000)     6194 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/uun_livecam/data/camera-manual/ptz.py
+-rw-------   0 hello     (1000) hello     (1000)     1415 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/uun_livecam/data/camera-manual/snapshot.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 10:27:32.371278 uun-livecam-0.5.2/uun_livecam/data/camera-manual/snapshots/
+-rw-------   0 hello     (1000) hello     (1000)        0 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/uun_livecam/data/camera-manual/snapshots/.gitkeeper
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 10:27:32.381278 uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/
+-rw-------   0 hello     (1000) hello     (1000)    38072 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/accesscontrol.wsdl
+-rw-------   0 hello     (1000) hello     (1000)    57255 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/actionengine.wsdl
+-rw-------   0 hello     (1000) hello     (1000)     7263 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/addressing
+-rw-------   0 hello     (1000) hello     (1000)    79284 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/advancedsecurity.wsdl
+-rw-------   0 hello     (1000) hello     (1000)    24131 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/analytics.wsdl
+-rw-------   0 hello     (1000) hello     (1000)    31976 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/analyticsdevice.wsdl
+-rw-------   0 hello     (1000) hello     (1000)    23286 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/b-2.xsd
+-rw-------   0 hello     (1000) hello     (1000)     5100 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/bf-2.xsd
+-rw-------   0 hello     (1000) hello     (1000)    20498 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/bw-2.wsdl
+-rw-------   0 hello     (1000) hello     (1000)    60231 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/deviceio.wsdl
+-rw-------   0 hello     (1000) hello     (1000)   163209 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/devicemgmt.wsdl
+-rw-------   0 hello     (1000) hello     (1000)    24593 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/display.wsdl
+-rw-------   0 hello     (1000) hello     (1000)    53648 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/doorcontrol.wsdl
+-rw-------   0 hello     (1000) hello     (1000)     6249 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/envelope
+-rw-------   0 hello     (1000) hello     (1000)    37688 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/events.wsdl
+-rw-------   0 hello     (1000) hello     (1000)    17998 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/imaging.wsdl
+-rw-------   0 hello     (1000) hello     (1000)      511 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/include
+-rw-------   0 hello     (1000) hello     (1000)   174812 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/media.wsdl
+-rw-------   0 hello     (1000) hello     (1000)   363349 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/onvif.xsd
+-rw-------   0 hello     (1000) hello     (1000)    54058 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/ptz.wsdl
+-rw-------   0 hello     (1000) hello     (1000)     3660 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/r-2.xsd
+-rw-------   0 hello     (1000) hello     (1000)    17214 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/receiver.wsdl
+-rw-------   0 hello     (1000) hello     (1000)    40704 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/recording.wsdl
+-rw-------   0 hello     (1000) hello     (1000)     5596 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/remotediscovery.wsdl
+-rw-------   0 hello     (1000) hello     (1000)    10581 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/replay.wsdl
+-rw-------   0 hello     (1000) hello     (1000)     3727 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/rw-2.wsdl
+-rw-------   0 hello     (1000) hello     (1000)    43139 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/search.wsdl
+-rw-------   0 hello     (1000) hello     (1000)     8960 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/t-1.xsd
+-rw-------   0 hello     (1000) hello     (1000)     3738 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/types.xsd
+-rw-------   0 hello     (1000) hello     (1000)     5849 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/ws-addr.xsd
+-rw-------   0 hello     (1000) hello     (1000)    10455 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/ws-discovery.xsd
+-rw-------   0 hello     (1000) hello     (1000)     8836 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/xml.xsd
+-rw-------   0 hello     (1000) hello     (1000)     1639 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/xmlmime
+-rw-------   0 hello     (1000) hello     (1000)     1690 2022-10-16 10:02:59.000000 uun-livecam-0.5.2/uun_livecam/data/sample-config.json
+-rwx------   0 hello     (1000) hello     (1000)       63 2022-10-16 10:03:00.000000 uun-livecam-0.5.2/uun_livecam/data/start.sh
+-rw-------   0 hello     (1000) hello     (1000)      285 2022-10-16 10:03:00.000000 uun-livecam-0.5.2/uun_livecam/data/systemd.service
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 10:27:32.381278 uun-livecam-0.5.2/uun_livecam/modules/
+-rw-------   0 hello     (1000) hello     (1000)     4113 2023-08-01 07:25:48.000000 uun-livecam-0.5.2/uun_livecam/modules/SnapCam.py
+-rw-------   0 hello     (1000) hello     (1000)     1286 2023-08-01 07:52:28.000000 uun-livecam-0.5.2/uun_livecam/modules/__init__.py
+-rw-------   0 hello     (1000) hello     (1000)    11240 2022-10-16 10:03:00.000000 uun-livecam-0.5.2/uun_livecam/onvif.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 10:27:32.391278 uun-livecam-0.5.2/uun_livecam/wsdl/
+-rw-------   0 hello     (1000) hello     (1000)    38072 2022-10-16 10:03:00.000000 uun-livecam-0.5.2/uun_livecam/wsdl/accesscontrol.wsdl
+-rw-------   0 hello     (1000) hello     (1000)    57255 2022-10-16 10:03:00.000000 uun-livecam-0.5.2/uun_livecam/wsdl/actionengine.wsdl
+-rw-------   0 hello     (1000) hello     (1000)     7263 2022-10-16 10:03:00.000000 uun-livecam-0.5.2/uun_livecam/wsdl/addressing
+-rw-------   0 hello     (1000) hello     (1000)    79284 2022-10-16 10:03:00.000000 uun-livecam-0.5.2/uun_livecam/wsdl/advancedsecurity.wsdl
+-rw-------   0 hello     (1000) hello     (1000)    24131 2022-10-16 10:03:00.000000 uun-livecam-0.5.2/uun_livecam/wsdl/analytics.wsdl
+-rw-------   0 hello     (1000) hello     (1000)    31976 2022-10-16 10:03:00.000000 uun-livecam-0.5.2/uun_livecam/wsdl/analyticsdevice.wsdl
+-rw-------   0 hello     (1000) hello     (1000)    23286 2022-10-16 10:03:00.000000 uun-livecam-0.5.2/uun_livecam/wsdl/b-2.xsd
+-rw-------   0 hello     (1000) hello     (1000)     5100 2022-10-16 10:03:00.000000 uun-livecam-0.5.2/uun_livecam/wsdl/bf-2.xsd
+-rw-------   0 hello     (1000) hello     (1000)    20498 2022-10-16 10:03:00.000000 uun-livecam-0.5.2/uun_livecam/wsdl/bw-2.wsdl
+-rw-------   0 hello     (1000) hello     (1000)    60231 2022-10-16 10:03:00.000000 uun-livecam-0.5.2/uun_livecam/wsdl/deviceio.wsdl
+-rw-------   0 hello     (1000) hello     (1000)   163209 2022-10-16 10:03:00.000000 uun-livecam-0.5.2/uun_livecam/wsdl/devicemgmt.wsdl
+-rw-------   0 hello     (1000) hello     (1000)    24593 2022-10-16 10:03:00.000000 uun-livecam-0.5.2/uun_livecam/wsdl/display.wsdl
+-rw-------   0 hello     (1000) hello     (1000)    53648 2022-10-16 10:03:00.000000 uun-livecam-0.5.2/uun_livecam/wsdl/doorcontrol.wsdl
+-rw-------   0 hello     (1000) hello     (1000)     6249 2022-10-16 10:03:00.000000 uun-livecam-0.5.2/uun_livecam/wsdl/envelope
+-rw-------   0 hello     (1000) hello     (1000)    37688 2022-10-16 10:03:00.000000 uun-livecam-0.5.2/uun_livecam/wsdl/events.wsdl
+-rw-------   0 hello     (1000) hello     (1000)    17998 2022-10-16 10:03:00.000000 uun-livecam-0.5.2/uun_livecam/wsdl/imaging.wsdl
+-rw-------   0 hello     (1000) hello     (1000)      511 2022-10-16 10:03:00.000000 uun-livecam-0.5.2/uun_livecam/wsdl/include
+-rw-------   0 hello     (1000) hello     (1000)   174812 2022-10-16 10:03:00.000000 uun-livecam-0.5.2/uun_livecam/wsdl/media.wsdl
+-rw-------   0 hello     (1000) hello     (1000)   363349 2022-10-16 10:03:00.000000 uun-livecam-0.5.2/uun_livecam/wsdl/onvif.xsd
+-rw-------   0 hello     (1000) hello     (1000)    54058 2022-10-16 10:03:00.000000 uun-livecam-0.5.2/uun_livecam/wsdl/ptz.wsdl
+-rw-------   0 hello     (1000) hello     (1000)     3660 2022-10-16 10:03:00.000000 uun-livecam-0.5.2/uun_livecam/wsdl/r-2.xsd
+-rw-------   0 hello     (1000) hello     (1000)    17214 2022-10-16 10:03:00.000000 uun-livecam-0.5.2/uun_livecam/wsdl/receiver.wsdl
+-rw-------   0 hello     (1000) hello     (1000)    40704 2022-10-16 10:03:00.000000 uun-livecam-0.5.2/uun_livecam/wsdl/recording.wsdl
+-rw-------   0 hello     (1000) hello     (1000)     5596 2022-10-16 10:03:00.000000 uun-livecam-0.5.2/uun_livecam/wsdl/remotediscovery.wsdl
+-rw-------   0 hello     (1000) hello     (1000)    10581 2022-10-16 10:03:00.000000 uun-livecam-0.5.2/uun_livecam/wsdl/replay.wsdl
+-rw-------   0 hello     (1000) hello     (1000)     3727 2022-10-16 10:03:00.000000 uun-livecam-0.5.2/uun_livecam/wsdl/rw-2.wsdl
+-rw-------   0 hello     (1000) hello     (1000)    43139 2022-10-16 10:03:00.000000 uun-livecam-0.5.2/uun_livecam/wsdl/search.wsdl
+-rw-------   0 hello     (1000) hello     (1000)     8960 2022-10-16 10:03:00.000000 uun-livecam-0.5.2/uun_livecam/wsdl/t-1.xsd
+-rw-------   0 hello     (1000) hello     (1000)     3738 2022-10-16 10:03:00.000000 uun-livecam-0.5.2/uun_livecam/wsdl/types.xsd
+-rw-------   0 hello     (1000) hello     (1000)     5849 2022-10-16 10:03:00.000000 uun-livecam-0.5.2/uun_livecam/wsdl/ws-addr.xsd
+-rw-------   0 hello     (1000) hello     (1000)    10455 2022-10-16 10:03:00.000000 uun-livecam-0.5.2/uun_livecam/wsdl/ws-discovery.xsd
+-rw-------   0 hello     (1000) hello     (1000)     8836 2022-10-16 10:03:00.000000 uun-livecam-0.5.2/uun_livecam/wsdl/xml.xsd
+-rw-------   0 hello     (1000) hello     (1000)     1639 2022-10-16 10:03:00.000000 uun-livecam-0.5.2/uun_livecam/wsdl/xmlmime
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 10:27:32.367945 uun-livecam-0.5.2/uun_livecam.egg-info/
+-rw-------   0 hello     (1000) hello     (1000)      462 2023-08-01 10:27:32.000000 uun-livecam-0.5.2/uun_livecam.egg-info/PKG-INFO
+-rw-------   0 hello     (1000) hello     (1000)     3390 2023-08-01 10:27:32.000000 uun-livecam-0.5.2/uun_livecam.egg-info/SOURCES.txt
+-rw-------   0 hello     (1000) hello     (1000)        1 2023-08-01 10:27:32.000000 uun-livecam-0.5.2/uun_livecam.egg-info/dependency_links.txt
+-rw-------   0 hello     (1000) hello     (1000)       26 2023-08-01 10:27:32.000000 uun-livecam-0.5.2/uun_livecam.egg-info/requires.txt
+-rw-------   0 hello     (1000) hello     (1000)       12 2023-08-01 10:27:32.000000 uun-livecam-0.5.2/uun_livecam.egg-info/top_level.txt
```

### Comparing `uun-livecam-0.5.1/LICENSE.md` & `uun-livecam-0.5.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/bin/uun-livecam-install` & `uun-livecam-0.5.2/bin/uun-livecam-install`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/setup.py` & `uun-livecam-0.5.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License"
     ],
     python_requires='>=3.6',
     install_requires=[
-        "uun-iot >= 0.7.3",
+        "uun-iot >= 0.9.1",
         "onvif-zeep"
     ],
     scripts=[
         "bin/" + name,
         "bin/" + name + "-install"
     ],
     package_data={
```

### Comparing `uun-livecam-0.5.1/uun_livecam/data/camera-manual/get-info.py` & `uun-livecam-0.5.2/uun_livecam/data/camera-manual/get-info.py`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/data/camera-manual/main.py` & `uun-livecam-0.5.2/uun_livecam/data/camera-manual/main.py`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/data/camera-manual/ptz-continuous.py` & `uun-livecam-0.5.2/uun_livecam/data/camera-manual/ptz-continuous.py`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/data/camera-manual/ptz.py` & `uun-livecam-0.5.2/uun_livecam/data/camera-manual/ptz.py`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/data/camera-manual/snapshot.py` & `uun-livecam-0.5.2/uun_livecam/data/camera-manual/snapshot.py`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/accesscontrol.wsdl` & `uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/accesscontrol.wsdl`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/actionengine.wsdl` & `uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/actionengine.wsdl`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/addressing` & `uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/addressing`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/advancedsecurity.wsdl` & `uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/advancedsecurity.wsdl`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/analytics.wsdl` & `uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/analytics.wsdl`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/analyticsdevice.wsdl` & `uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/analyticsdevice.wsdl`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/b-2.xsd` & `uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/b-2.xsd`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/bf-2.xsd` & `uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/bf-2.xsd`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/bw-2.wsdl` & `uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/bw-2.wsdl`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/deviceio.wsdl` & `uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/deviceio.wsdl`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/devicemgmt.wsdl` & `uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/devicemgmt.wsdl`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/display.wsdl` & `uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/display.wsdl`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/doorcontrol.wsdl` & `uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/doorcontrol.wsdl`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/envelope` & `uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/envelope`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/events.wsdl` & `uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/events.wsdl`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/imaging.wsdl` & `uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/imaging.wsdl`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/media.wsdl` & `uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/media.wsdl`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/onvif.xsd` & `uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/onvif.xsd`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/ptz.wsdl` & `uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/ptz.wsdl`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/r-2.xsd` & `uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/r-2.xsd`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/receiver.wsdl` & `uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/receiver.wsdl`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/recording.wsdl` & `uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/recording.wsdl`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/remotediscovery.wsdl` & `uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/remotediscovery.wsdl`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/replay.wsdl` & `uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/replay.wsdl`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/rw-2.wsdl` & `uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/rw-2.wsdl`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/search.wsdl` & `uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/search.wsdl`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/t-1.xsd` & `uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/t-1.xsd`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/types.xsd` & `uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/types.xsd`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/ws-addr.xsd` & `uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/ws-addr.xsd`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/ws-discovery.xsd` & `uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/ws-discovery.xsd`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/xml.xsd` & `uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/xml.xsd`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/data/camera-manual/wsdl/xmlmime` & `uun-livecam-0.5.2/uun_livecam/data/camera-manual/wsdl/xmlmime`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/data/sample-config.json` & `uun-livecam-0.5.2/uun_livecam/data/sample-config.json`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/modules/SnapCam.py` & `uun-livecam-0.5.2/uun_livecam/modules/SnapCam.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
                     if self._init_camera(cam_id):
                         logger.debug("Reiinitialization of camera `%s` done.", cam_id)
                     else:
                         logger.warning("Reiinitialization of camera `%s` failed.", cam_id)
                         continue
 
                 def on_snapshot_get(image_bin, position):
-                    timestamp = get_iso_timestamp(datetime.datetime.now())
+                    timestamp = get_iso_timestamp(datetime.datetime.now(datetime.timezone.utc))
                     self._send_data((cam_id, timestamp, image_bin, position))
 
                 t = threading.Thread(target=cam.loop, kwargs={'callback': on_snapshot_get})
                 t.start()
                 threads.append(t)
         
             # wait for all cameras to finish their tours
```

### Comparing `uun-livecam-0.5.1/uun_livecam/modules/__init__.py` & `uun-livecam-0.5.2/uun_livecam/modules/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         image_bin = snapshot[2]
         positions = snapshot[3]
         x = positions["x"]
         y = positions["y"]
         zoom = positions["zoom"]
         
         uucmd = config['uuApp']['uuCmdList']['snapshotCreate']
-        uuclient.multipart_request(uucmd, {
+        uuclient.multipart(uucmd, {
             'cameraCode': str(cam_id),
             'tourTs': str(timestamp),
             'x': str(x),
             'y': str(y),
             'zoom': str(zoom),
             'image': ('image.jpeg', image_bin, 'image/jpeg') 
         })
```

### Comparing `uun-livecam-0.5.1/uun_livecam/onvif.py` & `uun-livecam-0.5.2/uun_livecam/onvif.py`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/wsdl/accesscontrol.wsdl` & `uun-livecam-0.5.2/uun_livecam/wsdl/accesscontrol.wsdl`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/wsdl/actionengine.wsdl` & `uun-livecam-0.5.2/uun_livecam/wsdl/actionengine.wsdl`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/wsdl/addressing` & `uun-livecam-0.5.2/uun_livecam/wsdl/addressing`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/wsdl/advancedsecurity.wsdl` & `uun-livecam-0.5.2/uun_livecam/wsdl/advancedsecurity.wsdl`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/wsdl/analytics.wsdl` & `uun-livecam-0.5.2/uun_livecam/wsdl/analytics.wsdl`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/wsdl/analyticsdevice.wsdl` & `uun-livecam-0.5.2/uun_livecam/wsdl/analyticsdevice.wsdl`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/wsdl/b-2.xsd` & `uun-livecam-0.5.2/uun_livecam/wsdl/b-2.xsd`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/wsdl/bf-2.xsd` & `uun-livecam-0.5.2/uun_livecam/wsdl/bf-2.xsd`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/wsdl/bw-2.wsdl` & `uun-livecam-0.5.2/uun_livecam/wsdl/bw-2.wsdl`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/wsdl/deviceio.wsdl` & `uun-livecam-0.5.2/uun_livecam/wsdl/deviceio.wsdl`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/wsdl/devicemgmt.wsdl` & `uun-livecam-0.5.2/uun_livecam/wsdl/devicemgmt.wsdl`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/wsdl/display.wsdl` & `uun-livecam-0.5.2/uun_livecam/wsdl/display.wsdl`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/wsdl/doorcontrol.wsdl` & `uun-livecam-0.5.2/uun_livecam/wsdl/doorcontrol.wsdl`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/wsdl/envelope` & `uun-livecam-0.5.2/uun_livecam/wsdl/envelope`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/wsdl/events.wsdl` & `uun-livecam-0.5.2/uun_livecam/wsdl/events.wsdl`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/wsdl/imaging.wsdl` & `uun-livecam-0.5.2/uun_livecam/wsdl/imaging.wsdl`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/wsdl/media.wsdl` & `uun-livecam-0.5.2/uun_livecam/wsdl/media.wsdl`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/wsdl/onvif.xsd` & `uun-livecam-0.5.2/uun_livecam/wsdl/onvif.xsd`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/wsdl/ptz.wsdl` & `uun-livecam-0.5.2/uun_livecam/wsdl/ptz.wsdl`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/wsdl/r-2.xsd` & `uun-livecam-0.5.2/uun_livecam/wsdl/r-2.xsd`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/wsdl/receiver.wsdl` & `uun-livecam-0.5.2/uun_livecam/wsdl/receiver.wsdl`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/wsdl/recording.wsdl` & `uun-livecam-0.5.2/uun_livecam/wsdl/recording.wsdl`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/wsdl/remotediscovery.wsdl` & `uun-livecam-0.5.2/uun_livecam/wsdl/remotediscovery.wsdl`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/wsdl/replay.wsdl` & `uun-livecam-0.5.2/uun_livecam/wsdl/replay.wsdl`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/wsdl/rw-2.wsdl` & `uun-livecam-0.5.2/uun_livecam/wsdl/rw-2.wsdl`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/wsdl/search.wsdl` & `uun-livecam-0.5.2/uun_livecam/wsdl/search.wsdl`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/wsdl/t-1.xsd` & `uun-livecam-0.5.2/uun_livecam/wsdl/t-1.xsd`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/wsdl/types.xsd` & `uun-livecam-0.5.2/uun_livecam/wsdl/types.xsd`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/wsdl/ws-addr.xsd` & `uun-livecam-0.5.2/uun_livecam/wsdl/ws-addr.xsd`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/wsdl/ws-discovery.xsd` & `uun-livecam-0.5.2/uun_livecam/wsdl/ws-discovery.xsd`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/wsdl/xml.xsd` & `uun-livecam-0.5.2/uun_livecam/wsdl/xml.xsd`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam/wsdl/xmlmime` & `uun-livecam-0.5.2/uun_livecam/wsdl/xmlmime`

 * *Files identical despite different names*

### Comparing `uun-livecam-0.5.1/uun_livecam.egg-info/SOURCES.txt` & `uun-livecam-0.5.2/uun_livecam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

