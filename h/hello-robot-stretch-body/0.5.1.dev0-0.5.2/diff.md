# Comparing `tmp/hello_robot_stretch_body-0.5.1.dev0.tar.gz` & `tmp/hello_robot_stretch_body-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hello_robot_stretch_body-0.5.1.dev0.tar", last modified: Wed Jul 19 18:26:44 2023, max compression
+gzip compressed data, was "hello_robot_stretch_body-0.5.2.tar", last modified: Tue Aug  1 17:56:20 2023, max compression
```

## Comparing `hello_robot_stretch_body-0.5.1.dev0.tar` & `hello_robot_stretch_body-0.5.2.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-07-19 18:26:44.403867 hello_robot_stretch_body-0.5.1.dev0/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      916 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/LICENSE.md
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3237 2023-07-19 18:26:44.403867 hello_robot_stretch_body-0.5.1.dev0/PKG-INFO
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2262 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/README.md
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      255 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/deploy.sh
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-07-19 18:26:44.395867 hello_robot_stretch_body-0.5.1.dev0/hello_robot_stretch_body.egg-info/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3237 2023-07-19 18:26:44.000000 hello_robot_stretch_body-0.5.1.dev0/hello_robot_stretch_body.egg-info/PKG-INFO
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2008 2023-07-19 18:26:44.000000 hello_robot_stretch_body-0.5.1.dev0/hello_robot_stretch_body.egg-info/SOURCES.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        1 2023-07-19 18:26:44.000000 hello_robot_stretch_body-0.5.1.dev0/hello_robot_stretch_body.egg-info/dependency_links.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      578 2023-07-19 18:26:44.000000 hello_robot_stretch_body-0.5.1.dev0/hello_robot_stretch_body.egg-info/requires.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       18 2023-07-19 18:26:44.000000 hello_robot_stretch_body-0.5.1.dev0/hello_robot_stretch_body.egg-info/top_level.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       38 2023-07-19 18:26:44.403867 hello_robot_stretch_body-0.5.1.dev0/setup.cfg
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2084 2023-07-19 04:03:22.000000 hello_robot_stretch_body-0.5.1.dev0/setup.py
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-07-19 18:26:44.399867 hello_robot_stretch_body-0.5.1.dev0/stretch_body/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       34 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/stretch_body/__init__.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      970 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/stretch_body/arm.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    34473 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/stretch_body/base.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3304 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/stretch_body/cobbs_framing.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6086 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/stretch_body/device.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    42153 2023-07-19 04:04:03.000000 hello_robot_stretch_body-0.5.1.dev0/stretch_body/dynamixel_XL430.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    11462 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/stretch_body/dynamixel_X_chain.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    43830 2023-07-19 04:03:22.000000 hello_robot_stretch_body-0.5.1.dev0/stretch_body/dynamixel_hello_XL430.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3659 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/stretch_body/end_of_arm.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      571 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/stretch_body/end_of_arm_tools.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3055 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/stretch_body/head.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    21912 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/stretch_body/hello_utils.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1022 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/stretch_body/lift.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    39704 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/stretch_body/pimu.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    27354 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/stretch_body/prismatic_joint.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    21754 2023-07-19 04:09:53.000000 hello_robot_stretch_body-0.5.1.dev0/stretch_body/robot.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     8415 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/stretch_body/robot_collision.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6479 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/stretch_body/robot_collision_models.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6859 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/stretch_body/robot_monitor.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6949 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/stretch_body/robot_params.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    26094 2023-07-19 04:03:22.000000 hello_robot_stretch_body-0.5.1.dev0/stretch_body/robot_params_RE1V0.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    19672 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/stretch_body/robot_params_RE2V0.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     4504 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/stretch_body/robot_trace.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    12072 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/stretch_body/scope.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    61278 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/stretch_body/stepper.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3829 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/stretch_body/stretch_gripper.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    29097 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/stretch_body/trajectories.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    45367 2023-07-19 04:04:03.000000 hello_robot_stretch_body-0.5.1.dev0/stretch_body/transport.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      218 2023-07-19 18:24:57.000000 hello_robot_stretch_body-0.5.1.dev0/stretch_body/version.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    20335 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/stretch_body/wacc.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1934 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/stretch_body/wrist_yaw.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     9733 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/stretch_body/xbox_controller.py
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-07-19 18:26:44.399867 hello_robot_stretch_body-0.5.1.dev0/test/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       82 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/test/README.md
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        0 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/test/__init__.py
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-07-19 18:26:44.403867 hello_robot_stretch_body-0.5.1.dev0/test/rates/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     5866 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/test/rates/test_arm_command_at_max_rate.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1748 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/test/rates/test_comm_loads.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1727 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/test/rates/test_pimu_sync_100hz.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     4497 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/test/rates/test_robot_command_at_max_rate.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1112 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/test/rates/test_robot_dxl_rates.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3835 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/test/rates/test_robot_nondxl_rates.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1668 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/test/rates/test_single_nondxl_rates.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     5087 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/test/rates/test_thread_locks.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     5384 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/test/test_arm.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6818 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/test/test_base.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     9977 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/test/test_collisions.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3198 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/test/test_device.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1111 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/test/test_dxl_comms.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3737 2023-07-19 04:03:22.000000 hello_robot_stretch_body-0.5.1.dev0/test/test_dxl_vel.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     7882 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/test/test_dynamixel_XL430.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    14520 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/test/test_dynamixel_hello_XL430.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1435 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/test/test_end_of_arm.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1914 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/test/test_end_of_arm_tools.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3833 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/test/test_head.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    23286 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/test/test_hello_utils.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     4761 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/test/test_lift.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2069 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/test/test_pimu.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     9004 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/test/test_robot.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2391 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/test/test_robot_params.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    26117 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/test/test_steppers.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1657 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/test/test_stretch_gripper.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6263 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/test/test_sync.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     4381 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/test/test_timing_stats.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    29747 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/test/test_trajectories.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3918 2023-07-18 23:54:41.000000 hello_robot_stretch_body-0.5.1.dev0/test/test_wrist_yaw.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-08-01 17:56:20.154151 hello_robot_stretch_body-0.5.2/
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      916 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/LICENSE.md
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2774 2023-08-01 17:56:20.154151 hello_robot_stretch_body-0.5.2/PKG-INFO
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2262 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/README.md
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      255 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/deploy.sh
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-08-01 17:56:20.146150 hello_robot_stretch_body-0.5.2/hello_robot_stretch_body.egg-info/
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2774 2023-08-01 17:56:20.000000 hello_robot_stretch_body-0.5.2/hello_robot_stretch_body.egg-info/PKG-INFO
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2008 2023-08-01 17:56:20.000000 hello_robot_stretch_body-0.5.2/hello_robot_stretch_body.egg-info/SOURCES.txt
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        1 2023-08-01 17:56:20.000000 hello_robot_stretch_body-0.5.2/hello_robot_stretch_body.egg-info/dependency_links.txt
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      578 2023-08-01 17:56:20.000000 hello_robot_stretch_body-0.5.2/hello_robot_stretch_body.egg-info/requires.txt
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       18 2023-08-01 17:56:20.000000 hello_robot_stretch_body-0.5.2/hello_robot_stretch_body.egg-info/top_level.txt
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       38 2023-08-01 17:56:20.154151 hello_robot_stretch_body-0.5.2/setup.cfg
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2084 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/setup.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-08-01 17:56:20.150150 hello_robot_stretch_body-0.5.2/stretch_body/
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       34 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/stretch_body/__init__.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      970 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/stretch_body/arm.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    34473 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/stretch_body/base.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3304 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/stretch_body/cobbs_framing.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6086 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/stretch_body/device.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    42153 2023-08-01 00:01:04.000000 hello_robot_stretch_body-0.5.2/stretch_body/dynamixel_XL430.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    11462 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/stretch_body/dynamixel_X_chain.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    43830 2023-08-01 17:54:39.000000 hello_robot_stretch_body-0.5.2/stretch_body/dynamixel_hello_XL430.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3659 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/stretch_body/end_of_arm.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      571 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/stretch_body/end_of_arm_tools.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3055 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/stretch_body/head.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    21912 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/stretch_body/hello_utils.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1022 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/stretch_body/lift.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    39726 2023-07-31 21:21:56.000000 hello_robot_stretch_body-0.5.2/stretch_body/pimu.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    27354 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/stretch_body/prismatic_joint.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    21910 2023-07-31 23:11:09.000000 hello_robot_stretch_body-0.5.2/stretch_body/robot.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     8415 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/stretch_body/robot_collision.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6479 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/stretch_body/robot_collision_models.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6859 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/stretch_body/robot_monitor.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6949 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/stretch_body/robot_params.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    26094 2023-07-31 20:16:43.000000 hello_robot_stretch_body-0.5.2/stretch_body/robot_params_RE1V0.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    19672 2023-07-31 20:16:43.000000 hello_robot_stretch_body-0.5.2/stretch_body/robot_params_RE2V0.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     4504 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/stretch_body/robot_trace.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    12072 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/stretch_body/scope.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    61278 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/stretch_body/stepper.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3829 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/stretch_body/stretch_gripper.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    29097 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/stretch_body/trajectories.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    45367 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/stretch_body/transport.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      213 2023-08-01 17:55:42.000000 hello_robot_stretch_body-0.5.2/stretch_body/version.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    20335 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/stretch_body/wacc.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1934 2023-08-01 01:05:35.000000 hello_robot_stretch_body-0.5.2/stretch_body/wrist_yaw.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     9733 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/stretch_body/xbox_controller.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-08-01 17:56:20.154151 hello_robot_stretch_body-0.5.2/test/
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       82 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/test/README.md
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        0 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/test/__init__.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-08-01 17:56:20.154151 hello_robot_stretch_body-0.5.2/test/rates/
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     5866 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/test/rates/test_arm_command_at_max_rate.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1748 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/test/rates/test_comm_loads.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1727 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/test/rates/test_pimu_sync_100hz.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     4497 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/test/rates/test_robot_command_at_max_rate.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1112 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/test/rates/test_robot_dxl_rates.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3835 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/test/rates/test_robot_nondxl_rates.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1668 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/test/rates/test_single_nondxl_rates.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     5087 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/test/rates/test_thread_locks.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     5384 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/test/test_arm.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6818 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/test/test_base.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     9977 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/test/test_collisions.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3198 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/test/test_device.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1111 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/test/test_dxl_comms.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3737 2023-07-31 22:05:44.000000 hello_robot_stretch_body-0.5.2/test/test_dxl_vel.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     7882 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/test/test_dynamixel_XL430.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    14520 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/test/test_dynamixel_hello_XL430.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1435 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/test/test_end_of_arm.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1914 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/test/test_end_of_arm_tools.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3833 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/test/test_head.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    23286 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/test/test_hello_utils.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     4761 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/test/test_lift.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2069 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/test/test_pimu.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     9004 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/test/test_robot.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2391 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/test/test_robot_params.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    26117 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/test/test_steppers.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1657 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/test/test_stretch_gripper.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6263 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/test/test_sync.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     4381 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/test/test_timing_stats.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    29747 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/test/test_trajectories.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3918 2023-07-20 04:51:17.000000 hello_robot_stretch_body-0.5.2/test/test_wrist_yaw.py
```

### Comparing `hello_robot_stretch_body-0.5.1.dev0/LICENSE.md` & `hello_robot_stretch_body-0.5.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/PKG-INFO` & `hello_robot_stretch_body-0.5.2/hello_robot_stretch_body.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,73 +1,76 @@
 Metadata-Version: 2.1
-Name: hello_robot_stretch_body
-Version: 0.5.1.dev0
+Name: hello-robot-stretch-body
+Version: 0.5.2
 Summary: Stretch Body low level Python API
 Home-page: https://github.com/hello-robot/stretch_body
 Author: Hello Robot Inc.
 Author-email: support@hello-robot.com
 License: UNKNOWN
-Description: Stretch Body
-        ============
-        
-        The stretch_body package provides a low level Python API to the Hello Robot Stretch hardware. This package comes pre-installed on Stretch robots. Tutorials for using this package can be found [on the docs](https://docs.hello-robot.com/0.2/stretch-tutorials/stretch_body/).
-        
-        Installing
-        ----------
-        
-        This package comes pre-installed on Stretch robots. To install or upgrade to a stable Stretch Body for Python3, run:
-        
-        ```bash
-        $ python3 -m pip install --upgrade hello-robot-stretch-body
-        ```
-        
-        To install or upgrade to a pre-release of Stretch Body for Python3, run:
-        
-        ```bash
-        $ python3 -m pip install --upgrade --pre hello-robot-stretch-body
-        ```
-        
-        Please report feedback on the [Issue Tracker](https://github.com/hello-robot/stretch_body/issues) or the [Forum](https://forum.hello-robot.com/).
-        
-        Running tests
-        -------------
-        
-        There are a number of unit, functional, and performance tests within the `test/` folder, separated into test suites by different files. Suites are separated by a device or functionality within Stretch Body that is being tested.
-        
-        In Python3, run `python3 -m unittest test.test_<suite-name>`.
-        
-        For example, to run the `stretch_body.robot.Robot` functional tests, run:
-        
-        ```bash
-        $ git clone https://github.com/hello-robot/stretch_body.git
-        $ cd stretch_body/body
-        $ python3 -m unittest test.test_robot
-        ```
-        
-        Developing
-        ----------
-        
-        The source code for Stretch Body resides within the `stretch_body/` folder. You can install Stretch Body as "editable", and directly edit the source code to test changes.
-        
-        In Python3, run `python3 -m pip install -e .`
-        
-        For example, to test changes to `stretch_body.robot.Robot`, run:
-        
-        ```bash
-        $ python3 -m pip uninstall hello-robot-stretch-body # ensure previous Stretch Body installations are removed
-        $ git clone https://github.com/hello-robot/stretch_body.git
-        $ cd stretch_body/body
-        $ python3 -m pip install -e .
-        ```
-        
-        Now, make desired edits to the [stretch_body/body/stretch_body/robot.py](./stretch_body/robot.py) file. Software using Stretch Body is now using the modified `stretch_body.robot.Robot` class.
-        
-        Deploying
-        ---------
-        
-        Increment the version number and run the `deploy.sh` script. Verify the new release is reflected [on PyPI](https://pypi.org/project/hello-robot-stretch-body/).
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+Stretch Body
+============
+
+The stretch_body package provides a low level Python API to the Hello Robot Stretch hardware. This package comes pre-installed on Stretch robots. Tutorials for using this package can be found [on the docs](https://docs.hello-robot.com/0.2/stretch-tutorials/stretch_body/).
+
+Installing
+----------
+
+This package comes pre-installed on Stretch robots. To install or upgrade to a stable Stretch Body for Python3, run:
+
+```bash
+$ python3 -m pip install --upgrade hello-robot-stretch-body
+```
+
+To install or upgrade to a pre-release of Stretch Body for Python3, run:
+
+```bash
+$ python3 -m pip install --upgrade --pre hello-robot-stretch-body
+```
+
+Please report feedback on the [Issue Tracker](https://github.com/hello-robot/stretch_body/issues) or the [Forum](https://forum.hello-robot.com/).
+
+Running tests
+-------------
+
+There are a number of unit, functional, and performance tests within the `test/` folder, separated into test suites by different files. Suites are separated by a device or functionality within Stretch Body that is being tested.
+
+In Python3, run `python3 -m unittest test.test_<suite-name>`.
+
+For example, to run the `stretch_body.robot.Robot` functional tests, run:
+
+```bash
+$ git clone https://github.com/hello-robot/stretch_body.git
+$ cd stretch_body/body
+$ python3 -m unittest test.test_robot
+```
+
+Developing
+----------
+
+The source code for Stretch Body resides within the `stretch_body/` folder. You can install Stretch Body as "editable", and directly edit the source code to test changes.
+
+In Python3, run `python3 -m pip install -e .`
+
+For example, to test changes to `stretch_body.robot.Robot`, run:
+
+```bash
+$ python3 -m pip uninstall hello-robot-stretch-body # ensure previous Stretch Body installations are removed
+$ git clone https://github.com/hello-robot/stretch_body.git
+$ cd stretch_body/body
+$ python3 -m pip install -e .
+```
+
+Now, make desired edits to the [stretch_body/body/stretch_body/robot.py](./stretch_body/robot.py) file. Software using Stretch Body is now using the modified `stretch_body.robot.Robot` class.
+
+Deploying
+---------
+
+Increment the version number and run the `deploy.sh` script. Verify the new release is reflected [on PyPI](https://pypi.org/project/hello-robot-stretch-body/).
+
+
```

### Comparing `hello_robot_stretch_body-0.5.1.dev0/README.md` & `hello_robot_stretch_body-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/hello_robot_stretch_body.egg-info/PKG-INFO` & `hello_robot_stretch_body-0.5.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,73 +1,76 @@
 Metadata-Version: 2.1
-Name: hello-robot-stretch-body
-Version: 0.5.1.dev0
+Name: hello_robot_stretch_body
+Version: 0.5.2
 Summary: Stretch Body low level Python API
 Home-page: https://github.com/hello-robot/stretch_body
 Author: Hello Robot Inc.
 Author-email: support@hello-robot.com
 License: UNKNOWN
-Description: Stretch Body
-        ============
-        
-        The stretch_body package provides a low level Python API to the Hello Robot Stretch hardware. This package comes pre-installed on Stretch robots. Tutorials for using this package can be found [on the docs](https://docs.hello-robot.com/0.2/stretch-tutorials/stretch_body/).
-        
-        Installing
-        ----------
-        
-        This package comes pre-installed on Stretch robots. To install or upgrade to a stable Stretch Body for Python3, run:
-        
-        ```bash
-        $ python3 -m pip install --upgrade hello-robot-stretch-body
-        ```
-        
-        To install or upgrade to a pre-release of Stretch Body for Python3, run:
-        
-        ```bash
-        $ python3 -m pip install --upgrade --pre hello-robot-stretch-body
-        ```
-        
-        Please report feedback on the [Issue Tracker](https://github.com/hello-robot/stretch_body/issues) or the [Forum](https://forum.hello-robot.com/).
-        
-        Running tests
-        -------------
-        
-        There are a number of unit, functional, and performance tests within the `test/` folder, separated into test suites by different files. Suites are separated by a device or functionality within Stretch Body that is being tested.
-        
-        In Python3, run `python3 -m unittest test.test_<suite-name>`.
-        
-        For example, to run the `stretch_body.robot.Robot` functional tests, run:
-        
-        ```bash
-        $ git clone https://github.com/hello-robot/stretch_body.git
-        $ cd stretch_body/body
-        $ python3 -m unittest test.test_robot
-        ```
-        
-        Developing
-        ----------
-        
-        The source code for Stretch Body resides within the `stretch_body/` folder. You can install Stretch Body as "editable", and directly edit the source code to test changes.
-        
-        In Python3, run `python3 -m pip install -e .`
-        
-        For example, to test changes to `stretch_body.robot.Robot`, run:
-        
-        ```bash
-        $ python3 -m pip uninstall hello-robot-stretch-body # ensure previous Stretch Body installations are removed
-        $ git clone https://github.com/hello-robot/stretch_body.git
-        $ cd stretch_body/body
-        $ python3 -m pip install -e .
-        ```
-        
-        Now, make desired edits to the [stretch_body/body/stretch_body/robot.py](./stretch_body/robot.py) file. Software using Stretch Body is now using the modified `stretch_body.robot.Robot` class.
-        
-        Deploying
-        ---------
-        
-        Increment the version number and run the `deploy.sh` script. Verify the new release is reflected [on PyPI](https://pypi.org/project/hello-robot-stretch-body/).
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+Stretch Body
+============
+
+The stretch_body package provides a low level Python API to the Hello Robot Stretch hardware. This package comes pre-installed on Stretch robots. Tutorials for using this package can be found [on the docs](https://docs.hello-robot.com/0.2/stretch-tutorials/stretch_body/).
+
+Installing
+----------
+
+This package comes pre-installed on Stretch robots. To install or upgrade to a stable Stretch Body for Python3, run:
+
+```bash
+$ python3 -m pip install --upgrade hello-robot-stretch-body
+```
+
+To install or upgrade to a pre-release of Stretch Body for Python3, run:
+
+```bash
+$ python3 -m pip install --upgrade --pre hello-robot-stretch-body
+```
+
+Please report feedback on the [Issue Tracker](https://github.com/hello-robot/stretch_body/issues) or the [Forum](https://forum.hello-robot.com/).
+
+Running tests
+-------------
+
+There are a number of unit, functional, and performance tests within the `test/` folder, separated into test suites by different files. Suites are separated by a device or functionality within Stretch Body that is being tested.
+
+In Python3, run `python3 -m unittest test.test_<suite-name>`.
+
+For example, to run the `stretch_body.robot.Robot` functional tests, run:
+
+```bash
+$ git clone https://github.com/hello-robot/stretch_body.git
+$ cd stretch_body/body
+$ python3 -m unittest test.test_robot
+```
+
+Developing
+----------
+
+The source code for Stretch Body resides within the `stretch_body/` folder. You can install Stretch Body as "editable", and directly edit the source code to test changes.
+
+In Python3, run `python3 -m pip install -e .`
+
+For example, to test changes to `stretch_body.robot.Robot`, run:
+
+```bash
+$ python3 -m pip uninstall hello-robot-stretch-body # ensure previous Stretch Body installations are removed
+$ git clone https://github.com/hello-robot/stretch_body.git
+$ cd stretch_body/body
+$ python3 -m pip install -e .
+```
+
+Now, make desired edits to the [stretch_body/body/stretch_body/robot.py](./stretch_body/robot.py) file. Software using Stretch Body is now using the modified `stretch_body.robot.Robot` class.
+
+Deploying
+---------
+
+Increment the version number and run the `deploy.sh` script. Verify the new release is reflected [on PyPI](https://pypi.org/project/hello-robot-stretch-body/).
+
+
```

### Comparing `hello_robot_stretch_body-0.5.1.dev0/hello_robot_stretch_body.egg-info/SOURCES.txt` & `hello_robot_stretch_body-0.5.2/hello_robot_stretch_body.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/hello_robot_stretch_body.egg-info/requires.txt` & `hello_robot_stretch_body-0.5.2/hello_robot_stretch_body.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/setup.py` & `hello_robot_stretch_body-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/stretch_body/arm.py` & `hello_robot_stretch_body-0.5.2/stretch_body/arm.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/stretch_body/base.py` & `hello_robot_stretch_body-0.5.2/stretch_body/base.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/stretch_body/cobbs_framing.py` & `hello_robot_stretch_body-0.5.2/stretch_body/cobbs_framing.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/stretch_body/device.py` & `hello_robot_stretch_body-0.5.2/stretch_body/device.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/stretch_body/dynamixel_XL430.py` & `hello_robot_stretch_body-0.5.2/stretch_body/dynamixel_XL430.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/stretch_body/dynamixel_X_chain.py` & `hello_robot_stretch_body-0.5.2/stretch_body/dynamixel_X_chain.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/stretch_body/dynamixel_hello_XL430.py` & `hello_robot_stretch_body-0.5.2/stretch_body/dynamixel_hello_XL430.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/stretch_body/end_of_arm.py` & `hello_robot_stretch_body-0.5.2/stretch_body/end_of_arm.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/stretch_body/end_of_arm_tools.py` & `hello_robot_stretch_body-0.5.2/stretch_body/end_of_arm_tools.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/stretch_body/head.py` & `hello_robot_stretch_body-0.5.2/stretch_body/head.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/stretch_body/hello_utils.py` & `hello_robot_stretch_body-0.5.2/stretch_body/hello_utils.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/stretch_body/lift.py` & `hello_robot_stretch_body-0.5.2/stretch_body/lift.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/stretch_body/pimu.py` & `hello_robot_stretch_body-0.5.2/stretch_body/pimu.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,15 +188,15 @@
         if usb is None:
             usb = self.params['usb_name']
         self.transport = Transport(usb=usb, logger=self.logger)
         self.status = {'voltage': 0, 'current': 0, 'temp': 0,'cpu_temp': 0, 'cliff_range':[0,0,0,0], 'frame_id': 0,
                        'timestamp': 0,'at_cliff':[False,False,False,False], 'runstop_event': False, 'bump_event_cnt': 0,
                        'cliff_event': False, 'fan_on': False, 'buzzer_on': False, 'low_voltage_alert':False,'high_current_alert':False,'over_tilt_alert':False,
                        'charger_connected':False, 'boot_detected':False,'imu': self.imu.status,'debug':0,'state':0,'trace_on':0,
-                       'motor_sync_rate': 0, 'motor_sync_cnt': 0, 'motor_sync_queues': 0,
+                       'motor_sync_rate': 0, 'motor_sync_cnt': 0, 'motor_sync_queues': 0, 'motor_sync_drop': 0,
                        'transport': self.transport.status}
 
         self.status_zero=self.status.copy()
         self.status_aux = {'foo': 0}
 
         self._trigger=0
         self.ts_last_fan_on=None
```

### Comparing `hello_robot_stretch_body-0.5.1.dev0/stretch_body/prismatic_joint.py` & `hello_robot_stretch_body-0.5.2/stretch_body/prismatic_joint.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/stretch_body/robot.py` & `hello_robot_stretch_body-0.5.2/stretch_body/robot.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # #############################################################
 class DXLHeadStatusThread(threading.Thread):
     """
     This thread polls the status data of the Dynamixel devices
     at 15Hz
     """
     def __init__(self, robot, target_rate_hz=15.0):
-        threading.Thread.__init__(self)
+        threading.Thread.__init__(self, name = self.__class__.__name__)
         self.robot=robot
         self.robot_update_rate_hz = target_rate_hz
         self.stats = hello_utils.LoopStats(loop_name='DXLHeadStatusThread',target_loop_rate=self.robot_update_rate_hz)
         self.shutdown_flag = threading.Event()
         self.running=False
 
     def step(self):
@@ -50,15 +50,15 @@
 
 class DXLEndOfArmStatusThread(threading.Thread):
     """
     This thread polls the status data of the Dynamixel devices
     at 15Hz
     """
     def __init__(self, robot, target_rate_hz=15.0):
-        threading.Thread.__init__(self)
+        threading.Thread.__init__(self, name = self.__class__.__name__)
         self.robot=robot
         self.robot_update_rate_hz = target_rate_hz
         self.stats = hello_utils.LoopStats(loop_name='DXLEndOfArmStatusThread',target_loop_rate=self.robot_update_rate_hz)
         self.shutdown_flag = threading.Event()
         self.running = False
     def step(self):
         self.stats.mark_loop_start()
@@ -76,15 +76,15 @@
 class NonDXLStatusThread(threading.Thread):
     """
     This thread runs at 25Hz.
     It updates the status data of the Devices.
     It also steps the Sentry, Monitor, and Collision functions
     """
     def __init__(self, robot, target_rate_hz=25.0):
-        threading.Thread.__init__(self)
+        threading.Thread.__init__(self, name = self.__class__.__name__)
         self.robot=robot
         self.robot_update_rate_hz = target_rate_hz
         self.shutdown_flag = threading.Event()
         self.stats = hello_utils.LoopStats(loop_name='NonDXLStatusThread',target_loop_rate=self.robot_update_rate_hz)
         self.titr=0
         self.first_status = False
         self.loop = asyncio.new_event_loop()
@@ -115,15 +115,15 @@
 class SystemMonitorThread(threading.Thread):
     """
     This thread runs at 25Hz.
     It updates the status data of the Devices.
     It also steps the Sentry, Monitor, and Collision functions
     """
     def __init__(self, robot, target_rate_hz=25.0):
-        threading.Thread.__init__(self)
+        threading.Thread.__init__(self, name = self.__class__.__name__)
         self.robot=robot
         self.robot_update_rate_hz = target_rate_hz
         self.monitor_downrate_int = int(robot.params['rates']['SystemMonitorThread_monitor_downrate_int'])  # Step the monitor at every Nth iteration
         self.trace_downrate_int = int(robot.params['rates']['SystemMonitorThread_trace_downrate_int'])  # Step the trace at every Nth iteration
         self.sentry_downrate_int = int(robot.params['rates']['SystemMonitorThread_sentry_downrate_int']) # Step the sentry at every Nth iteration
         self.collision_downrate_int = int(robot.params['rates']['SystemMonitorThread_collision_downrate_int'])  # Step the monitor at every Nth iteration
         self.trajectory_downrate_int = int(robot.params['rates']['SystemMonitorThread_nondxl_trajectory_downrate_int'])  # Update hardware with waypoint trajectory segments at every Nth iteration
@@ -519,15 +519,15 @@
         self.end_of_arm.step_sentry(self)
     
     def start_event_loop(self):
         self.async_event_loop = asyncio.new_event_loop()
         def start_loop(loop):
             asyncio.set_event_loop(loop)
             loop.run_forever()
-        self.event_loop_thread = threading.Thread(target=start_loop, args=(self.async_event_loop,))
+        self.event_loop_thread = threading.Thread(target=start_loop, args=(self.async_event_loop,), name='AsyncEvenLoopThread')
         self.event_loop_thread.start()
     
     def stop_event_loop(self):
         try:
             if self.event_loop_thread:
                 self.async_event_loop.call_soon_threadsafe(self.async_event_loop.stop())
                 self.event_loop_thread.join()
```

### Comparing `hello_robot_stretch_body-0.5.1.dev0/stretch_body/robot_collision.py` & `hello_robot_stretch_body-0.5.2/stretch_body/robot_collision.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/stretch_body/robot_collision_models.py` & `hello_robot_stretch_body-0.5.2/stretch_body/robot_collision_models.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/stretch_body/robot_monitor.py` & `hello_robot_stretch_body-0.5.2/stretch_body/robot_monitor.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/stretch_body/robot_params.py` & `hello_robot_stretch_body-0.5.2/stretch_body/robot_params.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/stretch_body/robot_params_RE1V0.py` & `hello_robot_stretch_body-0.5.2/stretch_body/robot_params_RE1V0.py`

 * *Files 0% similar despite different names*

```diff
@@ -289,15 +289,15 @@
             'flip_encoder_polarity': 1,
             'iMax_neg': -2.8,
             'iMax_pos': 2.8,
             'i_contact_neg': -3.0,
             'i_contact_pos': 3.0,
             'i_safety_feedforward': 0.0,
             'pKd_d': 40.0,
-            'pKi_d': 0.0,
+            'pKi_d': 0.1,
             'pKi_limit': 200,
             'pKp_d': 8.0,
             'pLPF': 200,
             'phase_advance_d': 1.8,
             'pos_near_setpoint_d': 1.0,
             'safety_hold': 0,
             'safety_stiffness': 1.0,
@@ -361,15 +361,15 @@
             'flip_encoder_polarity': 0,
             'iMax_neg': -2.8,
             'iMax_pos': 2.8,
             'i_contact_neg': -3.0,
             'i_contact_pos': 3.0,
             'i_safety_feedforward': 0.0,
             'pKd_d': 40.0,
-            'pKi_d': 0.0,
+            'pKi_d': 0.1,
             'pKi_limit': 200,
             'pKp_d': 8.0,
             'pLPF': 200,
             'phase_advance_d': 1.8,
             'pos_near_setpoint_d': 1.0,
             'safety_hold': 0,
             'safety_stiffness': 1.0,
```

### Comparing `hello_robot_stretch_body-0.5.1.dev0/stretch_body/robot_params_RE2V0.py` & `hello_robot_stretch_body-0.5.2/stretch_body/robot_params_RE2V0.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,16 +286,16 @@
             'flip_encoder_polarity': 1,
             'iMax_neg': -4.35,
             'iMax_pos': 4.35,
             'i_contact_neg': -3.0,
             'i_contact_pos': 3.0,
             'i_safety_feedforward': 0.0,
             'pKd_d': 65.0,
-            'pKi_d': 0.01,
-            'pKi_limit': 50.0,
+            'pKi_d': 0.1,
+            'pKi_limit': 200.0,
             'pKp_d': 12.0,
             'pLPF': 80.0,
             'phase_advance_d': 1.8,
             'pos_near_setpoint_d': 1.0,
             'safety_hold': 0,
             'safety_stiffness': 1.0,
             'vKd_d': 0,
@@ -358,16 +358,16 @@
             'flip_encoder_polarity': 0,
             'iMax_neg': -4.35,
             'iMax_pos': 4.35,
             'i_contact_neg': -3.0,
             'i_contact_pos': 3.0,
             'i_safety_feedforward': 0.0,
             'pKd_d': 65.0,
-            'pKi_d': 0.01,
-            'pKi_limit': 50.0,
+            'pKi_d': 0.1,
+            'pKi_limit': 200.0,
             'pKp_d': 12.0,
             'pLPF': 80.0,
             'phase_advance_d': 1.8,
             'pos_near_setpoint_d': 1.0,
             'safety_hold': 0,
             'safety_stiffness': 1.0,
             'vKd_d': 0,
```

### Comparing `hello_robot_stretch_body-0.5.1.dev0/stretch_body/robot_trace.py` & `hello_robot_stretch_body-0.5.2/stretch_body/robot_trace.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/stretch_body/scope.py` & `hello_robot_stretch_body-0.5.2/stretch_body/scope.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/stretch_body/stepper.py` & `hello_robot_stretch_body-0.5.2/stretch_body/stepper.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/stretch_body/stretch_gripper.py` & `hello_robot_stretch_body-0.5.2/stretch_body/stretch_gripper.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/stretch_body/trajectories.py` & `hello_robot_stretch_body-0.5.2/stretch_body/trajectories.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/stretch_body/transport.py` & `hello_robot_stretch_body-0.5.2/stretch_body/transport.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/stretch_body/wacc.py` & `hello_robot_stretch_body-0.5.2/stretch_body/wacc.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/stretch_body/wrist_yaw.py` & `hello_robot_stretch_body-0.5.2/stretch_body/wrist_yaw.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/stretch_body/xbox_controller.py` & `hello_robot_stretch_body-0.5.2/stretch_body/xbox_controller.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/test/rates/test_arm_command_at_max_rate.py` & `hello_robot_stretch_body-0.5.2/test/rates/test_arm_command_at_max_rate.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/test/rates/test_comm_loads.py` & `hello_robot_stretch_body-0.5.2/test/rates/test_comm_loads.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/test/rates/test_pimu_sync_100hz.py` & `hello_robot_stretch_body-0.5.2/test/rates/test_pimu_sync_100hz.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/test/rates/test_robot_command_at_max_rate.py` & `hello_robot_stretch_body-0.5.2/test/rates/test_robot_command_at_max_rate.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/test/rates/test_robot_dxl_rates.py` & `hello_robot_stretch_body-0.5.2/test/rates/test_robot_dxl_rates.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/test/rates/test_robot_nondxl_rates.py` & `hello_robot_stretch_body-0.5.2/test/rates/test_robot_nondxl_rates.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/test/rates/test_single_nondxl_rates.py` & `hello_robot_stretch_body-0.5.2/test/rates/test_single_nondxl_rates.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/test/rates/test_thread_locks.py` & `hello_robot_stretch_body-0.5.2/test/rates/test_thread_locks.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/test/test_arm.py` & `hello_robot_stretch_body-0.5.2/test/test_arm.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/test/test_base.py` & `hello_robot_stretch_body-0.5.2/test/test_base.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/test/test_collisions.py` & `hello_robot_stretch_body-0.5.2/test/test_collisions.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/test/test_device.py` & `hello_robot_stretch_body-0.5.2/test/test_device.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/test/test_dxl_comms.py` & `hello_robot_stretch_body-0.5.2/test/test_dxl_comms.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/test/test_dxl_vel.py` & `hello_robot_stretch_body-0.5.2/test/test_dxl_vel.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/test/test_dynamixel_XL430.py` & `hello_robot_stretch_body-0.5.2/test/test_dynamixel_XL430.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/test/test_dynamixel_hello_XL430.py` & `hello_robot_stretch_body-0.5.2/test/test_dynamixel_hello_XL430.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/test/test_end_of_arm.py` & `hello_robot_stretch_body-0.5.2/test/test_end_of_arm.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/test/test_end_of_arm_tools.py` & `hello_robot_stretch_body-0.5.2/test/test_end_of_arm_tools.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/test/test_head.py` & `hello_robot_stretch_body-0.5.2/test/test_head.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/test/test_hello_utils.py` & `hello_robot_stretch_body-0.5.2/test/test_hello_utils.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/test/test_lift.py` & `hello_robot_stretch_body-0.5.2/test/test_lift.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/test/test_pimu.py` & `hello_robot_stretch_body-0.5.2/test/test_pimu.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/test/test_robot.py` & `hello_robot_stretch_body-0.5.2/test/test_robot.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/test/test_robot_params.py` & `hello_robot_stretch_body-0.5.2/test/test_robot_params.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/test/test_steppers.py` & `hello_robot_stretch_body-0.5.2/test/test_steppers.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/test/test_stretch_gripper.py` & `hello_robot_stretch_body-0.5.2/test/test_stretch_gripper.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/test/test_sync.py` & `hello_robot_stretch_body-0.5.2/test/test_sync.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/test/test_timing_stats.py` & `hello_robot_stretch_body-0.5.2/test/test_timing_stats.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/test/test_trajectories.py` & `hello_robot_stretch_body-0.5.2/test/test_trajectories.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.5.1.dev0/test/test_wrist_yaw.py` & `hello_robot_stretch_body-0.5.2/test/test_wrist_yaw.py`

 * *Files identical despite different names*

