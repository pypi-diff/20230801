# Comparing `tmp/arena-py-0.4.5.tar.gz` & `tmp/arena-py-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arena-py-0.4.5.tar", last modified: Wed Jul  5 21:56:10 2023, max compression
+gzip compressed data, was "arena-py-0.5.4.tar", last modified: Tue Aug  1 20:07:57 2023, max compression
```

## Comparing `arena-py-0.4.5.tar` & `arena-py-0.5.4.tar`

### file list

```diff
@@ -1,89 +1,90 @@
-drwxrwxr-x   0 edward    (1000) edward    (1000)        0 2023-07-05 21:56:10.172372 arena-py-0.4.5/
--rw-rw-r--   0 edward    (1000) edward    (1000)     1533 2023-05-26 22:34:51.000000 arena-py-0.4.5/LICENSE
--rw-rw-r--   0 edward    (1000) edward    (1000)     4417 2023-07-05 21:56:10.172372 arena-py-0.4.5/PKG-INFO
--rw-rw-r--   0 edward    (1000) edward    (1000)     3913 2023-07-05 20:31:34.000000 arena-py-0.4.5/README.md
-drwxrwxr-x   0 edward    (1000) edward    (1000)        0 2023-07-05 21:56:10.168372 arena-py-0.4.5/arena/
--rw-rw-r--   0 edward    (1000) edward    (1000)      279 2023-07-05 21:41:28.000000 arena-py-0.4.5/arena/__init__.py
--rwxrwxr-x   0 edward    (1000) edward    (1000)     3148 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/__main__.py
--rw-rw-r--   0 edward    (1000) edward    (1000)    12667 2023-07-05 20:21:44.000000 arena-py-0.4.5/arena/arena_mqtt.py
-drwxrwxr-x   0 edward    (1000) edward    (1000)        0 2023-07-05 21:56:10.168372 arena-py-0.4.5/arena/attributes/
--rw-rw-r--   0 edward    (1000) edward    (1000)     1022 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/attributes/__init__.py
--rw-rw-r--   0 edward    (1000) edward    (1000)     1031 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/attributes/animation.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      139 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/attributes/animation_mixer.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      175 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/attributes/attribute.py
--rw-rw-r--   0 edward    (1000) edward    (1000)     1135 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/attributes/color.py
--rw-rw-r--   0 edward    (1000) edward    (1000)     4974 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/attributes/data.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      362 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/attributes/goto_url.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      764 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/attributes/impulse.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      503 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/attributes/jitsi_video.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      811 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/attributes/landmark.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      611 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/attributes/material.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      237 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/attributes/morph.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      357 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/attributes/physics.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      496 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/attributes/position.py
--rw-rw-r--   0 edward    (1000) edward    (1000)     2681 2023-07-05 18:37:42.000000 arena-py-0.4.5/arena/attributes/rotation.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      355 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/attributes/scale.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      247 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/attributes/sound.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      475 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/attributes/text_input.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      152 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/attributes/video_control.py
--rw-rw-r--   0 edward    (1000) edward    (1000)    16461 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/auth.py
--rw-rw-r--   0 edward    (1000) edward    (1000)     1127 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/base_object.py
--rw-rw-r--   0 edward    (1000) edward    (1000)     2837 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/device.py
-drwxrwxr-x   0 edward    (1000) edward    (1000)        0 2023-07-05 21:56:10.168372 arena-py-0.4.5/arena/event_loop/
--rw-rw-r--   0 edward    (1000) edward    (1000)      267 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/event_loop/__init__.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      419 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/event_loop/async_worker.py
--rw-rw-r--   0 edward    (1000) edward    (1000)     2457 2023-07-05 21:41:28.000000 arena-py-0.4.5/arena/event_loop/asyncio_mqtt.py
--rw-rw-r--   0 edward    (1000) edward    (1000)     1749 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/event_loop/event_loop.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      651 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/event_loop/lazy_worker.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      841 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/event_loop/persistent_worker.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      129 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/event_loop/single_worker.py
--rw-rw-r--   0 edward    (1000) edward    (1000)     1171 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/event_loop/worker.py
-drwxrwxr-x   0 edward    (1000) edward    (1000)        0 2023-07-05 21:56:10.168372 arena-py-0.4.5/arena/events/
--rw-rw-r--   0 edward    (1000) edward    (1000)       25 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/events/__init__.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      984 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/events/event.py
-drwxrwxr-x   0 edward    (1000) edward    (1000)        0 2023-07-05 21:56:10.172372 arena-py-0.4.5/arena/objects/
--rw-rw-r--   0 edward    (1000) edward    (1000)     1289 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/objects/__init__.py
--rw-rw-r--   0 edward    (1000) edward    (1000)     6766 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/objects/arena_object.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      516 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/objects/box.py
--rw-rw-r--   0 edward    (1000) edward    (1000)     1569 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/objects/camera.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      236 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/objects/circle.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      228 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/objects/cone.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      243 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/objects/cylinder.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      260 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/objects/dodecahedron.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      236 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/objects/entity.py
--rw-rw-r--   0 edward    (1000) edward    (1000)     1320 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/objects/gltf.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      256 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/objects/icosahedron.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      249 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/objects/image.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      232 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/objects/light.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      332 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/objects/line.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      252 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/objects/octahedron.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      244 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/objects/particle.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      232 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/objects/plane.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      228 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/objects/ring.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      236 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/objects/sphere.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      256 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/objects/tetrahedron.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      264 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/objects/text.py
--rw-rw-r--   0 edward    (1000) edward    (1000)     1023 2023-07-05 18:37:42.000000 arena-py-0.4.5/arena/objects/thickline.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      232 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/objects/torus.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      248 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/objects/torus_knot.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      244 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/objects/triangle.py
--rw-rw-r--   0 edward    (1000) edward    (1000)    16309 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/scene.py
-drwxrwxr-x   0 edward    (1000) edward    (1000)        0 2023-07-05 21:56:10.172372 arena-py-0.4.5/arena/scripts/
--rw-rw-r--   0 edward    (1000) edward    (1000)        0 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/scripts/__init__.py
--rwxrwxr-x   0 edward    (1000) edward    (1000)      122 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/scripts/arena_py_permissions.py
--rwxrwxr-x   0 edward    (1000) edward    (1000)      557 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/scripts/arena_py_pub.py
--rwxrwxr-x   0 edward    (1000) edward    (1000)      118 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/scripts/arena_py_signout.py
--rwxrwxr-x   0 edward    (1000) edward    (1000)      559 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/scripts/arena_py_sub.py
--rwxrwxr-x   0 edward    (1000) edward    (1000)      229 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/scripts/arena_py_token.py
-drwxrwxr-x   0 edward    (1000) edward    (1000)        0 2023-07-05 21:56:10.172372 arena-py-0.4.5/arena/utils/
--rw-rw-r--   0 edward    (1000) edward    (1000)       25 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/utils/__init__.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      781 2023-05-26 22:34:51.000000 arena-py-0.4.5/arena/utils/utils.py
-drwxrwxr-x   0 edward    (1000) edward    (1000)        0 2023-07-05 21:56:10.172372 arena-py-0.4.5/arena_py.egg-info/
--rw-rw-r--   0 edward    (1000) edward    (1000)     4417 2023-07-05 21:56:10.000000 arena-py-0.4.5/arena_py.egg-info/PKG-INFO
--rw-rw-r--   0 edward    (1000) edward    (1000)     2057 2023-07-05 21:56:10.000000 arena-py-0.4.5/arena_py.egg-info/SOURCES.txt
--rw-rw-r--   0 edward    (1000) edward    (1000)        1 2023-07-05 21:56:10.000000 arena-py-0.4.5/arena_py.egg-info/dependency_links.txt
--rw-rw-r--   0 edward    (1000) edward    (1000)      308 2023-07-05 21:56:10.000000 arena-py-0.4.5/arena_py.egg-info/entry_points.txt
--rw-rw-r--   0 edward    (1000) edward    (1000)      125 2023-07-05 21:56:10.000000 arena-py-0.4.5/arena_py.egg-info/requires.txt
--rw-rw-r--   0 edward    (1000) edward    (1000)        6 2023-07-05 21:56:10.000000 arena-py-0.4.5/arena_py.egg-info/top_level.txt
--rw-rw-r--   0 edward    (1000) edward    (1000)       38 2023-07-05 21:56:10.172372 arena-py-0.4.5/setup.cfg
--rw-rw-r--   0 edward    (1000) edward    (1000)     1404 2023-07-05 21:54:55.000000 arena-py-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:07:57.113848 arena-py-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-08-01 20:07:46.000000 arena-py-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-08-01 20:07:57.113848 arena-py-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-08-01 20:07:46.000000 arena-py-0.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:07:57.105848 arena-py-0.5.4/arena/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3148 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14721 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/arena_mqtt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:07:57.109848 arena-py-0.5.4/arena/attributes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/attributes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/attributes/animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/attributes/animation_mixer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/attributes/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/attributes/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/attributes/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/attributes/goto_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/attributes/impulse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/attributes/jitsi_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/attributes/landmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/attributes/material.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/attributes/morph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/attributes/physics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/attributes/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/attributes/rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/attributes/scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/attributes/sound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/attributes/text_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/attributes/video_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16461 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/base_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:07:57.109848 arena-py-0.5.4/arena/event_loop/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/event_loop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/event_loop/async_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/event_loop/asyncio_mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/event_loop/event_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/event_loop/lazy_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/event_loop/persistent_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/event_loop/single_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/event_loop/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:07:57.109848 arena-py-0.5.4/arena/events/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/events/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:07:57.113848 arena-py-0.5.4/arena/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/objects/arena_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/objects/box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/objects/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/objects/circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/objects/cone.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/objects/cylinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/objects/dodecahedron.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/objects/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/objects/gltf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/objects/icosahedron.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/objects/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/objects/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/objects/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/objects/octahedron.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/objects/particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/objects/plane.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/objects/ring.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/objects/sphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/objects/tetrahedron.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/objects/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/objects/thickline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/objects/torus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/objects/torus_knot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/objects/triangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16492 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/scene.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:07:57.113848 arena-py-0.5.4/arena/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      122 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/scripts/arena_py_permissions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      557 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/scripts/arena_py_pub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      118 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/scripts/arena_py_signout.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      559 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/scripts/arena_py_sub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      229 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/scripts/arena_py_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:07:57.113848 arena-py-0.5.4/arena/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/utils/cmd_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-08-01 20:07:46.000000 arena-py-0.5.4/arena/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:07:57.113848 arena-py-0.5.4/arena_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-08-01 20:07:57.000000 arena-py-0.5.4/arena_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-08-01 20:07:57.000000 arena-py-0.5.4/arena_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:07:57.000000 arena-py-0.5.4/arena_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-08-01 20:07:57.000000 arena-py-0.5.4/arena_py.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-01 20:07:57.000000 arena-py-0.5.4/arena_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 20:07:57.000000 arena-py-0.5.4/arena_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 20:07:57.113848 arena-py-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-08-01 20:07:46.000000 arena-py-0.5.4/setup.py
```

### Comparing `arena-py-0.4.5/LICENSE` & `arena-py-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.5/PKG-INFO` & `arena-py-0.5.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arena-py
-Version: 0.4.5
+Version: 0.5.4
 Summary: Draw objects and run programs in the ARENA using Python!
 Home-page: https://github.com/arenaxr/ARENA-py
 Author: Conix Research Center
 Author-email: info@conix.io
 License: BSD 3-clause "New" or "Revised License"
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `arena-py-0.4.5/README.md` & `arena-py-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.5/arena/__main__.py` & `arena-py-0.5.4/arena/__main__.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.5/arena/arena_mqtt.py` & `arena-py-0.5.4/arena/arena_mqtt.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,32 +2,35 @@
 import asyncio
 import json
 import os
 import random
 import socket
 import ssl
 import sys
+from datetime import datetime
+import threading
 
 import paho.mqtt.client as mqtt
 
 from .auth import ArenaAuth
 from .event_loop import *
-
+from .utils import ArenaCmdInterpreter
 
 class ArenaMQTT(object):
     """
     Wrapper around Paho MQTT client and EventLoop.
     """
 
     scene = None
     device = None
     auth = None
 
     def __init__(
                 self,
+                web_host = "arenaxr.org",
                 realm = "realm",
                 network_latency_interval = 10000,  # run network latency update every 10s
                 on_msg_callback = None,
                 end_program_callback = None,
                 video = False,
                 debug = False,
                 **kwargs
@@ -35,15 +38,16 @@
         if os.environ.get("MQTTH"):
             self.web_host = os.environ["MQTTH"]
             print(f"Using Host from 'MQTTH' env variable: {self.web_host}")
         elif "host" in kwargs and kwargs["host"]:
             self.web_host = kwargs["host"]
             print(f"Using Host from 'host' input parameter: {self.web_host}")
         else:
-            sys.exit("ARENA webserver host argument (host) is unspecified or None, aborting...")
+            # Use default "web_host", helps avoid and web vs mqtt host and other user setup confusion
+            self.web_host = web_host
 
         if os.environ.get("REALM"):
             self.realm = os.environ["REALM"]
             print(f"Using Realm from 'REALM' env variable: {self.realm}")
         elif "realm" in kwargs and kwargs["realm"]:
             self.realm = kwargs["realm"]
             print(f"Using Realm from 'realm' input parameter: {self.realm}")
@@ -132,24 +136,36 @@
         # have all tasks wait until mqtt client is connected before starting
         self.mqtt_connect_evt = asyncio.Event()
         self.mqtt_connect_evt.clear()
 
         # set paho mqtt callbacks
         self.mqttc.on_connect = self.on_connect
         self.mqttc.on_disconnect = self.on_disconnect
+        self.mqttc.on_publish = self.on_publish
+
+        # setup msg counters
+        self.msg_io = { 'last_rcv_time': None, 'last_pub_time': None, 'rcv_msgs': 0, 'pub_msgs': 0, 'rcv_msgs_per_sec': 0.0, 'pub_msgs_per_sec': 0.0}
+        self.msg_rate_time_start = datetime.now()
 
         # add main message processing + callbacks loop to tasks
         self.run_async(self.process_message)
 
         # update network latency every network_latency_interval secs
         self.run_forever(self.network_latency_update,
                          interval_ms=network_latency_interval)
 
+        # update message rate every second
+        self.run_forever(self.msg_rate_update,
+                         interval_ms=1000)
+
         self.msg_queue = asyncio.Queue()
 
+        # setup event to let others wait on connection
+        self.connected_evt = threading.Event()
+
         # connect to mqtt broker
         if "port" in kwargs:
             port = kwargs["port"]
         else:
             port = 8883 # ARENA broker TLS 1.2 connection port
         if self.auth.verify(self.web_host):
             self.mqttc.tls_set()
@@ -158,14 +174,22 @@
             self.mqttc.tls_insecure_set(True)
         try:
             self.mqttc.connect(self.mqtt_host, port=port, keepalive=60)
         except Exception as err:
             print(f'MQTT connect error to {self.mqtt_host}, port={port}: Result Code={err}')
         self.mqttc.socket().setsockopt(socket.SOL_SOCKET, socket.SO_SNDBUF, 2048)
 
+        # check if we want to start the command interpreter
+        enable_interp = os.getenv("ENABLE_INTERPRETER", 'False').lower() in ('true', '1', 't')
+        if enable_interp:
+            self.cmd_interpreter = ArenaCmdInterpreter(self,
+                                                       show_attrs=('config_data', 'scene', 'users', 'all_objects', 'msg_io'),
+                                                       get_callables=('persisted_objs', 'persisted_scene_option', 'writable_scenes', 'user_list'))
+            self.cmd_interpreter.start_thread(self.connected_evt)
+
 
     def parse_cli(self):
         """
         Reusable command-line options to give apps flexible options to avoid hard-coding locations.
         """
         parser = argparse.ArgumentParser(description=("ARENA-py Application CLI"))
         parser.add_argument("-mh", "--host", type=str,
@@ -194,24 +218,30 @@
             "device": args.device,
             "position": app_position,
             "rotation": app_rotation,
             "scale": app_scale,
             "debug": args.debug,
         }
 
-
     def generate_client_id(self):
         """Returns a random 6 digit id"""
         return str(random.randrange(100000, 999999))
 
     def network_latency_update(self):
         """Update client latency in $NETWORK/latency"""
         # publish empty message with QoS of 2 to update latency
         self.mqttc.publish(self.latency_topic, "", qos=2)
 
+    def msg_rate_update(self):
+        """Update Message rate"""
+        elapsed = datetime.now() - self.msg_rate_time_start
+        if elapsed.seconds > 0:
+            self.msg_io['rcv_msgs_per_sec'] = round(self.msg_io['rcv_msgs']  / elapsed.seconds, 2)
+            self.msg_io['pub_msgs_per_sec'] = round(self.msg_io['pub_msgs']  / elapsed.seconds, 2)
+
     def run_once(self, func=None, **kwargs):
         """Runs a user-defined function on startup"""
         if func is not None:
             w = SingleWorker(self.event_loop, func, self.mqtt_connect_evt, **kwargs)
             self.event_loop.add_task(w)
         else:
             # if there is no func, we are in a decorator
@@ -280,24 +310,32 @@
         if rc == 0:
             self.mqtt_connect_evt.set()
 
             # listen to all messages in scene
             client.subscribe(self.subscribe_topic)
             client.message_callback_add(self.subscribe_topic, self.on_message)
 
+            # set event
+            self.connected_evt.set()
+
+            # reset msg rate time
+            self.msg_rate_time_start = datetime.now()
+
             print("Connected!")
             print("=====")
+
         else:
             print(f"Connection error! Result code={rc}")
 
     def on_message(self, client, userdata, msg):
         # ignore own messages
         if mqtt.topic_matches_sub(self.ignore_topic, msg.topic):
             return
-
+        self.msg_io['last_rcv_time'] = datetime.now()
+        self.msg_io['rcv_msgs'] = self.msg_io['rcv_msgs'] + 1
         self.msg_queue.put_nowait(msg)
 
     async def process_message(self):
         raise NotImplementedError("Must override process_message")
 
     def on_disconnect(self, client, userdata, rc):
         """Paho MQTT client on_disconnect callback"""
@@ -308,14 +346,18 @@
 
     def disconnect(self):
         """Disconnects Paho MQTT client"""
         if self.end_program_callback:
             self.end_program_callback(self)
         self.mqttc.disconnect()
 
+    def on_publish(self, client, userdata, mid):
+        self.msg_io['last_pub_time'] = datetime.now()
+        self.msg_io['pub_msgs'] = self.msg_io['pub_msgs'] + 1
+
     def message_callback_add(self, sub, callback):
         """Subscribes to new topic and adds callback"""
         self.mqttc.subscribe(sub)
         self.mqttc.message_callback_add(sub, callback)
 
     def message_callback_remove(self, sub):
         """Unsubscribes to topic and removes callback"""
```

### Comparing `arena-py-0.4.5/arena/attributes/__init__.py` & `arena-py-0.5.4/arena/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.5/arena/attributes/animation.py` & `arena-py-0.5.4/arena/attributes/animation.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.5/arena/attributes/color.py` & `arena-py-0.5.4/arena/attributes/color.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.5/arena/attributes/data.py` & `arena-py-0.5.4/arena/attributes/data.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.5/arena/attributes/impulse.py` & `arena-py-0.5.4/arena/attributes/impulse.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.5/arena/attributes/landmark.py` & `arena-py-0.5.4/arena/attributes/landmark.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.5/arena/attributes/material.py` & `arena-py-0.5.4/arena/attributes/material.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.5/arena/attributes/rotation.py` & `arena-py-0.5.4/arena/attributes/rotation.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.5/arena/auth.py` & `arena-py-0.5.4/arena/auth.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.5/arena/base_object.py` & `arena-py-0.5.4/arena/base_object.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.5/arena/device.py` & `arena-py-0.5.4/arena/device.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     :param str realm: Reserved topic fork for future use (optional).
     :param str namespace: Username of authenticated user or other namespace (automatic).
     :param str device: The name of the device, without namespace (required).
     """
 
     def __init__(
                 self,
+                host = "arenaxr.org",
                 realm = "realm",
                 network_latency_interval = 10000,  # run network latency update every 10s
                 on_msg_callback = None,
                 end_program_callback = None,
                 debug = False,
                 cli_args = False,
                 **kwargs
@@ -46,14 +47,15 @@
                 sys.exit("Device argument (device) cannot include '/', aborting...")
             self.device = kwargs["device"]
             print(f"Using Device from 'device' input parameter: {self.device}")
         else:
             sys.exit("Device argument (device) is unspecified or None, aborting...")
 
         super().__init__(
+            host,
             realm,
             network_latency_interval,
             on_msg_callback,
             end_program_callback,
             debug,
             **kwargs
         )
```

### Comparing `arena-py-0.4.5/arena/event_loop/asyncio_mqtt.py` & `arena-py-0.5.4/arena/event_loop/asyncio_mqtt.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.5/arena/event_loop/event_loop.py` & `arena-py-0.5.4/arena/event_loop/event_loop.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.5/arena/event_loop/lazy_worker.py` & `arena-py-0.5.4/arena/event_loop/lazy_worker.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.5/arena/event_loop/persistent_worker.py` & `arena-py-0.5.4/arena/event_loop/persistent_worker.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.5/arena/event_loop/worker.py` & `arena-py-0.5.4/arena/event_loop/worker.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.5/arena/events/event.py` & `arena-py-0.5.4/arena/events/event.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.5/arena/objects/__init__.py` & `arena-py-0.5.4/arena/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.5/arena/objects/arena_object.py` & `arena-py-0.5.4/arena/objects/arena_object.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.5/arena/objects/box.py` & `arena-py-0.5.4/arena/objects/box.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.5/arena/objects/camera.py` & `arena-py-0.5.4/arena/objects/camera.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.5/arena/objects/gltf.py` & `arena-py-0.5.4/arena/objects/gltf.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.5/arena/objects/thickline.py` & `arena-py-0.5.4/arena/objects/thickline.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.5/arena/scene.py` & `arena-py-0.5.4/arena/scene.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 
 from .arena_mqtt import ArenaMQTT
 from .attributes import *
 from .events import *
 from .objects import *
 from .utils import *
 
-
 class Scene(ArenaMQTT):
     """
     Gives access to an ARENA scene.
     Can create and execute various user-defined functions/tasks.
 
     :param str host: Hostname of the ARENA webserver (required).
     :param str realm: Reserved topic fork for future use (optional).
     :param str namespace: Username of authenticated user or other namespace (automatic).
     :param str scene: The name of the scene, without namespace (required).
     """
 
     def __init__(
                 self,
+                host = "arenaxr.org",
                 realm = "realm",
                 network_latency_interval = 10000,  # run network latency update every 10s
                 on_msg_callback = None,
                 new_obj_callback = None,
                 user_join_callback = None,
                 user_left_callback = None,
                 delete_obj_callback = None,
@@ -57,14 +57,15 @@
                 sys.exit("Scene argument (scene) cannot include '/', aborting...")
             self.scene = kwargs["scene"]
             print(f"Using Scene from 'scene' input parameter: {self.scene}")
         else:
             sys.exit("Scene argument (scene) is unspecified or None, aborting...")
 
         super().__init__(
+            host,
             realm,
             network_latency_interval,
             on_msg_callback,
             end_program_callback,
             video,
             debug,
             **kwargs
@@ -94,15 +95,19 @@
         if rc == 0:
             # create ARENA-py Objects from persist server
             # no need to return anything here
             self.get_persisted_objs()
 
     async def process_message(self):
         while True:
-            msg = await self.msg_queue.get()
+            try:
+                msg = await self.msg_queue.get()
+            except RuntimeError as e:
+                print(f"Ignoring error: {e}")
+                return
 
             # extract payload
             try:
                 payload_str = msg.payload.decode("utf-8", "ignore")
                 payload = json.loads(payload_str)
             except Exception as e:
                 print("Malformed payload, ignoring:")
```

### Comparing `arena-py-0.4.5/arena/scripts/arena_py_pub.py` & `arena-py-0.5.4/arena/scripts/arena_py_pub.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.5/arena/scripts/arena_py_sub.py` & `arena-py-0.5.4/arena/scripts/arena_py_sub.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.5/arena/utils/utils.py` & `arena-py-0.5.4/arena/utils/utils.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.5/arena_py.egg-info/PKG-INFO` & `arena-py-0.5.4/arena_py.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arena-py
-Version: 0.4.5
+Version: 0.5.4
 Summary: Draw objects and run programs in the ARENA using Python!
 Home-page: https://github.com/arenaxr/ARENA-py
 Author: Conix Research Center
 Author-email: info@conix.io
 License: BSD 3-clause "New" or "Revised License"
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `arena-py-0.4.5/arena_py.egg-info/SOURCES.txt` & `arena-py-0.5.4/arena_py.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 arena/scripts/__init__.py
 arena/scripts/arena_py_permissions.py
 arena/scripts/arena_py_pub.py
 arena/scripts/arena_py_signout.py
 arena/scripts/arena_py_sub.py
 arena/scripts/arena_py_token.py
 arena/utils/__init__.py
+arena/utils/cmd_interpreter.py
 arena/utils/utils.py
 arena_py.egg-info/PKG-INFO
 arena_py.egg-info/SOURCES.txt
 arena_py.egg-info/dependency_links.txt
 arena_py.egg-info/entry_points.txt
 arena_py.egg-info/requires.txt
 arena_py.egg-info/top_level.txt
```

### Comparing `arena-py-0.4.5/setup.py` & `arena-py-0.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as readme:
     long_description = readme.read()
 
 setuptools.setup(
     name="arena-py",
-    version="0.4.5",
+    version="0.5.4",
     author="Conix Research Center",
     author_email="info@conix.io",
     license="BSD 3-clause \"New\" or \"Revised License\"",
     description="Draw objects and run programs in the ARENA using Python!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/arenaxr/ARENA-py",
@@ -22,15 +22,15 @@
             'arena-py-signout=arena.scripts.arena_py_signout:main',
             'arena-py-sub=arena.scripts.arena_py_sub:main',
             'arena-py-token=arena.scripts.arena_py_token:main'
         ],
     },
     install_requires=[
         "aiohttp>=3.7.4",
-        "paho-mqtt~=1.6.1",
+        "paho-mqtt~=1.5.1",
         "requests~=2.28.1",
         "webcolors~=1.3",
         "google_auth_oauthlib~=0.5.2",
         "google-auth~=1.35.0",
         "PyJWT~=2.4.0"
     ],
     classifiers=[
```

