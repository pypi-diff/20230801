# Comparing `tmp/neon-skill-update-1.0.0.tar.gz` & `tmp/neon-skill-update-1.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-update-1.0.0.tar", last modified: Thu Jun 29 16:58:45 2023, max compression
+gzip compressed data, was "neon-skill-update-1.0.1a1.tar", last modified: Mon Jul 31 22:14:23 2023, max compression
```

## Comparing `neon-skill-update-1.0.0.tar` & `neon-skill-update-1.0.1a1.tar`

### file list

```diff
@@ -1,65 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:58:45.099940 neon-skill-update-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-29 16:58:45.099940 neon-skill-update-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    18436 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:58:45.091940 neon-skill-update-1.0.0/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:58:45.091940 neon-skill-update-1.0.0/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:58:45.095940 neon-skill-update-1.0.0/locale/en-us/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/alpha.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/ask_change_update_track.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/ask_download_image.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/ask_overwrite_drive.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/ask_update_configuration.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/check_error.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/check_updates.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/confirm_change_update_track.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/confirm_no_change_update_track.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/core_version.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/downloading_image.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/drive_instructions.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/error_installing_os.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/error_offline.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/installation_complete.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/not_updating.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/notify_download_complete.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/notify_download_failed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/notify_installation_complete.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/notify_installation_failed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/notify_update_available.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/notify_update_failure.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/notify_update_success.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/notify_writing_image.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/point.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/starting_installation.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/starting_update.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/up_to_date.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/update_core.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/update_track_already_set.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/word_beta.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/word_stable.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:58:45.095940 neon-skill-update-1.0.0/locale/en-us/intent/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/intent/core_version.intent
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/intent/update_configuration.intent
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/intent/update_device.intent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:58:45.095940 neon-skill-update-1.0.0/locale/en-us/vocab/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/vocab/beta.voc
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/vocab/change.voc
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/vocab/create.voc
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/vocab/media.voc
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/vocab/os.voc
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/vocab/stable.voc
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/vocab/updates.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:58:45.099940 neon-skill-update-1.0.0/neon_skill_update.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-29 16:58:45.000000 neon-skill-update-1.0.0/neon_skill_update.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-29 16:58:45.000000 neon-skill-update-1.0.0/neon_skill_update.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 16:58:45.000000 neon-skill-update-1.0.0/neon_skill_update.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-29 16:58:45.000000 neon-skill-update-1.0.0/neon_skill_update.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-29 16:58:45.000000 neon-skill-update-1.0.0/neon_skill_update.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 16:58:45.000000 neon-skill-update-1.0.0/neon_skill_update.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 16:58:45.099940 neon-skill-update-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:58:45.099940 neon-skill-update-1.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)    18648 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/test/test_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:14:23.208552 neon-skill-update-1.0.1a1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-31 22:14:23.208552 neon-skill-update-1.0.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    22527 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:14:23.188552 neon-skill-update-1.0.1a1/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:14:23.188552 neon-skill-update-1.0.1a1/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:14:23.204552 neon-skill-update-1.0.1a1/locale/en-us/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/alpha.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/ask_change_update_track.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/ask_download_image.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/ask_overwrite_drive.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/ask_update_configuration.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/check_error.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/check_updates.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/confirm_change_update_track.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/confirm_no_change_update_track.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/core_version.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/downloading_image.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/drive_instructions.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/error_installing_os.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/error_offline.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/error_updating_os.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/installation_complete.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/not_updating.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/notify_download_complete.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/notify_download_failed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/notify_downloading_update.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/notify_installation_complete.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/notify_installation_failed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/notify_update_available.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/notify_update_failure.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/notify_update_success.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/notify_writing_image.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/point.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/starting_installation.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/starting_update.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/up_to_date.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/update_core.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/update_restarting.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/update_system.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/update_track_already_set.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/word_beta.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/dialog/word_stable.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:14:23.204552 neon-skill-update-1.0.1a1/locale/en-us/intent/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/intent/core_version.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/intent/update_configuration.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/intent/update_device.intent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:14:23.204552 neon-skill-update-1.0.1a1/locale/en-us/vocab/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/vocab/beta.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/vocab/change.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/vocab/create.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/vocab/media.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/vocab/os.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/vocab/stable.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/locale/en-us/vocab/updates.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:14:23.208552 neon-skill-update-1.0.1a1/neon_skill_update.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-31 22:14:23.000000 neon-skill-update-1.0.1a1/neon_skill_update.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-07-31 22:14:23.000000 neon-skill-update-1.0.1a1/neon_skill_update.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 22:14:23.000000 neon-skill-update-1.0.1a1/neon_skill_update.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-31 22:14:23.000000 neon-skill-update-1.0.1a1/neon_skill_update.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-31 22:14:23.000000 neon-skill-update-1.0.1a1/neon_skill_update.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-31 22:14:23.000000 neon-skill-update-1.0.1a1/neon_skill_update.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 22:14:23.208552 neon-skill-update-1.0.1a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:14:23.208552 neon-skill-update-1.0.1a1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    18658 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/test/test_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-31 22:14:18.000000 neon-skill-update-1.0.1a1/version.py
```

### Comparing `neon-skill-update-1.0.0/LICENSE.md` & `neon-skill-update-1.0.1a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-update-1.0.0/PKG-INFO` & `neon-skill-update-1.0.1a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-update
-Version: 1.0.0
+Version: 1.0.1a1
 Home-page: https://github.com/NeonGeckoCom/skill-update
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-update-1.0.0/README.md` & `neon-skill-update-1.0.1a1/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-update-1.0.0/__init__.py` & `neon-skill-update-1.0.1a1/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,46 +25,76 @@
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import os
 
 from random import randint
+from threading import Event
 from typing import Optional
 from adapt.intent import IntentBuilder
 from neon_utils.validator_utils import numeric_confirmation_validator
+from ovos_bus_client import Message
 from ovos_utils import classproperty
 from ovos_utils.log import LOG
 from ovos_utils.process_utils import RuntimeRequirements
 from ovos_utils.network_utils import is_connected_http
 from neon_utils.skills import NeonSkill
 from neon_utils.user_utils import get_user_prefs
-from mycroft.skills import intent_file_handler, intent_handler
+from ovos_workshop.decorators import intent_file_handler, intent_handler
 
 
 class UpdateSkill(NeonSkill):
     def __init__(self, **kwargs):
         NeonSkill.__init__(self, **kwargs)
-        self.current_ver = None
-        self.latest_ver = None
+        self.current_core_ver = None
+        self.latest_core_ver = None
         self._update_filename = "update_signal"
+        self._os_updates_supported = None
+
+        self.add_event('mycroft.ready', self._on_ready)
+        self.add_event("update.gui.continue_installation",
+                       self.continue_os_installation)
+        self.add_event("update.gui.finish_installation",
+                       self.finish_os_installation)
+        self.add_event("update.gui.install_update", self.handle_update_device)
 
     @classproperty
     def runtime_requirements(self):
         return RuntimeRequirements(network_before_load=False,
                                    internet_before_load=False,
                                    gui_before_load=False,
                                    requires_internet=True,
                                    requires_network=True,
                                    requires_gui=False,
                                    no_internet_fallback=False,
                                    no_network_fallback=False,
                                    no_gui_fallback=True)
 
     @property
+    def os_updates_supported(self) -> bool:
+        if self._os_updates_supported is None:
+            try:
+                import neon_phal_plugin_device_updater
+                self._os_updates_supported = True
+            except ImportError:
+                self._os_updates_supported = False
+        return self._os_updates_supported
+
+    @property
+    def check_initramfs(self) -> bool:
+        return bool(self.settings.get("update_initramfs",
+                                      self.os_updates_supported))
+
+    @property
+    def check_squashfs(self) -> bool:
+        return bool(self.settings.get("update_squashfs",
+                                      self.os_updates_supported))
+
+    @property
     def notify_updates(self):
         return self.settings.get("notify_updates", True)
 
     @property
     def include_prerelease(self):
         return self.settings.get("include_prerelease", False)
 
@@ -77,33 +107,24 @@
     def image_url(self):
         return self.settings.get("image_url")
 
     @property
     def image_drive(self):
         return self.settings.get("image_drive") or "/dev/sdb"
 
-    # TODO: Move to __init__ after stable ovos-workshop
-    def initialize(self):
-        self.add_event('mycroft.ready', self._on_ready)
-        self.add_event("update.gui.continue_installation",
-                       self.continue_os_installation)
-        self.add_event("update.gui.finish_installation",
-                       self.finish_os_installation)
-        self.add_event("update.gui.install_update", self.handle_update_device)
-
     def _on_ready(self, message):
         LOG.debug("Checking latest core version")
         self._check_latest_core_release(message)
 
         update_stat = self._check_update_status()
         LOG.debug(f"Update status is {update_stat}")
         if not update_stat:
             # No update was attempted
             return
-        speak_version = self.pronounce_version(self.current_ver)
+        speak_version = self.pronounce_version(self.current_core_ver)
         if update_stat is True:
             LOG.debug("Update success")
             self.speak_dialog("notify_update_success",
                               {"version": speak_version})
         elif update_stat is False:
             LOG.warning("Update failed")
             self.speak_dialog("notify_update_failure",
@@ -116,25 +137,26 @@
         """
         response = self.bus.wait_for_response(
             message.forward("neon.core_updater.check_update",
                             {'include_prerelease': self.include_prerelease}),
             timeout=15)
         if response:
             LOG.debug(f"Got response: {response.data}")
-            self.current_ver = response.data.get("installed_version")
-            self.latest_ver = response.data.get("latest_version") or \
+            self.current_core_ver = response.data.get("installed_version")
+            self.latest_core_ver = response.data.get("latest_version") or \
                 response.data.get("new_version")
-            if not self.latest_ver:
+            if not self.latest_core_ver:
                 LOG.error(f"Expected string version and got none in response: "
                           f"{response.data}")
-            elif self.latest_ver != self.current_ver and \
+            elif self.latest_core_ver != self.current_core_ver and \
                     self.notify_updates and \
                     message.msg_type in ("mycroft.ready", "neon.update.check"):
-                text = self.dialog_renderer.render("notify_update_available",
-                                                   {"version": self.latest_ver})
+                text = self.dialog_renderer.render(
+                    "notify_update_available",
+                    {"version": self.latest_core_ver})
                 LOG.info("Update Available")
                 callback_data = {**message.data, **{"notification": text}}
                 self.gui.show_notification(text,
                                            action="update.gui.install_update",
                                            callback_data=callback_data)
 
         else:
@@ -152,43 +174,126 @@
 
     @intent_file_handler("update_device.intent")
     def handle_update_device(self, message):
         """
         Handle a user request to check for updates.
         :param message: message object associated with request
         """
-        if get_user_prefs(message)['response_mode'].get('hesitation'):
+        # Explicitly enabled for initramfs checks that involve file downloads
+        if get_user_prefs(message)['response_mode'].get('hesitation') or \
+                self.check_initramfs:
             self.speak_dialog("check_updates")
+        initramfs_available = False
+        squashfs_available = False
+
+        if self.check_initramfs:
+            initramfs_available = self._check_initramfs_update(message)
+        if self.check_squashfs:
+            squashfs_available = self._check_squashfs_update(message)
+
+        if initramfs_available or squashfs_available:
+            resp = self.ask_yesno("update_system")
+            if resp == "yes":
+                self.speak_dialog("starting_update", wait=True)
+
+                if initramfs_available:
+                    LOG.info("Updating initramfs")
+                    resp = self.bus.wait_for_response(
+                        message.forward("neon.update_initramfs"), timeout=30)
+                    if resp and resp.data.get("updated"):
+                        LOG.info("initramfs updated")
+                        # TODO: Speak?
+                    else:
+                        error = resp.data.get("error")
+                        LOG.error(f"initramfs update failed: {error}")
+                        self.speak_dialog("error_updating_os")
+                        return
+                if squashfs_available:
+                    self._write_update_signal("squashfs")
+
+                    self.gui.show_controlled_notification(
+                        self.translate("notify_downloading_update"))
+
+                    LOG.info("Updating squashfs")
+                    resp = self.bus.wait_for_response(
+                        message.forward("neon.update_squashfs"), timeout=1800)
+                    if not resp:
+                        LOG.warning(f"Timed out waiting for download")
+                        self.gui.remove_controlled_notification()
+                        self.speak_dialog("error_updating_os")
+                        return
+                    self.gui.remove_controlled_notification()
+                    if resp.data.get("new_version"):
+                        LOG.info("squashfs updated")
+                        self.speak_dialog("update_restarting", wait=True)
+                        self.bus.emit(message.forward("system.reboot"))
+                    else:
+                        error = "no response"
+                        if resp:
+                            error = resp.data.get("error")
+                        LOG.error(f"squashfs update failed: {error}")
+                        self.speak_dialog("error_updating_os")
+                        return
+
+                return
+        # No OS update available or user declined, check core updates
+        self._check_package_update(message)
+
+    def _check_initramfs_update(self, message) -> bool:
+        """
+        Check for an updated initramfs image
+        """
+        resp = self.bus.wait_for_response(message.forward(
+            "neon.check_update_initramfs"), timeout=10)
+        if resp and resp.data.get("update_available"):
+            LOG.info("Initramfs update available")
+            return True
+        LOG.debug("No initramfs update")
+        return False
+
+    def _check_squashfs_update(self, message) -> bool:
+        """
+        Check for an updated squashfs image
+        """
+        resp = self.bus.wait_for_response(message.forward(
+            "neon.check_update_squashfs"), timeout=10)
+        if resp and resp.data.get("update_available"):
+            LOG.info("Squashfs update available")
+            return True
+        LOG.debug("No Squashfs update")
+        return False
+
+    def _check_package_update(self, message):
         self._check_latest_core_release(message)
-        if not all((self.current_ver, self.latest_ver)):
+        if not all((self.current_core_ver, self.latest_core_ver)):
             self.speak_dialog("check_error")
             return
 
         # TODO: Support alternate update sources?
         if not is_connected_http("https://github.com"):
             LOG.warning(f"GitHub not available. Skipping update")
             self.speak_dialog("error_offline")
             return
 
-        if self.current_ver == self.latest_ver:
+        if self.current_core_ver == self.latest_core_ver:
             resp = self.ask_yesno(
                 "up_to_date",
-                {"version": self.pronounce_version(self.current_ver)})
+                {"version": self.pronounce_version(self.current_core_ver)})
         else:
             resp = self.ask_yesno(
                 "update_core",
-                {"new": self.pronounce_version(self.latest_ver),
-                 "old": self.pronounce_version(self.current_ver)})
+                {"new": self.pronounce_version(self.latest_core_ver),
+                 "old": self.pronounce_version(self.current_core_ver)})
         if resp == "yes":
             if message.data.get('notification'):
                 self._dismiss_notification(message)
-            self._write_update_signal(self.latest_ver)
+            self._write_update_signal(self.latest_core_ver)
             self.speak_dialog("starting_update", wait=True)
             self.bus.emit(message.forward("neon.core_updater.start_update",
-                                          {"version": self.latest_ver}))
+                                          {"version": self.latest_core_ver}))
         else:
             self.speak_dialog("not_updating")
 
     def _write_update_signal(self, new_ver: str):
         """
         Write a file with the version being updated to that can be checked upon
         next boot
@@ -209,28 +314,31 @@
                                        self._update_filename)
         if not os.path.exists(update_filepath):
             return None
         with open(update_filepath, 'r') as f:
             expected_ver = f.read()
         os.remove(update_filepath)
         LOG.info(f"Removed update signal at {update_filepath}")
-        if self.current_ver != expected_ver:
+        if expected_ver == "squashfs":
+            LOG.info("Updated squashFS")
+            return True
+        if self.current_core_ver != expected_ver:
             LOG.error(f"Update expected {expected_ver} but "
-                      f"{self.current_ver} is installed")
+                      f"{self.current_core_ver} is installed")
             return False
         return True
 
     @intent_file_handler("core_version.intent")
     def handle_core_version(self, message):
         """
         Handle a user request for the current installed version.
         :param message: message object associated with request
         """
         self._check_latest_core_release(message)
-        version = self.pronounce_version(self.current_ver)
+        version = self.pronounce_version(self.current_core_ver)
         LOG.debug(version)
         self.speak_dialog("core_version", {"version": version})
 
     @intent_file_handler("update_configuration.intent")
     def handle_update_configuration(self, message):
         """
         Handle a user request to update default configuration
@@ -301,37 +409,29 @@
     def on_download_complete(self, message):
         """
         After `handle_create_os_media`, this method will be called with the OS
         image download status. Displays a notification for the user to interact
         with to continue installation.
         :param message: message object associated with download completion
         """
-        # TODO: Use Notification API from ovos_utils
         if message.data.get("success"):
+            LOG.info(f"Showing Download Complete Notification")
             text = self.translate("notify_download_complete")
-            notification_data = {
-                "sender": self.skill_id,
-                "text": text,
-                "action": "update.gui.continue_installation",
-                "type": "transient",
-                "style": "info",
-                "callback_data": {**message.data, **{"notification": text}}
-            }
+            self.gui.show_notification(
+                content=text,
+                action="update.gui.continue_installation",
+                callback_data={**message.data, **{"notification": text}})
+
         else:
+            LOG.info(f"Showing Download Failed Notification")
             text = self.translate("notify_download_failed")
-            notification_data = {
-                "sender": self.skill_id,
-                "text": text,
-                "type": "transient",
-                "style": "error",
-                "callback_data": {**message.data, **{"notification": text}}
-            }
-        LOG.info(f"Showing Download Complete Notification: {notification_data}")
-        self.bus.emit(message.forward("ovos.notification.api.set",
-                                      notification_data))
+            self.gui.show_notification(content=text,
+                                       style="error",
+                                       callback_data={**message.data,
+                                                      **{"notification": text}})
 
     def continue_os_installation(self, message):
         """
         After the user interacts with the completed download notification,
         prompt confirmation to clear data
         :param message: message object associated with notification interaction
         """
@@ -362,38 +462,30 @@
         """
         After `continue_os_installation`, this method will be called with the
         image write status. Displays a notification telling the user they may
         restart and use the new image.
         """
         self.bus.emit(message.forward(
             "ovos.notification.api.remove.controlled"))
-        # TODO: Use Notification API from ovos_utils
         if message.data.get("success"):
+            LOG.info("Showing Write Complete Notification")
             text = self.translate("notify_installation_complete")
-            notification_data = {
-                "sender": self.skill_id,
-                "text": text,
-                "action": "update.gui.finish_installation",
-                "type": "transient",
-                "style": "info",
-                "callback_data": {**message.data, **{"notification": text}}
-            }
+            self.gui.show_notification(content=text,
+                                       action="update.gui.finish_installation",
+                                       callback_data={**message.data,
+                                                      **{"notification": text}})
+
         else:
+            LOG.info("Showing Write Failed Notification")
             text = self.translate("notify_installation_failed")
-            notification_data = {
-                "sender": self.skill_id,
-                "text": text,
-                "action": "update.gui.finish_installation",
-                "type": "transient",
-                "style": "error",
-                "callback_data": {**message.data, **{"notification": text}}
-            }
-        LOG.info(f"Showing Download Complete Notification: {notification_data}")
-        self.bus.emit(message.forward("ovos.notification.api.set",
-                                      notification_data))
+            self.gui.show_notification(content=text,
+                                       action="update.gui.finish_installation",
+                                       style="error",
+                                       callback_data={**message.data,
+                                                      **{"notification": text}})
 
     def finish_os_installation(self, message):
         """
         After the user interacts with the installation complete message, speak
         an error if installation failed or else speak instructions before
         shutting down.
         """
```

### Comparing `neon-skill-update-1.0.0/neon_skill_update.egg-info/PKG-INFO` & `neon-skill-update-1.0.1a1/neon_skill_update.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-update
-Version: 1.0.0
+Version: 1.0.1a1
 Home-page: https://github.com/NeonGeckoCom/skill-update
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-update-1.0.0/neon_skill_update.egg-info/SOURCES.txt` & `neon-skill-update-1.0.1a1/neon_skill_update.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -14,29 +14,33 @@
 locale/en-us/dialog/confirm_change_update_track.dialog
 locale/en-us/dialog/confirm_no_change_update_track.dialog
 locale/en-us/dialog/core_version.dialog
 locale/en-us/dialog/downloading_image.dialog
 locale/en-us/dialog/drive_instructions.dialog
 locale/en-us/dialog/error_installing_os.dialog
 locale/en-us/dialog/error_offline.dialog
+locale/en-us/dialog/error_updating_os.dialog
 locale/en-us/dialog/installation_complete.dialog
 locale/en-us/dialog/not_updating.dialog
 locale/en-us/dialog/notify_download_complete.dialog
 locale/en-us/dialog/notify_download_failed.dialog
+locale/en-us/dialog/notify_downloading_update.dialog
 locale/en-us/dialog/notify_installation_complete.dialog
 locale/en-us/dialog/notify_installation_failed.dialog
 locale/en-us/dialog/notify_update_available.dialog
 locale/en-us/dialog/notify_update_failure.dialog
 locale/en-us/dialog/notify_update_success.dialog
 locale/en-us/dialog/notify_writing_image.dialog
 locale/en-us/dialog/point.dialog
 locale/en-us/dialog/starting_installation.dialog
 locale/en-us/dialog/starting_update.dialog
 locale/en-us/dialog/up_to_date.dialog
 locale/en-us/dialog/update_core.dialog
+locale/en-us/dialog/update_restarting.dialog
+locale/en-us/dialog/update_system.dialog
 locale/en-us/dialog/update_track_already_set.dialog
 locale/en-us/dialog/word_beta.dialog
 locale/en-us/dialog/word_stable.dialog
 locale/en-us/intent/core_version.intent
 locale/en-us/intent/update_configuration.intent
 locale/en-us/intent/update_device.intent
 locale/en-us/vocab/beta.voc
```

### Comparing `neon-skill-update-1.0.0/setup.py` & `neon-skill-update-1.0.1a1/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-update-1.0.0/skill.json` & `neon-skill-update-1.0.1a1/skill.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9962121212121211%*

 * *Differences: {"'requirements'": "{'python': ['neon-phal-plugin-core-updater~=1.2', 'neon-utils~=1.6', "*

 * *                   "'ovos-workshop~=0.0.12', 'ovos_utils~=0.0.35']}"}*

```diff
@@ -28,17 +28,18 @@
         "x86_64",
         "ia64",
         "arm64",
         "arm"
     ],
     "requirements": {
         "python": [
-            "neon-phal-plugin-core-updater>=0.1.0,<2.0.0",
-            "neon-utils~=1.1",
-            "ovos_utils~=0.0.28"
+            "neon-phal-plugin-core-updater~=1.2",
+            "neon-utils~=1.6",
+            "ovos-workshop~=0.0.12",
+            "ovos_utils~=0.0.35"
         ],
         "skill": [],
         "system": {}
     },
     "short_description": "Skill to update Python packages, configuration, and to create new boot media.",
     "skillname": "skill-update",
     "summary": "Skill to update Python packages, configuration, and to create new boot media.",
```

### Comparing `neon-skill-update-1.0.0/test/test_skill.py` & `neon-skill-update-1.0.1a1/test/test_skill.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,21 +75,21 @@
 
     def test_handle_core_version(self):
         real_check_release = self.skill._check_latest_core_release
         self.skill._check_latest_core_release = Mock()
         test_message = Message("")
 
         # No alpha version
-        self.skill.current_ver = "22.10.0"
+        self.skill.current_core_ver = "22.10.0"
         self.skill.handle_core_version(test_message)
         self.skill._check_latest_core_release.assert_called_once_with(test_message)
         self.skill.speak_dialog.assert_called_with("core_version", {"version": "22 point 10 point 0"})
 
         # Alpha version
-        self.skill.current_ver = "22.10.1a10"
+        self.skill.current_core_ver = "22.10.1a10"
         self.skill.handle_core_version(test_message)
         self.skill._check_latest_core_release.assert_called_with(test_message)
         self.skill.speak_dialog.assert_called_with("core_version", {"version": "22 point 10 point 1 alpha 10"})
 
         self.skill._check_latest_core_release = real_check_release
 
     def test_handle_update_neon(self):
```

### Comparing `neon-skill-update-1.0.0/version.py` & `neon-skill-update-1.0.1a1/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "1.0.0"
+__version__ = "1.0.1a1"
```

