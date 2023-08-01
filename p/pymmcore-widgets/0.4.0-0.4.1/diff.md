# Comparing `tmp/pymmcore-widgets-0.4.0.tar.gz` & `tmp/pymmcore_widgets-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymmcore-widgets-0.4.0.tar", last modified: Thu Jul 27 22:56:11 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pymmcore-widgets-0.4.0.tar` & `pymmcore_widgets-0.4.1.tar`

### file list

```diff
@@ -1,135 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:56:11.267498 pymmcore-widgets-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/.cruft.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:56:11.255498 pymmcore-widgets-0.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/.github/TEST_FAIL_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:56:11.255498 pymmcore-widgets-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/.github/workflows/cron.yml
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/.github_changelog_generator
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-27 22:56:11.267498 pymmcore-widgets-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:56:11.255498 pymmcore-widgets-0.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/docs/_gen_widget_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/docs/_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:56:11.255498 pymmcore-widgets-0.4.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/docs/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:56:11.255498 pymmcore-widgets-0.4.0/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/docs/stylesheets/extra.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:56:11.259498 pymmcore-widgets-0.4.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/camera_roi_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/channel_group_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/channel_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/channel_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/configuration_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/default_camera_exposure_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/device_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/exposure_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/grid_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/group_preset_table_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/image_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/live_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/mda_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/objectives_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/pixel_size_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/position_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/presets_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/properties_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/property_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/property_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/shutters_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/snap_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/stage_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/state_device_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/time_plan_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/examples/z_stack_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 22:56:11.267498 pymmcore-widgets-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:56:11.251498 pymmcore-widgets-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:56:11.259498 pymmcore-widgets-0.4.0/src/pymmcore_widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17048 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_camera_roi_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_channel_group_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_channel_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_device_property_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_device_type_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_device_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_exposure_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:56:11.263498 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_group_preset_widget/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_group_preset_widget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_group_preset_widget/_add_first_preset_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_group_preset_widget/_add_group_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_group_preset_widget/_add_preset_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_group_preset_widget/_edit_group_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_group_preset_widget/_edit_preset_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    15111 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_group_preset_widget/_group_preset_table_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_image_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_live_button_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_load_system_cfg_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:56:11.263498 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_mda/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_mda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_mda/_autofocus_device_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    17375 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_mda/_channel_table_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_mda/_checkable_tabwidget_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_mda/_general_mda_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)    28046 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_mda/_grid_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    23943 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_mda/_mda_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    32010 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_mda/_positions_table_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_mda/_time_plan_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    12970 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_mda/_zstack_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_objective_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    20718 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_pixel_size_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    11624 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_presets_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_properties_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_property_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)    13904 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_property_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    13222 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_shutter_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_snap_button_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    13375 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_stage_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/_util.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:56:11.259498 pymmcore-widgets-0.4.0/src/pymmcore_widgets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-27 22:56:11.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-07-27 22:56:11.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 22:56:11.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 22:56:10.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-27 22:56:11.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 22:56:11.000000 pymmcore-widgets-0.4.0/src/pymmcore_widgets.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:56:11.267498 pymmcore-widgets-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_camera_roi_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_channel_group_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_channel_table_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_channel_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_combo_message_box_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     7658 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_config.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_core_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_device_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_exposure_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_grid_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    10006 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_group_preset_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_image_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_live_button.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_load_system_cfg_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    11033 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_mda_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_objective_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    15068 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_position_table_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_presets_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_prop_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_properties_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_property_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)    11019 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_shutter_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_snap_button_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_stage_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     9134 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_table_pixel_size_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tests/test_time_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-27 22:55:54.000000 pymmcore-widgets-0.4.0/tox.ini
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/src/pymmcore_widgets/__init__.py
+-rw-r--r--   0        0        0    17048 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/src/pymmcore_widgets/_camera_roi_widget.py
+-rw-r--r--   0        0        0     3060 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/src/pymmcore_widgets/_channel_group_widget.py
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/src/pymmcore_widgets/_channel_widget.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/src/pymmcore_widgets/_core.py
+-rw-r--r--   0        0        0     7961 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/src/pymmcore_widgets/_device_property_table.py
+-rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/src/pymmcore_widgets/_device_type_filter.py
+-rw-r--r--   0        0        0     8144 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/src/pymmcore_widgets/_device_widget.py
+-rw-r--r--   0        0        0     6134 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/src/pymmcore_widgets/_exposure_widget.py
+-rw-r--r--   0        0        0     4827 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/src/pymmcore_widgets/_image_widget.py
+-rw-r--r--   0        0        0     5768 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/src/pymmcore_widgets/_live_button_widget.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/src/pymmcore_widgets/_load_system_cfg_widget.py
+-rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/src/pymmcore_widgets/_objective_widget.py
+-rw-r--r--   0        0        0    20718 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/src/pymmcore_widgets/_pixel_size_widget.py
+-rw-r--r--   0        0        0    11624 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/src/pymmcore_widgets/_presets_widget.py
+-rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/src/pymmcore_widgets/_properties_widget.py
+-rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/src/pymmcore_widgets/_property_browser.py
+-rw-r--r--   0        0        0    13986 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/src/pymmcore_widgets/_property_widget.py
+-rw-r--r--   0        0        0    13220 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/src/pymmcore_widgets/_shutter_widget.py
+-rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/src/pymmcore_widgets/_snap_button_widget.py
+-rw-r--r--   0        0        0    13375 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/src/pymmcore_widgets/_stage_widget.py
+-rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/src/pymmcore_widgets/_util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/src/pymmcore_widgets/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/src/pymmcore_widgets/_group_preset_widget/__init__.py
+-rw-r--r--   0        0        0     5519 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/src/pymmcore_widgets/_group_preset_widget/_add_first_preset_widget.py
+-rw-r--r--   0        0        0     5726 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/src/pymmcore_widgets/_group_preset_widget/_add_group_widget.py
+-rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/src/pymmcore_widgets/_group_preset_widget/_add_preset_widget.py
+-rw-r--r--   0        0        0     6042 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/src/pymmcore_widgets/_group_preset_widget/_edit_group_widget.py
+-rw-r--r--   0        0        0     7796 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/src/pymmcore_widgets/_group_preset_widget/_edit_preset_widget.py
+-rw-r--r--   0        0        0    15150 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/src/pymmcore_widgets/_group_preset_widget/_group_preset_table_widget.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/src/pymmcore_widgets/_mda/__init__.py
+-rw-r--r--   0        0        0     5044 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/src/pymmcore_widgets/_mda/_autofocus_device_widget.py
+-rw-r--r--   0        0        0    16789 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/src/pymmcore_widgets/_mda/_channel_table_widget.py
+-rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/src/pymmcore_widgets/_mda/_checkable_tabwidget_widget.py
+-rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/src/pymmcore_widgets/_mda/_general_mda_widgets.py
+-rw-r--r--   0        0        0    27724 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/src/pymmcore_widgets/_mda/_grid_widget.py
+-rw-r--r--   0        0        0    18313 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/src/pymmcore_widgets/_mda/_mda_widget.py
+-rw-r--r--   0        0        0    30748 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/src/pymmcore_widgets/_mda/_positions_table_widget.py
+-rw-r--r--   0        0        0     8445 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/src/pymmcore_widgets/_mda/_time_plan_widget.py
+-rw-r--r--   0        0        0    13305 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/src/pymmcore_widgets/_mda/_zstack_widget.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/tests/conftest.py
+-rw-r--r--   0        0        0     6152 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/tests/test_camera_roi_widget.py
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/tests/test_channel_group_widget.py
+-rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/tests/test_channel_table_widget.py
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/tests/test_channel_widget.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/tests/test_combo_message_box_widget.py
+-rw-r--r--   0        0        0     7658 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/tests/test_config.cfg
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/tests/test_core_state.py
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/tests/test_device_widget.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/tests/test_exposure_widget.py
+-rw-r--r--   0        0        0     5736 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/tests/test_grid_widget.py
+-rw-r--r--   0        0        0    10006 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/tests/test_group_preset_widget.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/tests/test_image_preview.py
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/tests/test_live_button.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/tests/test_load_system_cfg_widget.py
+-rw-r--r--   0        0        0    10052 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/tests/test_mda_widget.py
+-rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/tests/test_objective_widget.py
+-rw-r--r--   0        0        0    16681 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/tests/test_position_table_widget.py
+-rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/tests/test_presets_widget.py
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/tests/test_prop_widget.py
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/tests/test_properties_widget.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/tests/test_property_browser.py
+-rw-r--r--   0        0        0    11019 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/tests/test_shutter_widget.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/tests/test_snap_button_widget.py
+-rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/tests/test_stage_widget.py
+-rw-r--r--   0        0        0     9134 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/tests/test_table_pixel_size_widget.py
+-rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/tests/test_time_table.py
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/LICENSE
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/README.md
+-rw-r--r--   0        0        0     4633 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 pymmcore_widgets-0.4.1/PKG-INFO
```

### Comparing `pymmcore-widgets-0.4.0/.gitignore` & `pymmcore_widgets-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.4.0/LICENSE` & `pymmcore_widgets-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.4.0/README.md` & `pymmcore_widgets-0.4.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # pymmcore-widgets
 
 [![License](https://img.shields.io/pypi/l/pymmcore-widgets.svg?color=green)](https://github.com/pymmcore-plus/pymmcore-widgets/raw/main/LICENSE)
-[![PyPI](https://img.shields.io/pypi/v/pymmcore-widgets.svg?color=green)](https://pypi.org/project/pymmcore-widgets)
 [![Python Version](https://img.shields.io/pypi/pyversions/pymmcore-widgets.svg?color=green)](https://python.org)
+[![PyPI](https://img.shields.io/pypi/v/pymmcore-widgets.svg?color=green)](https://pypi.org/project/pymmcore-widgets)
+[![Conda](https://img.shields.io/conda/vn/conda-forge/pymmcore-widgets)](https://anaconda.org/conda-forge/pymmcore-widgets)
 [![CI](https://github.com/pymmcore-plus/pymmcore-widgets/actions/workflows/ci.yml/badge.svg)](https://github.com/pymmcore-plus/pymmcore-widgets/actions/workflows/ci.yml)
+[![docs](https://github.com/pymmcore-plus/pymmcore-plus/actions/workflows/docs.yml/badge.svg)](https://pymmcore-plus.github.io/pymmcore-widgets/)
 [![codecov](https://codecov.io/gh/pymmcore-plus/pymmcore-widgets/branch/main/graph/badge.svg)](https://codecov.io/gh/pymmcore-plus/pymmcore-widgets)
 
 A set of widgets for the [pymmcore-plus](https://github.com/pymmcore-plus/pymmcore-plus) package.
 This package can be used to build custom user interfaces for micromanager in a python/Qt environment.
 
 [Documentation](https://pymmcore-plus.github.io/pymmcore-widgets)
```

### Comparing `pymmcore-widgets-0.4.0/pyproject.toml` & `pymmcore_widgets-0.4.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 # https://peps.python.org/pep-0517/
 [build-system]
-requires = ["setuptools>=45", "wheel", "setuptools-scm>=6.2"]
-build-backend = "setuptools.build_meta"
+requires = ["hatchling", "hatch-vcs"]
+build-backend = "hatchling.build"
+
+# https://hatch.pypa.io/latest/config/metadata/
+[tool.hatch.version]
+source = "vcs"
+
+# https://hatch.pypa.io/latest/config/build/#file-selection
+[tool.hatch.build.targets.sdist]
+include = ["/src", "/tests"]
+
+[tool.hatch.build.targets.wheel]
+only-include = ["src"]
+sources = ["src"]
 
 # https://peps.python.org/pep-0621/
 [project]
 name = "pymmcore-widgets"
 description = "A set of Qt-based widgets onto the pymmcore-plus model"
 readme = "README.md"
 requires-python = ">=3.8"
@@ -13,27 +25,37 @@
 authors = [
     { email = "federico.gasparoli@gmail.com", name = "Federico Gasparoli" },
     { email = "talley.lambert@gmail.com", name = "Talley Lambert" },
     { email = "ianhuntisaak@gmail.com", name = "Ian Hunt-Isaak" },
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
+    "Environment :: X11 Applications :: Qt",
+    "Intended Audience :: Developers",
+    "Intended Audience :: Science/Research",
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python",
+    "Topic :: Software Development :: Widget Sets",
+    "Topic :: System :: Hardware :: Hardware Drivers",
+    "Topic :: System :: Hardware",
+    "Topic :: Utilities",
+    "Typing :: Typed",
 ]
 dynamic = ["version"]
 dependencies = [
-    'pymmcore-plus>=0.6.6',
-    'useq-schema >=0.2.0',
-    'superqt[quantity] >=0.3.1',
     'fonticon-materialdesignicons6',
-    'qtpy',
+    'pymmcore-plus >=0.8.0',
+    'qtpy >=2.0',
+    'superqt[quantity] >=0.3.1',
+    'useq-schema >=0.4.1',
 ]
 
 # extras
 # https://peps.python.org/pep-0621/#dependencies-optional-dependencies
 [project.optional-dependencies]
 test = ["pytest>=6.0", "pytest-cov", "pytest-qt"]
 pyqt5 = ["PyQt5"]
@@ -56,87 +78,65 @@
 ]
 docs = [
     "vispy",
     "mkdocs",
     "mkdocs-material",
     "mkdocstrings-python",
     "mkdocs-literate-nav",
-    "mkdocs-gen-files"
+    "mkdocs-gen-files",
 ]
 
 [project.urls]
-homepage = "https://github.com/pymmcore-plus/pymmcore-widgets"
-repository = "https://github.com/pymmcore-plus/pymmcore-widgets"
-
-# same as console_scripts entry point
-# [project.scripts]
-# spam-cli = "spam:main_cli"
-
-# Entry points
-# https://peps.python.org/pep-0621/#entry-points
-# [project.entry-points."spam.magical"]
-# tomatoes = "spam:main_tomatoes"
-
-# https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
-[tool.setuptools]
-zip-safe = false
-include-package-data = true
-packages = { find = { where = ["src"], exclude = [] } }
-
-[tool.setuptools.package-data]
-"*" = ["py.typed"]
-
-# https://github.com/pypa/setuptools_scm/#pyprojecttoml-usage
-[tool.setuptools_scm]
-
-# https://pycqa.github.io/isort/docs/configuration/options.html
-[tool.isort]
-profile = "black"
+Homepage = "https://github.com/pymmcore-plus/pymmcore-widgets"
+"Source Code" = "https://github.com/pymmcore-plus/pymmcore-widgets"
+Documentation = "https://pymmcore-plus.github.io/pymmcore-widgets"
 
-# https://github.com/charliermarsh/ruff
+# https://beta.ruff.rs/docs/rules/
 [tool.ruff]
 line-length = 88
 target-version = "py38"
-src = ["src","tests"]
-extend-select = [
+src = ["src", "tests"]
+select = [
     "E",    # style errors
     "F",    # flakes
+    "W",    # warnings
     "D",    # pydocstyle
-    "I001", # isort
-    "UP",    # pyupgrade
-    # "N",  # pep8-naming
-    # "S",  # bandit
-    "C4",    # flake8-comprehensions
+    "I",    # isort
+    "UP",   # pyupgrade
+    "C4",   # flake8-comprehensions
     "B",    # flake8-bugbear
     "A001", # flake8-builtins
     "RUF",  # ruff-specific rules
+    "TID",  # tidy
+    "TCH",  # typecheck
+    # "SLF",  # private-access
 ]
 ignore = [
     "D100", # Missing docstring in public module
     "D107", # Missing docstring in __init__
     "D203", # 1 blank line required before class docstring
     "D212", # Multi-line docstring summary should start at the first line
     "D213", # Multi-line docstring summary should start at the second line
     "D401", # First line should be in imperative mood
     "D413", # Missing blank line after last section
     "D416", # Section name should end with a colon
-    "C901", # Function is too complex
 ]
 
-
 [tool.ruff.per-file-ignores]
-"tests/*.py" = ["D"]
+"tests/*.py" = ["D", "SLF"]
 
 # https://docs.pytest.org/en/6.2.x/customize.html
 [tool.pytest.ini_options]
 minversion = "6.0"
 testpaths = ["tests"]
 filterwarnings = [
     "error",
-    "ignore:distutils Version classes are deprecated"
+    "ignore:distutils Version classes are deprecated",
+    # warning, but not error, that will show up on useq<0.3.3
+    "ignore:GridRelative got unknown keyword:UserWarning",
 ]
 
 # https://mypy.readthedocs.io/en/stable/config_file.html
 [tool.mypy]
 files = "src/**/"
 strict = true
 disallow_any_generics = false
@@ -149,34 +149,24 @@
 # https://coverage.readthedocs.io/en/6.4/config.html
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "if TYPE_CHECKING:",
     "@overload",
     "except ImportError",
+    "raise AssertionError",
+    "if __name__ == .__main__.:",
+    "raise NotImplementedError",
 ]
-
-# https://github.com/cruft/cruft
-[tool.cruft]
-skip = ["tests"]
+[tool.coverage.run]
+source = ['pymmcore_widgets']
 
 # https://github.com/mgedmin/check-manifest#configuration
 [tool.check-manifest]
 ignore = [
-    ".cruft.json",
-    ".flake8",
     ".github_changelog_generator",
     ".pre-commit-config.yaml",
     "tests/**/*",
     "docs/**/*",
     "mkdocs.yml",
-    "tox.ini",
     "examples/**/*",
 ]
-
-# https://python-semantic-release.readthedocs.io/en/latest/configuration.html
-[tool.semantic_release]
-version_source = "tag_only"
-branch = "main"
-changelog_sections = "feature,fix,breaking,documentation,performance,chore,:boom:,:sparkles:,:children_crossing:,:lipstick:,:iphone:,:egg:,:chart_with_upwards_trend:,:ambulance:,:lock:,:bug:,:zap:,:goal_net:,:alien:,:wheelchair:,:speech_balloon:,:mag:,:apple:,:penguin:,:checkered_flag:,:robot:,:green_apple:,Other"
-# commit_parser=semantic_release.history.angular_parser
-build_command = "pip install build && python -m build"
```

### Comparing `pymmcore-widgets-0.4.0/src/pymmcore_widgets/__init__.py` & `pymmcore_widgets-0.4.1/src/pymmcore_widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_camera_roi_widget.py` & `pymmcore_widgets-0.4.1/src/pymmcore_widgets/_camera_roi_widget.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_channel_group_widget.py` & `pymmcore_widgets-0.4.1/src/pymmcore_widgets/_channel_group_widget.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_channel_widget.py` & `pymmcore_widgets-0.4.1/src/pymmcore_widgets/_channel_widget.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_core.py` & `pymmcore_widgets-0.4.1/src/pymmcore_widgets/_core.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_device_property_table.py` & `pymmcore_widgets-0.4.1/src/pymmcore_widgets/_device_property_table.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_device_type_filter.py` & `pymmcore_widgets-0.4.1/src/pymmcore_widgets/_device_type_filter.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_device_widget.py` & `pymmcore_widgets-0.4.1/src/pymmcore_widgets/_device_widget.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_exposure_widget.py` & `pymmcore_widgets-0.4.1/src/pymmcore_widgets/_exposure_widget.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_group_preset_widget/_add_first_preset_widget.py` & `pymmcore_widgets-0.4.1/src/pymmcore_widgets/_group_preset_widget/_add_first_preset_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,15 @@
     QTableWidget,
     QTableWidgetItem,
     QVBoxLayout,
     QWidget,
 )
 
 from pymmcore_widgets._property_widget import PropertyWidget
-
-from .._util import block_core
+from pymmcore_widgets._util import block_core
 
 
 class AddFirstPresetWidget(QDialog):
     """A widget to create the first specified group's preset."""
 
     def __init__(
         self,
```

### Comparing `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_group_preset_widget/_add_group_widget.py` & `pymmcore_widgets-0.4.1/src/pymmcore_widgets/_group_preset_widget/_add_group_widget.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 from __future__ import annotations
 
 import warnings
+from typing import TYPE_CHECKING
 
 from pymmcore_plus import CMMCorePlus
-from qtpy.QtGui import QCloseEvent
 from qtpy.QtWidgets import (
     QDialog,
     QGroupBox,
     QHBoxLayout,
     QLabel,
     QLineEdit,
     QPushButton,
     QSizePolicy,
     QVBoxLayout,
     QWidget,
 )
 
+from pymmcore_widgets._device_property_table import DevicePropertyTable
 from pymmcore_widgets._device_type_filter import DeviceTypeFilters
 
-from .._device_property_table import DevicePropertyTable
 from ._add_first_preset_widget import AddFirstPresetWidget
 
+if TYPE_CHECKING:
+    from qtpy.QtGui import QCloseEvent
+
 
 class AddGroupWidget(QDialog):
     """Widget to create a new group."""
 
     def __init__(self, *, parent: QWidget | None = None) -> None:
         super().__init__(parent=parent)
         self._mmc = CMMCorePlus.instance()
```

### Comparing `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_group_preset_widget/_add_preset_widget.py` & `pymmcore_widgets-0.4.1/src/pymmcore_widgets/_group_preset_widget/_add_preset_widget.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,15 @@
     QTableWidget,
     QTableWidgetItem,
     QVBoxLayout,
     QWidget,
 )
 
 from pymmcore_widgets._property_widget import PropertyWidget
-
-from .._util import block_core
+from pymmcore_widgets._util import block_core
 
 
 class AddPresetWidget(QDialog):
     """A widget to add presets to a specified group."""
 
     def __init__(self, group: str, *, parent: QWidget | None = None) -> None:
         super().__init__(parent=parent)
```

### Comparing `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_group_preset_widget/_edit_group_widget.py` & `pymmcore_widgets-0.4.1/src/pymmcore_widgets/_group_preset_widget/_edit_group_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,15 @@
     QSizePolicy,
     QVBoxLayout,
     QWidget,
 )
 
 from pymmcore_widgets._device_property_table import DevicePropertyTable
 from pymmcore_widgets._device_type_filter import DeviceTypeFilters
-
-from .._util import block_core
+from pymmcore_widgets._util import block_core
 
 
 class EditGroupWidget(QDialog):
     """Widget to edit the specified Group."""
 
     def __init__(self, group: str, *, parent: QWidget | None = None) -> None:
         super().__init__(parent=parent)
```

### Comparing `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_group_preset_widget/_edit_preset_widget.py` & `pymmcore_widgets-0.4.1/src/pymmcore_widgets/_group_preset_widget/_edit_preset_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,15 @@
     QTableWidgetItem,
     QVBoxLayout,
     QWidget,
 )
 from superqt.utils import signals_blocked
 
 from pymmcore_widgets._property_widget import PropertyWidget
-
-from .._util import block_core
+from pymmcore_widgets._util import block_core
 
 
 class EditPresetWidget(QDialog):
     """A widget to edit a specified group's presets."""
 
     def __init__(
         self, group: str, preset: str, *, parent: QWidget | None = None
@@ -189,15 +188,15 @@
             if (
                 dpv_preset == dev_prop_val
                 and self._preset == self.preset_name_lineedit.text()
             ):
                 if p == self._preset:
                     return
                 warnings.warn(
-                    "Threre is already a preset with the same "
+                    "There is already a preset with the same "
                     f"devices, properties and values: '{p}'.",
                     stacklevel=2,
                 )
                 self.info_lbl.setStyleSheet("color: magenta;")
                 self.info_lbl.setText(f"'{p}' already has the same properties!")
                 return
```

### Comparing `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_group_preset_widget/_group_preset_table_widget.py` & `pymmcore_widgets-0.4.1/src/pymmcore_widgets/_group_preset_widget/_group_preset_table_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,19 @@
     QSpacerItem,
     QTableWidget,
     QTableWidgetItem,
     QVBoxLayout,
     QWidget,
 )
 
+from pymmcore_widgets._core import load_system_config
 from pymmcore_widgets._presets_widget import PresetsWidget
 from pymmcore_widgets._property_widget import PropertyWidget
+from pymmcore_widgets._util import block_core
 
-from .._core import load_system_config
-from .._util import block_core
 from ._add_group_widget import AddGroupWidget
 from ._add_preset_widget import AddPresetWidget
 from ._edit_group_widget import EditGroupWidget
 from ._edit_preset_widget import EditPresetWidget
 
 UNNAMED_PRESET = "NewPreset"
 
@@ -321,26 +321,26 @@
             self.table_wdg.removeRow(matching_item[0].row())
 
     def _edit_group(self) -> None:
         selected_rows = {r.row() for r in self.table_wdg.selectedIndexes()}
         if not selected_rows or len(selected_rows) > 1:
             return
 
-        row = list(selected_rows)[0]
+        row = next(iter(selected_rows))
         group = self.table_wdg.item(row, 0).text()
         self._close_if_hasattr()
         self._edit_group_wdg = EditGroupWidget(group, parent=self)
         self._edit_group_wdg.show()
 
     def _add_preset(self) -> None:
         selected_rows = {r.row() for r in self.table_wdg.selectedIndexes()}
         if not selected_rows or len(selected_rows) > 1:
             return
 
-        row = list(selected_rows)[0]
+        row = next(iter(selected_rows))
         group = self.table_wdg.item(row, 0).text()
         wdg = self.table_wdg.cellWidget(row, 1)
 
         if isinstance(wdg, PropertyWidget):
             return
 
         self._close_if_hasattr()
@@ -381,15 +381,15 @@
                     self._mmc.deleteConfigGroup(group)
 
     def _edit_preset(self) -> None:
         selected_rows = {r.row() for r in self.table_wdg.selectedIndexes()}
         if not selected_rows or len(selected_rows) > 1:
             return
 
-        row = list(selected_rows)[0]
+        row = next(iter(selected_rows))
         group = self.table_wdg.item(row, 0).text()
         wdg = self.table_wdg.cellWidget(row, 1)
         if isinstance(wdg, PropertyWidget):
             return
         if isinstance(wdg, PresetsWidget):
             preset = wdg._combo.currentText()
         self._close_if_hasattr()
```

### Comparing `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_image_widget.py` & `pymmcore_widgets-0.4.1/src/pymmcore_widgets/_image_widget.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_live_button_widget.py` & `pymmcore_widgets-0.4.1/src/pymmcore_widgets/_live_button_widget.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_load_system_cfg_widget.py` & `pymmcore_widgets-0.4.1/src/pymmcore_widgets/_load_system_cfg_widget.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_mda/_channel_table_widget.py` & `pymmcore_widgets-0.4.1/src/pymmcore_widgets/_mda/_channel_table_widget.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import warnings
-from typing import TYPE_CHECKING, cast
+from typing import Iterable, cast
 
+import useq
 from fonticon_mdi6 import MDI6
 from pymmcore_plus import CMMCorePlus
 from qtpy.QtCore import QSize, Qt, Signal
 from qtpy.QtWidgets import (
     QAbstractSpinBox,
     QCheckBox,
     QComboBox,
@@ -21,28 +22,14 @@
     QTableWidget,
     QVBoxLayout,
     QWidget,
 )
 from superqt import fonticon
 from superqt.utils import signals_blocked
 
-if TYPE_CHECKING:
-    from typing_extensions import Required, TypedDict
-
-    class ChannelDict(TypedDict, total=False):
-        """Channel dictionary."""
-
-        config: Required[str]
-        group: str
-        exposure: float | None
-        z_offset: float
-        do_stack: bool
-        camera: str | None
-        acquire_every: int
-
 
 class ChannelTable(QWidget):
     """Widget providing options for setting up a multi-channel acquisition.
 
     The `value()` method returns a dictionary with the current state of the widget, in a
     format that matches one of the [useq-schema Channel
     specifications](https://pymmcore-plus.github.io/useq-schema/schema/axes/#useq.Channel).
@@ -165,20 +152,19 @@
     def _on_sys_cfg_loaded(self) -> None:
         self.clear()
         self._advanced_cbox.setChecked(False)
         self._on_advanced_toggled(False)
 
     def _on_group_deleted(self, group: str) -> None:
         """Remove rows that are using channels from the deleted group."""
-        row = 0
-        for ch in self.value():
-            if ch["group"] == group:
-                self._table.removeRow(row)
-            else:
-                row += 1
+        for r in reversed(range(self._table.rowCount())):
+            name_widget = cast("QComboBox", self._table.cellWidget(r, 0))
+            _grp = name_widget.itemData(name_widget.currentIndex(), self.CH_GROUP_ROLE)
+            if _grp == group:
+                self._table.removeRow(r)
 
     def _on_config_deleted(self, group: str, config: str) -> None:
         """Remove deleted config from channel combo if present."""
         for row in range(self._table.rowCount()):
             combo = cast(QComboBox, self._table.cellWidget(row, 0))
             items = [combo.itemText(ch) for ch in range(combo.count())]
             items_data = {
@@ -192,103 +178,104 @@
                 if self._mmc.getChannelGroup() != config:
                     combo.setCurrentText(self._mmc.getChannelGroup())
 
     def _on_advanced_toggled(self, state: bool) -> None:
         for c in range(2, self._table.columnCount()):
             self._table.setColumnHidden(c, not state)
 
-        if not state:
-            for v in self.value():
-                # if any of the advanced settings are different from their default
-                if v["z_offset"] != 0 or not v["do_stack"] or v["acquire_every"] != 1:
-                    self._warn_icon.show()
-                    return
-        self._warn_icon.hide()
+        if state:
+            self._warn_icon.hide()
+            return
+        # if any of the advanced settings are different from their default
+        for c in range(self._table.rowCount()):
+            if (
+                self._table.cellWidget(c, 2).value()
+                or not self._z_stack_checkbox(c).isChecked()
+                or self._table.cellWidget(c, 4).value() != 1
+            ):
+                self._warn_icon.show()
+                return
 
-    def _pick_first_unused_channel(self, available: tuple[str, ...]) -> str:
+    def _pick_first_unused_channel(self, channel_group: str) -> str:
         """Return index of first unused channel."""
-        used = set()
-        for row in range(self._table.rowCount()):
-            combo = cast(QComboBox, self._table.cellWidget(row, 0))
-            used.add(combo.currentText())
+        used = {
+            self._table.cellWidget(row, 0).currentText()
+            for row in range(self._table.rowCount())
+        }
 
+        available = self._mmc.getAvailableConfigs(channel_group)
         for ch in available:
             if ch not in used:
                 return ch
         return available[0]
 
     def _create_spinbox(
         self, range: tuple[int, int], double: bool = False
     ) -> QDoubleSpinBox:
         dspinbox = QDoubleSpinBox() if double else QSpinBox()
-        dspinbox.setButtonSymbols(QAbstractSpinBox.NoButtons)
+        dspinbox.setButtonSymbols(QAbstractSpinBox.ButtonSymbols.NoButtons)
         dspinbox.setRange(*range)
-        dspinbox.setAlignment(Qt.AlignCenter)
+        dspinbox.setAlignment(Qt.AlignmentFlag.AlignCenter)
         dspinbox.wheelEvent = lambda event: None  # block mouse scroll
         dspinbox.setKeyboardTracking(False)
         dspinbox.valueChanged.connect(self.valueChanged)
         return dspinbox
 
-    def _create_new_row(
-        self,
-        channel: str | None = None,
-        exposure: float | None = None,
-        channel_group: str | None = None,
-        z_offset: float = 0.0,
-        do_stack: bool = True,
-        acquire_every: int = 1,
-    ) -> None:
+    def _create_new_row(self, channel: useq.Channel | None = None) -> None:
         """Create a new row in the table.
 
         If 'channel' is not provided, the first unused channel will be used.
         If 'exposure' is not provided, the current exposure will be used (or 100).
         """
         if len(self._mmc.getLoadedDevices()) <= 1:
             warnings.warn("No devices loaded.", stacklevel=2)
             return
-
-        _channel_group = channel_group or self.channel_group_combo.currentText()
-
-        if not _channel_group:
-            warnings.warn("First select Micro-Manager 'ChannelGroup'.", stacklevel=2)
-            return
+        if channel:
+            _channel_group = channel.group
+        else:
+            _channel_group = self.channel_group_combo.currentText()
+            if not _channel_group:  # pragma: no cover
+                warnings.warn(
+                    "First select Micro-Manager 'ChannelGroup'.", stacklevel=2
+                )
+                return
+            channel_name = self._pick_first_unused_channel(_channel_group)
+            channel = useq.Channel(config=channel_name, group=_channel_group)
 
         # channel dropdown
         channel_combo = QComboBox()
-        available = self._mmc.getAvailableConfigs(_channel_group)
-        channel = channel or self._pick_first_unused_channel(available)
-        channel_combo.addItems(available)
+        channel_combo.addItems(self._mmc.getAvailableConfigs(channel.group))
         for i in range(channel_combo.count()):
             channel_combo.setItemData(i, _channel_group, self.CH_GROUP_ROLE)
-        channel_combo.setCurrentText(channel)
+        channel_combo.setCurrentText(channel.config)
 
         # exposure spinbox
         channel_exp_spinbox = self._create_spinbox((0, 10000), True)
         channel_exp_spinbox.setMinimum(1)
-        channel_exp_spinbox.setValue(exposure or self._mmc.getExposure() or 100)
+        channel_exp_spinbox.setValue(channel.exposure or self._mmc.getExposure() or 100)
 
         # z offset spinbox
         z_offset_spinbox = self._create_spinbox((-10000, 10000), True)
-        z_offset_spinbox.setValue(z_offset)
+        z_offset_spinbox.setValue(channel.z_offset)
 
         # z stack checkbox
         # creating a wrapper widget so that the checkbox appears centered.
         z_stack_wdg = QWidget()
         z_stack_layout = QHBoxLayout()
         z_stack_layout.setContentsMargins(0, 0, 0, 0)
-        z_stack_layout.setAlignment(Qt.AlignCenter)
+        z_stack_layout.setAlignment(Qt.AlignmentFlag.AlignCenter)
         z_stack_wdg.setLayout(z_stack_layout)
         z_stack_checkbox = QCheckBox()
-        z_stack_checkbox.setChecked(do_stack)
+        z_stack_checkbox.setChecked(channel.do_stack)
         z_stack_checkbox.stateChanged.connect(self.valueChanged)
         z_stack_layout.addWidget(z_stack_checkbox)
 
         # acqire every spinbox
         acquire_every_spinbox = self._create_spinbox((1, 10000))
-        acquire_every_spinbox.setValue(acquire_every)
+        acquire_every_spinbox.setValue(channel.acquire_every)
 
         idx = self._table.rowCount()
         self._table.insertRow(idx)
         self._table.setCellWidget(idx, 0, channel_combo)
         self._table.setCellWidget(idx, 1, channel_exp_spinbox)
         self._table.setCellWidget(idx, 2, z_offset_spinbox)
         self._table.setCellWidget(idx, 3, z_stack_wdg)
@@ -309,92 +296,79 @@
     def clear(self) -> None:
         """Clear the channel table."""
         if self._table.rowCount():
             self._table.clearContents()
             self._table.setRowCount(0)
             self.valueChanged.emit()
 
-    def value(self) -> list[ChannelDict]:
+    def value(self) -> list[useq.Channel]:
         """Return the current channels settings as a list of dictionaries.
 
         Note that the output will match the [useq-schema Channel
         specifications](https://pymmcore-plus.github.io/useq-schema/schema/axes/#useq.Channel).
         """
-        values: list[ChannelDict] = []
+        values: list[useq.Channel] = []
         for c in range(self._table.rowCount()):
             name_widget = cast("QComboBox", self._table.cellWidget(c, 0))
             exposure_widget = cast("QDoubleSpinBox", self._table.cellWidget(c, 1))
             if name_widget and exposure_widget:
-                values.append(
-                    {
-                        "config": name_widget.currentText(),
-                        "group": name_widget.itemData(
-                            name_widget.currentIndex(), self.CH_GROUP_ROLE
-                        ),
-                        "exposure": exposure_widget.value(),
-                        # NOTE: the columns representing these values *may* be hidden
-                        # ... but we are still using them
-                        "z_offset": (
-                            cast("QDoubleSpinBox", self._table.cellWidget(c, 2)).value()
-                        ),
-                        "do_stack": (self._z_stack_checkbox(c).isChecked()),
-                        "acquire_every": (
-                            cast("QSpinBox", self._table.cellWidget(c, 4)).value()
-                        ),
-                    }
+                channel = useq.Channel(
+                    config=name_widget.currentText(),
+                    group=name_widget.itemData(
+                        name_widget.currentIndex(), self.CH_GROUP_ROLE
+                    ),
+                    exposure=exposure_widget.value(),
+                    # NOTE: the columns representing these values *may* be hidden
+                    # ... but we are still using them
+                    z_offset=self._table.cellWidget(c, 2).value(),
+                    do_stack=self._z_stack_checkbox(c).isChecked(),
+                    acquire_every=self._table.cellWidget(c, 4).value(),
                 )
+                values.append(channel)
         return values
 
-    # note: this really ought to be ChannelDict, but it makes typing elsewhere harder
-    # TODO: also accept actual useq objects
-    def set_state(self, channels: list[dict]) -> None:
+    def set_state(self, channels: Iterable[str | dict | useq.Channel]) -> None:
         """Set the state of the widget.
 
         Parameters
         ----------
-        channels : list[dict]
-            A list of dictionaries following the [useq-schema Channel specifications](
+        channels : Iterable[dict | str | useq.Channel]
+            A list of objects that can be cast to a [useq-schema Channel](
             https://pymmcore-plus.github.io/useq-schema/schema/axes/#useq.Channel).
         """
         _advanced_bool = False
         with signals_blocked(self):
             self.clear()
+            curgroup = self.channel_group_combo.currentText()
             for channel in channels:
-                ch = channel.get("config")
-                group = channel.get("group")
-
-                if not ch:
-                    raise ValueError("Dictionary should contain channel 'config' name.")
-                avail_configs = self._mmc.getAvailableConfigs(
-                    group or self.channel_group_combo.currentText()
-                )
-                if ch not in avail_configs:
+                channel = useq.Channel.validate(channel)
+                avail_configs = self._mmc.getAvailableConfigs(channel.group or curgroup)
+                if channel.config not in avail_configs:
                     warnings.warn(
-                        f"'{ch}' config or its group doesn't exist in the "
-                        f"'{group}' ChannelGroup!",
+                        f"'{channel.config}' config or its group doesn't exist in the "
+                        f"'{channel.group}' ChannelGroup!",
                         stacklevel=2,
                     )
                     continue
 
-                exposure = channel.get("exposure") or self._mmc.getExposure()
-                z_offset = channel.get("z_offset") or 0.0
-                do_stack = channel["do_stack"] if "do_stack" in channel else True
-                acquire_every = channel.get("acquire_every") or 1
-                self._create_new_row(
-                    ch, exposure, group, z_offset, do_stack, acquire_every
-                )
+                self._create_new_row(channel)
 
                 # if any of the advanced settings are different from their default
-                if z_offset != 0.0 or not do_stack or acquire_every != 1:
+                if self._has_advanced_settings(channel):
                     _advanced_bool = True
 
             self._advanced_cbox.setChecked(_advanced_bool)
 
         self.valueChanged.emit()
 
+    def _has_advanced_settings(self, channel: useq.Channel) -> bool:
+        return bool(
+            channel.z_offset or not channel.do_stack or channel.acquire_every != 1
+        )
+
     def _disconnect(self) -> None:
         self._mmc.events.systemConfigurationLoaded.disconnect(self._on_sys_cfg_loaded)
         self._mmc.events.configGroupDeleted.disconnect(self._on_group_deleted)
         self._mmc.events.configDeleted.disconnect(self._on_config_deleted)
 
 
 class ChannelGroupCombo(QComboBox):
@@ -405,15 +379,15 @@
         parent: QWidget | None = None,
         *,
         channel_group: str | None = None,
         mmcore: CMMCorePlus | None = None,
     ) -> None:
         super().__init__(parent)
 
-        self.setSizeAdjustPolicy(QComboBox.AdjustToContents)
+        self.setSizeAdjustPolicy(QComboBox.SizeAdjustPolicy.AdjustToContents)
 
         self._mmc = mmcore or CMMCorePlus.instance()
         self._channel_group = channel_group or self._mmc.getChannelGroup()
 
         # connect core
         self._mmc.events.systemConfigurationLoaded.connect(self._on_sys_cfg_loaded)
         self._mmc.events.configGroupDeleted.connect(self._update_channel_group_combo)
```

### Comparing `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_mda/_checkable_tabwidget_widget.py` & `pymmcore_widgets-0.4.1/src/pymmcore_widgets/_mda/_checkable_tabwidget_widget.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_mda/_general_mda_widgets.py` & `pymmcore_widgets-0.4.1/src/pymmcore_widgets/_mda/_general_mda_widgets.py`

 * *Files 9% similar despite different names*

```diff
@@ -105,32 +105,14 @@
         self.acquisition_order_comboBox.addItems(
             ["tpgcz", "tpgzc", "tpcgz", "tpzgc", "pgtzc", "ptzgc", "ptcgz", "pgtcz"]
         )
         acq_wdg_layout.addWidget(acquisition_order_label)
         acq_wdg_layout.addWidget(self.acquisition_order_comboBox)
 
 
-class _MDATimeLabel(QWidget):
-    def __init__(self, *, parent: QWidget | None = None) -> None:
-        super().__init__(parent=parent)
-
-        wdg_lay = QHBoxLayout()
-        wdg_lay.setSpacing(5)
-        wdg_lay.setContentsMargins(10, 5, 10, 5)
-        wdg_lay.setAlignment(Qt.AlignmentFlag.AlignLeft)
-        self.setLayout(wdg_lay)
-
-        self._total_time_lbl = QLabel()
-        self._total_time_lbl.setAlignment(Qt.AlignmentFlag.AlignLeft)
-        self._total_time_lbl.setSizePolicy(
-            QSizePolicy.Policy.Fixed, QSizePolicy.Policy.Fixed
-        )
-        wdg_lay.addWidget(self._total_time_lbl)
-
-
 class _SaveLoadSequenceWidget(QWidget):
     def __init__(self, parent: QWidget | None = None) -> None:
         super().__init__(parent)
 
         self._save_button = QPushButton("Save")
         self._load_button = QPushButton("Load")
```

### Comparing `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_mda/_grid_widget.py` & `pymmcore_widgets-0.4.1/src/pymmcore_widgets/_mda/_grid_widget.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import math
 import warnings
-from typing import TYPE_CHECKING, Literal, cast
+from typing import Literal, cast
 
+import useq
 from pymmcore_plus import CMMCorePlus
 from qtpy.QtCore import Qt, Signal
 from qtpy.QtWidgets import (
     QAbstractSpinBox,
     QComboBox,
     QDoubleSpinBox,
     QGridLayout,
@@ -21,35 +22,17 @@
     QSpacerItem,
     QSpinBox,
     QTabWidget,
     QVBoxLayout,
     QWidget,
 )
 from superqt.utils import signals_blocked
-from useq import AnyGridPlan, GridFromEdges, GridRelative
-from useq._grid import OrderMode, RelativeTo
-
-from .._util import get_grid_type
-
-if TYPE_CHECKING:
-    from typing_extensions import TypedDict
-
-    class GridDict(TypedDict, total=False):
-        """Grid dictionary."""
-
-        overlap: float | tuple[float, float]
-        mode: OrderMode | str
-        rows: int
-        columns: int
-        relative_to: RelativeTo | str
-        top: float
-        left: float
-        bottom: float
-        right: float
+from useq._grid import OrderMode, RelativeTo  # TODO: fix private import
 
+from pymmcore_widgets._util import cast_grid_plan, fov_kwargs
 
 fixed_sizepolicy = QSizePolicy(QSizePolicy.Policy.Fixed, QSizePolicy.Policy.Fixed)
 
 
 class _TabWidget(QTabWidget):
     """Main Tab Widget containing all the grid options...
 
@@ -80,28 +63,28 @@
         # grid from corners
         self.corners = _FromCornersWdg(mmcore=self._mmc)
         self.corners.valueChanged.connect(self.valueChanged)
         self.addTab(self.corners, "Grid from Corners")
 
         self.currentChanged.connect(self._on_tab_changed)
 
-    def value(self) -> GridDict:
+    def value(self) -> useq.AnyGridPlan:
         if self.currentIndex() == 0:
             return self._rowcol.value()
         elif self.currentIndex() == 1:
             return self.edges.value()
         else:
             return self.corners.value()
 
-    def setValue(self, grid: GridDict) -> None:
-        grid_type = get_grid_type(grid)  # type: ignore
-        if isinstance(grid_type, GridRelative):
-            self._rowcol.setValue(grid)
-        elif isinstance(grid_type, GridFromEdges):
-            self.edges.setValue(grid)
+    def setValue(self, grid: dict | useq.AnyGridPlan) -> None:
+        _grid = cast_grid_plan(grid)
+        if isinstance(_grid, useq.GridRelative):
+            self._rowcol.setValue(_grid)
+        elif isinstance(_grid, useq.GridFromEdges):
+            self.edges.setValue(_grid)
         self.valueChanged.emit()
 
     def _on_tab_changed(self) -> None:
         self.valueChanged.emit()
 
 
 class _RowsColsWdg(QWidget):
@@ -159,39 +142,33 @@
         spin.setAlignment(Qt.AlignmentFlag.AlignCenter)
         spin.setKeyboardTracking(False)
         spin.valueChanged.connect(lambda: self.valueChanged.emit())
         layout.addWidget(label)
         layout.addWidget(spin)
         return spin
 
-    def value(self) -> GridDict:
-        """Return the _RowsColsWdg grid dictionary."""
-        return {
-            "rows": self.n_rows.value(),
-            "columns": self.n_columns.value(),
-            "relative_to": self.relative_combo.currentText(),
-        }
+    def value(self) -> useq.GridRelative:
+        """Return useq.GridRelative instance with state of widget."""
+        return useq.GridRelative(
+            rows=self.n_rows.value(),
+            columns=self.n_columns.value(),
+            relative_to=self.relative_combo.currentText(),
+        )
 
-    def setValue(self, grid: GridDict) -> None:
-        """Set the _RowsColsWdg grid dictionary."""
-        keys = ["rows", "columns"]
-        if any(item not in grid.keys() for item in keys):
-            warnings.warn(f"Grid dictionary must contain {keys} keys", stacklevel=2)
+    def setValue(self, grid: dict | useq.GridRelative) -> None:
+        """Set widget state from object that can be cast to useq.GridRelative."""
+        try:
+            _grid = useq.GridRelative.validate(grid)
+        except ValueError as e:  # pragma: no cover
+            warnings.warn(f"Invalid GridRelative value: {e}", stacklevel=2)
             return
 
-        self.n_rows.setValue(grid["rows"])
-        self.n_columns.setValue(grid["columns"])
-
-        if "relative_to" in grid:
-            self.relative_combo.setCurrentText(
-                grid["relative_to"]
-                if isinstance(grid["relative_to"], str)
-                else grid["relative_to"].value
-            )
-
+        self.n_rows.setValue(_grid.rows)
+        self.n_columns.setValue(_grid.columns)
+        self.relative_combo.setCurrentText(_grid.relative_to.value)
         self.valueChanged.emit()
 
 
 class _FromEdgesWdg(QWidget):
     """Widget for setting the grid's edges."""
 
     valueChanged = Signal()
@@ -225,35 +202,35 @@
         self.left.label.setFixedWidth(self.right.label.sizeHint().width() + 5)
 
         group_layout.addWidget(self.top, 0, 0)
         group_layout.addWidget(self.bottom, 1, 0)
         group_layout.addWidget(self.left, 0, 1)
         group_layout.addWidget(self.right, 1, 1)
 
-    def value(self) -> GridDict:
+    def value(self) -> useq.GridFromEdges:
         """Return the _FromEdgesWdg grid dictionary."""
-        return {
-            "top": cast("float", self.top.value()),
-            "bottom": cast("float", self.bottom.value()),
-            "left": cast("float", self.left.value()),
-            "right": cast("float", self.right.value()),
-        }
+        return useq.GridFromEdges(
+            top=self.top.value(),
+            bottom=self.bottom.value(),
+            left=self.left.value(),
+            right=self.right.value(),
+        )
 
-    def setValue(self, grid: GridDict) -> None:
+    def setValue(self, grid: dict | useq.GridFromEdges) -> None:
         """Set the _FromEdgesWdg grid dictionary."""
-        keys = ["top", "bottom", "left", "right"]
-        if any(item not in grid.keys() for item in keys):
-            warnings.warn(f"Grid dictionary must contain {keys} keys", stacklevel=2)
+        try:
+            _grid = useq.GridFromEdges.validate(grid)
+        except ValueError as e:  # pragma: no cover
+            warnings.warn(f"Invalid GridFromEdges value: {e}", stacklevel=2)
             return
 
-        self.top.setValue(grid["top"])
-        self.bottom.setValue(grid["bottom"])
-        self.left.setValue(grid["left"])
-        self.right.setValue(grid["right"])
-
+        self.top.setValue(_grid.top)
+        self.bottom.setValue(_grid.bottom)
+        self.left.setValue(_grid.left)
+        self.right.setValue(_grid.right)
         self.valueChanged.emit()
 
 
 class _FromCornersWdg(QWidget):
     """Widget for setting the grid's corners."""
 
     valueChanged = Signal()
@@ -277,35 +254,37 @@
 
         self.corner_1.label.setFixedWidth(self.corner_2.label.sizeHint().width() + 5)
         self.corner_2.label.setFixedWidth(self.corner_2.label.sizeHint().width() + 5)
 
         group_layout.addWidget(self.corner_1)
         group_layout.addWidget(self.corner_2)
 
-    def value(self) -> GridDict:
-        """Return the _FromCornersWdg grid dictionary."""
-        corner1_x, corner1_y = cast("tuple[float, float]", self.corner_1.value())
-        corner2_x, corner2_y = cast("tuple[float, float]", self.corner_2.value())
-        return {
-            "top": max(corner1_y, corner2_y),
-            "bottom": min(corner1_y, corner2_y),
-            "left": min(corner1_x, corner2_x),
-            "right": max(corner1_x, corner2_x),
-        }
+    def value(self) -> useq.GridFromEdges:
+        """Return Grid plan."""
+        # FIXME: how do we know we can type ignore here?
+        corner1_x, corner1_y = self.corner_1.value()  # type: ignore
+        corner2_x, corner2_y = self.corner_2.value()  # type: ignore
+
+        return useq.GridFromEdges(
+            top=max(corner1_y, corner2_y),
+            bottom=min(corner1_y, corner2_y),
+            left=min(corner1_x, corner2_x),
+            right=max(corner1_x, corner2_x),
+        )
 
-    def setValue(self, grid: GridDict) -> None:
-        """Set the _FromCornersWdg grid dictionary."""
-        keys = ["top", "bottom", "left", "right"]
-        if any(item not in grid.keys() for item in keys):
-            warnings.warn(f"Grid dictionary must contain {keys} keys", stacklevel=2)
+    def setValue(self, grid: dict | useq.GridFromEdges) -> None:
+        """Set value from object that can be cast to GridRelative."""
+        try:
+            _grid = useq.GridFromEdges.validate(grid)
+        except ValueError as e:  # pragma: no cover
+            warnings.warn(f"Invalid GridFromEdges value: {e}", stacklevel=2)
             return
 
-        self.corner_1.setValue((grid["left"], grid["top"]))
-        self.corner_2.setValue((grid["right"], grid["bottom"]))
-
+        self.corner_1.setValue((_grid.left, _grid.top))
+        self.corner_2.setValue((_grid.right, _grid.bottom))
         self.valueChanged.emit()
 
 
 class _DoubleSpinboxWidget(QWidget):
     """Double spinbox widget used by _FromEdgesWdg and _FromCornersWdg.
 
     It allows to set the grid's top, bottom, left, right, positions
@@ -380,15 +359,15 @@
             self.spinbox.setValue(self._mmc.getYPosition())
         elif self._label in {"left", "right"}:
             self.spinbox.setValue(self._mmc.getXPosition())
 
     def value(self) -> float | tuple[float, float]:
         if self._corners:
             return self.x_spinbox.value(), self.y_spinbox.value()
-        return self.spinbox.value()  # type: ignore
+        return cast(float, self.spinbox.value())
 
     def setValue(self, value: float | tuple[float, float]) -> None:
         if isinstance(value, tuple):
             self.x_spinbox.setValue(value[0])
             self.y_spinbox.setValue(value[1])
         else:
             self.spinbox.setValue(value)
@@ -445,37 +424,32 @@
         spin.setMinimumWidth(100)
         spin.setMaximum(100)
         spin.setAlignment(Qt.AlignmentFlag.AlignCenter)
         spin.setKeyboardTracking(False)
         spin.valueChanged.connect(lambda: self.valueChanged.emit())
         return spin
 
-    def value(self) -> GridDict:
+    def value(self) -> dict:
         return {
             "overlap": (self.overlap_spinbox_x.value(), self.overlap_spinbox_y.value()),
             "mode": self.ordermode_combo.currentText(),
         }
 
-    def setValue(self, value: GridDict) -> None:
-        if "overlap" not in value:
+    def setValue(self, value: dict | useq.AnyGridPlan) -> None:
+        try:
+            _grid = cast_grid_plan(value)
+        except ValueError as e:  # pragma: no cover
+            warnings.warn(f"Invalid grid value: {e}", stacklevel=2)
+            return
+        if not _grid:
             return
 
-        over_x, over_y = (
-            value["overlap"]
-            if isinstance(value["overlap"], tuple)
-            else (value["overlap"], value["overlap"])
-        )
-        self.overlap_spinbox_x.setValue(over_x)
-        self.overlap_spinbox_y.setValue(over_y)
-
-        if "mode" in value:
-            self.ordermode_combo.setCurrentText(
-                value["mode"] if isinstance(value["mode"], str) else value["mode"].value
-            )
-
+        self.overlap_spinbox_x.setValue(_grid.overlap[0])
+        self.overlap_spinbox_y.setValue(_grid.overlap[1])
+        self.ordermode_combo.setCurrentText(_grid.mode.value)
         self.valueChanged.emit()
 
 
 class _MoveToWidget(QGroupBox):
     """Widget used to move to a specific grid position.
 
     It requires a _TabWidget to be able to access the selected grid plan.
@@ -542,35 +516,39 @@
     def _move_to_row_col(self) -> None:
         """Move to a selected position depending on the used grid plan."""
         if self._current_position is None:
             curr_x, curr_y = (self._mmc.getXPosition(), self._mmc.getYPosition())
         else:
             curr_x, curr_y = self._current_position
 
-        grid = get_grid_type(self._tabwidget.value())  # type: ignore
+        grid = cast_grid_plan(self._tabwidget.value())
 
         if grid is None:
             return
 
-        if isinstance(grid, GridRelative) and (curr_x is None or curr_y is None):
+        if isinstance(grid, useq.GridRelative) and (curr_x is None or curr_y is None):
             return
 
         _move_to_row = int(self._move_to_row.currentText())
         _move_to_col = int(self._move_to_col.currentText())
 
         row = _move_to_row - 1 if _move_to_row > 0 else 0
         col = _move_to_col - 1 if _move_to_col > 0 else 0
 
         _, _, width, height = self._mmc.getROI(self._mmc.getCameraDevice())
         width = int(width * self._mmc.getPixelSizeUm())
         height = int(height * self._mmc.getPixelSizeUm())
 
+        # FIXME!!
+        # This is a major performance hit.
+        # There must be a more direct way to determine the proper x and y
+        # positions without checking all positions in the grid for equality.
         for pos in grid.iter_grid_positions(width, height):
             if pos.row == row and pos.col == col:
-                if isinstance(grid, GridRelative):
+                if isinstance(grid, useq.GridRelative):
                     xpos = curr_x + pos.x
                     ypos = curr_y + pos.y
                 else:
                     xpos = pos.x
                     ypos = pos.y
                 self._mmc.setXYPosition(xpos, ypos)
                 return
@@ -684,103 +662,109 @@
         self._mmc.events.systemConfigurationLoaded.connect(self._update_info)
         self._mmc.events.pixelSizeChanged.connect(self._update_info)
 
         self.destroyed.connect(self._disconnect)
 
     def _update_info(self) -> None:
         """Update the info label with the current grid size."""
-        if not self._mmc.getPixelSizeUm():
+        pix_size = self._mmc.getPixelSizeUm()
+        if not pix_size:
             self.info_lbl.setText(
                 "Height: _ mm    Width: _ mm    (Rows: _    Columns: _)"
             )
             return
 
-        _, _, width, height = self._mmc.getROI(self._mmc.getCameraDevice())
-        width = int(width * self._mmc.getPixelSizeUm())
-        height = int(height * self._mmc.getPixelSizeUm())
-        overlap_xcent_x, overlap_xcent_y = cast(
-            "tuple[float, float]", self.overlap_and_mode.value()["overlap"]
-        )
-        overlap_xcent_x = width * overlap_xcent_x / 100
-        overlap_xcent_y = height * overlap_xcent_y / 100
+        cur_grid = self.value()
 
-        if self.tab.currentIndex() == 0:
-            rows, cols = (self.tab.value()["rows"], self.tab.value()["columns"])
-            x = ((width - overlap_xcent_x) * cols) / 1000
-            y = ((height - overlap_xcent_y) * rows) / 1000
+        # TODO: i'm pretty sure all of this is done by useq already...
+        _, _, width, height = self._mmc.getROI(self._mmc.getCameraDevice())
+        width = int(width * pix_size)
+        height = int(height * pix_size)
+        overlap_x, overlap_y = cur_grid.overlap
+        overlap_x *= width / 100
+        overlap_y *= height / 100
+
+        if isinstance(cur_grid, useq.GridRelative):
+            x = (width - overlap_x) * cur_grid.columns / 1000
+            y = (height - overlap_y) * cur_grid.rows / 1000
+            rows = cur_grid.rows
+            cols = cur_grid.columns
         else:
-            top, bottom, left, right = cast(
-                "tuple[float, ...]", self.tab.value().values()
-            )
-
-            rows = math.ceil((abs(top - bottom) + height) / height)
-            cols = math.ceil((abs(right - left) + width) / width)
+            grid_width = abs(cur_grid.right - cur_grid.left) + width
+            grid_height = abs(cur_grid.top - cur_grid.bottom) + height
 
-            x = (abs(left - right) + width) / 1000
-            y = (abs(top - bottom) + height) / 1000
+            rows = math.ceil(grid_height / height)
+            cols = math.ceil(grid_width / width)
+            x = grid_width / 1000
+            y = grid_height / 1000
 
         self.info_lbl.setText(
-            f"Height: {round(y, 3)} mm    Width: {round(x, 3)} mm    "
+            f"Height: {y:.3f} mm    Width: {x:.3f} mm    "
             f"(Rows: {rows}    Columns: {cols})"
         )
 
         self.move_to._clear()
         self.move_to._add_items(
             [str(r) for r in range(1, rows + 1)], [str(r) for r in range(1, cols + 1)]
         )
 
-    # note: this really ought to be GridDict, but it makes typing harder
-    def value(self) -> dict:
+    def value(self) -> useq.AnyGridPlan:
         """Return the current GridPlan settings.
 
         Note that output dict will match the Channel from useq schema:
         <https://pymmcore-plus.github.io/useq-schema/schema/axes/#grid-plans>
         """
-        return {**self.tab.value(), **self.overlap_and_mode.value()}
+        replace = {**self.overlap_and_mode.value(), **fov_kwargs(self._mmc)}
+        return self.tab.value().replace(**replace)
 
-    def set_state(self, grid: dict | AnyGridPlan) -> None:
+    def set_state(self, grid: dict | useq.AnyGridPlan) -> None:
         """Set the state of the widget from a useq AnyGridPlan or dictionary."""
         with signals_blocked(self):
-            grid_plan = get_grid_type(grid) if isinstance(grid, dict) else grid
+            grid_plan = cast_grid_plan(grid)
+            if grid_plan is None:
+                # TODO: do we have a clear?
+                return
 
-            self.overlap_and_mode.setValue(grid_plan.dict())  # type: ignore
-            self.tab.setValue(grid_plan.dict())  # type: ignore
-            self.tab.setCurrentIndex(0) if isinstance(
-                grid_plan, GridRelative
-            ) else self.tab.setCurrentIndex(1)
+            self.overlap_and_mode.setValue(grid_plan)
+            self.tab.setValue(grid_plan)
+            idx = 0 if isinstance(grid_plan, useq.GridRelative) else 1
+            self.tab.setCurrentIndex(idx)
             self._update_info()
-        self.valueChanged.emit(self.value())
+        self.valueChanged.emit(grid_plan)
 
     def _emit_grid_positions(self) -> None:
         """Emit the grid positions if the pixel size is set."""
         if self._mmc.getPixelSizeUm() <= 0:
             raise ValueError("Pixel Size Not Set.")
 
-        if self.tab.currentIndex() > 0 and any(
-            str(v) == "0.0" for v in self.tab.value().values()
+        val = self.value()
+        if isinstance(val, useq.GridFromEdges) and not all(
+            (val.top, val.bottom, val.left, val.right)
         ):
             self._show_warning()
         else:
-            self.valueChanged.emit(self.value())
+            self.valueChanged.emit(val)
 
     def _show_warning(self) -> None:
         """Show a warning message if the user has not set all the grid positions."""
         if self.tab.currentIndex() == 1:
             msg = (
                 "Did you set all four 'top',  'bottom',  'left', and  'right'  "
                 "positions?"
             )
         elif self.tab.currentIndex() == 2:
             msg = "Did you set the both corner positions?"
 
         msgBox = QMessageBox()
-        msgBox.setIcon(QMessageBox.Warning)
+        msgBox.setIcon(QMessageBox.Icon.Warning)
         msgBox.setText(msg)
         msgBox.setWindowTitle("Grid from Edges")
-        msgBox.setStandardButtons(QMessageBox.Ok | QMessageBox.Cancel)
+        msgBox.setStandardButtons(
+            QMessageBox.StandardButton.Ok | QMessageBox.StandardButton.Cancel
+        )
 
-        if msgBox.exec() == QMessageBox.Ok:
+        if msgBox.exec() == QMessageBox.StandardButton.Ok:
             self.valueChanged.emit(self.value())
 
     def _disconnect(self) -> None:
         self._mmc.events.systemConfigurationLoaded.disconnect(self._update_info)
         self._mmc.events.pixelSizeChanged.disconnect(self._update_info)
```

### Comparing `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_mda/_mda_widget.py` & `pymmcore_widgets-0.4.1/src/pymmcore_widgets/_mda/_mda_widget.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 from __future__ import annotations
 
 import warnings
-from datetime import timedelta
 from pathlib import Path
 from typing import TYPE_CHECKING
 
+import useq
 from pymmcore_plus import CMMCorePlus
 from qtpy.QtCore import Qt
 from qtpy.QtWidgets import (
     QCheckBox,
     QFileDialog,
     QHBoxLayout,
     QScrollArea,
     QSizePolicy,
     QVBoxLayout,
     QWidget,
 )
 from useq import MDASequence
 
-from .._util import fmt_timedelta
 from ._channel_table_widget import ChannelTable
 from ._checkable_tabwidget_widget import CheckableTabWidget
 from ._general_mda_widgets import (
     _AcquisitionOrderWidget,
     _MDAControlButtons,
-    _MDATimeLabel,
     _SaveLoadSequenceWidget,
 )
 from ._grid_widget import GridWidget
 from ._positions_table_widget import PositionTable
 from ._time_plan_widget import TimePlanWidget
 from ._zstack_widget import ZStackWidget
 
@@ -113,15 +111,14 @@
         # Channels, Time, Z Stack, Positions and Grid widgets
         self.channel_widget = ChannelTable()
         self.time_widget = TimePlanWidget()
         self.stack_widget = ZStackWidget()
         self.stack_widget.setFixedHeight(self.stack_widget.minimumSizeHint().height())
         self.position_widget = PositionTable()
         self.grid_widget = Grid()
-        self.grid_widget.valueChanged.connect(self._update_total_time)
         self.grid_widget.layout().itemAt(
             self.grid_widget.layout().count() - 1
         ).widget().hide()  # hide add grid button
         self.grid_widget.setFixedHeight(self.grid_widget.sizeHint().height())
 
         # place widgets in a QWidget to control tab layout content margins
         wdgs = [
@@ -137,17 +134,14 @@
         # assign checkboxes to a variable
         self.ch_cbox = self._get_checkbox(0)
         self.z_cbox = self._get_checkbox(1)
         self.p_cbox = self._get_checkbox(2)
         self.t_cbox = self._get_checkbox(3)
         self.g_cbox = self._get_checkbox(4)
 
-        # info time label and buttons widgets
-        self.time_lbl = _MDATimeLabel()
-
         # savle load widget
         self._save_load = _SaveLoadSequenceWidget()
         self._save_load._save_button.clicked.connect(self._save_sequence)
         self._save_load._load_button.clicked.connect(self._load_sequence)
 
         # Acquisition order widget
         self.acquisition_order_widget = _AcquisitionOrderWidget()
@@ -165,54 +159,36 @@
         scroll.setAlignment(Qt.AlignmentFlag.AlignCenter)
         scroll.setWidget(self._central_widget)
 
         self.setLayout(QVBoxLayout())
         self.layout().setSpacing(10)
         self.layout().setContentsMargins(10, 10, 10, 10)
         self.layout().addWidget(scroll)
-        self.layout().addWidget(self.time_lbl)
         self.layout().addLayout(acq_order_run_layout)
 
         # CONNECTIONS
-        # connect tabs changed signal
         self._tab.currentChanged.connect(self._on_tab_changed)
-        # connect Channels, Time, Z Stack, Positions and Grid widgets
         self.channel_widget.valueChanged.connect(self._enable_run_btn)
-        self.channel_widget.valueChanged.connect(self._update_total_time)
-        self.channel_widget._advanced_cbox.toggled.connect(self._update_total_time)
-        self.time_widget.valueChanged.connect(self._update_total_time)
-        self.stack_widget.valueChanged.connect(self._update_total_time)
-        self.position_widget._advanced_cbox.toggled.connect(self._update_total_time)
-        self.position_widget.valueChanged.connect(self._update_total_time)
         # below not using lambda with position_widget below because it would cause
         # problems in closing the widget (see conftest _run_after_each_test fixture)
         self.position_widget.valueChanged.connect(self._on_positions_tab_changed)
-        # connect tab checkboxes
         self.ch_cbox.toggled.connect(self._enable_run_btn)
-        self.ch_cbox.toggled.connect(self._update_total_time)
-        self.z_cbox.toggled.connect(self._update_total_time)
-        self.t_cbox.toggled.connect(self._update_total_time)
-        self.p_cbox.toggled.connect(self._update_total_time)
         # not using lambda with p_cbox below because it would cause problems in closing
         # the widget (see conftest _run_after_each_test fixture)
         self.p_cbox.toggled.connect(self._on_positions_tab_changed)
-        self.g_cbox.toggled.connect(self._update_total_time)
-        # connect mmcore signals
         self._mmc.mda.events.sequenceStarted.connect(self._on_mda_started)
         self._mmc.mda.events.sequenceFinished.connect(self._on_mda_finished)
         self._mmc.events.systemConfigurationLoaded.connect(self._on_sys_cfg_loaded)
         self._mmc.events.configSet.connect(self._on_config_set)
         self._mmc.events.configGroupChanged.connect(self._on_config_set)
         self._mmc.events.channelGroupChanged.connect(self._enable_run_btn)
-        # connect run button
         if self._include_run_button:
             self.buttons_wdg = _MDAControlButtons()
             self.buttons_wdg.run_button.clicked.connect(self._on_run_clicked)
             self.buttons_wdg.run_button.show()
-            # connect buttons
             self.buttons_wdg.pause_button.released.connect(self._mmc.mda.toggle_pause)
             self.buttons_wdg.cancel_button.released.connect(self._mmc.mda.cancel)
             acq_order_run_layout.addWidget(self.buttons_wdg)
 
         self._on_sys_cfg_loaded()
 
         self.destroyed.connect(self._disconnect)
@@ -288,17 +264,14 @@
 
         Parameters
         ----------
         state : dict | MDASequence | str | Path
             MDASequence state in the form of a dict, MDASequence object, or a str or
             Path pointing to a sequence.yaml file
         """
-        # TODO: prevent _update_total_time from being called until
-        # all subcomponents have been set
-
         # sourcery skip: low-code-quality
         if isinstance(state, (str, Path)):
             state = MDASequence.parse_file(state)
         elif isinstance(state, dict):
             state = MDASequence(**state)
         if not isinstance(state, MDASequence):
             raise TypeError("state must be an MDASequence, dict, or yaml file")
@@ -345,74 +318,49 @@
     def get_state(self) -> MDASequence:
         """Get current state of widget and build a useq.MDASequence.
 
         Returns
         -------
         useq.MDASequence
         """
-        channels = (
-            self.channel_widget.value()
-            if self.ch_cbox.isChecked()
-            else [
-                {
-                    "config": self._mmc.getCurrentConfig(self._mmc.getChannelGroup()),
-                    "group": self._mmc.getChannelGroup(),
-                    "exposure": self._mmc.getExposure(),
-                    "z_offset": 0.0,
-                    "do_stack": True,
-                    "acquire_every": 1,
-                }
+        if self.ch_cbox.isChecked():
+            channels = self.channel_widget.value()
+        else:
+            group = self._mmc.getChannelGroup()
+            channels = [
+                useq.Channel(config=self._mmc.getCurrentConfig(group), group=group)
             ]
-        )
 
         stage_positions: list[PositionDict] = []
         if self.p_cbox.isChecked():
+            order_combo = self.acquisition_order_widget.acquisition_order_comboBox
+            axis_order = order_combo.currentText()
             for p in self.position_widget.value():
                 if p.get("sequence"):
-                    p_sequence = MDASequence(**p.get("sequence"))  # type: ignore
-                    p_sequence = p_sequence.replace(
-                        axis_order=self.acquisition_order_widget.acquisition_order_comboBox.currentText()
-                    )
-                    p_sequence.set_fov_size(self._get_fov_size())
-                    p["sequence"] = p_sequence
-                stage_positions.append(p)
+                    seq_kwargs = p.get("sequence") or {}
+                    seq_kwargs["axis_order"] = axis_order
+                    p_sequence = MDASequence(**seq_kwargs)
+                    p["sequence"] = p_sequence  # type: ignore  # FIXME
+                stage_positions.append(p)  # type: ignore
 
         if not stage_positions:
             stage_positions = self._get_current_position()
 
-        z_plan = self.stack_widget.value() if self.z_cbox.isChecked() else None
-        time_plan = self.time_widget.value() if self._uses_time() else None
-        grid_plan = self.grid_widget.value() if self.g_cbox.isChecked() else None
-
-        update_kwargs: dict = {}
-        if z_plan is not None:
-            update_kwargs["z_plan"] = z_plan
-        if time_plan is not None:
-            update_kwargs["time_plan"] = time_plan
-        if grid_plan is not None:
-            update_kwargs["grid_plan"] = grid_plan
-
         mda = MDASequence(
             axis_order=(
                 self.acquisition_order_widget.acquisition_order_comboBox.currentText()
             ),
             channels=channels,
             stage_positions=stage_positions,
-            **update_kwargs,
+            time_plan=self.time_widget.value() if self._uses_time() else None,
+            grid_plan=self.grid_widget.value() if self.g_cbox.isChecked() else None,
+            z_plan=self.stack_widget.value() if self.z_cbox.isChecked() else None,
         )
-        mda.set_fov_size(self._get_fov_size())
         return mda
 
-    def _get_fov_size(self) -> tuple[float, float]:
-        """Return image width and height in micron to be used for the grid plan."""
-        if px := self._mmc.getPixelSizeUm():
-            _, _, widtgh, height = self._mmc.getROI()
-            return (widtgh * px, height * px)
-        return (1.0, 1.0)
-
     def _get_current_position(self) -> list[PositionDict]:
         return [
             {
                 "name": "Pos000",
                 "x": (
                     self._mmc.getXPosition() if self._mmc.getXYStageDevice() else None
                 ),
@@ -453,113 +401,23 @@
             with open(filename) as file:
                 self.set_state(json.load(file))
 
     def _on_time_toggled(self, checked: bool) -> None:
         """Hide the warning if the time groupbox is unchecked."""
         if not checked and self.time_widget._warning_widget.isVisible():
             self.time_widget.setWarningVisible(False)
-        else:
-            self._update_total_time()
 
     def _uses_time(self) -> bool:
         """Hacky method to check whether the timebox is selected with any timepoints."""
         has_phases = self.time_widget._table.rowCount()
         return bool(self.t_cbox.isChecked() and has_phases)
 
     def _uses_autofocus(self) -> bool:
         return bool(self.p_cbox.isChecked() and self.position_widget._use_af())
 
-    def _update_total_time(self) -> None:
-        """Calculate the minimum total acquisition time info."""
-        # TODO: fix me!!!!!
-        if self._mmc.getChannelGroup() and self._mmc.getCurrentConfig(
-            self._mmc.getChannelGroup()
-        ):
-            if self.ch_cbox.isChecked() and not self.channel_widget._table.rowCount():
-                self.time_lbl._total_time_lbl.setText(
-                    "Minimum total acquisition time: 0 sec."
-                )
-                return
-
-        elif not self.ch_cbox.isChecked() or not self.channel_widget._table.rowCount():
-            self.time_lbl._total_time_lbl.setText(
-                "Minimum total acquisition time: 0 sec."
-            )
-            return
-
-        total_time: float = 0.0
-        _per_timepoints: dict[int, float] = {}
-        t_per_tp_msg = ""
-        _uses_time = self._uses_time()
-
-        for e in self.get_state():
-            if e.exposure is None:
-                continue
-
-            total_time = total_time + (e.exposure / 1000)
-            if _uses_time:
-                _t = e.index["t"]
-                _exp = e.exposure / 1000
-                _per_timepoints[_t] = _per_timepoints.get(_t, 0) + _exp
-
-        if _per_timepoints:
-            time_value = self.time_widget.value()
-
-            intervals = []
-            for phase in time_value["phases"]:  # type: ignore
-                interval = phase["interval"].total_seconds()
-                intervals.append(interval)
-                if phase.get("loops") is not None:
-                    total_time = total_time + (phase["loops"] - 1) * interval
-                else:
-                    total_time = total_time + phase["duration"].total_seconds()
-
-            # check if the interval(s) is smaller than the sum of the exposure times
-            sum_ch_exp = sum(
-                (c["exposure"] / 1000)
-                for c in self.channel_widget.value()
-                if c["exposure"] is not None
-            )
-            for i in intervals:
-                if 0 < i < sum_ch_exp:
-                    self.time_widget.setWarningVisible(True)
-                    break
-                else:
-                    self.time_widget.setWarningVisible(False)
-
-            # group by time
-            _group_by_time: dict[float, list[int]] = {
-                n: [k for k in _per_timepoints if _per_timepoints[k] == n]
-                for n in set(_per_timepoints.values())
-            }
-
-            t_per_tp_msg = "Minimum acquisition time per timepoint: "
-
-            if len(_group_by_time) == 1:
-                t_per_tp_msg = (
-                    f"\n{t_per_tp_msg}"
-                    f"{fmt_timedelta(timedelta(seconds=_per_timepoints[0]))}"
-                )
-            else:
-                acq_min = timedelta(seconds=min(_per_timepoints.values()))
-                t_per_tp_msg = (
-                    f"\n{t_per_tp_msg}{fmt_timedelta(acq_min)}"
-                    if self._uses_time()
-                    else ""
-                )
-        else:
-            t_per_tp_msg = ""
-            self.time_widget.setWarningVisible(False)
-
-        _min_tot_time = (
-            "Minimum total acquisition time: "
-            f"{fmt_timedelta(timedelta(seconds=total_time))}"
-        )
-        self.time_lbl._total_time_lbl.setText(f"{_min_tot_time}{t_per_tp_msg}")
-
     def _disconnect(self) -> None:
         self._mmc.mda.events.sequenceStarted.disconnect(self._on_mda_started)
         self._mmc.mda.events.sequenceFinished.disconnect(self._on_mda_finished)
         self._mmc.events.systemConfigurationLoaded.disconnect(self._on_sys_cfg_loaded)
         self._mmc.events.configSet.disconnect(self._on_config_set)
         self._mmc.events.configGroupChanged.disconnect(self._on_config_set)
         self._mmc.events.channelGroupChanged.disconnect(self._on_channel_group_changed)
```

### Comparing `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_mda/_positions_table_widget.py` & `pymmcore_widgets-0.4.1/src/pymmcore_widgets/_mda/_positions_table_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,37 +28,32 @@
     QTableWidgetItem,
     QVBoxLayout,
     QWidget,
 )
 from superqt import fonticon
 from superqt.fonticon import icon
 from superqt.utils import signals_blocked
-from useq import (  # type: ignore
-    AxesBasedAF,
-    GridFromEdges,
-    GridRelative,
-    MDASequence,
-    Position,
-)
+from useq import AxesBasedAF, GridFromEdges, GridRelative, MDASequence, Position
+
+from pymmcore_widgets._util import cast_grid_plan, fov_kwargs
 
-from .._util import get_grid_type
 from ._autofocus_device_widget import _AutofocusZDeviceWidget
 from ._grid_widget import GridWidget
 
 if TYPE_CHECKING:
     from typing_extensions import TypedDict
 
     class PositionDict(TypedDict, total=False):
         """Position dictionary."""
 
         x: float | None
         y: float | None
         z: float | None
         name: str | None
-        sequence: MDASequence | None
+        sequence: dict | None
 
 
 POS = "Pos"
 P = 0
 X = 1
 Y = 2
 Z = 3
@@ -146,16 +141,19 @@
 
         # autofocus
         af_groupbox = QGroupBox()
         af_groupbox_layout = QHBoxLayout()
         af_groupbox_layout.setSpacing(0)
         af_groupbox_layout.setContentsMargins(0, 0, 0, 0)
         af_groupbox.setLayout(af_groupbox_layout)
-        self._autofocus_wdg = _AutofocusZDeviceWidget()
-        self._autofocus_wdg.valueChanged.connect(self._on_autofocus_value_changed)
+        self._autofocus_wdg = _AutofocusZDeviceWidget(self)
+        self._autofocus_wdg._af_combo.currentTextChanged.connect(
+            self._on_af_wdg_changed
+        )
+        self._autofocus_wdg._af_checkbox.toggled.connect(self._on_af_wdg_changed)
         af_groupbox_layout.addWidget(self._autofocus_wdg)
         group_layout.addWidget(af_groupbox, 0, 0, 1, 2)
 
         # buttons
         buttons_wdg = QWidget()
         buttons_layout = QVBoxLayout()
         buttons_layout.setSpacing(10)
@@ -260,87 +258,51 @@
         self.destroyed.connect(self._disconnect)
 
         self._on_sys_cfg_loaded()
 
     def _on_sys_cfg_loaded(self) -> None:
         self.clear()
         self._set_table_header()
-        self._advanced_cbox.setEnabled(
-            bool(self._mmc.getLoadedDevicesOfType(DeviceType.XYStageDevice))
-        )
         advanced = self._advanced_cbox.isChecked()
         self._table.setColumnHidden(GRID, not advanced)
         self._table.setColumnHidden(AF, not self._use_af())
 
     def _on_property_changed(self, device: str, prop: str, value: str) -> None:
         # TODO: add 'propertyChanged.emit()' to pymmcore-plus setProperty() methods
-        if not self._mmc.getLoadedDevicesOfType(
-            DeviceType.XYStageDevice
-        ) and not self._mmc.getLoadedDevicesOfType(DeviceType.StageDevice):
+        if device != "Core" and prop not in {"Focus", "AutoFocus"}:
             return
-
-        if device != "Core" and prop not in {"Focus", "XYStage", "AutoFocus"}:
+        # if prop is 'Focus', rename column header with default ZStage or "Z"
+        if prop == "Focus":
+            name, idx = (self._mmc.getFocusDevice() or "Z", Z)
+        # if prop is 'AutoFocus' but not in use, return
+        elif not self._use_af():
             return
+        # if prop is 'AutoFocus', rename column header with 'autofocus_device_name'
+        # or 'Autofocus'
+        else:
+            name, idx = (self._get_af_device() or "Autofocus", AF)
 
-        # hide XY or Z columns if ZStage or XYStage are not loaded + remove cell values
-        indexes = {
-            "Focus": [Z],
-            "XYStage": [X, Y],
-            "AutoFocus": [AF],
-        }.get(prop, [])
-
-        for idx in indexes:
-            self._table.setColumnHidden(idx, not value)
-            for r in range(self._table.rowCount()):
-                self._table.removeCellWidget(r, idx)
-
-            # rename column header with default ZStage or Autofocus
-            if idx not in {Z, AF} or not self._use_af():
-                continue
-            name = self._mmc.getFocusDevice() if idx == Z else "Autofocus"
-            self._table.setHorizontalHeaderItem(idx, QTableWidgetItem(name))
+        self._table.setHorizontalHeaderItem(idx, QTableWidgetItem(name))
 
     def _set_table_header(self) -> None:
         self._table.setColumnCount(0)
-
-        if not self._mmc.getLoadedDevicesOfType(
-            DeviceType.XYStageDevice
-        ) and not self._mmc.getLoadedDevicesOfType(DeviceType.StageDevice):
-            self.clear()
-            return
-
-        xy = self._mmc.getLoadedDevicesOfType(DeviceType.XYStageDevice)
-        z = self._mmc.getFocusDevice() or None
-        header = (
-            [POS, "X", "Y"]
-            + ([self._mmc.getFocusDevice()] if z else ["Z"])
-            + ["Autofocus", "Grid"]
-        )
-        self._table.setColumnCount(len(header))
+        header = [POS, "X", "Y", self._mmc.getFocusDevice() or "Z", "Autofocus", "Grid"]
+        self._table.setColumnCount(6)
         self._table.setHorizontalHeaderLabels(header)
 
-        # hide columns if no XY and/or Z stage
-        if not xy:
-            self._table.setColumnHidden(X, True)
-            self._table.setColumnHidden(Y, True)
-        if not z:
-            self._table.setColumnHidden(Z, True)
-        if not xy and not z:
-            self._table.setColumnHidden(P, True)
-
-    def _on_autofocus_value_changed(self) -> None:
+    def _on_af_wdg_changed(self) -> None:
         self._table.setColumnHidden(AF, not self._use_af())
         if z_device := self._get_af_device():
             self._table.setHorizontalHeaderItem(AF, QTableWidgetItem(z_device))
-
         # if the signal is sent from the autofocus checkbox, do not delete cell widgets
-        if not isinstance(self.sender().sender(), QCheckBox):
-            # remove cell widgets in autofocus column
-            for r in range(self._table.rowCount()):
-                self._table.removeCellWidget(r, AF)
+        if isinstance(self.sender(), QCheckBox):
+            return
+        # remove cell widgets in autofocus column
+        for r in range(self._table.rowCount()):
+            self._table.removeCellWidget(r, AF)
 
     def _on_advanced_toggled(self, state: bool) -> None:
         self._table.setColumnHidden(GRID, not state)
 
         if not state:
             for v in self.value():
                 if v.get("sequence") and v.get("sequence").get("grid_plan"):  # type: ignore  # noqa E501
@@ -353,15 +315,15 @@
         self.go_button.setEnabled(len(rows) == 1)
         self.remove_button.setEnabled(len(rows) >= 1)
 
         self.replace_button.setEnabled(len(rows) == 1)
         if len(rows) == 1:
             item = self._table.item(next(iter(rows)), 0)
             grid_role = item.data(self.GRID_ROLE) if item else None
-            if grid_role and isinstance(get_grid_type(grid_role), GridFromEdges):
+            if grid_role and isinstance(cast_grid_plan(grid_role), GridFromEdges):
                 self.replace_button.setEnabled(False)
 
     def _add_position(self) -> None:
         if hasattr(self, "_grid_dialog"):
             self._grid_dialog.close()  # type: ignore
 
         name = f"Pos{self._table.rowCount():03d}"
@@ -384,16 +346,16 @@
         name: str | None,
         xpos: float | None,
         ypos: float | None,
         zpos: float | None,
         z_pos_autofocus: float | None,
         row: int | None = None,
     ) -> None:
-        if not self._mmc.getXYStageDevice() and not self._mmc.getFocusDevice():
-            raise ValueError("No XY and Z Stage devices selected.")
+        # if not self._mmc.getXYStageDevice() and not self._mmc.getFocusDevice():
+        #     return
 
         if row is None:
             row = self._add_position_row()
 
         self._add_table_item(name, row, P)
         self._add_table_value(xpos, row, X)
         self._add_table_value(ypos, row, Y)
@@ -438,15 +400,15 @@
         wdg.setLayout(layout)
         add_grid = QPushButton()
         add_grid.setIcon(icon(MDI6.plus_thick, color=(0, 255, 0)))
         add_grid.setIconSize(QSize(25, 25))
         add_grid.setFixedHeight(25)
         add_grid.setSizePolicy(QSizePolicy.Policy.Fixed, QSizePolicy.Policy.Fixed)
         add_grid.setContextMenuPolicy(Qt.CustomContextMenu)
-        # for righ-click menu
+        # for right-click menu
         add_grid.customContextMenuRequested.connect(self._show_apply_to_all_menu)
         add_grid.clicked.connect(self._show_grid_widget)
         remove_grid = QPushButton()
         remove_grid.setIcon(icon(MDI6.close_thick, color="magenta"))
         remove_grid.setIconSize(QSize(25, 25))
         remove_grid.setFixedHeight(25)
         remove_grid.setSizePolicy(QSizePolicy.Policy.Fixed, QSizePolicy.Policy.Fixed)
@@ -492,15 +454,15 @@
         if item.data(self.GRID_ROLE):
             self._grid_wdg.set_state(item.data(self.GRID_ROLE))
 
         self._grid_dialog.show()
 
     def _add_grid_plan(self, grid: dict, row: int | None = None) -> None:
         # sourcery skip: extract-method
-        grid_type = get_grid_type(grid)
+        grid_type = cast_grid_plan(grid)
 
         if grid_type is None or row is None:
             return
 
         self._table.item(row, P).setData(self.GRID_ROLE, grid)
         self._table.item(row, P).setToolTip(self._create_tooltip(grid))
 
@@ -519,15 +481,15 @@
             self._add_table_value(first_pos.x, row, X)
             self._add_table_value(first_pos.y, row, Y)
 
         self._enable_button()
         self.valueChanged.emit()
 
     def _create_tooltip(self, grid: dict) -> str:
-        grid_type = get_grid_type(grid)
+        grid_type = cast_grid_plan(grid)
 
         if grid_type is None:
             return ""
 
         tooltip: dict[str, Any] = {}
         if isinstance(grid_type, GridRelative):
             tooltip["rows"] = grid["rows"]
@@ -556,15 +518,15 @@
         btn = cast(QPushButton, self.sender())
         row = self._table.indexAt(btn.parent().pos()).row()
         grid_role = self._table.item(row, P).data(self.GRID_ROLE)
 
         # return if not grid or if absolute grid_plan
         if not grid_role:
             return
-        if isinstance(get_grid_type(grid_role), GridFromEdges):
+        if isinstance(cast_grid_plan(grid_role), GridFromEdges):
             return
 
         # define where the menu appear on click
         parentPosition = btn.mapToGlobal(QPoint(0, 0))
         menuPosition = parentPosition + QPos
 
         popMenu = QMenu(self)
@@ -673,28 +635,30 @@
         """
         if not self._table.rowCount():
             return []
 
         values: list = []
 
         for row in range(self._table.rowCount()):
-            grid_role = self._table.item(row, P).data(self.GRID_ROLE)
+            item = cast("QTableWidgetItem", self._table.item(row, P))
+            grid_role = item.data(self.GRID_ROLE)
             af_plan = self._get_autofocus_plan(row)
-
-            value = {
-                "name": self._table.item(row, P).text(),
+            value: PositionDict = {
+                "name": item.text(),
                 "x": self._get_table_value(row, X),
                 "y": self._get_table_value(row, Y),
                 "z": self._get_table_value(row, Z),
-                "sequence": {} if grid_role or af_plan else None,
             }
+            sequence = {}
             if grid_role:
-                value["sequence"]["grid_plan"] = grid_role
+                grid_role.update(fov_kwargs(self._mmc))
+                sequence["grid_plan"] = grid_role
             if af_plan:
-                value["sequence"]["autofocus_plan"] = af_plan
+                sequence["autofocus_plan"] = af_plan
+            value["sequence"] = sequence or None
 
             values.append(value)
 
         return values
 
     def _get_autofocus_plan(self, row: int) -> dict[str, Any] | None:
         """Return the autofocus plan for the specified row."""
@@ -719,17 +683,14 @@
         clear : bool
             By default True. If True, the current positions list is cleared before the
             specified one is added.
         """
         if not isinstance(positions, Sequence):
             raise TypeError("The 'positions' arguments has to be a 'Sequence' type.")
 
-        if not self._mmc.getXYStageDevice() and not self._mmc.getFocusDevice():
-            raise ValueError("No XY and Z Stage devices loaded.")
-
         # variables used for autofocus devaice name check
         rows = set(range(self._table.rowCount()))
         z_af_devicies = set()
 
         with signals_blocked(self):
             if clear:
                 self.clear()
@@ -746,16 +707,16 @@
                 z_af_pos: float | None = None
                 grid_plan = None
 
                 if pos_seq := position.get("sequence"):
                     if isinstance(pos_seq, MDASequence):
                         if pos_seq.grid_plan:
                             grid_plan = pos_seq.grid_plan.dict()
-                        if isinstance(pos_seq.autofocus_plan, AxesBasedAF):  # type: ignore  # noqa
-                            autofocus = pos_seq.autofocus_plan.dict()  # type: ignore
+                        if isinstance(pos_seq.autofocus_plan, AxesBasedAF):
+                            autofocus = pos_seq.autofocus_plan.dict()
                     else:
                         grid_plan = pos_seq.get("grid_plan", None)
                         autofocus = pos_seq.get("autofocus_plan")
 
                     # add autofocus position if autofocus is used
                     if autofocus:
                         af_device = autofocus.get("autofocus_device_name", None)
```

### Comparing `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_mda/_time_plan_widget.py` & `pymmcore_widgets-0.4.1/src/pymmcore_widgets/_mda/_time_plan_widget.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 from __future__ import annotations
 
 import warnings
 from datetime import timedelta
 from typing import TYPE_CHECKING, cast
 
-from fonticon_mdi6 import MDI6
 from pymmcore_plus import CMMCorePlus
-from qtpy.QtCore import QSize, Qt, Signal
-from qtpy.QtGui import QIcon
+from qtpy.QtCore import Qt, Signal
 from qtpy.QtWidgets import (
     QAbstractSpinBox,
     QDoubleSpinBox,
     QGridLayout,
-    QHBoxLayout,
-    QLabel,
     QPushButton,
     QSizePolicy,
     QSpacerItem,
     QSpinBox,
     QTableWidget,
     QVBoxLayout,
     QWidget,
 )
-from superqt import QQuantity, fonticon
+from superqt import QQuantity
 from superqt.utils import signals_blocked
 from useq import MDASequence, MultiPhaseTimePlan, TIntervalLoops
 
 if TYPE_CHECKING:
     from typing_extensions import TypedDict
 
     class TimeDict(TypedDict, total=False):
@@ -61,15 +57,14 @@
         Optional [`pymmcore_plus.CMMCorePlus`][] micromanager core.
         By default, None. If not specified, the widget will use the active
         (or create a new)
         [`CMMCorePlus.instance`][pymmcore_plus.core._mmcore_plus.CMMCorePlus.instance].
     """
 
     valueChanged = Signal()
-    _warning_widget: QWidget
 
     def __init__(
         self,
         parent: QWidget | None = None,
         *,
         mmcore: CMMCorePlus | None = None,
     ) -> None:
@@ -120,37 +115,14 @@
         layout_buttons.addWidget(self._add_button)
         layout_buttons.addWidget(self._remove_button)
         layout_buttons.addWidget(self._clear_button)
         layout_buttons.addItem(spacer)
 
         group_layout.addWidget(buttons_wdg, 0, 1)
 
-        # warning Icon (exclamation mark)
-        self._warning_icon = QLabel()
-        self.setWarningIcon(MDI6.exclamation_thick)
-        self._warning_icon.setAlignment(Qt.AlignmentFlag.AlignLeft)
-        self._warning_icon.setSizePolicy(
-            QSizePolicy.Policy.Fixed, QSizePolicy.Policy.Fixed
-        )
-        # warning message
-        self._warning_msg = QLabel()
-        self.setWarningMessage("Interval shorter than acquisition time per timepoint.")
-        # warning widget (icon + message)
-        self._warning_widget = QWidget()
-        _warning_layout = QHBoxLayout()
-        _warning_layout.setSpacing(0)
-        _warning_layout.setContentsMargins(0, 0, 0, 0)
-        self._warning_widget.setLayout(_warning_layout)
-        _warning_layout.addWidget(self._warning_icon)
-        _warning_layout.addWidget(self._warning_msg)
-        self._warning_widget.setStyleSheet("color:magenta")
-        self._warning_widget.hide()
-
-        group_layout.addWidget(self._warning_widget, 1, 0, 1, 2)
-
         self._mmc.events.systemConfigurationLoaded.connect(self._clear)
 
         self.destroyed.connect(self._disconnect)
 
     def _create_new_row(
         self,
         interval: timedelta | None = None,
@@ -203,30 +175,14 @@
     def _clear(self) -> None:
         """Clear the time table."""
         if self._table.rowCount():
             self._table.clearContents()
             self._table.setRowCount(0)
         self.valueChanged.emit()
 
-    def setWarningMessage(self, msg: str) -> None:
-        """Set the text of the warning message."""
-        self._warning_msg.setText(msg)
-
-    def setWarningIcon(self, icon: str | QIcon) -> None:
-        """Set the icon of the warning message."""
-        if isinstance(icon, str):
-            _icon: QIcon = fonticon.icon(MDI6.exclamation_thick, color="magenta")
-        else:
-            _icon = icon
-        self._warning_icon.setPixmap(_icon.pixmap(QSize(30, 30)))
-
-    def setWarningVisible(self, visible: bool = True) -> None:
-        """Set the visibility of the warning message."""
-        self._warning_widget.setVisible(visible)
-
     def value(self) -> MultiPhaseTimeDict:
         """Return the current time plan as a dictionary.
 
         Note that the output will match the [useq-schema
         MultiPhaseTimePlan specifications](
         https://pymmcore-plus.github.io/useq-schema/schema/axes/#useq.MultiPhaseTimePlan
         ).
```

### Comparing `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_mda/_zstack_widget.py` & `pymmcore_widgets-0.4.1/src/pymmcore_widgets/_mda/_zstack_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, cast
 
+import useq
 from pymmcore_plus import CMMCorePlus
 from qtpy.QtCore import Qt, Signal
 from qtpy.QtWidgets import (
     QAbstractSpinBox,
     QDoubleSpinBox,
     QGridLayout,
     QGroupBox,
@@ -221,15 +222,15 @@
     mmcore : CMMCorePlus | None
         Optional [`pymmcore_plus.CMMCorePlus`][] micromanager core.
         By default, None. If not specified, the widget will use the active
         (or create a new)
         [`CMMCorePlus.instance`][pymmcore_plus.core._mmcore_plus.CMMCorePlus.instance].
     """
 
-    valueChanged = Signal(dict)
+    valueChanged = Signal(object)
 
     _MAX_STEP = 100000
     _NIMG_PREFIX = "Number of Images:"
 
     def __init__(
         self,
         parent: QWidget | None = None,
@@ -291,23 +292,29 @@
             self._update_and_emit()
 
     def _update_and_emit(self) -> None:
         """Update the number of images readout and emit the valueChanged signal."""
         self.n_images_label.setText(f"{self._NIMG_PREFIX} {self.n_images()}")
         self.valueChanged.emit(self.value())
 
-    def value(self) -> dict:
-        """Return the current z-stack settings as a dictionary.
+    def value(self) -> useq.ZRangeAround | useq.ZAboveBelow | useq.ZTopBottom:
+        """Return the current settings as a useq Z Plan.
 
         Note that the output will match one of the [useq-schema Z Plan
         specifications](https://pymmcore-plus.github.io/useq-schema/schema/axes/#z-plans).
         """
         value = cast("ZPicker", self._zmode_tabs.currentWidget()).value()
         value["step"] = self._zstep_spinbox.value()
-        return value
+        if "range" in value:
+            return useq.ZRangeAround(**value)
+        elif "above" in value:
+            return useq.ZAboveBelow(**value)
+        elif "top" in value:
+            return useq.ZTopBottom(**value)
+        raise ValueError(f"Unexpected value: {value}")  # pragma: no cover
 
     def n_images(self) -> int:
         """Return the current number of images in the z-stack."""
         step = self._zstep_spinbox.value()
         _range = cast("ZPicker", self._zmode_tabs.currentWidget()).z_range()
         return int(round((_range / step) + 1))
```

### Comparing `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_objective_widget.py` & `pymmcore_widgets-0.4.1/src/pymmcore_widgets/_objective_widget.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_pixel_size_widget.py` & `pymmcore_widgets-0.4.1/src/pymmcore_widgets/_pixel_size_widget.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_presets_widget.py` & `pymmcore_widgets-0.4.1/src/pymmcore_widgets/_presets_widget.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_properties_widget.py` & `pymmcore_widgets-0.4.1/src/pymmcore_widgets/_properties_widget.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """Whereas PropertyWidget shows a single property, PropertiesWidget is a container.
 
 It shows a number of properties, filtered by a given set of tags.
 """
 from __future__ import annotations
 
-import re
-from typing import Iterable, cast
+from typing import TYPE_CHECKING, Iterable, cast
 
 from pymmcore_plus import CMMCorePlus
 from qtpy.QtWidgets import QGridLayout, QLabel, QWidget
 
 from ._property_widget import PropertyWidget
 
+if TYPE_CHECKING:
+    import re
+
 
 class PropertiesWidget(QWidget):
     """Convenience container to control a specific set of PropertyWidgets.
 
     Properties can be filtered by a number of criteria, which are passed to
     [`CMMCorePlus.iterProperties`][pymmcore_plus.core._mmcore_plus.CMMCorePlus.iterProperties].
```

### Comparing `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_property_browser.py` & `pymmcore_widgets-0.4.1/src/pymmcore_widgets/_property_browser.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_property_widget.py` & `pymmcore_widgets-0.4.1/src/pymmcore_widgets/_property_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,31 +79,31 @@
             self.setDecimals(dec)
         return super().setValue(  # type: ignore [no-any-return]
             _stretch_range_to_contain(self, float(v))
         )
 
 
 class _RangedMixin:
-    _cast: type[int] | type[float] = float
+    type_cast: type[int] | type[float] = float
 
     # prefer horizontal orientation
     def __init__(  # type: ignore
         self, orientation=Qt.Orientation.Horizontal, parent: QWidget | None = None
     ) -> None:
         super().__init__(orientation, parent)  # type: ignore
 
     def setValue(self, v: float) -> None:
-        val = _stretch_range_to_contain(self, self._cast(v))
+        val = _stretch_range_to_contain(self, self.type_cast(v))
         return super().setValue(val)  # type: ignore
 
 
 class RangedIntegerWidget(_RangedMixin, QLabeledSlider):
     """Slider suited to managing ranged integer values."""
 
-    _cast = int
+    type_cast = int
 
 
 class RangedFloatWidget(_RangedMixin, QLabeledDoubleSlider):
     """Slider suited to managing ranged float values."""
 
 
 class IntBoolWidget(QCheckBox):
@@ -239,16 +239,16 @@
         if not mmcore.hasPropertyLimits(dev, prop):
             return IntegerWidget() if ptype is PropertyType.Integer else FloatWidget()
         wdg = (
             RangedIntegerWidget()
             if ptype is PropertyType.Integer
             else RangedFloatWidget()
         )
-        wdg.setMinimum(wdg._cast(mmcore.getPropertyLowerLimit(dev, prop)))
-        wdg.setMaximum(wdg._cast(mmcore.getPropertyUpperLimit(dev, prop)))
+        wdg.setMinimum(wdg.type_cast(mmcore.getPropertyLowerLimit(dev, prop)))
+        wdg.setMaximum(wdg.type_cast(mmcore.getPropertyUpperLimit(dev, prop)))
         return wdg
     return cast(PPropValueWidget, StringWidget())
 
 
 # -----------------------------------------------------------------------
 # Main public facing QWidget.
 # -----------------------------------------------------------------------
@@ -295,49 +295,54 @@
         if device_label not in self._mmc.getLoadedDevices():
             raise ValueError(f"Device not loaded: {device_label!r}")
 
         if not self._mmc.hasProperty(device_label, prop_name):
             names = self._mmc.getDevicePropertyNames(device_label)
             raise ValueError(
                 f"Device {device_label!r} has no property {prop_name!r}. "
-                f"Availble property names include: {names}"
+                f"Available property names include: {names}"
             )
 
         self._updates_core: bool = True  # whether to update the core on value change
         self._device_label = device_label
         self._prop_name = prop_name
 
         self.setLayout(QHBoxLayout())
         self.layout().setContentsMargins(0, 0, 0, 0)
 
         # Create the widget based on property type and allowed choices
         self._value_widget = _creat_prop_widget(self._mmc, device_label, prop_name)
         # set current value from core
-        self._value_widget.setValue(self._mmc.getProperty(device_label, prop_name))
+        self._try_update_from_core()
+
         self._mmc.events.propertyChanged.connect(self._on_core_change)
         self._value_widget.valueChanged.connect(self._on_value_widget_change)
 
         self.layout().addWidget(cast(QWidget, self._value_widget))
         self.destroyed.connect(self._disconnect)
 
+    def _try_update_from_core(self) -> None:
+        # set current value from core, ignoring errors
+        with contextlib.suppress(RuntimeError, ValueError):
+            self._value_widget.setValue(self._mmc.getProperty(*self._dp))
+
     # connect events and queue for disconnection on widget destroyed
     def _on_core_change(self, dev_label: str, prop_name: str, new_val: Any) -> None:
         if dev_label == self._device_label and prop_name == self._prop_name:
             with utils.signals_blocked(self._value_widget):
                 self._value_widget.setValue(new_val)
 
     def _on_value_widget_change(self, value: Any) -> None:
         if not self._updates_core:
             return
         try:
             self._mmc.setProperty(self._device_label, self._prop_name, value)
         except (RuntimeError, ValueError):
             # if there's an error when updating mmcore, reset widget value to mmcore
-            real_value = self._mmc.getProperty(self._device_label, self._prop_name)
-            self._value_widget.setValue(real_value)
+            self._try_update_from_core()
 
     def _disconnect(self) -> None:
         with contextlib.suppress(RuntimeError):
             self._mmc.events.propertyChanged.disconnect(self._on_core_change)
 
     def value(self) -> Any:
         """Get value.
@@ -377,15 +382,15 @@
     def refresh(self) -> None:
         """Update the value of the widget from mmcore.
 
         (If all goes well this shouldn't be necessary, but if a propertyChanged
         event is missed, this can be used).
         """
         with utils.signals_blocked(self._value_widget):
-            self._value_widget.setValue(self._mmc.getProperty(*self._dp))
+            self._try_update_from_core()
 
     def propertyType(self) -> PropertyType:
         """Return property type."""
         return self._mmc.getPropertyType(*self._dp)
 
     def deviceType(self) -> DeviceType:
         """Return property type."""
```

### Comparing `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_shutter_widget.py` & `pymmcore_widgets-0.4.1/src/pymmcore_widgets/_shutter_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         self.destroyed.connect(self._disconnect)
 
     @property
     def icon_open(self) -> str:
         """
         Set the icon of the QPushButton when the shutter is open.
 
-        The icon_open.setter icon string should be any key recognizeable as
+        The icon_open.setter icon string should be any key recognizable as
         a superqt fonticon (e.g. mdi6.abacus).
         Default = MDI6.hexagon_outline (https://github.com/templarian/MaterialDesign).
         Note that MDI6 is installed by default, you must install other fonts
         if you want to use them.
         """
         return self._icon_open
 
@@ -102,15 +102,15 @@
         self._icon_open = icon_o
 
     @property
     def icon_closed(self) -> str:
         """
         Set the icon of the QPushButton when the shutter is closed.
 
-        The icon_closed.setter icon string should be any key recognizeable as
+        The icon_closed.setter icon string should be any key recognizable as
         a superqt fonticon (e.g. mdi6.abacus).
         Default = MDI6.hexagon_slice_6 (https://github.com/templarian/MaterialDesign).
         Note that MDI6 is installed by default, you must install other fonts
         if you want to use them.
         """
         return self._icon_closed
```

### Comparing `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_snap_button_widget.py` & `pymmcore_widgets-0.4.1/src/pymmcore_widgets/_snap_button_widget.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_stage_widget.py` & `pymmcore_widgets-0.4.1/src/pymmcore_widgets/_stage_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,22 +127,22 @@
         self._step.setButtonSymbols(QSpinBox.ButtonSymbols.NoButtons)
         self._step.setAlignment(AlignCenter)
 
         self._btns = QWidget()
         self._btns.setLayout(QGridLayout())
         self._btns.layout().setContentsMargins(0, 0, 0, 0)
         self._btns.layout().setSpacing(0)
-        for glpyh, (row, col, *_) in self.BTNS.items():
+        for glyph, (row, col, *_) in self.BTNS.items():
             btn = QPushButton()
             btn.setAutoRepeat(True)
             btn.setFlat(True)
             btn.setFixedSize(self.BTN_SIZE, self.BTN_SIZE)
             btn.setFocusPolicy(Qt.FocusPolicy.NoFocus)
             btn.setCursor(Qt.CursorShape.PointingHandCursor)
-            setTextIcon(btn, glpyh)
+            setTextIcon(btn, glyph)
             btn.clicked.connect(self._on_click)
             self._btns.layout().addWidget(btn, row, col, AlignCenter)
 
         self._btns.layout().addWidget(self._step, 3, 3, AlignCenter)
         self._set_visible_levels(self._levels)  # type: ignore
         self._set_xy_visible()
         self._update_ttips()
```

### Comparing `pymmcore-widgets-0.4.0/src/pymmcore_widgets/_util.py` & `pymmcore_widgets-0.4.1/src/pymmcore_widgets/_util.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from __future__ import annotations
 
-from datetime import timedelta
 from typing import ContextManager, Sequence
 
+import useq
 from pymmcore_plus import CMMCorePlus
 from pymmcore_plus.core.events import CMMCoreSignaler, PCoreSignaler
 from qtpy.QtWidgets import (
     QComboBox,
     QDialog,
     QDialogButtonBox,
     QLabel,
     QVBoxLayout,
     QWidget,
 )
 from superqt.utils import signals_blocked
-from useq import AnyGridPlan, MDASequence
 
 
 class ComboMessageBox(QDialog):
     """Dialog that presents a combo box of `items`."""
 
     def __init__(
         self,
@@ -82,57 +81,30 @@
     elif candidates:
         dialog = ComboMessageBox(candidates, "Select Objective Device:", parent=parent)
         if dialog.exec_() == dialog.DialogCode.Accepted:
             return dialog.currentText()
     return None
 
 
-def _select_output_unit(duration: float) -> tuple[float, str]:
-    if duration < 1.0:
-        return duration * 1000, "ms"
-    elif duration < 60.0:
-        return duration, "sec"
-    elif duration < 3600.0:
-        return duration / 60, "min"
-    else:
-        return duration / 3600, "hours"
-
-
 def block_core(mmcore_events: CMMCoreSignaler | PCoreSignaler) -> ContextManager:
     """Block core signals."""
     if isinstance(mmcore_events, CMMCoreSignaler):
         return mmcore_events.blocked()  # type: ignore
     elif isinstance(mmcore_events, PCoreSignaler):
         return signals_blocked(mmcore_events)  # type: ignore
 
 
-def fmt_timedelta(time: timedelta) -> str:
-    """Take timedelta and return formatted string.
-
-    Examples
-    --------
-    >>> fmt_timedelta(timedelta(seconds=100))
-    '01 min  40 sec'
-    >>> fmt_timedelta(timedelta(minutes=320, seconds=2500))
-    '06 hours  01 min  40 sec'
-    """
-    d = "day" if time.days == 1 else "days"
-    _time = str(time).replace(f" {d}, ", ":") if time.days >= 1 else f"0:{time!s}"
-    out: list = []
-    keys = ["days", "hours", "min", "sec", "ms"]
-    for i, t in enumerate(_time.split(":")):
-        if i == 3:
-            s = t.split(".")
-            if len(s) == 2:
-                sec = f"{int(s[0]):02d} sec " if int(s[0]) > 0 else ""
-                ms = f"{int(s[1][:3]):03d} ms" if int(s[1][:3]) > 0 else ""
-                out.append(f"{sec}{ms}")
-            else:
-                out.append(f"{int(s[0]):02d} sec") if int(s[0]) > 0 else ""
-        else:
-            out.append(f"{int(float(t)):02d} {keys[i]}") if int(float(t)) > 0 else ""
-    return "  ".join(out)
+def cast_grid_plan(grid: dict | useq.AnyGridPlan) -> useq.AnyGridPlan | None:
+    """Get the grid type from the grid_plan."""
+    if not grid:
+        return None
+    if isinstance(grid, dict):
+        return useq.MDASequence(grid_plan=grid).grid_plan
+    return grid
 
 
-def get_grid_type(grid: dict) -> AnyGridPlan | None:
-    """Get the grid type from the grid_plan."""
-    return MDASequence(grid_plan=grid).grid_plan
+def fov_kwargs(core: CMMCorePlus) -> dict:
+    """Return image width and height in micron to be used for the grid plan."""
+    if px := core.getPixelSizeUm():
+        *_, width, height = core.getROI()
+        return {"fov_width": (width * px) or None, "fov_height": (height * px) or None}
+    return {}
```

### Comparing `pymmcore-widgets-0.4.0/tests/conftest.py` & `pymmcore_widgets-0.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.4.0/tests/test_camera_roi_widget.py` & `pymmcore_widgets-0.4.1/tests/test_camera_roi_widget.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.4.0/tests/test_channel_group_widget.py` & `pymmcore_widgets-0.4.1/tests/test_channel_group_widget.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.4.0/tests/test_channel_table_widget.py` & `pymmcore_widgets-0.4.1/tests/test_channel_table_widget.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
-from qtpy.QtWidgets import QComboBox
+import useq
 
 from pymmcore_widgets._mda import ChannelTable
 
 if TYPE_CHECKING:
     from pytestqt.qtbot import QtBot
+    from qtpy.QtWidgets import QComboBox
 
 
 def _values(combo: QComboBox) -> list:
     return [combo.itemText(i) for i in range(combo.count())]
 
 
 def test_channel_table_widget(qtbot: QtBot):
@@ -53,51 +54,23 @@
         ct._mmc.deleteConfigGroup("Camera")
     assert ct._table.rowCount() == 1
 
     ct._clear_button.click()
     assert not ct._table.rowCount()
 
 
-def test_set_get_state(qtbot: QtBot):
+def test_set_get_state(qtbot: QtBot) -> None:
     ct = ChannelTable(channel_group="Camera")
     qtbot.addWidget(ct)
 
     state = [
-        {
-            "config": "Cy5",
-            "group": "Channel",
-            "exposure": 100.0,
-            "z_offset": 0.0,
-            "do_stack": True,
-            "acquire_every": 1,
-        },
-        {
-            "config": "DAPI",
-            "group": "Channel",
-            "exposure": 100.0,
-            "z_offset": 10.0,
-            "do_stack": True,
-            "acquire_every": 1,
-        },
-        {
-            "config": "HighRes",
-            "group": "Camera",
-            "exposure": 100.0,
-            "z_offset": 0.0,
-            "do_stack": False,
-            "acquire_every": 1,
-        },
-        {
-            "config": "Cy5",
-            "group": "Channel",
-            "exposure": 100.0,
-            "z_offset": 0.0,
-            "do_stack": True,
-            "acquire_every": 2,
-        },
+        useq.Channel(config="Cy5", exposure=100.0),
+        useq.Channel(config="DAPI", exposure=100.0, z_offset=10.0),
+        useq.Channel(config="HighRes", group="Camera", exposure=100.0, do_stack=False),
+        useq.Channel(config="Cy5", exposure=100.0, acquire_every=2),
     ]
 
     assert not ct._advanced_cbox.isChecked()
     ct.set_state(state)
 
     assert ct._table.rowCount() == 4
     assert ct._table.cellWidget(0, 0).currentText() == "Cy5"
```

### Comparing `pymmcore-widgets-0.4.0/tests/test_channel_widget.py` & `pymmcore_widgets-0.4.1/tests/test_channel_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
-from pymmcore_plus import CMMCorePlus
 from qtpy.QtWidgets import QComboBox
 
 from pymmcore_widgets._channel_widget import ChannelWidget
 from pymmcore_widgets._presets_widget import PresetsWidget
 from pymmcore_widgets._util import block_core
 
 if TYPE_CHECKING:
+    from pymmcore_plus import CMMCorePlus
     from pytestqt.qtbot import QtBot
 
 
 def test_channel_widget(qtbot: QtBot, global_mmcore: CMMCorePlus):
     wdg = ChannelWidget()
     qtbot.addWidget(wdg)
```

### Comparing `pymmcore-widgets-0.4.0/tests/test_combo_message_box_widget.py` & `pymmcore_widgets-0.4.1/tests/test_combo_message_box_widget.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.4.0/tests/test_config.cfg` & `pymmcore_widgets-0.4.1/tests/test_config.cfg`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.4.0/tests/test_core_state.py` & `pymmcore_widgets-0.4.1/tests/test_core_state.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from __future__ import annotations
 
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
 import pytest
-from pymmcore_plus import CMMCorePlus
-from qtpy.QtWidgets import QWidget
 
 import pymmcore_widgets as pmmw
 
+if TYPE_CHECKING:
+    from pymmcore_plus import CMMCorePlus
+    from qtpy.QtWidgets import QWidget
+
 ALL_WIDGETS: dict[type[QWidget], dict[str, Any]] = {
     pmmw.CameraRoiWidget: {},
     pmmw.ChannelGroupWidget: {},
     pmmw.ChannelTable: {},
     pmmw.ChannelWidget: {},
     pmmw.ConfigurationWidget: {},
     pmmw.DefaultCameraExposureWidget: {},
```

### Comparing `pymmcore-widgets-0.4.0/tests/test_device_widget.py` & `pymmcore_widgets-0.4.1/tests/test_device_widget.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.4.0/tests/test_exposure_widget.py` & `pymmcore_widgets-0.4.1/tests/test_exposure_widget.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 import pytest
-from pymmcore_plus import CMMCorePlus
 
 from pymmcore_widgets import DefaultCameraExposureWidget
 
 if TYPE_CHECKING:
+    from pymmcore_plus import CMMCorePlus
     from pytestqt.qtbot import QtBot
 
 
 def test_exposure_widget(qtbot: QtBot, global_mmcore: CMMCorePlus):
     global_mmcore.setExposure(15)
     wdg = DefaultCameraExposureWidget(mmcore=global_mmcore)
     qtbot.addWidget(wdg)
```

### Comparing `pymmcore-widgets-0.4.0/tests/test_grid_widget.py` & `pymmcore_widgets-0.4.1/tests/test_grid_widget.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 from unittest.mock import Mock, call
 
-from pymmcore_plus import CMMCorePlus
-from useq import GridFromEdges, GridRelative
-from useq._grid import OrderMode, RelativeTo
+import useq
 
 from pymmcore_widgets._mda import GridWidget
 
 if TYPE_CHECKING:
+    from pymmcore_plus import CMMCorePlus
     from pytestqt.qtbot import QtBot
 
 
 def test_mda_grid(qtbot: QtBot, global_mmcore: CMMCorePlus):
     grid_wdg = GridWidget()
     qtbot.addWidget(grid_wdg)
 
@@ -40,15 +39,17 @@
     grid_wdg.valueChanged.connect(mock)
 
     grid_wdg._emit_grid_positions()
 
     mock.assert_has_calls([call(grid_wdg.value())])
 
     grid_wdg.set_state(
-        GridFromEdges(top=256, bottom=-256, left=-256, right=256, overlap=(0.0, 50.0))
+        useq.GridFromEdges(
+            top=256, bottom=-256, left=-256, right=256, overlap=(0.0, 50.0)
+        )
     )
 
     assert (
         grid_wdg.info_lbl.text()
         == "Height: 0.768 mm    Width: 0.768 mm    (Rows: 3    Columns: 3)"
     )
 
@@ -57,107 +58,63 @@
     mock.assert_has_calls([call(grid_wdg.value())])
 
 
 def test_grid_set_and_get_state(qtbot: QtBot, global_mmcore: CMMCorePlus):
     grid_wdg = GridWidget()
     qtbot.addWidget(grid_wdg)
 
-    grid_wdg.set_state(
-        {"rows": 3, "columns": 3, "overlap": 15.0, "relative_to": "top_left"}
+    grid_rel = useq.GridRelative(
+        rows=3, columns=3, relative_to="top_left", overlap=15.0, mode="row_wise_snake"
     )
-    assert grid_wdg.value() == {
-        "overlap": (15.0, 15.0),
-        "mode": "row_wise_snake",
-        "rows": 3,
-        "columns": 3,
-        "relative_to": "top_left",
-    }
-    assert grid_wdg.tab.currentIndex() == 0
 
-    # using RelativeTo enum
-    grid_wdg.set_state(
-        {"rows": 3, "columns": 3, "overlap": 15.0, "relative_to": RelativeTo.top_left}
-    )
-    assert grid_wdg.value() == {
-        "overlap": (15.0, 15.0),
-        "mode": "row_wise_snake",
-        "rows": 3,
-        "columns": 3,
-        "relative_to": "top_left",
-    }
+    grid_wdg.set_state(grid_rel.dict())
+    assert grid_wdg.value().replace(fov_width=None, fov_height=None) == grid_rel
     assert grid_wdg.tab.currentIndex() == 0
 
     # using GridPlan (and not dict)
-    grid_wdg.set_state(
-        GridFromEdges(top=512, bottom=-512, left=-512, right=512, mode="spiral")
+    grid_abs = useq.GridFromEdges(
+        top=512, bottom=-512, left=-512, right=512, mode="spiral"
     )
-    assert grid_wdg.value() == {
-        "overlap": (0.0, 0.0),
-        "mode": "spiral",
-        "top": 512.0,
-        "bottom": -512.0,
-        "left": -512.0,
-        "right": 512.0,
-    }
+    grid_wdg.set_state(grid_abs)
+
+    assert grid_wdg.value().replace(fov_width=None, fov_height=None) == grid_abs
     assert grid_wdg.tab.currentIndex() == 1
 
+    grid_abs2 = grid_abs.replace(mode="row_wise_snake", overlap=(10.0, 0.0))
     # using OrderMode enum
-    grid_wdg.set_state(
-        {
-            "overlap": (10.0, 0.0),
-            # "mode": "row_wise_snake",
-            "mode": OrderMode.row_wise_snake,
-            "top": 512.0,
-            "bottom": -512.0,
-            "left": -512.0,
-            "right": 512.0,
-        }
-    )
-    assert grid_wdg.value() == {
-        "overlap": (10.0, 0.0),
-        "mode": "row_wise_snake",
-        "top": 512.0,
-        "bottom": -512.0,
-        "left": -512.0,
-        "right": 512.0,
-    }
+    grid_wdg.set_state(grid_abs2.dict())
+    assert grid_wdg.value().replace(fov_width=None, fov_height=None) == grid_abs2
     assert grid_wdg.tab.currentIndex() == 1
 
 
 def test_grid_from_edges_set_button(qtbot: QtBot, global_mmcore: CMMCorePlus):
     grid_wdg = GridWidget()
     qtbot.addWidget(grid_wdg)
     mmc = global_mmcore
 
-    assert grid_wdg.tab.edges.value() == {
-        "top": 0.0,
-        "bottom": 0.0,
-        "left": 0.0,
-        "right": 0.0,
-    }
+    assert grid_wdg.tab.edges.value() == useq.GridFromEdges(
+        top=0.0, bottom=0.0, left=0.0, right=0.0
+    )
 
     mmc.setXYPosition(100.0, 200.0)
     grid_wdg.tab.edges.top.set_button.click()
     grid_wdg.tab.edges.left.set_button.click()
-    assert grid_wdg.tab.edges.value() == {
-        "top": 200.0,
-        "bottom": 0.0,
-        "left": 100.0,
-        "right": 0.0,
-    }
+    assert grid_wdg.tab.edges.value() == useq.GridFromEdges(
+        top=200.0, bottom=0.0, left=100.0, right=0.0
+    )
 
 
 def test_grid_on_px_size_changed(qtbot: QtBot, global_mmcore: CMMCorePlus):
     grid_wdg = GridWidget()
     qtbot.addWidget(grid_wdg)
     mmc = global_mmcore
 
     assert mmc.getProperty("Objective", "Label") == "Nikon 10X S Fluor"
     assert mmc.getPixelSizeUm() == 1.0
-    grid_wdg.set_state(GridRelative(rows=2, columns=2))
+    grid_wdg.set_state(useq.GridRelative(rows=2, columns=2))
     assert (
         grid_wdg.info_lbl.text()
         == "Height: 1.024 mm    Width: 1.024 mm    (Rows: 2    Columns: 2)"
     )
 
     with qtbot.waitSignal(mmc.events.pixelSizeChanged):
         mmc.setPixelSizeUm("Res10x", 0.5)
```

### Comparing `pymmcore-widgets-0.4.0/tests/test_group_preset_widget.py` & `pymmcore_widgets-0.4.1/tests/test_group_preset_widget.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.4.0/tests/test_image_preview.py` & `pymmcore_widgets-0.4.1/tests/test_image_preview.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.4.0/tests/test_live_button.py` & `pymmcore_widgets-0.4.1/tests/test_live_button.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.4.0/tests/test_load_system_cfg_widget.py` & `pymmcore_widgets-0.4.1/tests/test_load_system_cfg_widget.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.4.0/tests/test_mda_widget.py` & `pymmcore_widgets-0.4.1/tests/test_mda_widget.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 from __future__ import annotations
 
 import tempfile
 from pathlib import Path
-from typing import TYPE_CHECKING, cast
+from typing import TYPE_CHECKING
 from unittest.mock import MagicMock, patch
 
-from pymmcore_plus import CMMCorePlus
 from qtpy.QtWidgets import QFileDialog
 from useq import MDASequence
 
 from pymmcore_widgets._mda import MDAWidget
 
 if TYPE_CHECKING:
+    from pymmcore_plus import CMMCorePlus
     from pytestqt.qtbot import QtBot
-    from qtpy.QtWidgets import QSpinBox
-    from superqt import QQuantity
 
 
-def test_mda_widget_load_state(qtbot: QtBot):
+def test_mda_widget_load_state(qtbot: QtBot) -> None:
     wdg = MDAWidget(include_run_button=True)
     qtbot.addWidget(wdg)
     assert wdg.position_widget._table.rowCount() == 0
     assert wdg.channel_widget._table.rowCount() == 0
     assert not wdg.t_cbox.isChecked()
 
     wdg._enable_widgets(False)
@@ -58,15 +56,20 @@
             },
             {
                 "name": "Pos002",
                 "x": 111,
                 "y": 0,
                 "z": 15,
                 "sequence": {
-                    "grid_plan": {"rows": 2, "columns": 2},
+                    "grid_plan": {
+                        "rows": 2,
+                        "columns": 2,
+                        "fov_height": 512,
+                        "fov_width": 512,
+                    },
                     "autofocus_plan": {
                         "autofocus_device_name": "Z",
                         "axes": ("t", "p", "g"),
                         "autofocus_motor_offset": 10.0,
                     },
                 },
             },
@@ -75,23 +78,27 @@
                 "x": 1,
                 "y": 2,
                 "z": 3,
                 "sequence": {
                     "grid_plan": {
                         "rows": 2,
                         "columns": 2,
+                        "fov_height": 512,
+                        "fov_width": 512,
                         "mode": "row_wise_snake",
                         "overlap": (0.0, 0.0),
                     },
                 },
             },
         ),
         grid_plan={
             "rows": 1,
             "columns": 2,
+            "fov_height": 512,
+            "fov_width": 512,
             "mode": "row_wise_snake",
             "overlap": (0.0, 0.0),
         },
     )
     mocks = []
     for subcomponent in [
         wdg.time_widget,
@@ -168,77 +175,14 @@
     assert wdg.stack_widget.isEnabled()
     assert not wdg.grid_widget.isEnabled()
     assert not wdg.buttons_wdg.run_button.isHidden()
     assert wdg.buttons_wdg.pause_button.isHidden()
     assert wdg.buttons_wdg.cancel_button.isHidden()
 
 
-def test_gui_labels(qtbot: QtBot, global_mmcore: CMMCorePlus):
-    # sourcery skip: extract-duplicate-method
-    global_mmcore.setExposure(100)
-    wdg = MDAWidget(include_run_button=True)
-    qtbot.addWidget(wdg)
-    wdg.show()
-
-    wdg.ch_cbox.setChecked(True)
-    assert wdg.channel_widget._table.rowCount() == 0
-    wdg.channel_widget._add_button.click()
-    assert wdg.channel_widget._table.rowCount() == 1
-    assert wdg.channel_widget._table.cellWidget(0, 1).value() == 100.0
-
-    assert not wdg.t_cbox.isChecked()
-    wdg.t_cbox.setChecked(True)
-    wdg.time_widget._add_button.click()
-
-    txt = (
-        "Minimum total acquisition time: 100 ms"
-        "\nMinimum acquisition time per timepoint: 100 ms"
-    )
-    assert wdg.time_lbl._total_time_lbl.text() == txt
-    assert wdg.time_widget._warning_widget.isHidden()
-
-    assert wdg.t_cbox.isChecked()
-    interval = cast("QQuantity", wdg.time_widget._table.cellWidget(0, 0))
-    timepoint = cast("QSpinBox", wdg.time_widget._table.cellWidget(0, 1))
-    interval.setValue(1, "ms")
-    timepoint.setValue(2)
-
-    txt = (
-        "Minimum total acquisition time: 201 ms"
-        "\nMinimum acquisition time per timepoint: 100 ms"
-    )
-    assert wdg.time_lbl._total_time_lbl.text() == txt
-    assert not wdg.time_widget._warning_widget.isHidden()
-
-    wdg.channel_widget._add_button.click()
-    wdg.channel_widget._advanced_cbox.setChecked(True)
-    wdg.channel_widget._table.cellWidget(1, 4).setValue(2)
-    wdg.channel_widget._table.cellWidget(1, 1).setValue(100.0)
-    assert not wdg.time_widget._warning_widget.isHidden()
-    interval.setValue(200, "ms")
-    timepoint.setValue(4)
-    assert wdg.time_widget._warning_widget.isHidden()
-
-    txt = (
-        "Minimum total acquisition time: 01 sec 200 ms"
-        "\nMinimum acquisition time per timepoint: 100 ms"
-    )
-    assert wdg.time_lbl._total_time_lbl.text() == txt
-
-    wdg.time_widget._add_button.click()
-    timepoint = cast("QSpinBox", wdg.time_widget._table.cellWidget(1, 1))
-    timepoint.setValue(2)
-
-    txt = (
-        "Minimum total acquisition time: 02 sec 400 ms"
-        "\nMinimum acquisition time per timepoint: 100 ms"
-    )
-    assert wdg.time_lbl._total_time_lbl.text() == txt
-
-
 def test_enable_run_button(qtbot: QtBot, global_mmcore: CMMCorePlus):
     wdg = MDAWidget(include_run_button=True)
     qtbot.addWidget(wdg)
     wdg.show()
     mmc = global_mmcore
 
     assert mmc.getChannelGroup() == "Channel"
@@ -300,30 +244,61 @@
                 axis_order="tpgcz",
                 stage_positions=[
                     {
                         "x": 10,
                         "y": 20,
                         "z": 50,
                         "name": "test_name",
-                        "sequence": MDASequence(grid_plan={"rows": 2, "columns": 3}),
+                        "sequence": MDASequence(
+                            grid_plan={
+                                "rows": 2,
+                                "columns": 3,
+                                "fov_height": 512,
+                                "fov_width": 512,
+                            }
+                        ),
                     },
                 ],
                 channels=[
                     {"config": "Cy5", "exposure": 50},
                     {
                         "config": "DAPI",
                         "exposure": 100.0,
                         "do_stack": False,
                         "acquire_every": 3,
                     },
                 ],
                 time_plan=[{"interval": 3, "loops": 3}, {"interval": 5, "loops": 10}],
                 z_plan={"range": 1.0, "step": 0.5},
-                grid_plan={"rows": 2, "columns": 1},
+                grid_plan={
+                    "rows": 2,
+                    "columns": 1,
+                    "fov_height": 512,
+                    "fov_width": 512,
+                },
             )
             mda.set_state(seq)
 
             mda._save_sequence()
 
             with patch.object(QFileDialog, "getOpenFileName", _path):
                 mda._load_sequence()
                 assert mda.get_state() == seq
+
+
+def test_set_state_without_xystage(global_mmcore: CMMCorePlus, qtbot: QtBot):
+    mmc = global_mmcore
+    mmc.unloadDevice("XY")
+    mmc.unloadDevice("Z")
+    wdg = MDAWidget(include_run_button=True)
+    qtbot.addWidget(wdg)
+
+    p_table = wdg.position_widget._table
+    mda = MDASequence(stage_positions=[(10, 20, 30)])
+    wdg.set_state(mda)
+
+    assert p_table.rowCount() == 1
+    assert not mmc.getXYStageDevice()
+    assert not mmc.getFocusDevice()
+    assert wdg.get_state().stage_positions[0].x == 10
+    assert wdg.get_state().stage_positions[0].y == 20
+    assert wdg.get_state().stage_positions[0].z == 30
```

### Comparing `pymmcore-widgets-0.4.0/tests/test_objective_widget.py` & `pymmcore_widgets-0.4.1/tests/test_objective_widget.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 from unittest.mock import Mock, call, patch
 
 import pytest
-from pymmcore_plus import CMMCorePlus
 from qtpy.QtWidgets import QDialog
 
 from pymmcore_widgets._objective_widget import ObjectivesWidget
 from pymmcore_widgets._util import ComboMessageBox
 
 if TYPE_CHECKING:
+    from pymmcore_plus import CMMCorePlus
     from pytestqt.qtbot import QtBot
 
 
 def test_objective_widget_changes_objective(global_mmcore: CMMCorePlus, qtbot: QtBot):
     obj_wdg = ObjectivesWidget()
     qtbot.addWidget(obj_wdg)
```

### Comparing `pymmcore-widgets-0.4.0/tests/test_position_table_widget.py` & `pymmcore_widgets-0.4.1/tests/test_position_table_widget.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 import json
 import tempfile
 from pathlib import Path
 from typing import TYPE_CHECKING, Any
 from unittest.mock import patch
 
 import pytest
-from pymmcore_plus import CMMCorePlus
 from qtpy.QtWidgets import QFileDialog, QTableWidget
 
 from pymmcore_widgets._mda import PositionTable
 
 if TYPE_CHECKING:
+    from pymmcore_plus import CMMCorePlus
     from pytestqt.qtbot import QtBot
 
 
 P = 0
 X = 1
 Y = 2
 Z = 3
@@ -166,130 +166,139 @@
                 "top": 100.0,
             }
         },
     }
     return pos_1, pos_2, pos_3
 
 
+def _wdg_value_no_fov(wdg: PositionTable):
+    val = wdg.value()
+    for pos in val:
+        if "sequence" in pos and "grid_plan" in (pos["sequence"] or {}):
+            pos["sequence"]["grid_plan"].pop("fov_height")
+            pos["sequence"]["grid_plan"].pop("fov_width")
+    return val
+
+
 def test_relative_grid_position(
     global_mmcore: CMMCorePlus, qtbot: QtBot, pos: tuple[dict[str, Any], ...]
 ):
     pos_1, pos_2, _ = pos
 
-    p = PositionTable()
-    qtbot.addWidget(p)
+    pos_wdg = PositionTable()
+    qtbot.addWidget(pos_wdg)
 
     mmc = global_mmcore
-    tb = p._table
+    tb = pos_wdg._table
 
     assert not tb.rowCount()
 
     mmc.setXYPosition(100, 200)
-    p.add_button.click()
+    pos_wdg.add_button.click()
     assert tb.rowCount() == 1
     assert tb.isColumnHidden(GRID)
 
-    p._advanced_cbox.setChecked(True)
-    assert p._warn_icon.isHidden()
+    pos_wdg._advanced_cbox.setChecked(True)
+    assert pos_wdg._warn_icon.isHidden()
     assert not tb.isColumnHidden(GRID)
 
-    add_grid_btn, remove_grid_btn = p._get_grid_buttons(0)
+    add_grid_btn, remove_grid_btn = pos_wdg._get_grid_buttons(0)
     assert remove_grid_btn.isHidden()
 
     grid_plan = pos_1["sequence"]["grid_plan"]
-    p._add_grid_plan(grid_plan, 0)
+    pos_wdg._add_grid_plan(grid_plan, 0)
 
     assert not remove_grid_btn.isHidden()
     assert add_grid_btn.text() == "Edit"
-    assert tb.item(0, 0).data(p.GRID_ROLE) == {
+    assert tb.item(0, 0).data(pos_wdg.GRID_ROLE) == {
         "columns": 2,
         "mode": "spiral",
         "overlap": (10.0, 5.0),
         "relative_to": "center",
         "rows": 2,
     }
     assert tb.item(0, 0).toolTip() == (
         "rows: 2,  columns: 2,  relative_to: center,  overlap: (10.0, 5.0),  "
         "mode: spiral"
     )
 
-    assert p.value() == [pos_1]
+    assert _wdg_value_no_fov(pos_wdg) == [pos_1]
 
     mmc.waitForSystem()
     mmc.setXYPosition(10, 20)
-    p.add_button.click()
-    p._apply_grid_to_all_positions(0)
+    pos_wdg.add_button.click()
+    pos_wdg._apply_grid_to_all_positions(0)
     assert tb.item(1, 0).toolTip() == tb.item(0, 0).toolTip()
 
-    assert p.value() == [pos_1, pos_2]
+    assert _wdg_value_no_fov(pos_wdg) == [pos_1, pos_2]
 
-    p._advanced_cbox.setChecked(False)
-    assert not p._warn_icon.isHidden()
-    assert p.value() == [pos_1, pos_2]
+    pos_wdg._advanced_cbox.setChecked(False)
+    assert not pos_wdg._warn_icon.isHidden()
+    assert _wdg_value_no_fov(pos_wdg) == [pos_1, pos_2]
 
-    p._advanced_cbox.setChecked(True)
+    pos_wdg._advanced_cbox.setChecked(True)
     remove_grid_btn.click()
     assert remove_grid_btn.isHidden()
 
 
 def test_absolute_grid_position(
     global_mmcore: CMMCorePlus, qtbot: QtBot, pos: tuple[dict[str, Any], ...]
 ):
     _, _, pos_3 = pos
-    p = PositionTable()
-    qtbot.addWidget(p)
+    pos_wdg = PositionTable()
+    qtbot.addWidget(pos_wdg)
 
-    tb = p._table
+    tb = pos_wdg._table
 
     assert not tb.rowCount()
 
-    p.add_button.click()
+    pos_wdg.add_button.click()
     assert tb.rowCount() == 1
-    p._advanced_cbox.setChecked(True)
+    pos_wdg._advanced_cbox.setChecked(True)
 
-    _, remove_grid_btn = p._get_grid_buttons(0)
+    _, remove_grid_btn = pos_wdg._get_grid_buttons(0)
     assert remove_grid_btn.isHidden()
 
     grid_plan = pos_3["sequence"]["grid_plan"]
-    p._add_grid_plan(grid_plan, 0)
+    pos_wdg._add_grid_plan(grid_plan, 0)
 
-    assert tb.item(0, 0).data(p.GRID_ROLE) == {
+    assert tb.item(0, 0).data(pos_wdg.GRID_ROLE) == {
         "bottom": 0.0,
         "left": 0.0,
         "mode": "row_wise_snake",
         "overlap": (0.0, 0.0),
         "right": 50.0,
         "top": 100.0,
     }
 
     assert tb.item(0, 0).toolTip() == (
         "top: 100.0,  bottom: 0.0,  left: 0.0,  right: 50.0,  overlap: (0.0, 0.0),  "
         "mode: row_wise_snake"
     )
     pos_3["name"] = "Pos000"
     pos_3["y"] = 100.0
-    assert p.value() == [pos_3]
+    assert _wdg_value_no_fov(pos_wdg) == [pos_3]
 
 
 def test_pos_table_set_and_get_state(
     global_mmcore: CMMCorePlus, qtbot: QtBot, pos: tuple[dict[str, Any], ...]
 ):
     pos_1, pos_2, pos_3 = pos
-    p = PositionTable()
-    qtbot.addWidget(p)
+    pos_wdg = PositionTable()
+    qtbot.addWidget(pos_wdg)
 
-    p.set_state([pos_1, pos_2, pos_3])
-    assert p._warn_icon.isHidden()
+    pos_wdg.set_state([pos_1, pos_2, pos_3])
+    assert pos_wdg._warn_icon.isHidden()
     pos_3["y"] = 100.0
-    assert p.value() == [pos_1, pos_2, pos_3]
-    assert p._advanced_cbox.isChecked()
+    assert _wdg_value_no_fov(pos_wdg) == [pos_1, pos_2, pos_3]
+    assert pos_wdg._advanced_cbox.isChecked()
 
-    p._advanced_cbox.setChecked(False)
-    assert not p._warn_icon.isHidden()
-    assert p.value() == [pos_1, pos_2, pos_3]
+    pos_wdg._advanced_cbox.setChecked(False)
+    assert not pos_wdg._warn_icon.isHidden()
+    assert _wdg_value_no_fov(pos_wdg) == [pos_1, pos_2, pos_3]
 
 
 def test_autofocus_position(global_mmcore: CMMCorePlus, qtbot: QtBot):
     p = PositionTable()
     qtbot.addWidget(p)
 
     mmc = global_mmcore
@@ -320,16 +329,14 @@
     mmc.unloadDevice("Z")
 
     p = PositionTable()
     qtbot.addWidget(p)
 
     tb = p._table
 
-    assert tb.isColumnHidden(Z)
-
     mmc.setXYPosition(100, 200)
     mmc.setPosition("Z1", 45)
     mmc.waitForSystem()
 
     p._autofocus_wdg.setValue({"autofocus_device_name": "Z1"})
     assert not tb.isColumnHidden(AF)
 
@@ -350,16 +357,14 @@
     qtbot.addWidget(p)
 
     tb = p._table
 
     mmc.setPosition("Z1", 45)
     mmc.waitForSystem()
 
-    assert tb.isColumnHidden(X)
-    assert tb.isColumnHidden(Y)
     assert tb.isColumnHidden(AF)
 
     p._autofocus_wdg.setValue({"autofocus_device_name": "Z1"})
     assert not tb.isColumnHidden(AF)
     with pytest.warns(UserWarning, match="Autofocus Device is not Locked in Focus"):
         p.add_button.click()
     assert _get_values(tb, 0) == ["Pos000", 0.0, 45.0]
@@ -368,15 +373,15 @@
 def test_no_autofocus(global_mmcore: CMMCorePlus, qtbot: QtBot):
     mmc = global_mmcore
     mmc.unloadDevice("Autofocus")
 
     p = PositionTable()
     qtbot.addWidget(p)
 
-    assert not p._autofocus_wdg._autofocus_checkbox.isEnabled()
+    assert not p._autofocus_wdg._af_checkbox.isEnabled()
     assert p._autofocus_wdg.value() == {"autofocus_device_name": None}
 
 
 def test_set_state_with_autofocus(global_mmcore: CMMCorePlus, qtbot: QtBot):
     p = PositionTable()
     qtbot.addWidget(p)
     tb = p._table
@@ -394,15 +399,15 @@
             }
         },
     }
 
     p.set_state([pos])
 
     assert not tb.isColumnHidden(AF)
-    assert p._autofocus_wdg._autofocus_checkbox.isChecked()
+    assert p._autofocus_wdg._af_checkbox.isChecked()
     assert p._autofocus_wdg.value() == {
         "autofocus_device_name": "Z1",
         "axes": ("t", "p", "g"),
     }
     assert _get_values(tb, 0) == ["Pos000", 10.0, 20.0, 30.0, 45.0]
 
     assert p.value() == [pos]
@@ -453,23 +458,43 @@
         "rows": 2,
         "relative_to": "center",
         "overlap": (0.0, 0.0),
         "mode": "spiral",
     }
 
 
-def test_on_property_changed(global_mmcore: CMMCorePlus, qtbot: QtBot):
+def test_on_property_changed_focus(global_mmcore: CMMCorePlus, qtbot: QtBot):
     p = PositionTable()
     qtbot.addWidget(p)
     tb = p._table
     mmc = global_mmcore
 
-    assert not tb.isColumnHidden(Z)
+    mmc.setProperty("Core", "Focus", "Z1")
+    assert tb.horizontalHeaderItem(Z).text() == "Z1"
     mmc.setProperty("Core", "Focus", "")
-    assert tb.isColumnHidden(Z)
+    assert tb.horizontalHeaderItem(Z).text() == "Z"
+
+
+def test_on_property_changed_autofocus(global_mmcore: CMMCorePlus, qtbot: QtBot):
+    p = PositionTable()
+    qtbot.addWidget(p)
+    mmc = global_mmcore
+
+    mmc.setProperty("Core", "AutoFocus", "")
+    assert p._autofocus_wdg.value()["autofocus_device_name"] is None
+    assert not p._autofocus_wdg._af_checkbox.isEnabled()
+    assert not p._autofocus_wdg._af_checkbox.isChecked()
+    assert not p._autofocus_wdg._af_combo.isVisible()
+
+    mmc.setProperty("Core", "AutoFocus", "Autofocus")
+    p._autofocus_wdg._af_checkbox.setChecked(True)
+    assert p._autofocus_wdg.value()["autofocus_device_name"] == "Z1"
+    assert p._autofocus_wdg._af_checkbox.isEnabled()
+    assert p._autofocus_wdg._af_checkbox.isChecked()
+    assert not p._autofocus_wdg._af_combo.isHidden()
 
 
 def _pos_for_save_load(load: bool):
     """Return a list of positions for saving or loading.
 
     The difference ios that for loading the axes are a tuple and for saving a list.
     """
@@ -518,26 +543,31 @@
 
             pos = _pos_for_save_load(load=False)
             p.set_state(pos)
             assert p._table.rowCount() == 3
 
             p._save_positions()
 
-            file = list(Path(tmp).iterdir())[0]
+            file = next(iter(Path(tmp).iterdir()))
 
-            assert json.loads(file.read_text()) == pos
+            from_disk = json.loads(file.read_text())
+            for item in from_disk:
+                if "sequence" in item and "grid_plan" in (item["sequence"] or {}):
+                    item["sequence"]["grid_plan"].pop("fov_height")
+                    item["sequence"]["grid_plan"].pop("fov_width")
+            assert from_disk == pos
 
             p.clear()
             assert p.value() == []
             assert p._table.rowCount() == 0
 
             with patch.object(QFileDialog, "getOpenFileName", _path):
                 p._load_positions()
                 assert p._table.rowCount() == 3
-                assert p.value() == _pos_for_save_load(load=True)
+                assert _wdg_value_no_fov(p) == _pos_for_save_load(load=True)
 
 
 def test_set_state_with_different_z_af_devicies(
     global_mmcore: CMMCorePlus, qtbot: QtBot
 ):
     p = PositionTable()
     qtbot.addWidget(p)
@@ -579,10 +609,10 @@
         },
     }
 
     with pytest.warns(UserWarning, match="Autofocus device Z2 not loaded"):
         p.set_state([pos])
 
     assert tb.isColumnHidden(AF)
-    assert not p._autofocus_wdg._autofocus_checkbox.isChecked()
+    assert not p._autofocus_wdg._af_checkbox.isChecked()
     assert p._autofocus_wdg.value() == {"autofocus_device_name": None}
     assert _get_values(tb, 0) == ["Pos000", 10.0, 20.0, 30.0]
```

### Comparing `pymmcore-widgets-0.4.0/tests/test_presets_widget.py` & `pymmcore_widgets-0.4.1/tests/test_presets_widget.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.4.0/tests/test_prop_widget.py` & `pymmcore_widgets-0.4.1/tests/test_prop_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pymmcore_widgets import PropertyWidget
 
 # not sure how else to parametrize the test without instantiating here at import ...
 # NOTE: in the default 'MMConfig_demo.cgf', the device called 'LED'
 # is a mock State Device (DStateDevice) device from the 'DemoCamera DHub.
 # We are excluding the dev-prop 'LED-Number of positions' because
 # it is not an actual property of the device, but it is only used
-# in the micromanager "Hardwre Confoguration Wizard" to set the number
+# in the micromanager "Hardwre Configuration Wizard" to set the number
 # of states (by default, 10) that the mock device can have.
 CORE = CMMCorePlus()
 CORE.loadSystemConfiguration()
 dev_props = [
     (dev, prop)
     for dev in CORE.getLoadedDevices()
     for prop in CORE.getDevicePropertyNames(dev)
```

### Comparing `pymmcore-widgets-0.4.0/tests/test_properties_widget.py` & `pymmcore_widgets-0.4.1/tests/test_properties_widget.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.4.0/tests/test_property_browser.py` & `pymmcore_widgets-0.4.1/tests/test_property_browser.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.4.0/tests/test_shutter_widget.py` & `pymmcore_widgets-0.4.1/tests/test_shutter_widget.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.4.0/tests/test_snap_button_widget.py` & `pymmcore_widgets-0.4.1/tests/test_snap_button_widget.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.4.0/tests/test_stage_widget.py` & `pymmcore_widgets-0.4.1/tests/test_stage_widget.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.4.0/tests/test_table_pixel_size_widget.py` & `pymmcore_widgets-0.4.1/tests/test_table_pixel_size_widget.py`

 * *Files identical despite different names*

### Comparing `pymmcore-widgets-0.4.0/tests/test_time_table.py` & `pymmcore_widgets-0.4.1/tests/test_time_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
 from datetime import timedelta
 from typing import TYPE_CHECKING, cast
 
 import pytest
 from pydantic import ValidationError
-from qtpy.QtWidgets import QSpinBox, QTableWidget
-from superqt import QQuantity
 
 from pymmcore_widgets._mda import TimePlanWidget
 
 if TYPE_CHECKING:
     from pytestqt.qtbot import QtBot
+    from qtpy.QtWidgets import QSpinBox, QTableWidget
+    from superqt import QQuantity
 
 INTERVAL = 0
 TIMEPOINTS = 1
 
 
 def _value(table: QTableWidget, row: int):
     interval = cast("QQuantity", table.cellWidget(row, INTERVAL))
```

