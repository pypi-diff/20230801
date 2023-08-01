# Comparing `tmp/cutlet-0.2.1.tar.gz` & `tmp/cutlet-0.2.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cutlet-0.2.1.tar", last modified: Mon Jul 31 13:52:19 2023, max compression
+gzip compressed data, was "cutlet-0.2.1a1.tar", last modified: Tue Aug  1 13:24:08 2023, max compression
```

## Comparing `cutlet-0.2.1.tar` & `cutlet-0.2.1a1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:52:19.941105 cutlet-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:52:19.941105 cutlet-0.2.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-31 13:51:40.000000 cutlet-0.2.1/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:52:19.941105 cutlet-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-31 13:51:40.000000 cutlet-0.2.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-31 13:51:40.000000 cutlet-0.2.1/.github/workflows/linux.yml
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-31 13:51:40.000000 cutlet-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-31 13:51:40.000000 cutlet-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-31 13:51:40.000000 cutlet-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-07-31 13:52:19.941105 cutlet-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-07-31 13:51:40.000000 cutlet-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:52:19.941105 cutlet-0.2.1/cutlet/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-31 13:51:40.000000 cutlet-0.2.1/cutlet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-31 13:51:40.000000 cutlet-0.2.1/cutlet/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    13237 2023-07-31 13:51:40.000000 cutlet-0.2.1/cutlet/cutlet.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-31 13:51:40.000000 cutlet-0.2.1/cutlet/exceptions.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-07-31 13:51:40.000000 cutlet-0.2.1/cutlet/mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:52:19.941105 cutlet-0.2.1/cutlet/test/
--rw-r--r--   0 runner    (1001) docker     (123)    27191 2023-07-31 13:51:40.000000 cutlet-0.2.1/cutlet/test/blns.json
--rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-07-31 13:51:40.000000 cutlet-0.2.1/cutlet/test/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-31 13:51:40.000000 cutlet-0.2.1/cutlet/test/test_fuzz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:52:19.941105 cutlet-0.2.1/cutlet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-07-31 13:52:19.000000 cutlet-0.2.1/cutlet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-31 13:52:19.000000 cutlet-0.2.1/cutlet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 13:52:19.000000 cutlet-0.2.1/cutlet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-31 13:52:19.000000 cutlet-0.2.1/cutlet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-31 13:52:19.000000 cutlet-0.2.1/cutlet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-31 13:52:19.000000 cutlet-0.2.1/cutlet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)   340278 2023-07-31 13:51:40.000000 cutlet-0.2.1/cutlet.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:52:19.941105 cutlet-0.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)   189912 2023-07-31 13:51:40.000000 cutlet-0.2.1/docs/cutlet.html
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-31 13:51:40.000000 cutlet-0.2.1/docs/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    90584 2023-07-31 13:51:40.000000 cutlet-0.2.1/docs/search.js
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-31 13:51:40.000000 cutlet-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-31 13:51:40.000000 cutlet-0.2.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-31 13:51:40.000000 cutlet-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 13:52:19.941105 cutlet-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-31 13:51:40.000000 cutlet-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:24:08.977757 cutlet-0.2.1a1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:24:08.973757 cutlet-0.2.1a1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-01 13:23:10.000000 cutlet-0.2.1a1/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:24:08.977757 cutlet-0.2.1a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-08-01 13:23:10.000000 cutlet-0.2.1a1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-01 13:23:10.000000 cutlet-0.2.1a1/.github/workflows/linux.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-01 13:23:10.000000 cutlet-0.2.1a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-01 13:23:10.000000 cutlet-0.2.1a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-01 13:23:10.000000 cutlet-0.2.1a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-08-01 13:24:08.977757 cutlet-0.2.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-08-01 13:23:10.000000 cutlet-0.2.1a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:24:08.977757 cutlet-0.2.1a1/cutlet/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-01 13:23:10.000000 cutlet-0.2.1a1/cutlet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-01 13:23:10.000000 cutlet-0.2.1a1/cutlet/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13237 2023-08-01 13:23:10.000000 cutlet-0.2.1a1/cutlet/cutlet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-01 13:23:10.000000 cutlet-0.2.1a1/cutlet/exceptions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-08-01 13:23:10.000000 cutlet-0.2.1a1/cutlet/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:24:08.977757 cutlet-0.2.1a1/cutlet/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    27191 2023-08-01 13:23:10.000000 cutlet-0.2.1a1/cutlet/test/blns.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-08-01 13:23:10.000000 cutlet-0.2.1a1/cutlet/test/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-08-01 13:23:10.000000 cutlet-0.2.1a1/cutlet/test/test_fuzz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:24:08.977757 cutlet-0.2.1a1/cutlet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-08-01 13:24:08.000000 cutlet-0.2.1a1/cutlet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-08-01 13:24:08.000000 cutlet-0.2.1a1/cutlet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 13:24:08.000000 cutlet-0.2.1a1/cutlet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-01 13:24:08.000000 cutlet-0.2.1a1/cutlet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-01 13:24:08.000000 cutlet-0.2.1a1/cutlet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-01 13:24:08.000000 cutlet-0.2.1a1/cutlet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   340278 2023-08-01 13:23:10.000000 cutlet-0.2.1a1/cutlet.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:24:08.977757 cutlet-0.2.1a1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   189912 2023-08-01 13:23:10.000000 cutlet-0.2.1a1/docs/cutlet.html
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-01 13:23:10.000000 cutlet-0.2.1a1/docs/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    90584 2023-08-01 13:23:10.000000 cutlet-0.2.1a1/docs/search.js
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-01 13:23:10.000000 cutlet-0.2.1a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-01 13:23:10.000000 cutlet-0.2.1a1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-08-01 13:23:10.000000 cutlet-0.2.1a1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 13:24:08.977757 cutlet-0.2.1a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-01 13:23:10.000000 cutlet-0.2.1a1/setup.py
```

### Comparing `cutlet-0.2.1/.github/workflows/docs.yml` & `cutlet-0.2.1a1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `cutlet-0.2.1/.github/workflows/linux.yml` & `cutlet-0.2.1a1/.github/workflows/linux.yml`

 * *Files 12% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 on: [push]
 
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [3.7, 3.8, 3.9, "3.10"]
+        python-version: [3.7, 3.8, 3.9, "3.10", "3.11"]
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install deps
       shell: bash
       run: |
         python -m pip install --upgrade setuptools wheel pip setuptools-scm
         pip install fugashi[unidic-lite] jaconv pytest hypothesis
@@ -26,11 +26,11 @@
     - name: Publish to PyPI if tagged
       if: startsWith(github.ref, 'refs/tags') && matrix.python-version == 3.8
       env:
         TWINE_USERNAME: "23"
         TWINE_PASSWORD: ${{ secrets.PYPI_PASSWORD }}
       run: |
         python -m pip install --upgrade pip
-        pip install twine setuptools-scm
-        python setup.py sdist
+        pip install twine setuptools-scm build
+        python -m build
         twine upload dist/cutlet*.tar.gz
```

### Comparing `cutlet-0.2.1/LICENSE` & `cutlet-0.2.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `cutlet-0.2.1/PKG-INFO` & `cutlet-0.2.1a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cutlet
-Version: 0.2.1
+Version: 0.2.1a1
 Summary: Romaji converter
 Home-page: https://github.com/polm/cutlet
 Author: Paul O'Leary McCann
 Author-email: polm@dampfkraft.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Japanese
 Requires-Python: >=3.5
```

### Comparing `cutlet-0.2.1/README.md` & `cutlet-0.2.1a1/README.md`

 * *Files identical despite different names*

### Comparing `cutlet-0.2.1/cutlet/cutlet.py` & `cutlet-0.2.1a1/cutlet/cutlet.py`

 * *Files identical despite different names*

### Comparing `cutlet-0.2.1/cutlet/mapping.py` & `cutlet-0.2.1a1/cutlet/mapping.py`

 * *Files identical despite different names*

### Comparing `cutlet-0.2.1/cutlet/test/blns.json` & `cutlet-0.2.1a1/cutlet/test/blns.json`

 * *Files identical despite different names*

### Comparing `cutlet-0.2.1/cutlet/test/test_basic.py` & `cutlet-0.2.1a1/cutlet/test/test_basic.py`

 * *Files identical despite different names*

### Comparing `cutlet-0.2.1/cutlet/test/test_fuzz.py` & `cutlet-0.2.1a1/cutlet/test/test_fuzz.py`

 * *Files identical despite different names*

### Comparing `cutlet-0.2.1/cutlet.egg-info/PKG-INFO` & `cutlet-0.2.1a1/cutlet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cutlet
-Version: 0.2.1
+Version: 0.2.1a1
 Summary: Romaji converter
 Home-page: https://github.com/polm/cutlet
 Author: Paul O'Leary McCann
 Author-email: polm@dampfkraft.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Japanese
 Requires-Python: >=3.5
```

### Comparing `cutlet-0.2.1/cutlet.egg-info/SOURCES.txt` & `cutlet-0.2.1a1/cutlet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cutlet-0.2.1/cutlet.png` & `cutlet-0.2.1a1/cutlet.png`

 * *Files identical despite different names*

### Comparing `cutlet-0.2.1/docs/cutlet.html` & `cutlet-0.2.1a1/docs/cutlet.html`

 * *Files identical despite different names*

### Comparing `cutlet-0.2.1/docs/search.js` & `cutlet-0.2.1a1/docs/search.js`

 * *Files identical despite different names*

### Comparing `cutlet-0.2.1/setup.py` & `cutlet-0.2.1a1/setup.py`

 * *Files identical despite different names*

