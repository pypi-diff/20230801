# Comparing `tmp/quickconf-0.2.0a3.tar.gz` & `tmp/quickconf-0.2.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickconf-0.2.0a3.tar", last modified: Tue Aug  1 19:23:36 2023, max compression
+gzip compressed data, was "quickconf-0.2.0a5.tar", last modified: Tue Aug  1 20:26:29 2023, max compression
```

## Comparing `quickconf-0.2.0a3.tar` & `quickconf-0.2.0a5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:23:36.753342 quickconf-0.2.0a3/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:23:36.745342 quickconf-0.2.0a3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:23:36.749342 quickconf-0.2.0a3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-01 19:23:16.000000 quickconf-0.2.0a3/.version
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-08-01 19:23:36.749342 quickconf-0.2.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:23:36.749342 quickconf-0.2.0a3/demo/
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/demo/example.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/demo/settings.toml
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/demo/settings_updated.toml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/demo/typecheck.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 19:23:36.753342 quickconf-0.2.0a3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:23:36.745342 quickconf-0.2.0a3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:23:36.749342 quickconf-0.2.0a3/src/quickconf/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/src/quickconf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-01 19:23:16.000000 quickconf-0.2.0a3/src/quickconf/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15097 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/src/quickconf/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:23:36.749342 quickconf-0.2.0a3/src/quickconf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-08-01 19:23:36.000000 quickconf-0.2.0a3/src/quickconf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-08-01 19:23:36.000000 quickconf-0.2.0a3/src/quickconf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 19:23:36.000000 quickconf-0.2.0a3/src/quickconf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-01 19:23:36.000000 quickconf-0.2.0a3/src/quickconf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-01 19:23:36.000000 quickconf-0.2.0a3/src/quickconf.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:23:36.749342 quickconf-0.2.0a3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/tests/test_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:26:29.194818 quickconf-0.2.0a5/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-01 20:26:13.000000 quickconf-0.2.0a5/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:26:29.190818 quickconf-0.2.0a5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:26:29.190818 quickconf-0.2.0a5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-08-01 20:26:13.000000 quickconf-0.2.0a5/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-08-01 20:26:13.000000 quickconf-0.2.0a5/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-08-01 20:26:13.000000 quickconf-0.2.0a5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-08-01 20:26:13.000000 quickconf-0.2.0a5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-01 20:26:17.000000 quickconf-0.2.0a5/.version
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-08-01 20:26:13.000000 quickconf-0.2.0a5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-08-01 20:26:29.194818 quickconf-0.2.0a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-08-01 20:26:13.000000 quickconf-0.2.0a5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:26:29.194818 quickconf-0.2.0a5/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-08-01 20:26:13.000000 quickconf-0.2.0a5/demo/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-01 20:26:13.000000 quickconf-0.2.0a5/demo/settings.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-01 20:26:13.000000 quickconf-0.2.0a5/demo/settings_updated.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-01 20:26:13.000000 quickconf-0.2.0a5/demo/typecheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-08-01 20:26:13.000000 quickconf-0.2.0a5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 20:26:13.000000 quickconf-0.2.0a5/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 20:26:29.194818 quickconf-0.2.0a5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:26:29.190818 quickconf-0.2.0a5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:26:29.194818 quickconf-0.2.0a5/src/quickconf/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-01 20:26:13.000000 quickconf-0.2.0a5/src/quickconf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-01 20:26:17.000000 quickconf-0.2.0a5/src/quickconf/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15097 2023-08-01 20:26:13.000000 quickconf-0.2.0a5/src/quickconf/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:26:29.194818 quickconf-0.2.0a5/src/quickconf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-08-01 20:26:29.000000 quickconf-0.2.0a5/src/quickconf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-08-01 20:26:29.000000 quickconf-0.2.0a5/src/quickconf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:26:29.000000 quickconf-0.2.0a5/src/quickconf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-01 20:26:29.000000 quickconf-0.2.0a5/src/quickconf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-01 20:26:29.000000 quickconf-0.2.0a5/src/quickconf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:26:29.194818 quickconf-0.2.0a5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-01 20:26:13.000000 quickconf-0.2.0a5/tests/test_conf.py
```

### Comparing `quickconf-0.2.0a3/.github/workflows/release.yml` & `quickconf-0.2.0a5/.github/workflows/release.yml`

 * *Files 7% similar despite different names*

```diff
@@ -24,20 +24,23 @@
         id: check-version
         run: |
           pattern="^refs\/tags\/v([0-9]+\.[0-9]+\.[0-9]+(-(a|alpha|b|beta|dev)[0-9]+)?)$"
           [[ "${{ github.ref }}" =~ $pattern ]]
           version="${BASH_REMATCH[1]}"
           if [ ! -z "${BASH_REMATCH[2]}" ]
           then
-              version="${version/-/}"
-              version="${version/alpha/a}"
-              version="${version/beta/b}"
-              echo ::set-output name=prerelease::true
+            version="${version/-/}"
+            version="${version/alpha/a}"
+            version="${version/beta/b}"
+            pre="true"
+          else
+            pre="false"
           fi
-          echo ::set-output name=version::$version
+          echo "prerelease=$pre" >> "$GITHUB_OUTPUT"
+          echo "version=$version" >> "$GITHUB_OUTPUT"
 
       - name: Checkout repo
         uses: actions/checkout@v3
 
       - name: Write version files
         env:
           VERSION: ${{ steps.check-version.outputs.version }}
@@ -66,14 +69,16 @@
           name: dist
           path: dist/
 
       - name: Create release
         uses: ncipollo/release-action@v1
         with:
           artifacts: "dist/*"
+          name: ${{ steps.check-version.outputs.version }}
           draft: false
           allowUpdates: true
           generateReleaseNotes: true
-          prerelease: steps.check-version.outputs.prerelease == 'true'
+          removeArtifacts: true
+          prerelease: ${{ steps.check-version.outputs.prerelease }}
 
       - name: Publish to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `quickconf-0.2.0a3/.github/workflows/tests.yml` & `quickconf-0.2.0a5/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `quickconf-0.2.0a3/.gitignore` & `quickconf-0.2.0a5/.gitignore`

 * *Files identical despite different names*

### Comparing `quickconf-0.2.0a3/.pre-commit-config.yaml` & `quickconf-0.2.0a5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `quickconf-0.2.0a3/LICENSE` & `quickconf-0.2.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `quickconf-0.2.0a3/PKG-INFO` & `quickconf-0.2.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickconf
-Version: 0.2.0a3
+Version: 0.2.0a5
 Summary: Simple and flexible TOML-file based configurations framework
 Author-email: Kenneth Trelborg Vestergaard <mortencombat@fastmail.com>
 Project-URL: Homepage, https://github.com/mortencombat/quickconf
 Project-URL: Repository, https://github.com/mortencombat/quickconf
 Keywords: configuration,settings,options,toml
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `quickconf-0.2.0a3/README.md` & `quickconf-0.2.0a5/README.md`

 * *Files identical despite different names*

### Comparing `quickconf-0.2.0a3/demo/example.py` & `quickconf-0.2.0a5/demo/example.py`

 * *Files identical despite different names*

### Comparing `quickconf-0.2.0a3/pyproject.toml` & `quickconf-0.2.0a5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `quickconf-0.2.0a3/src/quickconf/core.py` & `quickconf-0.2.0a5/src/quickconf/core.py`

 * *Files identical despite different names*

### Comparing `quickconf-0.2.0a3/src/quickconf.egg-info/PKG-INFO` & `quickconf-0.2.0a5/src/quickconf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickconf
-Version: 0.2.0a3
+Version: 0.2.0a5
 Summary: Simple and flexible TOML-file based configurations framework
 Author-email: Kenneth Trelborg Vestergaard <mortencombat@fastmail.com>
 Project-URL: Homepage, https://github.com/mortencombat/quickconf
 Project-URL: Repository, https://github.com/mortencombat/quickconf
 Keywords: configuration,settings,options,toml
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `quickconf-0.2.0a3/src/quickconf.egg-info/SOURCES.txt` & `quickconf-0.2.0a5/src/quickconf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

