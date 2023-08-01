# Comparing `tmp/htmx-components-flask-0.0.1.tar.gz` & `tmp/htmx-components-flask-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htmx-components-flask-0.0.1.tar", last modified: Wed Jul 26 00:11:10 2023, max compression
+gzip compressed data, was "htmx-components-flask-0.0.2.tar", last modified: Tue Aug  1 21:45:26 2023, max compression
```

## Comparing `htmx-components-flask-0.0.1.tar` & `htmx-components-flask-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-07-26 00:11:10.430963 htmx-components-flask-0.0.1/
--rw-rw-r--   0 neil      (1000) neil      (1000)       43 2023-07-25 23:16:29.000000 htmx-components-flask-0.0.1/.gitignore
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-07-26 00:11:10.422963 htmx-components-flask-0.0.1/.vscode/
--rw-rw-r--   0 neil      (1000) neil      (1000)       68 2023-07-25 23:09:12.000000 htmx-components-flask-0.0.1/.vscode/settings.json
--rw-rw-r--   0 neil      (1000) neil      (1000)     1070 2023-07-25 23:06:16.000000 htmx-components-flask-0.0.1/LICENSE
--rw-rw-r--   0 neil      (1000) neil      (1000)      260 2023-07-26 00:11:10.430963 htmx-components-flask-0.0.1/PKG-INFO
--rw-rw-r--   0 neil      (1000) neil      (1000)       75 2023-07-25 23:57:15.000000 htmx-components-flask-0.0.1/README.md
--rw-rw-r--   0 neil      (1000) neil      (1000)      351 2023-07-26 00:10:42.000000 htmx-components-flask-0.0.1/pyproject.toml
--rw-rw-r--   0 neil      (1000) neil      (1000)       38 2023-07-26 00:11:10.430963 htmx-components-flask-0.0.1/setup.cfg
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-07-26 00:11:10.418963 htmx-components-flask-0.0.1/src/
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-07-26 00:11:10.422963 htmx-components-flask-0.0.1/src/htmx_components_flask/
--rw-rw-r--   0 neil      (1000) neil      (1000)     1087 2023-07-25 23:52:56.000000 htmx-components-flask-0.0.1/src/htmx_components_flask/__init__.py
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-07-26 00:11:10.418963 htmx-components-flask-0.0.1/src/htmx_components_flask/templates/
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-07-26 00:11:10.426963 htmx-components-flask-0.0.1/src/htmx_components_flask/templates/htmx_components_flask/
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-07-26 00:11:10.430963 htmx-components-flask-0.0.1/src/htmx_components_flask/templates/htmx_components_flask/form/
--rw-rw-r--   0 neil      (1000) neil      (1000)       89 2023-07-25 23:51:56.000000 htmx-components-flask-0.0.1/src/htmx_components_flask/templates/htmx_components_flask/form/description.html
--rw-rw-r--   0 neil      (1000) neil      (1000)       92 2023-07-25 23:51:59.000000 htmx-components-flask-0.0.1/src/htmx_components_flask/templates/htmx_components_flask/form/errors.html
--rw-rw-r--   0 neil      (1000) neil      (1000)     2674 2023-07-25 23:56:48.000000 htmx-components-flask-0.0.1/src/htmx_components_flask/templates/htmx_components_flask/form/horizontal.html
--rw-rw-r--   0 neil      (1000) neil      (1000)     1048 2023-07-25 23:36:03.000000 htmx-components-flask-0.0.1/src/htmx_components_flask/templates/htmx_components_flask/pager.html
--rw-rw-r--   0 neil      (1000) neil      (1000)      380 2023-07-25 23:35:59.000000 htmx-components-flask-0.0.1/src/htmx_components_flask/templates/htmx_components_flask/sortlink.html
--rw-rw-r--   0 neil      (1000) neil      (1000)     2969 2023-07-25 23:36:30.000000 htmx-components-flask-0.0.1/src/htmx_components_flask/templates/htmx_components_flask/viewgrid.html
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-07-26 00:11:10.426963 htmx-components-flask-0.0.1/src/htmx_components_flask.egg-info/
--rw-rw-r--   0 neil      (1000) neil      (1000)      260 2023-07-26 00:11:10.000000 htmx-components-flask-0.0.1/src/htmx_components_flask.egg-info/PKG-INFO
--rw-rw-r--   0 neil      (1000) neil      (1000)      794 2023-07-26 00:11:10.000000 htmx-components-flask-0.0.1/src/htmx_components_flask.egg-info/SOURCES.txt
--rw-rw-r--   0 neil      (1000) neil      (1000)        1 2023-07-26 00:11:10.000000 htmx-components-flask-0.0.1/src/htmx_components_flask.egg-info/dependency_links.txt
--rw-rw-r--   0 neil      (1000) neil      (1000)       48 2023-07-26 00:11:10.000000 htmx-components-flask-0.0.1/src/htmx_components_flask.egg-info/requires.txt
--rw-rw-r--   0 neil      (1000) neil      (1000)       22 2023-07-26 00:11:10.000000 htmx-components-flask-0.0.1/src/htmx_components_flask.egg-info/top_level.txt
+drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-08-01 21:45:26.695448 htmx-components-flask-0.0.2/
+-rw-rw-r--   0 neil      (1000) neil      (1000)       50 2023-07-26 00:11:37.000000 htmx-components-flask-0.0.2/.gitignore
+drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-08-01 21:45:26.675448 htmx-components-flask-0.0.2/.vscode/
+-rw-rw-r--   0 neil      (1000) neil      (1000)       68 2023-07-25 23:09:12.000000 htmx-components-flask-0.0.2/.vscode/settings.json
+-rw-rw-r--   0 neil      (1000) neil      (1000)     1070 2023-07-25 23:06:16.000000 htmx-components-flask-0.0.2/LICENSE
+-rw-rw-r--   0 neil      (1000) neil      (1000)     1823 2023-08-01 21:45:26.691448 htmx-components-flask-0.0.2/PKG-INFO
+-rw-rw-r--   0 neil      (1000) neil      (1000)     1561 2023-08-01 20:43:29.000000 htmx-components-flask-0.0.2/README.md
+-rw-rw-r--   0 neil      (1000) neil      (1000)      434 2023-08-01 21:44:48.000000 htmx-components-flask-0.0.2/pyproject.toml
+-rw-rw-r--   0 neil      (1000) neil      (1000)       38 2023-08-01 21:45:26.695448 htmx-components-flask-0.0.2/setup.cfg
+drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-08-01 21:45:26.667448 htmx-components-flask-0.0.2/src/
+drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-08-01 21:45:26.679448 htmx-components-flask-0.0.2/src/htmx_components_flask/
+-rw-rw-r--   0 neil      (1000) neil      (1000)     1180 2023-08-01 20:42:25.000000 htmx-components-flask-0.0.2/src/htmx_components_flask/__init__.py
+drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-08-01 21:45:26.671448 htmx-components-flask-0.0.2/src/htmx_components_flask/templates/
+drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-08-01 21:45:26.687448 htmx-components-flask-0.0.2/src/htmx_components_flask/templates/htmx_components_flask/
+drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-08-01 21:45:26.691448 htmx-components-flask-0.0.2/src/htmx_components_flask/templates/htmx_components_flask/form/
+-rw-rw-r--   0 neil      (1000) neil      (1000)       89 2023-07-25 23:51:56.000000 htmx-components-flask-0.0.2/src/htmx_components_flask/templates/htmx_components_flask/form/description.html
+-rw-rw-r--   0 neil      (1000) neil      (1000)       92 2023-07-25 23:51:59.000000 htmx-components-flask-0.0.2/src/htmx_components_flask/templates/htmx_components_flask/form/errors.html
+-rw-rw-r--   0 neil      (1000) neil      (1000)     2674 2023-07-25 23:56:48.000000 htmx-components-flask-0.0.2/src/htmx_components_flask/templates/htmx_components_flask/form/horizontal.html
+-rw-rw-r--   0 neil      (1000) neil      (1000)     2969 2023-08-01 20:14:38.000000 htmx-components-flask-0.0.2/src/htmx_components_flask/templates/htmx_components_flask/gridview.html
+-rw-rw-r--   0 neil      (1000) neil      (1000)     1048 2023-07-25 23:36:03.000000 htmx-components-flask-0.0.2/src/htmx_components_flask/templates/htmx_components_flask/pager.html
+-rw-rw-r--   0 neil      (1000) neil      (1000)      380 2023-07-25 23:35:59.000000 htmx-components-flask-0.0.2/src/htmx_components_flask/templates/htmx_components_flask/sortlink.html
+-rw-rw-r--   0 neil      (1000) neil      (1000)     2744 2023-08-01 20:02:43.000000 htmx-components-flask-0.0.2/src/htmx_components_flask/templates/htmx_components_flask/treeview.html
+drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-08-01 21:45:26.683448 htmx-components-flask-0.0.2/src/htmx_components_flask.egg-info/
+-rw-rw-r--   0 neil      (1000) neil      (1000)     1823 2023-08-01 21:45:26.000000 htmx-components-flask-0.0.2/src/htmx_components_flask.egg-info/PKG-INFO
+-rw-rw-r--   0 neil      (1000) neil      (1000)      866 2023-08-01 21:45:26.000000 htmx-components-flask-0.0.2/src/htmx_components_flask.egg-info/SOURCES.txt
+-rw-rw-r--   0 neil      (1000) neil      (1000)        1 2023-08-01 21:45:26.000000 htmx-components-flask-0.0.2/src/htmx_components_flask.egg-info/dependency_links.txt
+-rw-rw-r--   0 neil      (1000) neil      (1000)       46 2023-08-01 21:45:26.000000 htmx-components-flask-0.0.2/src/htmx_components_flask.egg-info/requires.txt
+-rw-rw-r--   0 neil      (1000) neil      (1000)       22 2023-08-01 21:45:26.000000 htmx-components-flask-0.0.2/src/htmx_components_flask.egg-info/top_level.txt
```

### Comparing `htmx-components-flask-0.0.1/LICENSE` & `htmx-components-flask-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `htmx-components-flask-0.0.1/src/htmx_components_flask/__init__.py` & `htmx-components-flask-0.0.2/src/htmx_components_flask/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 from lxml import etree, html
 
 htmx_components_flask = Blueprint(
     "htmx_components_flask", __name__, template_folder="templates"
 )
 
 
+@htmx_components_flask.app_context_processor
+def jinja_globals():
+    return dict(int=int)
+
+
 @htmx_components_flask.app_template_filter("url_encode")
 def url_encode(s: str) -> str:
     return werkzeug.urls.url_encode(s)
 
 
 @htmx_components_flask.app_template_filter("partition")
 def partition(value: str, missing: str, sep: str = ",") -> tuple[str, str]:
```

### Comparing `htmx-components-flask-0.0.1/src/htmx_components_flask/templates/htmx_components_flask/form/horizontal.html` & `htmx-components-flask-0.0.2/src/htmx_components_flask/templates/htmx_components_flask/form/horizontal.html`

 * *Files identical despite different names*

### Comparing `htmx-components-flask-0.0.1/src/htmx_components_flask/templates/htmx_components_flask/pager.html` & `htmx-components-flask-0.0.2/src/htmx_components_flask/templates/htmx_components_flask/pager.html`

 * *Files identical despite different names*

### Comparing `htmx-components-flask-0.0.1/src/htmx_components_flask/templates/htmx_components_flask/viewgrid.html` & `htmx-components-flask-0.0.2/src/htmx_components_flask/templates/htmx_components_flask/gridview.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {# constants #}
 {% set prefix = grid_config.prefix %}
-{% set TABLE_ID = prefix~"viewgrid" %}
+{% set TABLE_ID = prefix~"gridview" %}
 {% set PAGE_PARAM = prefix~"page" %}
 {% set SEARCH_PARAM = prefix~"q" %}
 {% set SORT_PARAM = prefix~"sort" %}
 {% set SPINNER_ID = prefix~"spinner"%}
 
 
 {# state #}
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 {# constants #} {% set prefix = grid_config.prefix %} {% set TABLE_ID =
-prefix~"viewgrid" %} {% set PAGE_PARAM = prefix~"page" %} {% set SEARCH_PARAM =
+prefix~"gridview" %} {% set PAGE_PARAM = prefix~"page" %} {% set SEARCH_PARAM =
 prefix~"q" %} {% set SORT_PARAM = prefix~"sort" %} {% set SPINNER_ID =
 prefix~"spinner"%} {# state #} {% set q = request.args.get(SEARCH_PARAM, "") %}
 {% set page = request.args.get(PAGE_PARAM, 1)|int%} {% set sorts =
 request.args.getlist(SORT_PARAM)|map("partition", "asc")|list%} {% set records,
 total_pages = grid_config.get_records(page=page, sorts=sorts, q=q) %} {% set
 columns = grid_config.columns %} {% set search_args = request.args.copy() %} {%
 set _ = search_args.pop(SEARCH_PARAM,None) %} {% set _ = search_args.pop
```

### Comparing `htmx-components-flask-0.0.1/src/htmx_components_flask.egg-info/SOURCES.txt` & `htmx-components-flask-0.0.2/src/htmx_components_flask.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -5,13 +5,14 @@
 .vscode/settings.json
 src/htmx_components_flask/__init__.py
 src/htmx_components_flask.egg-info/PKG-INFO
 src/htmx_components_flask.egg-info/SOURCES.txt
 src/htmx_components_flask.egg-info/dependency_links.txt
 src/htmx_components_flask.egg-info/requires.txt
 src/htmx_components_flask.egg-info/top_level.txt
+src/htmx_components_flask/templates/htmx_components_flask/gridview.html
 src/htmx_components_flask/templates/htmx_components_flask/pager.html
 src/htmx_components_flask/templates/htmx_components_flask/sortlink.html
-src/htmx_components_flask/templates/htmx_components_flask/viewgrid.html
+src/htmx_components_flask/templates/htmx_components_flask/treeview.html
 src/htmx_components_flask/templates/htmx_components_flask/form/description.html
 src/htmx_components_flask/templates/htmx_components_flask/form/errors.html
 src/htmx_components_flask/templates/htmx_components_flask/form/horizontal.html
```

