# Comparing `tmp/spacy_wrap-1.4.3.tar.gz` & `tmp/spacy_wrap-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacy_wrap-1.4.3.tar", last modified: Mon May 22 23:41:08 2023, max compression
+gzip compressed data, was "spacy_wrap-1.4.4.tar", last modified: Tue Aug  1 16:26:40 2023, max compression
```

## Comparing `spacy_wrap-1.4.3.tar` & `spacy_wrap-1.4.4.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:41:08.690876 spacy_wrap-1.4.3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:41:08.682875 spacy_wrap-1.4.3/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:41:08.682875 spacy_wrap-1.4.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)      731 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/.github/ISSUE_TEMPLATE/01_bugs.md
--rw-r--r--   0 root         (0) root         (0)      418 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/.github/ISSUE_TEMPLATE/02_docs.md
--rw-r--r--   0 root         (0) root         (0)      291 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/.github/ISSUE_TEMPLATE/03_feature-request.md
--rw-r--r--   0 root         (0) root         (0)      617 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 root         (0) root         (0)      776 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/.github/dependabot.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:41:08.682875 spacy_wrap-1.4.3/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0 root         (0) root         (0)     1141 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/.github/workflows/documentation.yml
--rw-r--r--   0 root         (0) root         (0)     1673 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)      867 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/.github/workflows/stale.yml
--rw-r--r--   0 root         (0) root         (0)     2842 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/.github/workflows/tests.yml
--rw-r--r--   0 root         (0) root         (0)      213 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/.gitignore
--rw-r--r--   0 root         (0) root         (0)      797 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)     3054 2023-05-22 23:40:57.000000 spacy_wrap-1.4.3/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     1075 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2760 2023-05-22 23:41:08.690876 spacy_wrap-1.4.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      393 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/citation.cff
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:41:08.686876 spacy_wrap-1.4.3/docs/
--rw-r--r--   0 root         (0) root         (0)      633 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:41:08.686876 spacy_wrap-1.4.3/docs/_static/
--rw-r--r--   0 root         (0) root         (0)     4286 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/docs/_static/favicon.ico
--rw-r--r--   0 root         (0) root         (0)   289957 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/docs/_static/icon.png
--rw-r--r--   0 root         (0) root         (0)   289957 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/docs/_static/icon_dark.png
--rw-r--r--   0 root         (0) root         (0)     4325 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)     2533 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/docs/faq.rst
--rw-r--r--   0 root         (0) root         (0)     2504 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)      584 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/docs/installation.rst
--rw-r--r--   0 root         (0) root         (0)     1768 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/docs/news.rst
--rw-r--r--   0 root         (0) root         (0)      930 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/docs/wrap.pipeline_component.rst
--rw-r--r--   0 root         (0) root         (0)     3606 2023-05-22 23:40:57.000000 spacy_wrap-1.4.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     8025 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/readme.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-22 23:41:08.690876 spacy_wrap-1.4.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:41:08.678875 spacy_wrap-1.4.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:41:08.686876 spacy_wrap-1.4.3/src/spacy_wrap/
--rw-r--r--   0 root         (0) root         (0)      486 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/src/spacy_wrap/__init__.py
--rw-r--r--   0 root         (0) root         (0)      239 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/src/spacy_wrap/about.py
--rw-r--r--   0 root         (0) root         (0)     5999 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/src/spacy_wrap/architectures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:41:08.690876 spacy_wrap-1.4.3/src/spacy_wrap/layers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/src/spacy_wrap/layers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5698 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/src/spacy_wrap/layers/clf_transformer_model.py
--rw-r--r--   0 root         (0) root         (0)    15473 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/src/spacy_wrap/pipeline_component_seq_clf.py
--rw-r--r--   0 root         (0) root         (0)    20552 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/src/spacy_wrap/pipeline_component_tok_clf.py
--rw-r--r--   0 root         (0) root         (0)     5022 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/src/spacy_wrap/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:41:08.690876 spacy_wrap-1.4.3/src/spacy_wrap.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2760 2023-05-22 23:41:08.000000 spacy_wrap-1.4.3/src/spacy_wrap.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1219 2023-05-22 23:41:08.000000 spacy_wrap-1.4.3/src/spacy_wrap.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 23:41:08.000000 spacy_wrap-1.4.3/src/spacy_wrap.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      499 2023-05-22 23:41:08.000000 spacy_wrap-1.4.3/src/spacy_wrap.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      647 2023-05-22 23:41:08.000000 spacy_wrap-1.4.3/src/spacy_wrap.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-05-22 23:41:08.000000 spacy_wrap-1.4.3/src/spacy_wrap.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:41:08.690876 spacy_wrap-1.4.3/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3480 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/tests/test_seq_clf_transformer.py
--rw-r--r--   0 root         (0) root         (0)     6989 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/tests/test_tok_clf_transformer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:26:40.380675 spacy_wrap-1.4.4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:26:40.376675 spacy_wrap-1.4.4/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:26:40.376675 spacy_wrap-1.4.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)      731 2023-08-01 16:26:28.000000 spacy_wrap-1.4.4/.github/ISSUE_TEMPLATE/01_bugs.md
+-rw-r--r--   0 root         (0) root         (0)      418 2023-08-01 16:26:28.000000 spacy_wrap-1.4.4/.github/ISSUE_TEMPLATE/02_docs.md
+-rw-r--r--   0 root         (0) root         (0)      291 2023-08-01 16:26:28.000000 spacy_wrap-1.4.4/.github/ISSUE_TEMPLATE/03_feature-request.md
+-rw-r--r--   0 root         (0) root         (0)      617 2023-08-01 16:26:28.000000 spacy_wrap-1.4.4/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 root         (0) root         (0)      776 2023-08-01 16:26:28.000000 spacy_wrap-1.4.4/.github/dependabot.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:26:40.376675 spacy_wrap-1.4.4/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-08-01 16:26:28.000000 spacy_wrap-1.4.4/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0 root         (0) root         (0)     1141 2023-08-01 16:26:28.000000 spacy_wrap-1.4.4/.github/workflows/documentation.yml
+-rw-r--r--   0 root         (0) root         (0)     1673 2023-08-01 16:26:28.000000 spacy_wrap-1.4.4/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)      867 2023-08-01 16:26:28.000000 spacy_wrap-1.4.4/.github/workflows/stale.yml
+-rw-r--r--   0 root         (0) root         (0)     2842 2023-08-01 16:26:28.000000 spacy_wrap-1.4.4/.github/workflows/tests.yml
+-rw-r--r--   0 root         (0) root         (0)      213 2023-08-01 16:26:28.000000 spacy_wrap-1.4.4/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      794 2023-08-01 16:26:28.000000 spacy_wrap-1.4.4/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)     3231 2023-08-01 16:26:29.000000 spacy_wrap-1.4.4/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-08-01 16:26:28.000000 spacy_wrap-1.4.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2760 2023-08-01 16:26:40.380675 spacy_wrap-1.4.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      393 2023-08-01 16:26:28.000000 spacy_wrap-1.4.4/citation.cff
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:26:40.376675 spacy_wrap-1.4.4/docs/
+-rw-r--r--   0 root         (0) root         (0)      633 2023-08-01 16:26:28.000000 spacy_wrap-1.4.4/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:26:40.376675 spacy_wrap-1.4.4/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)     4286 2023-08-01 16:26:28.000000 spacy_wrap-1.4.4/docs/_static/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)   289957 2023-08-01 16:26:28.000000 spacy_wrap-1.4.4/docs/_static/icon.png
+-rw-r--r--   0 root         (0) root         (0)   289957 2023-08-01 16:26:28.000000 spacy_wrap-1.4.4/docs/_static/icon_dark.png
+-rw-r--r--   0 root         (0) root         (0)     4325 2023-08-01 16:26:28.000000 spacy_wrap-1.4.4/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     2533 2023-08-01 16:26:28.000000 spacy_wrap-1.4.4/docs/faq.rst
+-rw-r--r--   0 root         (0) root         (0)     2504 2023-08-01 16:26:28.000000 spacy_wrap-1.4.4/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)      584 2023-08-01 16:26:28.000000 spacy_wrap-1.4.4/docs/installation.rst
+-rw-r--r--   0 root         (0) root         (0)     1768 2023-08-01 16:26:28.000000 spacy_wrap-1.4.4/docs/news.rst
+-rw-r--r--   0 root         (0) root         (0)      930 2023-08-01 16:26:28.000000 spacy_wrap-1.4.4/docs/wrap.pipeline_component.rst
+-rw-r--r--   0 root         (0) root         (0)     3577 2023-08-01 16:26:29.000000 spacy_wrap-1.4.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     8025 2023-08-01 16:26:28.000000 spacy_wrap-1.4.4/readme.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-01 16:26:40.380675 spacy_wrap-1.4.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:26:40.372675 spacy_wrap-1.4.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:26:40.380675 spacy_wrap-1.4.4/src/spacy_wrap/
+-rw-r--r--   0 root         (0) root         (0)      486 2023-08-01 16:26:28.000000 spacy_wrap-1.4.4/src/spacy_wrap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      239 2023-08-01 16:26:28.000000 spacy_wrap-1.4.4/src/spacy_wrap/about.py
+-rw-r--r--   0 root         (0) root         (0)     5999 2023-08-01 16:26:28.000000 spacy_wrap-1.4.4/src/spacy_wrap/architectures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:26:40.380675 spacy_wrap-1.4.4/src/spacy_wrap/layers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 16:26:28.000000 spacy_wrap-1.4.4/src/spacy_wrap/layers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5698 2023-08-01 16:26:28.000000 spacy_wrap-1.4.4/src/spacy_wrap/layers/clf_transformer_model.py
+-rw-r--r--   0 root         (0) root         (0)    15523 2023-08-01 16:26:28.000000 spacy_wrap-1.4.4/src/spacy_wrap/pipeline_component_seq_clf.py
+-rw-r--r--   0 root         (0) root         (0)    20602 2023-08-01 16:26:28.000000 spacy_wrap-1.4.4/src/spacy_wrap/pipeline_component_tok_clf.py
+-rw-r--r--   0 root         (0) root         (0)     5022 2023-08-01 16:26:28.000000 spacy_wrap-1.4.4/src/spacy_wrap/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:26:40.380675 spacy_wrap-1.4.4/src/spacy_wrap.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2760 2023-08-01 16:26:40.000000 spacy_wrap-1.4.4/src/spacy_wrap.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1219 2023-08-01 16:26:40.000000 spacy_wrap-1.4.4/src/spacy_wrap.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 16:26:40.000000 spacy_wrap-1.4.4/src/spacy_wrap.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      499 2023-08-01 16:26:40.000000 spacy_wrap-1.4.4/src/spacy_wrap.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      618 2023-08-01 16:26:40.000000 spacy_wrap-1.4.4/src/spacy_wrap.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-08-01 16:26:40.000000 spacy_wrap-1.4.4/src/spacy_wrap.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:26:40.380675 spacy_wrap-1.4.4/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 16:26:28.000000 spacy_wrap-1.4.4/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3480 2023-08-01 16:26:28.000000 spacy_wrap-1.4.4/tests/test_seq_clf_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     6989 2023-08-01 16:26:28.000000 spacy_wrap-1.4.4/tests/test_tok_clf_transformer.py
```

### Comparing `spacy_wrap-1.4.3/.github/ISSUE_TEMPLATE/01_bugs.md` & `spacy_wrap-1.4.4/.github/ISSUE_TEMPLATE/01_bugs.md`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.3/.github/ISSUE_TEMPLATE/config.yml` & `spacy_wrap-1.4.4/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.3/.github/dependabot.yml` & `spacy_wrap-1.4.4/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.3/.github/workflows/dependabot_automerge.yml` & `spacy_wrap-1.4.4/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.3/.github/workflows/documentation.yml` & `spacy_wrap-1.4.4/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.3/.github/workflows/release.yml` & `spacy_wrap-1.4.4/.github/workflows/release.yml`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
       # Checkout action is required for token to persist
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
           token: ${{ secrets.RELEASE }}
 
       - name: Python Semantic Release
-        uses: relekang/python-semantic-release@v7.33.1
+        uses: relekang/python-semantic-release@v7.34.6
         with:
           github_token: ${{ secrets.RELEASE }}
           # Remember to copy the [semantic_release] section from pyproject.toml
           # as well
           # To enable pypi,
           # 1) Set upload_to_pypi to true in  pyproject.toml and
           # 2) Set the pypi_token in the repo
```

### Comparing `spacy_wrap-1.4.3/.github/workflows/stale.yml` & `spacy_wrap-1.4.4/.github/workflows/stale.yml`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.3/.github/workflows/tests.yml` & `spacy_wrap-1.4.4/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.3/.pre-commit-config.yaml` & `spacy_wrap-1.4.4/.pre-commit-config.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 default_stages: [commit, push]
 
 repos:
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.4.0
+    rev: v3.10.1
     hooks:
       - id: pyupgrade
 
   - repo: https://github.com/bwhmather/ssort
     rev: v0.11.6
     hooks:
       - id: ssort
 
   - repo: https://github.com/asottile/add-trailing-comma
-    rev: v2.4.0
+    rev: v3.0.1
     hooks:
       - id: add-trailing-comma
 
   - repo: https://github.com/PyCQA/docformatter
-    rev: v1.7.1
+    rev: v1.7.5
     hooks:
       - id: docformatter
         args: [--in-place]
 
   - repo: https://github.com/psf/black
-    rev: 23.3.0
+    rev: 23.7.0
     hooks:
       - id: black
         args: [--line-length, "88"]
 
-  - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.269
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.0.280
     hooks:
       - id: ruff
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.3.0
+    rev: v1.4.1
     hooks:
       - id: mypy
```

### Comparing `spacy_wrap-1.4.3/CHANGELOG.md` & `spacy_wrap-1.4.4/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.4.4 (2023-08-01)
+
+### Fix
+
+* Relax upper bound on versions ([`1a7d301`](https://github.com/KennethEnevoldsen/spacy-wrap/commit/1a7d301311bcd605e54d21c2eff0d540018d204c))
+
 ## v1.4.3 (2023-05-22)
 ### Fix
 * Ensure no Nones in iob tokens ([`8fa954a`](https://github.com/KennethEnevoldsen/spacy-wrap/commit/8fa954a70a1cb76ff350b6c32ea461fd85ad369b))
 
 ## v1.4.2 (2023-05-01)
 ### Fix
 * Relaxed upper bound of dev. dependencies ([`f9c8a87`](https://github.com/KennethEnevoldsen/spacy-wrap/commit/f9c8a878ef0d4a03019925bb97af658a4a2bf658))
```

### Comparing `spacy_wrap-1.4.3/LICENSE` & `spacy_wrap-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.3/PKG-INFO` & `spacy_wrap-1.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy_wrap
-Version: 1.4.3
+Version: 1.4.4
 Summary: Wrappers for including pre-trained transformers in spaCy pipelines
 Author-email: Kenneth Enevoldsen <kennethcenevoldsen@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Kenneth Enevoldsen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `spacy_wrap-1.4.3/docs/Makefile` & `spacy_wrap-1.4.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.3/docs/_static/favicon.ico` & `spacy_wrap-1.4.4/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.3/docs/_static/icon.png` & `spacy_wrap-1.4.4/docs/_static/icon.png`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.3/docs/_static/icon_dark.png` & `spacy_wrap-1.4.4/docs/_static/icon_dark.png`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.3/docs/conf.py` & `spacy_wrap-1.4.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.3/docs/faq.rst` & `spacy_wrap-1.4.4/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.3/docs/index.rst` & `spacy_wrap-1.4.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.3/docs/installation.rst` & `spacy_wrap-1.4.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.3/docs/news.rst` & `spacy_wrap-1.4.4/docs/news.rst`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.3/docs/wrap.pipeline_component.rst` & `spacy_wrap-1.4.4/docs/wrap.pipeline_component.rst`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.3/pyproject.toml` & `spacy_wrap-1.4.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "spacy_wrap"
-version = "1.4.3"
+version = "1.4.4"
 description = "Wrappers for including pre-trained transformers in spaCy pipelines"
 authors = [{name = "Kenneth Enevoldsen", email = "kennethcenevoldsen@gmail.com"}]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
@@ -24,30 +24,30 @@
     "text analysis",
     "natural language processing",
     "text mining",
     "text analytics",
 ]
 
 dependencies = [
-    "spacy_transformers>=1.2.1,<1.3.0",
-    "spacy>=3.2.1,<3.6.0",
-    "thinc>=8.0.13,<8.2.0",
+    "spacy_transformers>=1.2.1",
+    "spacy>=3.2.1",
+    "thinc>=8.0.13",
 ]
 
 requires-python = ">=3.8"
 
 [project.urls]
 homepage = "https://github.com/KennethEnevoldsen/spacy-wrap"
 repository = "https://github.com/KennethEnevoldsen/spacy-wrap"
 documentation = "https://kennethenevoldsen.github.io/spacy-wrap/"
 
 [project.optional-dependencies]
 style = [
     "black==22.12.0",
-    "pre-commit>=2.20.0,<2.21.0",
+    "pre-commit>=2.20.0",
     "ruff==0.0.263",
     "mypy==0.991"
 ]
 tests = [
     "pytest>=7.1.3",
     "pytest-cov>=3.0.0",
 ]
```

### Comparing `spacy_wrap-1.4.3/readme.md` & `spacy_wrap-1.4.4/readme.md`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.3/src/spacy_wrap/architectures.py` & `spacy_wrap-1.4.4/src/spacy_wrap/architectures.py`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.3/src/spacy_wrap/layers/clf_transformer_model.py` & `spacy_wrap-1.4.4/src/spacy_wrap/layers/clf_transformer_model.py`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.3/src/spacy_wrap/pipeline_component_seq_clf.py` & `spacy_wrap-1.4.4/src/spacy_wrap/pipeline_component_seq_clf.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,30 +246,36 @@
             get_examples (Callable[[], Iterable[Example]]): Optional function that
                 returns gold-standard Example objects.
             nlp (Language): The current nlp object.
         """
         self.__initialize_component()
 
     def to_disk(
-        self, path: Union[str, Path], *, exclude: Iterable[str] = tuple()
+        self,
+        path: Union[str, Path],
+        *,
+        exclude: Iterable[str] = tuple(),
     ) -> None:
         """Serialize the pipe to disk.
 
         Args:
             path (str / Path): Path to a directory.
             exclude (Iterable[str]): String names of serialization fields to exclude.
         """
         serialize = {}
         serialize["cfg"] = lambda p: srsly.write_json(p, self.cfg)
         serialize["vocab"] = self.vocab.to_disk
         serialize["model"] = self.model.to_disk
         util.to_disk(path, serialize, exclude)
 
     def from_disk(
-        self, path: Union[str, Path], *, exclude: Iterable[str] = tuple()
+        self,
+        path: Union[str, Path],
+        *,
+        exclude: Iterable[str] = tuple(),
     ) -> "SequenceClassificationTransformer":
         """Load the pipe from disk.
 
         Args:
             path (str / Path): Path to a directory.
             exclude (Iterable[str]): String names of serialization fields to exclude.
```

### Comparing `spacy_wrap-1.4.3/src/spacy_wrap/pipeline_component_tok_clf.py` & `spacy_wrap-1.4.4/src/spacy_wrap/pipeline_component_tok_clf.py`

 * *Files 2% similar despite different names*

```diff
@@ -350,30 +350,36 @@
 
         Args:
             nlp (Language): The current nlp object.
         """
         self.__initialize_component()
 
     def to_disk(
-        self, path: Union[str, Path], *, exclude: Iterable[str] = tuple()
+        self,
+        path: Union[str, Path],
+        *,
+        exclude: Iterable[str] = tuple(),
     ) -> None:
         """Serialize the pipe to disk.
 
         Args:
             path (str / Path): Path to a directory.
             exclude (Iterable[str]): String names of serialization fields to exclude.
         """
         serialize = {}
         serialize["cfg"] = lambda p: srsly.write_json(p, self.cfg)
         serialize["vocab"] = self.vocab.to_disk
         serialize["model"] = self.model.to_disk
         util.to_disk(path, serialize, exclude)
 
     def from_disk(
-        self, path: Union[str, Path], *, exclude: Iterable[str] = tuple()
+        self,
+        path: Union[str, Path],
+        *,
+        exclude: Iterable[str] = tuple(),
     ) -> "TokenClassificationTransformer":
         """Load the pipe from disk.
 
         Args:
             path (str / Path): Path to a directory.
             exclude (Iterable[str]): String names of serialization fields to exclude.
```

### Comparing `spacy_wrap-1.4.3/src/spacy_wrap/util.py` & `spacy_wrap-1.4.4/src/spacy_wrap/util.py`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.3/src/spacy_wrap.egg-info/PKG-INFO` & `spacy_wrap-1.4.4/src/spacy_wrap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy-wrap
-Version: 1.4.3
+Version: 1.4.4
 Summary: Wrappers for including pre-trained transformers in spaCy pipelines
 Author-email: Kenneth Enevoldsen <kennethcenevoldsen@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Kenneth Enevoldsen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `spacy_wrap-1.4.3/src/spacy_wrap.egg-info/SOURCES.txt` & `spacy_wrap-1.4.4/src/spacy_wrap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.3/src/spacy_wrap.egg-info/requires.txt` & `spacy_wrap-1.4.4/src/spacy_wrap.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-spacy_transformers<1.3.0,>=1.2.1
-spacy<3.6.0,>=3.2.1
-thinc<8.2.0,>=8.0.13
+spacy_transformers>=1.2.1
+spacy>=3.2.1
+thinc>=8.0.13
 
 [cuda]
 cupy>=5.0.0b4
 
 [cuda100]
 cupy-cuda100>=5.0.0b4
 
@@ -40,14 +40,14 @@
 furo>=2022.12.7
 sphinx-copybutton>=0.5.1
 sphinxext-opengraph>=0.7.3
 sphinx_design>=0.3.0
 
 [style]
 black==22.12.0
-pre-commit<2.21.0,>=2.20.0
+pre-commit>=2.20.0
 ruff==0.0.263
 mypy==0.991
 
 [tests]
 pytest>=7.1.3
 pytest-cov>=3.0.0
```

### Comparing `spacy_wrap-1.4.3/tests/test_seq_clf_transformer.py` & `spacy_wrap-1.4.4/tests/test_seq_clf_transformer.py`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.3/tests/test_tok_clf_transformer.py` & `spacy_wrap-1.4.4/tests/test_tok_clf_transformer.py`

 * *Files identical despite different names*

