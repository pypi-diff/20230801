# Comparing `tmp/wagtailcodeblock-1.29.0.0.tar.gz` & `tmp/wagtailcodeblock-1.29.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtailcodeblock-1.29.0.0.tar", last modified: Sun Mar  5 17:43:31 2023, max compression
+gzip compressed data, was "/var/www-dev/tallen/wagtailcodeblock/dist/.tmp-lx92f_wj/wagtailcodeblock-1.29.0.1.tar", last modified: Tue Aug  1 13:35:32 2023, max compression
```

## Comparing `wagtailcodeblock-1.29.0.0.tar` & `wagtailcodeblock-1.29.0.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 tallen    (1000) tallen    (1000)        0 2023-03-05 17:43:31.720853 wagtailcodeblock-1.29.0.0/
--rw-r--r--   0 tallen    (1000) tallen    (1000)       76 2023-03-04 15:11:37.000000 wagtailcodeblock-1.29.0.0/.coveragerc
--rw-r--r--   0 tallen    (1000) tallen    (1000)      581 2023-03-04 15:11:37.000000 wagtailcodeblock-1.29.0.0/.gitignore
--rw-r--r--   0 tallen    (1000) tallen    (1000)     1539 2023-03-04 15:11:37.000000 wagtailcodeblock-1.29.0.0/LICENSE
--rw-r--r--   0 tallen    (1000) tallen    (1000)    11771 2023-03-05 17:43:31.720853 wagtailcodeblock-1.29.0.0/PKG-INFO
--rw-r--r--   0 tallen    (1000) tallen    (1000)    10495 2023-03-04 16:14:56.000000 wagtailcodeblock-1.29.0.0/README.md
--rw-r--r--   0 tallen    (1000) tallen    (1000)     1565 2023-03-05 17:38:08.000000 wagtailcodeblock-1.29.0.0/conftest.py
-drwxr-xr-x   0 tallen    (1000) tallen    (1000)        0 2023-03-05 17:43:31.710853 wagtailcodeblock-1.29.0.0/docs/
-drwxr-xr-x   0 tallen    (1000) tallen    (1000)        0 2023-03-05 17:43:31.720853 wagtailcodeblock-1.29.0.0/docs/img/
--rw-r--r--   0 tallen    (1000) tallen    (1000)    86480 2023-03-04 16:17:13.000000 wagtailcodeblock-1.29.0.0/docs/img/screenshot-editor.png
--rwxr-xr-x   0 tallen    (1000) tallen    (1000)      625 2023-03-04 15:11:37.000000 wagtailcodeblock-1.29.0.0/manage.py
--rw-r--r--   0 tallen    (1000) tallen    (1000)     1434 2023-03-04 16:25:56.000000 wagtailcodeblock-1.29.0.0/pyproject.toml
--rw-r--r--   0 tallen    (1000) tallen    (1000)      117 2023-03-04 15:11:37.000000 wagtailcodeblock-1.29.0.0/pytest.ini
--rw-r--r--   0 tallen    (1000) tallen    (1000)       58 2023-03-04 15:11:37.000000 wagtailcodeblock-1.29.0.0/requirements_test.txt
--rw-r--r--   0 tallen    (1000) tallen    (1000)       38 2023-03-05 17:43:31.720853 wagtailcodeblock-1.29.0.0/setup.cfg
-drwxr-xr-x   0 tallen    (1000) tallen    (1000)        0 2023-03-05 17:43:31.720853 wagtailcodeblock-1.29.0.0/tests/
--rw-r--r--   0 tallen    (1000) tallen    (1000)        0 2023-03-04 15:11:37.000000 wagtailcodeblock-1.29.0.0/tests/__init__.py
-drwxr-xr-x   0 tallen    (1000) tallen    (1000)        0 2023-03-05 17:43:31.720853 wagtailcodeblock-1.29.0.0/tests/migrations/
--rw-r--r--   0 tallen    (1000) tallen    (1000)     3041 2023-03-04 15:11:37.000000 wagtailcodeblock-1.29.0.0/tests/migrations/0001_initial.py
--rw-r--r--   0 tallen    (1000) tallen    (1000)        0 2023-03-04 15:11:37.000000 wagtailcodeblock-1.29.0.0/tests/migrations/__init__.py
--rw-r--r--   0 tallen    (1000) tallen    (1000)      501 2023-03-04 15:11:37.000000 wagtailcodeblock-1.29.0.0/tests/models.py
--rw-r--r--   0 tallen    (1000) tallen    (1000)     1677 2023-03-04 15:11:37.000000 wagtailcodeblock-1.29.0.0/tests/settings.py
--rw-r--r--   0 tallen    (1000) tallen    (1000)      291 2023-03-05 17:38:08.000000 wagtailcodeblock-1.29.0.0/tests/test_blocks.py
--rw-r--r--   0 tallen    (1000) tallen    (1000)      368 2023-03-04 15:11:37.000000 wagtailcodeblock-1.29.0.0/tests/urls.py
--rw-r--r--   0 tallen    (1000) tallen    (1000)      571 2023-03-05 17:38:08.000000 wagtailcodeblock-1.29.0.0/tox.ini
-drwxr-xr-x   0 tallen    (1000) tallen    (1000)        0 2023-03-05 17:43:31.720853 wagtailcodeblock-1.29.0.0/wagtailcodeblock/
--rw-r--r--   0 tallen    (1000) tallen    (1000)        0 2023-03-04 15:11:37.000000 wagtailcodeblock-1.29.0.0/wagtailcodeblock/__init__.py
--rw-r--r--   0 tallen    (1000) tallen    (1000)      167 2023-03-05 17:43:31.000000 wagtailcodeblock-1.29.0.0/wagtailcodeblock/_version.py
--rw-r--r--   0 tallen    (1000) tallen    (1000)     3004 2023-03-04 15:11:37.000000 wagtailcodeblock-1.29.0.0/wagtailcodeblock/blocks.py
--rw-r--r--   0 tallen    (1000) tallen    (1000)     1147 2023-03-05 17:38:23.000000 wagtailcodeblock-1.29.0.0/wagtailcodeblock/settings.py
-drwxr-xr-x   0 tallen    (1000) tallen    (1000)        0 2023-03-05 17:43:31.720853 wagtailcodeblock-1.29.0.0/wagtailcodeblock/static/
-drwxr-xr-x   0 tallen    (1000) tallen    (1000)        0 2023-03-05 17:43:31.720853 wagtailcodeblock-1.29.0.0/wagtailcodeblock/static/wagtailcodeblock/
-drwxr-xr-x   0 tallen    (1000) tallen    (1000)        0 2023-03-05 17:43:31.720853 wagtailcodeblock-1.29.0.0/wagtailcodeblock/static/wagtailcodeblock/css/
--rw-r--r--   0 tallen    (1000) tallen    (1000)      256 2023-03-04 15:11:37.000000 wagtailcodeblock-1.29.0.0/wagtailcodeblock/static/wagtailcodeblock/css/wagtail-code-block.css
--rw-r--r--   0 tallen    (1000) tallen    (1000)      190 2023-03-04 15:11:37.000000 wagtailcodeblock-1.29.0.0/wagtailcodeblock/static/wagtailcodeblock/css/wagtail-code-block.min.css
-drwxr-xr-x   0 tallen    (1000) tallen    (1000)        0 2023-03-05 17:43:31.720853 wagtailcodeblock-1.29.0.0/wagtailcodeblock/static/wagtailcodeblock/js/
--rw-r--r--   0 tallen    (1000) tallen    (1000)     1303 2023-03-04 15:11:37.000000 wagtailcodeblock-1.29.0.0/wagtailcodeblock/static/wagtailcodeblock/js/wagtailcodeblock.js
-drwxr-xr-x   0 tallen    (1000) tallen    (1000)        0 2023-03-05 17:43:31.720853 wagtailcodeblock-1.29.0.0/wagtailcodeblock/templates/
-drwxr-xr-x   0 tallen    (1000) tallen    (1000)        0 2023-03-05 17:43:31.720853 wagtailcodeblock-1.29.0.0/wagtailcodeblock/templates/wagtailcodeblock/
--rwxr-xr-x   0 tallen    (1000) tallen    (1000)     2496 2023-03-04 15:11:37.000000 wagtailcodeblock-1.29.0.0/wagtailcodeblock/templates/wagtailcodeblock/code_block.html
--rwxr-xr-x   0 tallen    (1000) tallen    (1000)     1344 2023-03-04 15:11:37.000000 wagtailcodeblock-1.29.0.0/wagtailcodeblock/templates/wagtailcodeblock/code_block_form.html
--rw-r--r--   0 tallen    (1000) tallen    (1000)      166 2023-03-04 15:11:37.000000 wagtailcodeblock-1.29.0.0/wagtailcodeblock/templates/wagtailcodeblock/raw_code.html
-drwxr-xr-x   0 tallen    (1000) tallen    (1000)        0 2023-03-05 17:43:31.720853 wagtailcodeblock-1.29.0.0/wagtailcodeblock/templatetags/
--rw-r--r--   0 tallen    (1000) tallen    (1000)        0 2023-03-04 15:11:37.000000 wagtailcodeblock-1.29.0.0/wagtailcodeblock/templatetags/__init__.py
--rw-r--r--   0 tallen    (1000) tallen    (1000)     2693 2023-03-04 15:11:37.000000 wagtailcodeblock-1.29.0.0/wagtailcodeblock/templatetags/wagtailcodeblock_tags.py
--rw-r--r--   0 tallen    (1000) tallen    (1000)     1095 2023-03-04 15:11:37.000000 wagtailcodeblock-1.29.0.0/wagtailcodeblock/wagtail_hooks.py
-drwxr-xr-x   0 tallen    (1000) tallen    (1000)        0 2023-03-05 17:43:31.720853 wagtailcodeblock-1.29.0.0/wagtailcodeblock.egg-info/
--rw-r--r--   0 tallen    (1000) tallen    (1000)    11771 2023-03-05 17:43:31.000000 wagtailcodeblock-1.29.0.0/wagtailcodeblock.egg-info/PKG-INFO
--rw-r--r--   0 tallen    (1000) tallen    (1000)     1129 2023-03-05 17:43:31.000000 wagtailcodeblock-1.29.0.0/wagtailcodeblock.egg-info/SOURCES.txt
--rw-r--r--   0 tallen    (1000) tallen    (1000)        1 2023-03-05 17:43:31.000000 wagtailcodeblock-1.29.0.0/wagtailcodeblock.egg-info/dependency_links.txt
--rw-r--r--   0 tallen    (1000) tallen    (1000)       11 2023-03-05 17:43:31.000000 wagtailcodeblock-1.29.0.0/wagtailcodeblock.egg-info/requires.txt
--rw-r--r--   0 tallen    (1000) tallen    (1000)       17 2023-03-05 17:43:31.000000 wagtailcodeblock-1.29.0.0/wagtailcodeblock.egg-info/top_level.txt
+drwx------   0 tallen   (86646) wrds     (60359)        0 2023-08-01 13:35:32.334122 wagtailcodeblock-1.29.0.1/
+-rw-------   0 tallen   (86646) wrds     (60359)       76 2022-01-19 22:06:35.000000 wagtailcodeblock-1.29.0.1/.coveragerc
+-rw-------   0 tallen   (86646) wrds     (60359)      675 2023-07-27 13:28:51.000000 wagtailcodeblock-1.29.0.1/.gitignore
+-rw-------   0 tallen   (86646) wrds     (60359)     1539 2022-01-19 22:06:35.000000 wagtailcodeblock-1.29.0.1/LICENSE
+-rw-------   0 tallen   (86646) wrds     (60359)    11898 2023-08-01 13:35:32.333122 wagtailcodeblock-1.29.0.1/PKG-INFO
+-rw-------   0 tallen   (86646) wrds     (60359)    10495 2023-07-27 13:29:29.000000 wagtailcodeblock-1.29.0.1/README.md
+-rw-------   0 tallen   (86646) wrds     (60359)     1383 2023-07-27 13:29:29.000000 wagtailcodeblock-1.29.0.1/conftest.py
+drwx------   0 tallen   (86646) wrds     (60359)        0 2023-08-01 13:35:32.308122 wagtailcodeblock-1.29.0.1/docs/
+drwx------   0 tallen   (86646) wrds     (60359)        0 2023-08-01 13:35:32.316121 wagtailcodeblock-1.29.0.1/docs/img/
+-rw-------   0 tallen   (86646) wrds     (60359)    86480 2023-07-27 13:29:29.000000 wagtailcodeblock-1.29.0.1/docs/img/screenshot-editor.png
+-rwx------   0 tallen   (86646) wrds     (60359)      625 2022-01-19 22:06:35.000000 wagtailcodeblock-1.29.0.1/manage.py
+-rw-------   0 tallen   (86646) wrds     (60359)     1612 2023-08-01 13:22:50.000000 wagtailcodeblock-1.29.0.1/pyproject.toml
+-rw-------   0 tallen   (86646) wrds     (60359)      117 2022-01-19 22:06:35.000000 wagtailcodeblock-1.29.0.1/pytest.ini
+-rw-------   0 tallen   (86646) wrds     (60359)       58 2022-05-23 14:46:50.000000 wagtailcodeblock-1.29.0.1/requirements_test.txt
+-rw-------   0 tallen   (86646) wrds     (60359)       38 2023-08-01 13:35:32.334122 wagtailcodeblock-1.29.0.1/setup.cfg
+drwx------   0 tallen   (86646) wrds     (60359)        0 2023-08-01 13:35:32.317122 wagtailcodeblock-1.29.0.1/tests/
+-rw-------   0 tallen   (86646) wrds     (60359)        0 2022-05-23 14:05:24.000000 wagtailcodeblock-1.29.0.1/tests/__init__.py
+drwx------   0 tallen   (86646) wrds     (60359)        0 2023-08-01 13:35:32.317122 wagtailcodeblock-1.29.0.1/tests/migrations/
+-rw-------   0 tallen   (86646) wrds     (60359)     3041 2022-05-23 13:31:16.000000 wagtailcodeblock-1.29.0.1/tests/migrations/0001_initial.py
+-rw-------   0 tallen   (86646) wrds     (60359)        0 2022-01-19 22:06:35.000000 wagtailcodeblock-1.29.0.1/tests/migrations/__init__.py
+-rw-------   0 tallen   (86646) wrds     (60359)      587 2023-07-25 19:54:27.000000 wagtailcodeblock-1.29.0.1/tests/models.py
+-rw-------   0 tallen   (86646) wrds     (60359)     1705 2023-07-25 19:47:55.000000 wagtailcodeblock-1.29.0.1/tests/settings.py
+-rw-------   0 tallen   (86646) wrds     (60359)      291 2023-07-27 13:29:29.000000 wagtailcodeblock-1.29.0.1/tests/test_blocks.py
+-rw-------   0 tallen   (86646) wrds     (60359)      368 2022-05-23 13:31:16.000000 wagtailcodeblock-1.29.0.1/tests/urls.py
+-rw-------   0 tallen   (86646) wrds     (60359)      571 2023-07-27 13:29:29.000000 wagtailcodeblock-1.29.0.1/tox.ini
+drwx------   0 tallen   (86646) wrds     (60359)        0 2023-08-01 13:35:32.318122 wagtailcodeblock-1.29.0.1/wagtailcodeblock/
+-rw-------   0 tallen   (86646) wrds     (60359)        0 2022-01-19 22:06:35.000000 wagtailcodeblock-1.29.0.1/wagtailcodeblock/__init__.py
+-rw-------   0 tallen   (86646) wrds     (60359)      167 2023-08-01 13:35:32.000000 wagtailcodeblock-1.29.0.1/wagtailcodeblock/_version.py
+-rw-------   0 tallen   (86646) wrds     (60359)     3004 2022-05-23 13:31:16.000000 wagtailcodeblock-1.29.0.1/wagtailcodeblock/blocks.py
+-rw-------   0 tallen   (86646) wrds     (60359)     1147 2023-07-27 13:29:29.000000 wagtailcodeblock-1.29.0.1/wagtailcodeblock/settings.py
+drwx------   0 tallen   (86646) wrds     (60359)        0 2023-08-01 13:35:32.308122 wagtailcodeblock-1.29.0.1/wagtailcodeblock/static/
+drwx------   0 tallen   (86646) wrds     (60359)        0 2023-08-01 13:35:32.308122 wagtailcodeblock-1.29.0.1/wagtailcodeblock/static/wagtailcodeblock/
+drwx------   0 tallen   (86646) wrds     (60359)        0 2023-08-01 13:35:32.329122 wagtailcodeblock-1.29.0.1/wagtailcodeblock/static/wagtailcodeblock/css/
+-rw-------   0 tallen   (86646) wrds     (60359)      256 2022-01-19 22:06:35.000000 wagtailcodeblock-1.29.0.1/wagtailcodeblock/static/wagtailcodeblock/css/wagtail-code-block.css
+-rw-------   0 tallen   (86646) wrds     (60359)      190 2022-01-19 22:06:35.000000 wagtailcodeblock-1.29.0.1/wagtailcodeblock/static/wagtailcodeblock/css/wagtail-code-block.min.css
+drwx------   0 tallen   (86646) wrds     (60359)        0 2023-08-01 13:35:32.329122 wagtailcodeblock-1.29.0.1/wagtailcodeblock/static/wagtailcodeblock/js/
+-rw-------   0 tallen   (86646) wrds     (60359)     1303 2023-07-27 13:29:29.000000 wagtailcodeblock-1.29.0.1/wagtailcodeblock/static/wagtailcodeblock/js/wagtailcodeblock.js
+drwx------   0 tallen   (86646) wrds     (60359)        0 2023-08-01 13:35:32.308122 wagtailcodeblock-1.29.0.1/wagtailcodeblock/templates/
+drwx------   0 tallen   (86646) wrds     (60359)        0 2023-08-01 13:35:32.330122 wagtailcodeblock-1.29.0.1/wagtailcodeblock/templates/wagtailcodeblock/
+-rwx------   0 tallen   (86646) wrds     (60359)     2792 2023-08-01 13:19:58.000000 wagtailcodeblock-1.29.0.1/wagtailcodeblock/templates/wagtailcodeblock/code_block.html
+-rwx------   0 tallen   (86646) wrds     (60359)     1344 2022-01-19 22:06:35.000000 wagtailcodeblock-1.29.0.1/wagtailcodeblock/templates/wagtailcodeblock/code_block_form.html
+-rw-------   0 tallen   (86646) wrds     (60359)      166 2022-01-19 22:06:35.000000 wagtailcodeblock-1.29.0.1/wagtailcodeblock/templates/wagtailcodeblock/raw_code.html
+drwx------   0 tallen   (86646) wrds     (60359)        0 2023-08-01 13:35:32.333122 wagtailcodeblock-1.29.0.1/wagtailcodeblock/templatetags/
+-rw-------   0 tallen   (86646) wrds     (60359)        0 2022-01-19 22:06:35.000000 wagtailcodeblock-1.29.0.1/wagtailcodeblock/templatetags/__init__.py
+-rw-------   0 tallen   (86646) wrds     (60359)     2450 2023-08-01 13:19:58.000000 wagtailcodeblock-1.29.0.1/wagtailcodeblock/templatetags/wagtailcodeblock_tags.py
+-rw-------   0 tallen   (86646) wrds     (60359)     1095 2022-05-23 13:31:16.000000 wagtailcodeblock-1.29.0.1/wagtailcodeblock/wagtail_hooks.py
+drwx------   0 tallen   (86646) wrds     (60359)        0 2023-08-01 13:35:32.319121 wagtailcodeblock-1.29.0.1/wagtailcodeblock.egg-info/
+-rw-------   0 tallen   (86646) wrds     (60359)    11898 2023-08-01 13:35:32.000000 wagtailcodeblock-1.29.0.1/wagtailcodeblock.egg-info/PKG-INFO
+-rw-------   0 tallen   (86646) wrds     (60359)     1129 2023-08-01 13:35:32.000000 wagtailcodeblock-1.29.0.1/wagtailcodeblock.egg-info/SOURCES.txt
+-rw-------   0 tallen   (86646) wrds     (60359)        1 2023-08-01 13:35:32.000000 wagtailcodeblock-1.29.0.1/wagtailcodeblock.egg-info/dependency_links.txt
+-rw-------   0 tallen   (86646) wrds     (60359)       57 2023-08-01 13:35:32.000000 wagtailcodeblock-1.29.0.1/wagtailcodeblock.egg-info/requires.txt
+-rw-------   0 tallen   (86646) wrds     (60359)       17 2023-08-01 13:35:32.000000 wagtailcodeblock-1.29.0.1/wagtailcodeblock.egg-info/top_level.txt
```

### Comparing `wagtailcodeblock-1.29.0.0/LICENSE` & `wagtailcodeblock-1.29.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtailcodeblock-1.29.0.0/PKG-INFO` & `wagtailcodeblock-1.29.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtailcodeblock
-Version: 1.29.0.0
+Version: 1.29.0.1
 Summary: Wagtail Code Block provides PrismJS syntax highlighting in Wagtail.
 Author-email: Tim Allen <tallen@wharton.upenn.edu>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/FlipperPA/wagtailcodeblock
 Project-URL: Repository, https://github.com/FlipperPA/wagtailcodeblock
 Project-URL: Documentation, https://github.com/FlipperPA/wagtailcodeblock
 Keywords: wagtail,cms,contact,syntax,code,highlighting,highlighter
@@ -14,17 +14,20 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 3
+Classifier: Framework :: Wagtail :: 4
+Classifier: Framework :: Wagtail :: 5
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Wagtail Code Block
```

### Comparing `wagtailcodeblock-1.29.0.0/README.md` & `wagtailcodeblock-1.29.0.1/README.md`

 * *Files identical despite different names*

### Comparing `wagtailcodeblock-1.29.0.0/conftest.py` & `wagtailcodeblock-1.29.0.1/conftest.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,33 +9,31 @@
 
 
 @pytest.fixture
 def test_page(db):
     """
     Create a root page in the same way Wagtail does in migrations. See:
     https://github.com/wagtail/wagtail/blob/main/wagtail/core/migrations/0002_initial_data.py#L12  # noqa
-    """
-    """
-    We should created the home and vendor pages at the same time so they can be done in
-    any order, since both require a Site.
+
+    Then create the test page.
     """
     page_content_type, created = ContentType.objects.get_or_create(
         model="page", app_label="wagtailcore"
     )
-    # Locale.objects.create(language_code="en")
+
     root_page, created = Page.objects.get_or_create(
         title="Root",
         slug="root",
         content_type=page_content_type,
         path="0001",
         depth=1,
         numchild=1,
         url_path="/",
     )
-    # Create homepage
+
     test_page, created = CodeBlockPage.objects.get_or_create(
         # Required Wagtail Page fields
         title="TEST Wagtail Code Block Page",
         slug="wagtail-code-block",
         content_type=page_content_type,
         path="00010002",
         depth=2,
```

### Comparing `wagtailcodeblock-1.29.0.0/docs/img/screenshot-editor.png` & `wagtailcodeblock-1.29.0.1/docs/img/screenshot-editor.png`

 * *Files identical despite different names*

### Comparing `wagtailcodeblock-1.29.0.0/manage.py` & `wagtailcodeblock-1.29.0.1/manage.py`

 * *Files identical despite different names*

### Comparing `wagtailcodeblock-1.29.0.0/pyproject.toml` & `wagtailcodeblock-1.29.0.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools", "setuptools-scm"]
+requires = ["setuptools>=67", "setuptools_scm>=7", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 write_to = "wagtailcodeblock/_version.py"
 
 [project]
 name = "wagtailcodeblock"
@@ -11,33 +11,37 @@
     {name = "Tim Allen", email = "tallen@wharton.upenn.edu"},
 ]
 description = "Wagtail Code Block provides PrismJS syntax highlighting in Wagtail."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["wagtail", "cms", "contact", "syntax", "code", "highlighting", "highlighter"]
 license = {text = "BSD-3-Clause"}
-classifiers=[
+classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Framework :: Django",
     "Framework :: Wagtail",
     "Framework :: Wagtail :: 3",
+    "Framework :: Wagtail :: 4",
+    "Framework :: Wagtail :: 5",
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
 ]
 dependencies = [
-    "wagtail>=3",
+    "wagtail>=4",
+    'importlib-metadata; python_version<"3.8"',
 ]
 dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/FlipperPA/wagtailcodeblock"
 "Repository" = "https://github.com/FlipperPA/wagtailcodeblock"
 "Documentation" = "https://github.com/FlipperPA/wagtailcodeblock"
```

### Comparing `wagtailcodeblock-1.29.0.0/tests/migrations/0001_initial.py` & `wagtailcodeblock-1.29.0.1/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtailcodeblock-1.29.0.0/tests/settings.py` & `wagtailcodeblock-1.29.0.1/tests/settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from django.conf import settings
 
+WAGTAILADMIN_BASE_URL = "https://example.com"
+ALLOWED_HOSTS = ["*"]
 SECRET_KEY = "tests"
 DEBUG = True
 USE_TZ = True
 
 TEMPLATES = [
     {
         "BACKEND": "django.template.backends.django.DjangoTemplates",
@@ -41,15 +43,14 @@
     "django.middleware.security.SecurityMiddleware",
     "django.contrib.sessions.middleware.SessionMiddleware",
     "django.middleware.common.CommonMiddleware",
     "django.middleware.csrf.CsrfViewMiddleware",
     "django.contrib.auth.middleware.AuthenticationMiddleware",
     "django.contrib.messages.middleware.MessageMiddleware",
     "django.middleware.clickjacking.XFrameOptionsMiddleware",
-    "wagtail.middleware.SiteMiddleware",
 ]
 
 ROOT_URLCONF = "tests.urls"
 
 DATABASES = {
     "default": {"ENGINE": "django.db.backends.sqlite3", "NAME": "test_db.sqlite3"}
 }
```

### Comparing `wagtailcodeblock-1.29.0.0/tox.ini` & `wagtailcodeblock-1.29.0.1/tox.ini`

 * *Files identical despite different names*

### Comparing `wagtailcodeblock-1.29.0.0/wagtailcodeblock/blocks.py` & `wagtailcodeblock-1.29.0.1/wagtailcodeblock/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtailcodeblock-1.29.0.0/wagtailcodeblock/settings.py` & `wagtailcodeblock-1.29.0.1/wagtailcodeblock/settings.py`

 * *Files identical despite different names*

### Comparing `wagtailcodeblock-1.29.0.0/wagtailcodeblock/static/wagtailcodeblock/js/wagtailcodeblock.js` & `wagtailcodeblock-1.29.0.1/wagtailcodeblock/static/wagtailcodeblock/js/wagtailcodeblock.js`

 * *Files identical despite different names*

### Comparing `wagtailcodeblock-1.29.0.0/wagtailcodeblock/templates/wagtailcodeblock/code_block.html` & `wagtailcodeblock-1.29.0.1/wagtailcodeblock/templates/wagtailcodeblock/code_block.html`

 * *Files 10% similar despite different names*

```diff
@@ -9,19 +9,24 @@
             blocks on this page. This will ensure we only load the minimum payload. */
             if(typeof loadPrismLanguage != 'function') {
                 window.loadPrismLanguage = function(language) {
                     var libraries = [
                         {
                             "id": "code-block-prismjs",
                             "url": "//cdnjs.cloudflare.com/ajax/libs/prism/{% prism_version %}/prism.min.js"
-                        },
-                        {
-                            "id": "code-block-prismjs-" + language,
-                            "url": "//cdnjs.cloudflare.com/ajax/libs/prism/{% prism_version %}/components/prism-" + language + ".min.js"
                         }
+                        /*Since there is no html.min.js this check makes sure we
+                        bypass the loading of the script when syntax is set to HTML */
+                        {% if val != "html" %}
+                            ,
+                            {
+                                "id": "code-block-prismjs-" + language,
+                                "url": "//cdnjs.cloudflare.com/ajax/libs/prism/{% prism_version %}/components/prism-" + language + ".min.js"
+                            }
+                        {% endif %}
                         {% line_numbers_js %}
                         {% toolbar_js %}
                         {% copy_to_clipboard_js %}
                     ];
 
                     for(const library of libraries) {
                         if(document.getElementById(library["id"]) == null) {
```

### Comparing `wagtailcodeblock-1.29.0.0/wagtailcodeblock/templates/wagtailcodeblock/code_block_form.html` & `wagtailcodeblock-1.29.0.1/wagtailcodeblock/templates/wagtailcodeblock/code_block_form.html`

 * *Files identical despite different names*

### Comparing `wagtailcodeblock-1.29.0.0/wagtailcodeblock/templatetags/wagtailcodeblock_tags.py` & `wagtailcodeblock-1.29.0.1/wagtailcodeblock/templatetags/wagtailcodeblock_tags.py`

 * *Files 13% similar despite different names*

```diff
@@ -75,21 +75,14 @@
 
     if get_line_numbers():
         script += (
             f"""<link href="{PRISM_PREFIX}{PRISM_VERSION}/plugins/line-numbers/"""
             """prism-line-numbers.min.css" rel="stylesheet">"""
         )
 
-    if get_copy_to_clipboard():
-        toolbar = True
-        script += (
-            f"""<link href="{PRISM_PREFIX}{PRISM_VERSION}/plugins/copy-to-clipboard/"""
-            """prism-copy-to-clipboard.min.css" rel="stylesheet">"""
-        )
-
     if toolbar is True:
         script += (
             f"""<link href="{PRISM_PREFIX}{PRISM_VERSION}/plugins/toolbar/"""
             """prism-toolbar.min.css" rel="stylesheet">"""
         )
 
     return mark_safe(script)
```

### Comparing `wagtailcodeblock-1.29.0.0/wagtailcodeblock/wagtail_hooks.py` & `wagtailcodeblock-1.29.0.1/wagtailcodeblock/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtailcodeblock-1.29.0.0/wagtailcodeblock.egg-info/PKG-INFO` & `wagtailcodeblock-1.29.0.1/wagtailcodeblock.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtailcodeblock
-Version: 1.29.0.0
+Version: 1.29.0.1
 Summary: Wagtail Code Block provides PrismJS syntax highlighting in Wagtail.
 Author-email: Tim Allen <tallen@wharton.upenn.edu>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/FlipperPA/wagtailcodeblock
 Project-URL: Repository, https://github.com/FlipperPA/wagtailcodeblock
 Project-URL: Documentation, https://github.com/FlipperPA/wagtailcodeblock
 Keywords: wagtail,cms,contact,syntax,code,highlighting,highlighter
@@ -14,17 +14,20 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 3
+Classifier: Framework :: Wagtail :: 4
+Classifier: Framework :: Wagtail :: 5
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Wagtail Code Block
```

### Comparing `wagtailcodeblock-1.29.0.0/wagtailcodeblock.egg-info/SOURCES.txt` & `wagtailcodeblock-1.29.0.1/wagtailcodeblock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

