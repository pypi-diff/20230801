# Comparing `tmp/streamlit_extras-0.2.7.tar.gz` & `tmp/streamlit_extras-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_extras-0.2.7.tar", max compression
+gzip compressed data, was "streamlit_extras-0.3.0.tar", max compression
```

## Comparing `streamlit_extras-0.2.7.tar` & `streamlit_extras-0.3.0.tar`

### file list

```diff
@@ -1,40 +1,46 @@
--rw-r--r--   0        0        0    11357 2023-04-03 14:33:38.260281 streamlit_extras-0.2.7/LICENSE
--rw-r--r--   0        0        0     2675 2023-04-03 14:33:38.260281 streamlit_extras-0.2.7/README.md
--rw-r--r--   0        0        0     2038 2023-04-03 14:33:38.264281 streamlit_extras-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     1599 2023-04-03 14:33:38.264281 streamlit_extras-0.2.7/src/streamlit_extras/__init__.py
--rw-r--r--   0        0        0      751 2023-04-03 14:33:38.264281 streamlit_extras-0.2.7/src/streamlit_extras/add_vertical_space/__init__.py
--rw-r--r--   0        0        0    15296 2023-04-03 14:33:38.264281 streamlit_extras-0.2.7/src/streamlit_extras/altex/__init__.py
--rw-r--r--   0        0        0     1003 2023-04-03 14:33:38.264281 streamlit_extras-0.2.7/src/streamlit_extras/annotated_text/__init__.py
--rw-r--r--   0        0        0     1507 2023-04-03 14:33:38.264281 streamlit_extras-0.2.7/src/streamlit_extras/app_logo/__init__.py
--rw-r--r--   0        0        0     3590 2023-04-03 14:33:38.264281 streamlit_extras-0.2.7/src/streamlit_extras/badges/__init__.py
--rw-r--r--   0        0        0     1929 2023-04-03 14:33:38.264281 streamlit_extras-0.2.7/src/streamlit_extras/buy_me_a_coffee/__init__.py
--rw-r--r--   0        0        0      814 2023-04-03 14:33:38.264281 streamlit_extras-0.2.7/src/streamlit_extras/camera_input_live/__init__.py
--rw-r--r--   0        0        0      699 2023-04-03 14:33:38.264281 streamlit_extras-0.2.7/src/streamlit_extras/card/__init__.py
--rw-r--r--   0        0        0     5263 2023-04-03 14:33:38.264281 streamlit_extras-0.2.7/src/streamlit_extras/chart_annotations/__init__.py
--rw-r--r--   0        0        0     5742 2023-04-03 14:33:38.264281 streamlit_extras-0.2.7/src/streamlit_extras/chart_container/__init__.py
--rw-r--r--   0        0        0     4428 2023-04-03 14:33:38.264281 streamlit_extras-0.2.7/src/streamlit_extras/colored_header/__init__.py
--rw-r--r--   0        0        0      761 2023-04-03 14:33:38.264281 streamlit_extras-0.2.7/src/streamlit_extras/customize_running/__init__.py
--rw-r--r--   0        0        0     8840 2023-04-03 14:33:38.264281 streamlit_extras-0.2.7/src/streamlit_extras/dataframe_explorer/__init__.py
--rw-r--r--   0        0        0     3505 2023-04-03 14:33:38.264281 streamlit_extras-0.2.7/src/streamlit_extras/echo_expander/__init__.py
--rw-r--r--   0        0        0     1732 2023-04-03 14:33:38.264281 streamlit_extras-0.2.7/src/streamlit_extras/embed_code/__init__.py
--rw-r--r--   0        0        0      702 2023-04-03 14:33:38.264281 streamlit_extras-0.2.7/src/streamlit_extras/faker/__init__.py
--rw-r--r--   0        0        0     4817 2023-04-03 14:33:38.264281 streamlit_extras-0.2.7/src/streamlit_extras/function_explorer/__init__.py
--rw-r--r--   0        0        0      790 2023-04-03 14:33:38.264281 streamlit_extras-0.2.7/src/streamlit_extras/image_coordinates/__init__.py
--rw-r--r--   0        0        0     2407 2023-04-03 14:33:38.264281 streamlit_extras-0.2.7/src/streamlit_extras/image_in_tables/__init__.py
--rw-r--r--   0        0        0     1539 2023-04-03 14:33:38.264281 streamlit_extras-0.2.7/src/streamlit_extras/keyboard_text/__init__.py
--rw-r--r--   0        0        0     2329 2023-04-03 14:33:38.264281 streamlit_extras-0.2.7/src/streamlit_extras/keyboard_url/__init__.py
--rw-r--r--   0        0        0     4808 2023-04-03 14:33:38.264281 streamlit_extras-0.2.7/src/streamlit_extras/let_it_rain/__init__.py
--rw-r--r--   0        0        0     2218 2023-04-03 14:33:38.264281 streamlit_extras-0.2.7/src/streamlit_extras/mandatory_date_range/__init__.py
--rw-r--r--   0        0        0     1703 2023-04-03 14:33:38.264281 streamlit_extras-0.2.7/src/streamlit_extras/markdownlit/__init__.py
--rw-r--r--   0        0        0     3450 2023-04-03 14:33:38.264281 streamlit_extras-0.2.7/src/streamlit_extras/mention/__init__.py
--rw-r--r--   0        0        0     1712 2023-04-03 14:33:38.264281 streamlit_extras-0.2.7/src/streamlit_extras/metric_cards/__init__.py
--rw-r--r--   0        0        0     2674 2023-04-03 14:33:38.264281 streamlit_extras-0.2.7/src/streamlit_extras/no_default_selectbox/__init__.py
--rw-r--r--   0        0        0      908 2023-04-03 14:33:38.264281 streamlit_extras-0.2.7/src/streamlit_extras/st_keyup/__init__.py
--rw-r--r--   0        0        0     1368 2023-04-03 14:33:38.264281 streamlit_extras-0.2.7/src/streamlit_extras/stateful_button/__init__.py
--rw-r--r--   0        0        0     2132 2023-04-03 14:33:38.264281 streamlit_extras-0.2.7/src/streamlit_extras/stodo/__init__.py
--rw-r--r--   0        0        0      996 2023-04-03 14:33:38.264281 streamlit_extras-0.2.7/src/streamlit_extras/stoggle/__init__.py
--rw-r--r--   0        0        0     1579 2023-04-03 14:33:38.264281 streamlit_extras-0.2.7/src/streamlit_extras/switch_page_button/__init__.py
--rw-r--r--   0        0        0     1046 2023-04-03 14:33:38.264281 streamlit_extras-0.2.7/src/streamlit_extras/toggle_switch/__init__.py
--rw-r--r--   0        0        0     1058 2023-04-03 14:33:38.264281 streamlit_extras-0.2.7/src/streamlit_extras/vertical_slider/__init__.py
--rw-r--r--   0        0        0     2058 2023-04-03 14:33:38.264281 streamlit_extras-0.2.7/src/streamlit_extras/word_importances/__init__.py
--rw-r--r--   0        0        0     3933 1970-01-01 00:00:00.000000 streamlit_extras-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-01 15:02:55.884169 streamlit_extras-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2675 2023-08-01 15:02:55.884169 streamlit_extras-0.3.0/README.md
+-rw-r--r--   0        0        0     2038 2023-08-01 15:02:55.888170 streamlit_extras-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1599 2023-08-01 15:02:55.888170 streamlit_extras-0.3.0/src/streamlit_extras/__init__.py
+-rw-r--r--   0        0        0      751 2023-08-01 15:02:55.888170 streamlit_extras-0.3.0/src/streamlit_extras/add_vertical_space/__init__.py
+-rw-r--r--   0        0        0    15296 2023-08-01 15:02:55.888170 streamlit_extras-0.3.0/src/streamlit_extras/altex/__init__.py
+-rw-r--r--   0        0        0     1003 2023-08-01 15:02:55.888170 streamlit_extras-0.3.0/src/streamlit_extras/annotated_text/__init__.py
+-rw-r--r--   0        0        0     1507 2023-08-01 15:02:55.888170 streamlit_extras-0.3.0/src/streamlit_extras/app_logo/__init__.py
+-rw-r--r--   0        0        0     3590 2023-08-01 15:02:55.888170 streamlit_extras-0.3.0/src/streamlit_extras/badges/__init__.py
+-rw-r--r--   0        0        0     1929 2023-08-01 15:02:55.888170 streamlit_extras-0.3.0/src/streamlit_extras/buy_me_a_coffee/__init__.py
+-rw-r--r--   0        0        0      814 2023-08-01 15:02:55.888170 streamlit_extras-0.3.0/src/streamlit_extras/camera_input_live/__init__.py
+-rw-r--r--   0        0        0      699 2023-08-01 15:02:55.888170 streamlit_extras-0.3.0/src/streamlit_extras/card/__init__.py
+-rw-r--r--   0        0        0     5263 2023-08-01 15:02:55.888170 streamlit_extras-0.3.0/src/streamlit_extras/chart_annotations/__init__.py
+-rw-r--r--   0        0        0     5742 2023-08-01 15:02:55.888170 streamlit_extras-0.3.0/src/streamlit_extras/chart_container/__init__.py
+-rw-r--r--   0        0        0     4428 2023-08-01 15:02:55.888170 streamlit_extras-0.3.0/src/streamlit_extras/colored_header/__init__.py
+-rw-r--r--   0        0        0      761 2023-08-01 15:02:55.888170 streamlit_extras-0.3.0/src/streamlit_extras/customize_running/__init__.py
+-rw-r--r--   0        0        0     8840 2023-08-01 15:02:55.888170 streamlit_extras-0.3.0/src/streamlit_extras/dataframe_explorer/__init__.py
+-rw-r--r--   0        0        0     3505 2023-08-01 15:02:55.888170 streamlit_extras-0.3.0/src/streamlit_extras/echo_expander/__init__.py
+-rw-r--r--   0        0        0     1732 2023-08-01 15:02:55.888170 streamlit_extras-0.3.0/src/streamlit_extras/embed_code/__init__.py
+-rw-r--r--   0        0        0      702 2023-08-01 15:02:55.888170 streamlit_extras-0.3.0/src/streamlit_extras/faker/__init__.py
+-rw-r--r--   0        0        0     4817 2023-08-01 15:02:55.888170 streamlit_extras-0.3.0/src/streamlit_extras/function_explorer/__init__.py
+-rw-r--r--   0        0        0     5581 2023-08-01 15:02:55.888170 streamlit_extras-0.3.0/src/streamlit_extras/grid/__init__.py
+-rw-r--r--   0        0        0      790 2023-08-01 15:02:55.888170 streamlit_extras-0.3.0/src/streamlit_extras/image_coordinates/__init__.py
+-rw-r--r--   0        0        0     2407 2023-08-01 15:02:55.888170 streamlit_extras-0.3.0/src/streamlit_extras/image_in_tables/__init__.py
+-rw-r--r--   0        0        0     1539 2023-08-01 15:02:55.888170 streamlit_extras-0.3.0/src/streamlit_extras/keyboard_text/__init__.py
+-rw-r--r--   0        0        0     2329 2023-08-01 15:02:55.888170 streamlit_extras-0.3.0/src/streamlit_extras/keyboard_url/__init__.py
+-rw-r--r--   0        0        0     4808 2023-08-01 15:02:55.888170 streamlit_extras-0.3.0/src/streamlit_extras/let_it_rain/__init__.py
+-rw-r--r--   0        0        0     2218 2023-08-01 15:02:55.888170 streamlit_extras-0.3.0/src/streamlit_extras/mandatory_date_range/__init__.py
+-rw-r--r--   0        0        0     1703 2023-08-01 15:02:55.888170 streamlit_extras-0.3.0/src/streamlit_extras/markdownlit/__init__.py
+-rw-r--r--   0        0        0     3450 2023-08-01 15:02:55.888170 streamlit_extras-0.3.0/src/streamlit_extras/mention/__init__.py
+-rw-r--r--   0        0        0     1712 2023-08-01 15:02:55.888170 streamlit_extras-0.3.0/src/streamlit_extras/metric_cards/__init__.py
+-rw-r--r--   0        0        0     2674 2023-08-01 15:02:55.888170 streamlit_extras-0.3.0/src/streamlit_extras/no_default_selectbox/__init__.py
+-rw-r--r--   0        0        0     3248 2023-08-01 15:02:55.888170 streamlit_extras-0.3.0/src/streamlit_extras/row/__init__.py
+-rw-r--r--   0        0        0     5177 2023-08-01 15:02:55.888170 streamlit_extras-0.3.0/src/streamlit_extras/sandbox/__init__.py
+-rw-r--r--   0        0        0      908 2023-08-01 15:02:55.888170 streamlit_extras-0.3.0/src/streamlit_extras/st_keyup/__init__.py
+-rw-r--r--   0        0        0     1368 2023-08-01 15:02:55.888170 streamlit_extras-0.3.0/src/streamlit_extras/stateful_button/__init__.py
+-rw-r--r--   0        0        0     4288 2023-08-01 15:02:55.888170 streamlit_extras-0.3.0/src/streamlit_extras/stateful_chat/__init__.py
+-rw-r--r--   0        0        0     2132 2023-08-01 15:02:55.888170 streamlit_extras-0.3.0/src/streamlit_extras/stodo/__init__.py
+-rw-r--r--   0        0        0      996 2023-08-01 15:02:55.888170 streamlit_extras-0.3.0/src/streamlit_extras/stoggle/__init__.py
+-rw-r--r--   0        0        0     4878 2023-08-01 15:02:55.888170 streamlit_extras-0.3.0/src/streamlit_extras/streaming_write/__init__.py
+-rw-r--r--   0        0        0     2529 2023-08-01 15:02:55.888170 streamlit_extras-0.3.0/src/streamlit_extras/stylable_container/__init__.py
+-rw-r--r--   0        0        0     1579 2023-08-01 15:02:55.888170 streamlit_extras-0.3.0/src/streamlit_extras/switch_page_button/__init__.py
+-rw-r--r--   0        0        0     1046 2023-08-01 15:02:55.888170 streamlit_extras-0.3.0/src/streamlit_extras/toggle_switch/__init__.py
+-rw-r--r--   0        0        0     1058 2023-08-01 15:02:55.888170 streamlit_extras-0.3.0/src/streamlit_extras/vertical_slider/__init__.py
+-rw-r--r--   0        0        0     2058 2023-08-01 15:02:55.888170 streamlit_extras-0.3.0/src/streamlit_extras/word_importances/__init__.py
+-rw-r--r--   0        0        0     3947 1970-01-01 00:00:00.000000 streamlit_extras-0.3.0/PKG-INFO
```

### Comparing `streamlit_extras-0.2.7/LICENSE` & `streamlit_extras-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.2.7/README.md` & `streamlit_extras-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.2.7/pyproject.toml` & `streamlit_extras-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "streamlit-extras"
-version = "0.2.7"
-license = "Apache 2.0"
+version = "0.3.0"
+license = "Apache-2.0"
 description = "A library to discover, try, install and share Streamlit extras"
 authors = ["Arnaud Miribel <arnaudmiribel@gmail.com>", "Zachary Blackwood <zachary@streamlit.io>"]
 readme = "README.md"
 packages = [{include = "streamlit_extras", from = "src"}]
 exclude = ["gallery/"]
 keywords = [
     "python",
```

### Comparing `streamlit_extras-0.2.7/src/streamlit_extras/__init__.py` & `streamlit_extras-0.3.0/src/streamlit_extras/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.2.7/src/streamlit_extras/add_vertical_space/__init__.py` & `streamlit_extras-0.3.0/src/streamlit_extras/add_vertical_space/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.2.7/src/streamlit_extras/altex/__init__.py` & `streamlit_extras-0.3.0/src/streamlit_extras/altex/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.2.7/src/streamlit_extras/annotated_text/__init__.py` & `streamlit_extras-0.3.0/src/streamlit_extras/annotated_text/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.2.7/src/streamlit_extras/app_logo/__init__.py` & `streamlit_extras-0.3.0/src/streamlit_extras/app_logo/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.2.7/src/streamlit_extras/badges/__init__.py` & `streamlit_extras-0.3.0/src/streamlit_extras/badges/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.2.7/src/streamlit_extras/buy_me_a_coffee/__init__.py` & `streamlit_extras-0.3.0/src/streamlit_extras/buy_me_a_coffee/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.2.7/src/streamlit_extras/camera_input_live/__init__.py` & `streamlit_extras-0.3.0/src/streamlit_extras/camera_input_live/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.2.7/src/streamlit_extras/card/__init__.py` & `streamlit_extras-0.3.0/src/streamlit_extras/card/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.2.7/src/streamlit_extras/chart_annotations/__init__.py` & `streamlit_extras-0.3.0/src/streamlit_extras/chart_annotations/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.2.7/src/streamlit_extras/chart_container/__init__.py` & `streamlit_extras-0.3.0/src/streamlit_extras/chart_container/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.2.7/src/streamlit_extras/colored_header/__init__.py` & `streamlit_extras-0.3.0/src/streamlit_extras/colored_header/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.2.7/src/streamlit_extras/customize_running/__init__.py` & `streamlit_extras-0.3.0/src/streamlit_extras/customize_running/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.2.7/src/streamlit_extras/dataframe_explorer/__init__.py` & `streamlit_extras-0.3.0/src/streamlit_extras/dataframe_explorer/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.2.7/src/streamlit_extras/echo_expander/__init__.py` & `streamlit_extras-0.3.0/src/streamlit_extras/echo_expander/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.2.7/src/streamlit_extras/embed_code/__init__.py` & `streamlit_extras-0.3.0/src/streamlit_extras/embed_code/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.2.7/src/streamlit_extras/faker/__init__.py` & `streamlit_extras-0.3.0/src/streamlit_extras/faker/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.2.7/src/streamlit_extras/function_explorer/__init__.py` & `streamlit_extras-0.3.0/src/streamlit_extras/function_explorer/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.2.7/src/streamlit_extras/image_coordinates/__init__.py` & `streamlit_extras-0.3.0/src/streamlit_extras/image_coordinates/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.2.7/src/streamlit_extras/image_in_tables/__init__.py` & `streamlit_extras-0.3.0/src/streamlit_extras/image_in_tables/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.2.7/src/streamlit_extras/keyboard_text/__init__.py` & `streamlit_extras-0.3.0/src/streamlit_extras/keyboard_text/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.2.7/src/streamlit_extras/keyboard_url/__init__.py` & `streamlit_extras-0.3.0/src/streamlit_extras/keyboard_url/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.2.7/src/streamlit_extras/let_it_rain/__init__.py` & `streamlit_extras-0.3.0/src/streamlit_extras/let_it_rain/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.2.7/src/streamlit_extras/mandatory_date_range/__init__.py` & `streamlit_extras-0.3.0/src/streamlit_extras/mandatory_date_range/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.2.7/src/streamlit_extras/markdownlit/__init__.py` & `streamlit_extras-0.3.0/src/streamlit_extras/markdownlit/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.2.7/src/streamlit_extras/mention/__init__.py` & `streamlit_extras-0.3.0/src/streamlit_extras/mention/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.2.7/src/streamlit_extras/metric_cards/__init__.py` & `streamlit_extras-0.3.0/src/streamlit_extras/metric_cards/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.2.7/src/streamlit_extras/no_default_selectbox/__init__.py` & `streamlit_extras-0.3.0/src/streamlit_extras/no_default_selectbox/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.2.7/src/streamlit_extras/st_keyup/__init__.py` & `streamlit_extras-0.3.0/src/streamlit_extras/st_keyup/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.2.7/src/streamlit_extras/stateful_button/__init__.py` & `streamlit_extras-0.3.0/src/streamlit_extras/stateful_button/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.2.7/src/streamlit_extras/stodo/__init__.py` & `streamlit_extras-0.3.0/src/streamlit_extras/stodo/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.2.7/src/streamlit_extras/stoggle/__init__.py` & `streamlit_extras-0.3.0/src/streamlit_extras/stoggle/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.2.7/src/streamlit_extras/switch_page_button/__init__.py` & `streamlit_extras-0.3.0/src/streamlit_extras/switch_page_button/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.2.7/src/streamlit_extras/toggle_switch/__init__.py` & `streamlit_extras-0.3.0/src/streamlit_extras/toggle_switch/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.2.7/src/streamlit_extras/vertical_slider/__init__.py` & `streamlit_extras-0.3.0/src/streamlit_extras/vertical_slider/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.2.7/src/streamlit_extras/word_importances/__init__.py` & `streamlit_extras-0.3.0/src/streamlit_extras/word_importances/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_extras-0.2.7/PKG-INFO` & `streamlit_extras-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: streamlit-extras
-Version: 0.2.7
+Version: 0.3.0
 Summary: A library to discover, try, install and share Streamlit extras
-License: Apache 2.0
+License: Apache-2.0
 Keywords: python,streamlit,ui,data
 Author: Arnaud Miribel
 Author-email: arnaudmiribel@gmail.com
 Requires-Python: >=3.8, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*
-Classifier: License :: Other/Proprietary License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: htbuilder (==0.6.1)
 Requires-Dist: markdownlit (>=0.0.5)
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: streamlit-extras Version: 0.2.7 Summary: A library
-to discover, try, install and share Streamlit extras License: Apache 2.0
+Metadata-Version: 2.1 Name: streamlit-extras Version: 0.3.0 Summary: A library
+to discover, try, install and share Streamlit extras License: Apache-2.0
 Keywords: python,streamlit,ui,data Author: Arnaud Miribel Author-email:
 arnaudmiribel@gmail.com Requires-Python: >=3.8, !=2.7.*, !=3.0.*, !=3.1.*,
-!=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.* Classifier: License ::
-Other/Proprietary License Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+!=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.* Classifier: License :: OSI
+Approved :: Apache Software License Classifier: Programming Language :: Python
+:: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: htbuilder
 (==0.6.1) Requires-Dist: markdownlit (>=0.0.5) Requires-Dist: protobuf
 (!=3.20.2) Requires-Dist: st-annotated-text (>=3.0.0) Requires-Dist: streamlit
 (>=1.0.0) Requires-Dist: streamlit-camera-input-live (>=0.2.0) Requires-Dist:
 streamlit-card (>=0.0.4) Requires-Dist: streamlit-embedcode (>=0.1.2) Requires-
 Dist: streamlit-faker (>=0.0.2) Requires-Dist: streamlit-image-coordinates
```

