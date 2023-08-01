# Comparing `tmp/ipywidgets-8.0.7.tar.gz` & `tmp/ipywidgets-8.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipywidgets-8.0.7.tar", last modified: Tue Jul  4 15:09:36 2023, max compression
+gzip compressed data, was "ipywidgets-8.1.0.tar", last modified: Tue Aug  1 07:35:26 2023, max compression
```

## Comparing `ipywidgets-8.0.7.tar` & `ipywidgets-8.1.0.tar`

### file list

```diff
@@ -1,83 +1,84 @@
-drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-07-04 15:09:36.903366 ipywidgets-8.0.7/
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     1513 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/LICENSE
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      459 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/MANIFEST.in
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     1963 2023-07-04 15:09:36.903366 ipywidgets-8.0.7/PKG-INFO
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      880 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/README.md
-drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-07-04 15:09:36.883366 ipywidgets-8.0.7/ipywidgets/
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     1932 2023-04-04 12:50:27.000000 ipywidgets-8.0.7/ipywidgets/__init__.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      610 2023-07-04 15:09:15.000000 ipywidgets-8.0.7/ipywidgets/_version.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    11287 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/embed.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     2883 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/state.schema.json
-drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-07-04 15:09:36.884366 ipywidgets-8.0.7/ipywidgets/tests/
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)        0 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/tests/__init__.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     6803 2023-04-04 12:50:27.000000 ipywidgets-8.0.7/ipywidgets/tests/test_embed.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      595 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/view.schema.json
-drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-07-04 15:09:36.896366 ipywidgets-8.0.7/ipywidgets/widgets/
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     1709 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/__init__.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      639 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/docutils.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     2290 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/domwidget.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    20414 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/interaction.py
-drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-07-04 15:09:36.902366 ipywidgets-8.0.7/ipywidgets/widgets/tests/
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)        0 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/tests/__init__.py
-drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-07-04 15:09:36.902366 ipywidgets-8.0.7/ipywidgets/widgets/tests/data/
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    36297 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/tests/data/jupyter-logo-transparent.png
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     2133 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/tests/test_datetime_serializers.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      673 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/tests/test_docutils.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    17123 2023-04-04 12:50:27.000000 ipywidgets-8.0.7/ipywidgets/widgets/tests/test_interaction.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     1005 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/tests/test_link.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     5619 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/tests/test_selectioncontainer.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      732 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/tests/test_send_state.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    11017 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/tests/test_set_state.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     7239 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/tests/test_traits.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     2478 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/tests/test_utils.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     2606 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/tests/test_widget.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      995 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/tests/test_widget_box.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      369 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/tests/test_widget_button.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     4169 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/tests/test_widget_datetime.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      606 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/tests/test_widget_float.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     4422 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/tests/test_widget_image.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     2655 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/tests/test_widget_naive_datetime.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     7466 2023-04-04 12:50:27.000000 ipywidgets-8.0.7/ipywidgets/widgets/tests/test_widget_output.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     3372 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/tests/test_widget_selection.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     1796 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/tests/test_widget_string.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    28435 2023-04-04 12:50:27.000000 ipywidgets-8.0.7/ipywidgets/widgets/tests/test_widget_templates.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     2469 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/tests/test_widget_time.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     4164 2023-04-04 12:50:27.000000 ipywidgets-8.0.7/ipywidgets/widgets/tests/test_widget_upload.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     2407 2023-04-04 12:50:27.000000 ipywidgets-8.0.7/ipywidgets/widgets/tests/utils.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    14919 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/trait_types.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     2608 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/utils.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      817 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/valuewidget.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    35076 2023-04-04 12:50:27.000000 ipywidgets-8.0.7/ipywidgets/widgets/widget.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     4328 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/widget_bool.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     3731 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/widget_box.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     4204 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/widget_button.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      807 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/widget_color.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     2320 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/widget_controller.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      622 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/widget_core.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     2597 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/widget_date.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     4134 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/widget_datetime.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     2278 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/widget_description.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    15028 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/widget_float.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    12125 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/widget_int.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     7067 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/widget_layout.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     3708 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/widget_link.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     7783 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/widget_media.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     6823 2023-04-04 12:50:27.000000 ipywidgets-8.0.7/ipywidgets/widgets/widget_output.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    24457 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/widget_selection.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     4198 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/widget_selectioncontainer.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     6869 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/widget_string.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      559 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/widget_style.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     3498 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/widget_tagsinput.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    15507 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/widget_templates.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     2779 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/widget_time.py
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     4637 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/ipywidgets/widgets/widget_upload.py
-drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-07-04 15:09:36.884366 ipywidgets-8.0.7/ipywidgets.egg-info/
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     1963 2023-07-04 15:09:36.000000 ipywidgets-8.0.7/ipywidgets.egg-info/PKG-INFO
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     2681 2023-07-04 15:09:36.000000 ipywidgets-8.0.7/ipywidgets.egg-info/SOURCES.txt
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)        1 2023-07-04 15:09:36.000000 ipywidgets-8.0.7/ipywidgets.egg-info/dependency_links.txt
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)        1 2023-07-04 15:09:36.000000 ipywidgets-8.0.7/ipywidgets.egg-info/not-zip-safe
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      160 2023-07-04 15:09:36.000000 ipywidgets-8.0.7/ipywidgets.egg-info/requires.txt
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)       11 2023-07-04 15:09:36.000000 ipywidgets-8.0.7/ipywidgets.egg-info/top_level.txt
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      229 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/pyproject.toml
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     1432 2023-07-04 15:09:36.904366 ipywidgets-8.0.7/setup.cfg
--rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      235 2023-03-22 12:27:09.000000 ipywidgets-8.0.7/setup.py
+drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-08-01 07:35:26.818381 ipywidgets-8.1.0/
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     1513 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/LICENSE
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      459 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/MANIFEST.in
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     1963 2023-08-01 07:35:26.818381 ipywidgets-8.1.0/PKG-INFO
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      880 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/README.md
+drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-08-01 07:35:26.796381 ipywidgets-8.1.0/ipywidgets/
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     1728 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/__init__.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      610 2023-08-01 07:35:08.000000 ipywidgets-8.1.0/ipywidgets/_version.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      764 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/comm.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    11287 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/embed.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     2883 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/state.schema.json
+drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-08-01 07:35:26.800381 ipywidgets-8.1.0/ipywidgets/tests/
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)        0 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/tests/__init__.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     6729 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/tests/test_embed.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      595 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/view.schema.json
+drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-08-01 07:35:26.811381 ipywidgets-8.1.0/ipywidgets/widgets/
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     1709 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/__init__.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      639 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/docutils.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     2290 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/domwidget.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    20414 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/interaction.py
+drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-08-01 07:35:26.817381 ipywidgets-8.1.0/ipywidgets/widgets/tests/
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)        0 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/tests/__init__.py
+drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-08-01 07:35:26.817381 ipywidgets-8.1.0/ipywidgets/widgets/tests/data/
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    36297 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/tests/data/jupyter-logo-transparent.png
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     2111 2023-07-31 12:53:54.000000 ipywidgets-8.1.0/ipywidgets/widgets/tests/test_datetime_serializers.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      673 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/tests/test_docutils.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    17123 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/tests/test_interaction.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     1005 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/tests/test_link.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     5619 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/tests/test_selectioncontainer.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      732 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/tests/test_send_state.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    11017 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/tests/test_set_state.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     8361 2023-07-31 14:37:23.000000 ipywidgets-8.1.0/ipywidgets/widgets/tests/test_traits.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     2478 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/tests/test_utils.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     2606 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/tests/test_widget.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      995 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/tests/test_widget_box.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      369 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/tests/test_widget_button.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     4147 2023-07-31 12:53:54.000000 ipywidgets-8.1.0/ipywidgets/widgets/tests/test_widget_datetime.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      606 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/tests/test_widget_float.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     4422 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/tests/test_widget_image.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     2633 2023-07-31 12:53:54.000000 ipywidgets-8.1.0/ipywidgets/widgets/tests/test_widget_naive_datetime.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     7466 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/tests/test_widget_output.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     3372 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/tests/test_widget_selection.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     1796 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/tests/test_widget_string.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    28435 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/tests/test_widget_templates.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     2447 2023-07-31 12:53:54.000000 ipywidgets-8.1.0/ipywidgets/widgets/tests/test_widget_time.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     4164 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/tests/test_widget_upload.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     2407 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/tests/utils.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    16270 2023-07-31 14:37:23.000000 ipywidgets-8.1.0/ipywidgets/widgets/trait_types.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     2608 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/utils.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      817 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/valuewidget.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    34879 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/widget.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     4328 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/widget_bool.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     3731 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/widget_box.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     4204 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/widget_button.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      807 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/widget_color.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     2320 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/widget_controller.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      622 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/widget_core.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     2597 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/widget_date.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     4134 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/widget_datetime.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     2278 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/widget_description.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    15028 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/widget_float.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    12125 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/widget_int.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     7067 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/widget_layout.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     3708 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/widget_link.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     7783 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/widget_media.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     6823 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/widget_output.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    24457 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/widget_selection.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     4198 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/widget_selectioncontainer.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     6869 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/widget_string.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      559 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/widget_style.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     3498 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/widget_tagsinput.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    15507 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/widget_templates.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     2779 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/widget_time.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     4637 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/ipywidgets/widgets/widget_upload.py
+drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-08-01 07:35:26.800381 ipywidgets-8.1.0/ipywidgets.egg-info/
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     1963 2023-08-01 07:35:26.000000 ipywidgets-8.1.0/ipywidgets.egg-info/PKG-INFO
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     2700 2023-08-01 07:35:26.000000 ipywidgets-8.1.0/ipywidgets.egg-info/SOURCES.txt
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)        1 2023-08-01 07:35:26.000000 ipywidgets-8.1.0/ipywidgets.egg-info/dependency_links.txt
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)        1 2023-08-01 07:35:26.000000 ipywidgets-8.1.0/ipywidgets.egg-info/not-zip-safe
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      155 2023-08-01 07:35:26.000000 ipywidgets-8.1.0/ipywidgets.egg-info/requires.txt
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)       11 2023-08-01 07:35:26.000000 ipywidgets-8.1.0/ipywidgets.egg-info/top_level.txt
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      229 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/pyproject.toml
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     1427 2023-08-01 07:35:26.818381 ipywidgets-8.1.0/setup.cfg
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      235 2023-07-31 12:53:52.000000 ipywidgets-8.1.0/setup.py
```

### Comparing `ipywidgets-8.0.7/LICENSE` & `ipywidgets-8.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/PKG-INFO` & `ipywidgets-8.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipywidgets
-Version: 8.0.7
+Version: 8.1.0
 Summary: Jupyter interactive widgets
 Home-page: http://jupyter.org
 Author: Jupyter Development Team
 Author-email: jupyter@googlegroups.com
 License: BSD 3-Clause License
 Keywords: Interactive,Interpreter,Shell,Web,ipython,widgets,Jupyter
 Platform: Linux
```

### Comparing `ipywidgets-8.0.7/README.md` & `ipywidgets-8.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/__init__.py` & `ipywidgets-8.1.0/ipywidgets/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,38 +17,32 @@
 accessible as a `value` attribute.
 """
 
 # Must import __version__ first to avoid errors importing this file during the build process. See https://github.com/pypa/setuptools/issues/1724#issuecomment-627241822
 from ._version import __version__, __protocol_version__, __jupyter_widgets_controls_version__, __jupyter_widgets_base_version__
 
 import os
+import sys
 
 from traitlets import link, dlink
 from IPython import get_ipython
-try:
-    from comm import get_comm_manager
-except ImportError:
-    def get_comm_manager():
-        ip = get_ipython()
-
-        if ip is not None and getattr(ip, "kernel", None) is not None:
-            return get_ipython().kernel.comm_manager
 
 from .widgets import *
 
 
 def load_ipython_extension(ip):
     """Set up Jupyter to work with widgets"""
     if not hasattr(ip, 'kernel'):
         return
     register_comm_target()
 
 def register_comm_target(kernel=None):
     """Register the jupyter.widget comm target"""
-    comm_manager = get_comm_manager()
+    from . import comm
+    comm_manager = comm.get_comm_manager()
     if comm_manager is None:
         return
     comm_manager.register_target('jupyter.widget', Widget.handle_comm_opened)
     comm_manager.register_target('jupyter.widget.control', Widget.handle_control_comm_opened)
 
 def _handle_ipython():
     """Register with the comm target at import if running in Jupyter"""
```

### Comparing `ipywidgets-8.0.7/ipywidgets/_version.py` & `ipywidgets-8.1.0/ipywidgets/_version.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Jupyter Development Team.
 # Distributed under the terms of the Modified BSD License.
 
-__version__ = '8.0.7'
+__version__ = '8.1.0'
 
 __protocol_version__ = '2.1.0'
 __control_protocol_version__ = '1.0.0'
 
 # These are *protocol* versions for each package, *not* npm versions. To check, look at each package's src/version.ts file for the protocol version the package implements.
 __jupyter_widgets_base_version__ = '2.0.0'
 __jupyter_widgets_output_version__ = '1.0.0'
```

### Comparing `ipywidgets-8.0.7/ipywidgets/embed.py` & `ipywidgets-8.1.0/ipywidgets/embed.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/state.schema.json` & `ipywidgets-8.1.0/ipywidgets/state.schema.json`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/tests/test_embed.py` & `ipywidgets-8.1.0/ipywidgets/tests/test_embed.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,14 @@
 import os
 import re
 import tempfile
 import shutil
 
 import traitlets
 
-# This has a byproduct of setting up the comms
-import ipykernel.ipkernel
-
 from ..widgets import IntSlider, IntText, Text, Widget, jslink, HBox, widget_serialization, widget as widget_module
 from ..embed import embed_data, embed_snippet, embed_minimal_html, dependency_state
 
 
 class CaseWidget(Widget):
     """Widget to test dependency traversal"""
```

### Comparing `ipywidgets-8.0.7/ipywidgets/view.schema.json` & `ipywidgets-8.1.0/ipywidgets/view.schema.json`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/__init__.py` & `ipywidgets-8.1.0/ipywidgets/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/docutils.py` & `ipywidgets-8.1.0/ipywidgets/widgets/docutils.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/domwidget.py` & `ipywidgets-8.1.0/ipywidgets/widgets/domwidget.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/interaction.py` & `ipywidgets-8.1.0/ipywidgets/widgets/interaction.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/tests/data/jupyter-logo-transparent.png` & `ipywidgets-8.1.0/ipywidgets/widgets/tests/data/jupyter-logo-transparent.png`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/tests/test_datetime_serializers.py` & `ipywidgets-8.1.0/ipywidgets/widgets/tests/test_datetime_serializers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python
 # coding: utf-8
 
 # Copyright (c) Vidar Tonaas Fauske.
 # Distributed under the terms of the Modified BSD License.
 
 import pytest
```

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/tests/test_docutils.py` & `ipywidgets-8.1.0/ipywidgets/widgets/tests/test_docutils.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/tests/test_interaction.py` & `ipywidgets-8.1.0/ipywidgets/widgets/tests/test_interaction.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/tests/test_link.py` & `ipywidgets-8.1.0/ipywidgets/widgets/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/tests/test_selectioncontainer.py` & `ipywidgets-8.1.0/ipywidgets/widgets/tests/test_selectioncontainer.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/tests/test_send_state.py` & `ipywidgets-8.1.0/ipywidgets/widgets/tests/test_send_state.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/tests/test_set_state.py` & `ipywidgets-8.1.0/ipywidgets/widgets/tests/test_set_state.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/tests/test_traits.py` & `ipywidgets-8.1.0/ipywidgets/widgets/tests/test_traits.py`

 * *Files 27% similar despite different names*

```diff
@@ -48,23 +48,40 @@
         'rgb(0, 0, 0)', # rgb
         'rgb( 20,70,50 )', # rgb with spaces
         'rgba(10,10,10, 0.5)', # rgba with float alpha
         'rgba(255, 255, 255, 255)', # out of bounds alpha (spec says clamp to 1)
         'hsl(0.0, .0, 0)', # hsl
         'hsl( 0.5,0.3,0 )', # hsl with spaces
         'hsla(10,10,10, 0.5)', # rgba with float alpha
+        'var(--my-color)', # CSS variable without fallback
+        'var(--my-color-with_separators)', # CSS variable without fallback
+        'var(--my-color,)', # CSS variable with empty fallback
+        'var(--my-color-æ)', # CSS variable with non-ascii characters
+        'var(--my-color-\u1234)', # CSS variable with unicode characters
+        r'var(--my-color-\\1234)', # CSS variable escaped hex character
+        'var(--my-color-\.)', # CSS variable with escaped characters
+        'var(--my-color,black)', # CSS variable with named color fallback
+        'var(--my-color, black)', # CSS variable with named color fallback
+        'var(--my-color, rgb(20, 70, 50))', # CSS variable with rgb color fallback
+        'var(--my-color, #fff)', # CSS variable with rgb color fallback
     ]
     _bad_values = [
         "vanilla", "blues",  # Invalid color names
         1.2, 0.0,  # Should fail with float input
         0, 1, 2,  # Should fail with int input
         'rgb(0.4, 512, -40)',
         'hsl(0.4, 512, -40)',
         'rgba(0, 0, 0)',
         'hsla(0, 0, 0)',
+        'var(-my-color)', # wrong identifier
+        'var(--my-color-\u2041)', # invalid unicode codepoint
+        'var(my-color, black)', # wrong identifier
+        'var(my-color-., black)', # invalid character in identifier
+        'var(--my-color, vanilla)', # wrong fallback
+        'var(--my-color, rgba(0,0,0))', # wrong fallback
         None,
     ]
 
 
 class ColorTraitWithNone(HasTraits):
     value = Color("black", allow_none=True)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/tests/test_utils.py` & `ipywidgets-8.1.0/ipywidgets/widgets/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/tests/test_widget.py` & `ipywidgets-8.1.0/ipywidgets/widgets/tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/tests/test_widget_box.py` & `ipywidgets-8.1.0/ipywidgets/widgets/tests/test_widget_box.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/tests/test_widget_datetime.py` & `ipywidgets-8.1.0/ipywidgets/widgets/tests/test_widget_datetime.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python
 # coding: utf-8
 
 # Copyright (c) Jupyter Development Team.
 # Distributed under the terms of the Modified BSD License.
 
 import pytest
```

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/tests/test_widget_float.py` & `ipywidgets-8.1.0/ipywidgets/widgets/tests/test_widget_float.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/tests/test_widget_image.py` & `ipywidgets-8.1.0/ipywidgets/widgets/tests/test_widget_image.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/tests/test_widget_naive_datetime.py` & `ipywidgets-8.1.0/ipywidgets/widgets/tests/test_widget_naive_datetime.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python
 # coding: utf-8
 
 # Copyright (c) Vidar Tonaas Fauske.
 # Distributed under the terms of the Modified BSD License.
 
 import pytest
```

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/tests/test_widget_output.py` & `ipywidgets-8.1.0/ipywidgets/widgets/tests/test_widget_output.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/tests/test_widget_selection.py` & `ipywidgets-8.1.0/ipywidgets/widgets/tests/test_widget_selection.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/tests/test_widget_string.py` & `ipywidgets-8.1.0/ipywidgets/widgets/tests/test_widget_string.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/tests/test_widget_templates.py` & `ipywidgets-8.1.0/ipywidgets/widgets/tests/test_widget_templates.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/tests/test_widget_time.py` & `ipywidgets-8.1.0/ipywidgets/widgets/tests/test_widget_time.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python
 # coding: utf-8
 
 # Copyright (c) Vidar Tonaas Fauske.
 # Distributed under the terms of the Modified BSD License.
 
 import pytest
```

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/tests/test_widget_upload.py` & `ipywidgets-8.1.0/ipywidgets/widgets/tests/test_widget_upload.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/tests/utils.py` & `ipywidgets-8.1.0/ipywidgets/widgets/tests/utils.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/trait_types.py` & `ipywidgets-8.1.0/ipywidgets/widgets/trait_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,46 +9,90 @@
 import traitlets
 import datetime as dt
 
 
 _color_names = ['aliceblue', 'antiquewhite', 'aqua', 'aquamarine', 'azure', 'beiae', 'bisque', 'black', 'blanchedalmond', 'blue', 'blueviolet', 'brown', 'burlywood', 'cadetblue', 'chartreuse', 'chocolate', 'coral', 'cornflowerblue', 'cornsilk', 'crimson', 'cyan', 'darkblue', 'darkcyan', 'darkgoldenrod', 'darkgray', 'darkgrey', 'darkgreen', 'darkkhaki', 'darkmagenta', 'darkolivegreen', 'darkorange', 'darkorchid', 'darkred', 'darksalmon', 'darkseagreen', 'darkslateblue', 'darkslategray', 'darkslategrey', 'darkturquoise', 'darkviolet', 'deeppink', 'deepskyblue', 'dimgray', 'dimgrey', 'dodgerblue', 'firebrick', 'floralwhite', 'forestgreen', 'fuchsia', 'gainsboro', 'ghostwhite', 'gold', 'goldenrod', 'gray', 'grey', 'green', 'greenyellow', 'honeydew', 'hotpink', 'indianred ', 'indigo ', 'ivory', 'khaki', 'lavender', 'lavenderblush', 'lawngreen', 'lemonchiffon', 'lightblue', 'lightcoral', 'lightcyan', 'lightgoldenrodyellow', 'lightgray', 'lightgrey', 'lightgreen', 'lightpink', 'lightsalmon', 'lightseagreen', 'lightskyblue', 'lightslategray', 'lightslategrey', 'lightsteelblue', 'lightyellow', 'lime', 'limegreen', 'linen', 'magenta', 'maroon', 'mediumaquamarine', 'mediumblue', 'mediumorchid', 'mediumpurple', 'mediumseagreen', 'mediumslateblue', 'mediumspringgreen', 'mediumturquoise', 'mediumvioletred', 'midnightblue', 'mintcream', 'mistyrose', 'moccasin', 'navajowhite', 'navy', 'oldlace', 'olive', 'olivedrab', 'orange', 'orangered', 'orchid', 'palegoldenrod', 'palegreen', 'paleturquoise', 'palevioletred', 'papayawhip', 'peachpuff', 'peru', 'pink', 'plum', 'powderblue', 'purple', 'rebeccapurple', 'red', 'rosybrown', 'royalblue', 'saddlebrown', 'salmon', 'sandybrown', 'seagreen', 'seashell', 'sienna', 'silver', 'skyblue', 'slateblue', 'slategray', 'slategrey', 'snow', 'springgreen', 'steelblue', 'tan', 'teal', 'thistle', 'tomato', 'transparent', 'turquoise', 'violet', 'wheat', 'white', 'whitesmoke', 'yellow', 'yellowgreen']
 
 # Regex colors #fff and #ffffff
-_color_hex_re = re.compile(r'#[a-fA-F0-9]{3}(?:[a-fA-F0-9]{3})?$')
+_color_hex = r'#[a-fA-F0-9]{3}(?:[a-fA-F0-9]{3})?'
+_color_hex_re = re.compile(fr'^{_color_hex}$')
 # Regex colors #ffff and #ffffffff (includes alpha value)
-_color_hexa_re = re.compile(r'^#[a-fA-F0-9]{4}(?:[a-fA-F0-9]{4})?$')
+_color_hexa = r'#[a-fA-F0-9]{4}(?:[a-fA-F0-9]{4})?'
+_color_hexa_re = re.compile(fr'^{_color_hexa}$')
 
 # Helpers (float percent, int percent with optional surrounding whitespace)
 _color_frac_percent = r'\s*(\d+(\.\d*)?|\.\d+)?%?\s*'
 _color_int_percent = r'\s*\d+%?\s*'
 
 # rgb(), rgba(), hsl() and hsla() format strings
 _color_rgb = r'rgb\({ip},{ip},{ip}\)'
 _color_rgba = r'rgba\({ip},{ip},{ip},{fp}\)'
 _color_hsl = r'hsl\({fp},{fp},{fp}\)'
 _color_hsla = r'hsla\({fp},{fp},{fp},{fp}\)'
 
 # Regex colors rgb/rgba/hsl/hsla
-_color_rgbhsl_re = re.compile('({})|({})|({})|({})'.format(
+_color_rgbhsl = '({})|({})|({})|({})'.format(
     _color_rgb, _color_rgba, _color_hsl, _color_hsla
-).format(ip=_color_int_percent, fp=_color_frac_percent))
+).format(ip=_color_int_percent, fp=_color_frac_percent)
+_color_rgbhsl_re = re.compile(_color_rgbhsl)
+
+# Support for CSS variables.
+# For production rules, see: https://drafts.csswg.org/css-syntax-3/#tokenization
+
+_escape = r'\\([0-9a-fA-F]{1-6}\s?|[^0-9a-fA-F\s])'
+_non_ascii = r''.join(
+    (
+        r'\u00B7',
+        r'\u00C0-\u00D6',
+        r'\u00C0-\u00D6',
+        r'\u00D8-\u00F6',
+        r'\u00F8-\u037D',
+        r'\u037F-\u1FFF',
+        r'\u200C',
+        r'\u200D',
+        r'\u203F',
+        r'\u2040',
+        r'\u2070-\u218F',
+        r'\u2C00-\u2FEF',
+        r'\u3001-\uD7FF',
+        r'\uF900-\uFDCF',
+        r'\uFDF0-\uFFFD',
+        r'\u10000'
+    )
+)
+
+# Custom CSS identifier
+_custom_ident = fr'--([a-zA-Z0-9_\-{_non_ascii}]|{_escape})+'
+
+# Matching for CSS variables with valid color fallback declaration values.
+#
+# A CSS variable consists of a custom identifier starting with '--'.
+# The 'var()' function can be used for substituting the custom property into
+# the value of another property.
+#
+# Here we further restrict the fallback values to be valid colors.
+
+_css_color = fr'({"|".join(_color_names)}|({_color_rgbhsl})|({_color_hex})|({_color_hexa}))'
+_css_var_fallback_color = fr'var\({_custom_ident}(,\s*({_css_color}\s*)?)?\)'
+_color_var_re = re.compile(_css_var_fallback_color)
 
 
 class Color(traitlets.Unicode):
     """A string holding a valid HTML color such as 'blue', '#060482', '#A80'"""
 
     info_text = 'a valid HTML color'
     default_value = traitlets.Undefined
 
     def validate(self, obj, value):
         if value is None and self.allow_none:
             return value
         if isinstance(value, str):
             if (value.lower() in _color_names or _color_hex_re.match(value) or
-                _color_hexa_re.match(value) or _color_rgbhsl_re.match(value)):
+                _color_hexa_re.match(value) or _color_rgbhsl_re.match(value) or
+                _color_var_re.match(value)):
                 return value
 
         self.error(obj, value)
 
 
 class Datetime(traitlets.TraitType):
     """A trait type holding a Python datetime object"""
```

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/utils.py` & `ipywidgets-8.1.0/ipywidgets/widgets/utils.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/valuewidget.py` & `ipywidgets-8.1.0/ipywidgets/widgets/valuewidget.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/widget.py` & `ipywidgets-8.1.0/ipywidgets/widgets/widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 # Copyright (c) Jupyter Development Team.
 # Distributed under the terms of the Modified BSD License.
 
 """Base Widget class.  Allows user to create widgets in the back-end that render
 in the Jupyter notebook front-end.
 """
 import os
+import sys
 import typing
 from contextlib import contextmanager
 from collections.abc import Iterable
 from IPython import get_ipython
 from traitlets import (
     Any, HasTraits, Unicode, Dict, Instance, List, Int, Set, Bytes, observe, default, Container,
     Undefined)
 from json import loads as jsonloads, dumps as jsondumps
+from .. import comm
 
 from base64 import standard_b64encode
 
 from .utils import deprecation, _get_frame
 
 from .._version import __protocol_version__, __control_protocol_version__, __jupyter_widgets_base_version__
 
@@ -520,23 +522,15 @@
                         data={'state': state, 'buffer_paths': buffer_paths},
                         buffers=buffers,
                         metadata={'version': __protocol_version__}
                         )
             if self._model_id is not None:
                 args['comm_id'] = self._model_id
 
-            try:
-                from comm import create_comm
-            except ImportError:
-                def create_comm(**kwargs):
-                    from ipykernel.comm import Comm
-
-                    return Comm(**kwargs)
-
-            self.comm = create_comm(**args)
+            self.comm = comm.create_comm(**args)
 
     @observe('comm')
     def _comm_changed(self, change):
         """Called when the comm is changed."""
         if change['new'] is None:
             return
         self._model_id = self.model_id
```

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/widget_bool.py` & `ipywidgets-8.1.0/ipywidgets/widgets/widget_bool.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/widget_box.py` & `ipywidgets-8.1.0/ipywidgets/widgets/widget_box.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/widget_button.py` & `ipywidgets-8.1.0/ipywidgets/widgets/widget_button.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/widget_color.py` & `ipywidgets-8.1.0/ipywidgets/widgets/widget_color.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/widget_controller.py` & `ipywidgets-8.1.0/ipywidgets/widgets/widget_controller.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/widget_core.py` & `ipywidgets-8.1.0/ipywidgets/widgets/widget_core.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/widget_date.py` & `ipywidgets-8.1.0/ipywidgets/widgets/widget_date.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/widget_datetime.py` & `ipywidgets-8.1.0/ipywidgets/widgets/widget_datetime.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/widget_description.py` & `ipywidgets-8.1.0/ipywidgets/widgets/widget_description.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/widget_float.py` & `ipywidgets-8.1.0/ipywidgets/widgets/widget_float.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/widget_int.py` & `ipywidgets-8.1.0/ipywidgets/widgets/widget_int.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/widget_layout.py` & `ipywidgets-8.1.0/ipywidgets/widgets/widget_layout.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/widget_link.py` & `ipywidgets-8.1.0/ipywidgets/widgets/widget_link.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/widget_media.py` & `ipywidgets-8.1.0/ipywidgets/widgets/widget_media.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/widget_output.py` & `ipywidgets-8.1.0/ipywidgets/widgets/widget_output.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/widget_selection.py` & `ipywidgets-8.1.0/ipywidgets/widgets/widget_selection.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/widget_selectioncontainer.py` & `ipywidgets-8.1.0/ipywidgets/widgets/widget_selectioncontainer.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/widget_string.py` & `ipywidgets-8.1.0/ipywidgets/widgets/widget_string.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/widget_style.py` & `ipywidgets-8.1.0/ipywidgets/widgets/widget_style.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/widget_tagsinput.py` & `ipywidgets-8.1.0/ipywidgets/widgets/widget_tagsinput.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/widget_templates.py` & `ipywidgets-8.1.0/ipywidgets/widgets/widget_templates.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/widget_time.py` & `ipywidgets-8.1.0/ipywidgets/widgets/widget_time.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets/widgets/widget_upload.py` & `ipywidgets-8.1.0/ipywidgets/widgets/widget_upload.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.0.7/ipywidgets.egg-info/PKG-INFO` & `ipywidgets-8.1.0/ipywidgets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipywidgets
-Version: 8.0.7
+Version: 8.1.0
 Summary: Jupyter interactive widgets
 Home-page: http://jupyter.org
 Author: Jupyter Development Team
 Author-email: jupyter@googlegroups.com
 License: BSD 3-Clause License
 Keywords: Interactive,Interpreter,Shell,Web,ipython,widgets,Jupyter
 Platform: Linux
```

### Comparing `ipywidgets-8.0.7/ipywidgets.egg-info/SOURCES.txt` & `ipywidgets-8.1.0/ipywidgets.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 ipywidgets/__init__.py
 ipywidgets/_version.py
+ipywidgets/comm.py
 ipywidgets/embed.py
 ipywidgets/state.schema.json
 ipywidgets/view.schema.json
 ipywidgets.egg-info/PKG-INFO
 ipywidgets.egg-info/SOURCES.txt
 ipywidgets.egg-info/dependency_links.txt
 ipywidgets.egg-info/not-zip-safe
```

### Comparing `ipywidgets-8.0.7/setup.cfg` & `ipywidgets-8.1.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 	Framework :: Jupyter
 
 [options]
 python_requires = >=3.7
 zip_safe = False
 packages = find:
 install_requires = 
-	ipykernel>=4.5.1
+	comm>=0.1.3
 	ipython>=6.1.0
 	traitlets>=4.3.1
 	widgetsnbextension~=4.0.7
 	jupyterlab_widgets~=3.0.7
 
 [options.extras_require]
 test =
```

