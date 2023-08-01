# Comparing `tmp/hatch_ci-0.0.2b8.tar.gz` & `tmp/hatch_ci-0.0.2b9.tar.gz`

## Comparing `hatch_ci-0.0.2b8.tar` & `hatch_ci-0.0.2b9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/.gitattributes
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/Makefile
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/.github/workflows/beta.yml
--rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/.github/workflows/master.yml
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/.github/workflows/tags.yml
--rw-r--r--   0        0        0    18965 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage.xml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage/coverage_html.js
--rw-r--r--   0        0        0     5116 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943___init___py.html
--rw-r--r--   0        0        0    26555 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943___main___py.html
--rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_common_py.html
--rw-r--r--   0        0        0     6437 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_hooks_py.html
--rw-r--r--   0        0        0    82207 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_scm_py.html
--rw-r--r--   0        0        0    84461 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_tools_py.html
--rw-r--r--   0        0        0    22034 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_version_hook_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage/favicon_32.png
--rw-r--r--   0        0        0     6471 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage/keybd_open.png
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage/style.css
--rw-r--r--   0        0        0    19337 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/junit/junit.html
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/junit/junit.xml
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/mypy/index.html
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/mypy/mypy-html.css
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/__init__.py.html
--rw-r--r--   0        0        0    13889 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/__main__.py.html
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/common.py.html
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/hooks.py.html
--rw-r--r--   0        0        0    44011 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/scm.py.html
--rw-r--r--   0        0        0    49030 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/tools.py.html
--rw-r--r--   0        0        0    14045 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/version_hook.py.html
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/src/hatch_ci/__init__.py
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/src/hatch_ci/__main__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/src/hatch_ci/common.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/src/hatch_ci/hooks.py
--rw-r--r--   0        0        0     7291 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/src/hatch_ci/scm.py
--rw-r--r--   0        0        0     8240 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/src/hatch_ci/tools.py
--rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/src/hatch_ci/version_hook.py
--rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/tests/conftest.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/tests/requirements.txt
--rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/tests/test_scm.py
--rw-r--r--   0        0        0     7570 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/tests/test_tools.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/LICENSE.txt
--rw-r--r--   0        0        0     7067 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/README.md
--rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/pyproject.toml
--rw-r--r--   0        0        0     7977 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/.gitattributes
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/Makefile
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/.github/workflows/beta.yml
+-rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/.github/workflows/master.yml
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/.github/workflows/tags.yml
+-rw-r--r--   0        0        0    19454 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/coverage.xml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/coverage/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/coverage/coverage_html.js
+-rw-r--r--   0        0        0     5116 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/coverage/d_7005a4ce5d73f943___init___py.html
+-rw-r--r--   0        0        0    26555 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/coverage/d_7005a4ce5d73f943___main___py.html
+-rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/coverage/d_7005a4ce5d73f943_common_py.html
+-rw-r--r--   0        0        0     6437 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/coverage/d_7005a4ce5d73f943_hooks_py.html
+-rw-r--r--   0        0        0    82207 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/coverage/d_7005a4ce5d73f943_scm_py.html
+-rw-r--r--   0        0        0    84461 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/coverage/d_7005a4ce5d73f943_tools_py.html
+-rw-r--r--   0        0        0    22034 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/coverage/d_7005a4ce5d73f943_version_hook_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/coverage/favicon_32.png
+-rw-r--r--   0        0        0     6471 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/coverage/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/coverage/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/coverage/keybd_open.png
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/coverage/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/coverage/style.css
+-rw-r--r--   0        0        0    19337 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/junit/junit.html
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/junit/junit.xml
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/mypy/index.html
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/mypy/mypy-html.css
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/mypy/html/src/hatch_ci/__init__.py.html
+-rw-r--r--   0        0        0    13889 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/mypy/html/src/hatch_ci/__main__.py.html
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/mypy/html/src/hatch_ci/common.py.html
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/mypy/html/src/hatch_ci/hooks.py.html
+-rw-r--r--   0        0        0    44011 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/mypy/html/src/hatch_ci/scm.py.html
+-rw-r--r--   0        0        0    49030 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/mypy/html/src/hatch_ci/tools.py.html
+-rw-r--r--   0        0        0    14045 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/mypy/html/src/hatch_ci/version_hook.py.html
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/src/hatch_ci/__init__.py
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/src/hatch_ci/__main__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/src/hatch_ci/common.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/src/hatch_ci/hooks.py
+-rw-r--r--   0        0        0     7291 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/src/hatch_ci/scm.py
+-rw-r--r--   0        0        0     8240 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/src/hatch_ci/tools.py
+-rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/src/hatch_ci/version_hook.py
+-rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/tests/conftest.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/tests/requirements.txt
+-rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/tests/test_scm.py
+-rw-r--r--   0        0        0     7570 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/tests/test_tools.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/LICENSE.txt
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/README.md
+-rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/pyproject.toml
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b9/PKG-INFO
```

### Comparing `hatch_ci-0.0.2b8/.pre-commit-config.yaml` & `hatch_ci-0.0.2b9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.2b8/.github/workflows/beta.yml` & `hatch_ci-0.0.2b9/.github/workflows/beta.yml`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.2b8/.github/workflows/master.yml` & `hatch_ci-0.0.2b9/.github/workflows/master.yml`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.2b8/.github/workflows/tags.yml` & `hatch_ci-0.0.2b9/.github/workflows/tags.yml`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage.xml` & `hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/coverage.xml`

 * *Files 5% similar despite different names*

#### Comparing `hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage.xml` & `hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/coverage.xml`

```diff
@@ -1,16 +1,16 @@
 <?xml version="1.0" encoding="utf-8"?>
-<coverage version="7.2.7" timestamp="1690518716348" lines-valid="380" lines-covered="278" line-rate="0.7316" branches-valid="134" branches-covered="95" branch-rate="0.709" complexity="0">
+<coverage version="7.2.7" timestamp="1690531708184" lines-valid="380" lines-covered="278" line-rate="0.7316" branches-valid="154" branches-covered="113" branch-rate="0.7338" complexity="0">
   <!-- Generated by coverage.py: https://coverage.readthedocs.io/en/7.2.7 -->
   <!-- Based on https://raw.githubusercontent.com/cobertura/web/master/htdocs/xml/coverage-04.dtd -->
   <sources>
     <source>/home/runner/work/hatch-ci/hatch-ci</source>
   </sources>
   <packages>
-    <package name="src.hatch_ci" line-rate="0.7316" branch-rate="0.709" complexity="0">
+    <package name="src.hatch_ci" line-rate="0.7316" branch-rate="0.7338" complexity="0">
       <classes>
         <class name="__init__.py" filename="src/hatch_ci/__init__.py" complexity="0" line-rate="1" branch-rate="1">
           <methods/>
           <lines>
             <line number="1" hits="1"/>
             <line number="2" hits="1"/>
           </lines>
@@ -63,25 +63,25 @@
         </class>
         <class name="common.py" filename="src/hatch_ci/common.py" complexity="0" line-rate="0" branch-rate="1">
           <methods/>
           <lines>
             <line number="1" hits="0"/>
           </lines>
         </class>
-        <class name="hooks.py" filename="src/hatch_ci/hooks.py" complexity="0" line-rate="0" branch-rate="1">
+        <class name="hooks.py" filename="src/hatch_ci/hooks.py" complexity="0" line-rate="0" branch-rate="0">
           <methods/>
           <lines>
             <line number="1" hits="0"/>
             <line number="3" hits="0"/>
             <line number="6" hits="0"/>
-            <line number="7" hits="0"/>
+            <line number="7" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="exit,6"/>
             <line number="8" hits="0"/>
           </lines>
         </class>
-        <class name="scm.py" filename="src/hatch_ci/scm.py" complexity="0" line-rate="0.8165" branch-rate="0.74">
+        <class name="scm.py" filename="src/hatch_ci/scm.py" complexity="0" line-rate="0.8165" branch-rate="0.7833">
           <methods/>
           <lines>
             <line number="3" hits="1"/>
             <line number="5" hits="1"/>
             <line number="6" hits="1"/>
             <line number="7" hits="1"/>
             <line number="8" hits="1"/>
@@ -117,15 +117,15 @@
             <line number="61" hits="1"/>
             <line number="62" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="63" hits="1"/>
             <line number="64" hits="1"/>
             <line number="66" hits="1"/>
             <line number="67" hits="1"/>
             <line number="69" hits="1"/>
-            <line number="70" hits="1"/>
+            <line number="70" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="71" hits="0"/>
             <line number="74" hits="1"/>
             <line number="75" hits="1"/>
             <line number="76" hits="1"/>
             <line number="77" hits="1"/>
             <line number="78" hits="1"/>
             <line number="80" hits="1"/>
@@ -147,30 +147,30 @@
             <line number="106" hits="1"/>
             <line number="107" hits="1"/>
             <line number="109" hits="1"/>
             <line number="110" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="111" hits="1"/>
             <line number="114" hits="1"/>
             <line number="115" hits="1"/>
-            <line number="116" hits="1"/>
+            <line number="116" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="117" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="118,119"/>
             <line number="118" hits="0"/>
             <line number="119" hits="0"/>
             <line number="121" hits="0"/>
             <line number="122" hits="0"/>
             <line number="124" hits="0"/>
             <line number="125" hits="0"/>
             <line number="127" hits="0"/>
             <line number="128" hits="0"/>
             <line number="136" hits="0"/>
             <line number="138" hits="1"/>
             <line number="139" hits="1"/>
             <line number="140" hits="1"/>
             <line number="142" hits="1"/>
-            <line number="143" hits="1"/>
+            <line number="143" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="144" hits="1"/>
             <line number="145" hits="1"/>
             <line number="146" hits="1"/>
             <line number="147" hits="0"/>
             <line number="148" hits="0"/>
             <line number="149" hits="1"/>
             <line number="151" hits="1"/>
@@ -198,27 +198,27 @@
             <line number="190" hits="1"/>
             <line number="191" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="192"/>
             <line number="192" hits="0"/>
             <line number="193" hits="1"/>
             <line number="194" hits="1"/>
             <line number="195" hits="1"/>
             <line number="197" hits="1"/>
-            <line number="198" hits="1"/>
+            <line number="198" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="199" hits="1"/>
             <line number="200" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="201" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="202" hits="1"/>
             <line number="203" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="204" hits="1"/>
             <line number="205" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="208"/>
             <line number="206" hits="1"/>
             <line number="208" hits="0"/>
             <line number="209" hits="1"/>
             <line number="211" hits="1"/>
-            <line number="212" hits="1"/>
+            <line number="212" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="213" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="exit,exit"/>
             <line number="219" hits="1"/>
             <line number="225" hits="1"/>
             <line number="227" hits="1"/>
             <line number="228" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="229"/>
             <line number="229" hits="0"/>
             <line number="230" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="231"/>
@@ -236,15 +236,15 @@
             <line number="254" hits="1"/>
             <line number="255" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="256"/>
             <line number="256" hits="0"/>
             <line number="257" hits="1"/>
             <line number="258" hits="0"/>
           </lines>
         </class>
-        <class name="tools.py" filename="src/hatch_ci/tools.py" complexity="0" line-rate="0.9423" branch-rate="0.8286">
+        <class name="tools.py" filename="src/hatch_ci/tools.py" complexity="0" line-rate="0.9423" branch-rate="0.8462">
           <methods/>
           <lines>
             <line number="1" hits="1"/>
             <line number="3" hits="1"/>
             <line number="4" hits="1"/>
             <line number="5" hits="1"/>
             <line number="6" hits="1"/>
@@ -256,28 +256,28 @@
             <line number="17" hits="1"/>
             <line number="20" hits="1"/>
             <line number="21" hits="1"/>
             <line number="24" hits="1"/>
             <line number="25" hits="1"/>
             <line number="28" hits="1"/>
             <line number="29" hits="1"/>
-            <line number="30" hits="1"/>
+            <line number="30" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="31" hits="1"/>
             <line number="32" hits="1"/>
             <line number="33" hits="1"/>
             <line number="34" hits="1"/>
             <line number="36" hits="1"/>
             <line number="39" hits="1"/>
             <line number="40" hits="1"/>
             <line number="41" hits="1"/>
             <line number="43" hits="1"/>
-            <line number="44" hits="1"/>
+            <line number="44" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="45" hits="1"/>
             <line number="47" hits="1"/>
-            <line number="48" hits="1"/>
+            <line number="48" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="49" hits="1"/>
             <line number="51" hits="1"/>
             <line number="52" hits="1"/>
             <line number="53" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="54" hits="1"/>
             <line number="55" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="56" hits="1"/>
@@ -353,15 +353,15 @@
             <line number="185" hits="1"/>
             <line number="186" hits="1"/>
             <line number="187" hits="1"/>
             <line number="188" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="189" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="190" hits="1"/>
             <line number="191" hits="1"/>
-            <line number="193" hits="1"/>
+            <line number="193" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="194" hits="1"/>
             <line number="195" hits="1"/>
             <line number="198" hits="1"/>
             <line number="213" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="214" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="215" hits="1"/>
             <line number="216" hits="1"/>
```

### Comparing `hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage/coverage_html.js` & `hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/coverage/coverage_html.js`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943___init___py.html` & `hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/coverage/d_7005a4ce5d73f943___init___py.html`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943___main___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-28 04:31 +0000
+            created at 2023-07-28 08:08 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -89,13 +89,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943___main___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-28 04:31 +0000
+            created at 2023-07-28 08:08 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 2 statements   2 run 0 missing 0 excluded 0 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-07-28 04:31 +0000
+at 2023-07-28 08:08 +0000
 
 
 1__version__ = "0.0.2" 
 2__hash__ = "" 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-07-28 04:31 +0000
+at 2023-07-28 08:08 +0000
```

### Comparing `hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943___main___py.html` & `hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/coverage/d_7005a4ce5d73f943___main___py.html`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_common_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-28 04:31 +0000
+            created at 2023-07-28 08:08 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -167,13 +167,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_common_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-28 04:31 +0000
+            created at 2023-07-28 08:08 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 41 statements   0 run 41 missing 2 excluded 0 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-07-28 04:31 +0000
+at 2023-07-28 08:08 +0000
 
 
 1from __future__ import annotations 
 2 
 3import argparse 
 4import functools 
 5import logging 
@@ -94,8 +94,8 @@
 76 run(**parse_args()) 
 77 
 78 
 79if __name__ == "__main__": 
 80 main() 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-07-28 04:31 +0000
+at 2023-07-28 08:08 +0000
```

### Comparing `hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_common_py.html` & `hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/coverage/d_7005a4ce5d73f943_common_py.html`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943___main___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_hooks_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-28 04:31 +0000
+            created at 2023-07-28 08:08 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -88,13 +88,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943___main___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_hooks_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-28 04:31 +0000
+            created at 2023-07-28 08:08 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,14 +7,14 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 1 statements   0 run 1 missing 0 excluded 0 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-07-28 04:31 +0000
+at 2023-07-28 08:08 +0000
 
 
 1PLUGIN_NAME = "ci" 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-07-28 04:31 +0000
+at 2023-07-28 08:08 +0000
```

### Comparing `hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_hooks_py.html` & `hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/coverage/d_7005a4ce5d73f943_hooks_py.html`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_common_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_scm_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-28 04:31 +0000
+            created at 2023-07-28 08:08 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -95,13 +95,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_common_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_scm_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-28 04:31 +0000
+            created at 2023-07-28 08:08 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,21 +7,21 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 5 statements   0 run 5 missing 0 excluded 0 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-07-28 04:31 +0000
+at 2023-07-28 08:08 +0000
 
 
 1from hatchling.plugin import hookimpl 
 2 
 3from hatch_ci.version_hook import CIVersionSource 
 4 
 5 
 6@hookimpl 
 7def hatch_register_version_source(): 
 8 return CIVersionSource 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-07-28 04:31 +0000
+at 2023-07-28 08:08 +0000
```

### Comparing `hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_scm_py.html` & `hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/coverage/d_7005a4ce5d73f943_scm_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for src/hatch_ci/scm.py: 80%</title>
+    <title>Coverage for src/hatch_ci/scm.py: 81%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>src/hatch_ci/scm.py</b>:
-            <span class="pc_cov">80%</span>
+            <span class="pc_cov">81%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_hooks_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_tools_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-28 04:31 +0000
+            created at 2023-07-28 08:08 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -345,13 +345,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_hooks_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_tools_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-28 04:31 +0000
+            created at 2023-07-28 08:08 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
 
-****** Coverage for src/hatch_ci/scm.py: 80% ******
+****** Coverage for src/hatch_ci/scm.py: 81% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x p   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 158 statements   129 run 29 missing 0 excluded 7 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-07-28 04:31 +0000
+at 2023-07-28 08:08 +0000
 
 
 1# see https://pypi.org/project/setuptools-github 
 2# copy of setuptools_github.scm 
 3from __future__ import annotations 
 4 
 5import dataclasses as dc 
@@ -279,8 +279,8 @@
 255 if str(cur) == cur.root: 255&#x202F;&#x219B;&#x202F;256line 255 didn't jump
 to line 256, because the condition on line 255 was never true
 256 break 
 257 cur = cur.parent 
 258 return None 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-07-28 04:31 +0000
+at 2023-07-28 08:08 +0000
```

### Comparing `hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_tools_py.html` & `hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/coverage/d_7005a4ce5d73f943_tools_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_scm_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_version_hook_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-28 04:31 +0000
+            created at 2023-07-28 08:08 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -368,13 +368,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_scm_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_version_hook_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-28 04:31 +0000
+            created at 2023-07-28 08:08 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 156 statements   147 run 9 missing 0 excluded 8 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-07-28 04:31 +0000
+at 2023-07-28 08:08 +0000
 
 
 1from __future__ import annotations 
 2 
 3import ast 
 4import json 
 5import re 
@@ -305,8 +305,8 @@
 277 short = gdata["sha"] + ("*" if dirty else "") 
 278 
 279 set_module_var(path, "__version__", version) 
 280 set_module_var(path, "__hash__", short) 
 281 return version 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-07-28 04:31 +0000
+at 2023-07-28 08:08 +0000
```

### Comparing `hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_version_hook_py.html` & `hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/coverage/d_7005a4ce5d73f943_version_hook_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_tools_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-28 04:31 +0000
+            created at 2023-07-28 08:08 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -166,13 +166,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_tools_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-28 04:31 +0000
+            created at 2023-07-28 08:08 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 17 statements   0 run 17 missing 0 excluded 0 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-07-28 04:31 +0000
+at 2023-07-28 08:08 +0000
 
 
 1from hatchling.version.source.plugin.interface import VersionSourceInterface 
 2 
 3from .common import PLUGIN_NAME 
 4 
 5 
@@ -92,8 +92,8 @@
 76 f"no 'version-file' key for plugin {self.PLUGIN_NAME}" 
 77 ) 
 78 version = tools.update_version(initfile, getenv("GITHUB_DUMP"),
 abort=False) 
 79 return {"version": version} 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-07-28 04:31 +0000
+at 2023-07-28 08:08 +0000
```

### Comparing `hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage/favicon_32.png` & `hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/coverage/favicon_32.png`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage/index.html` & `hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/coverage/index.html`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             </div>
         </aside>
         <form id="filter_container">
             <input id="filter" type="text" value="" placeholder="filter..." />
         </form>
         <p class="text">
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-28 04:31 +0000
+            created at 2023-07-28 08:08 +0000
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
@@ -93,35 +93,35 @@
                 <td class="right" data-ratio="0 1">0%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_7005a4ce5d73f943_hooks_py.html">src/hatch_ci/hooks.py</a></td>
                 <td>5</td>
                 <td>5</td>
                 <td>0</td>
+                <td>2</td>
                 <td>0</td>
-                <td>0</td>
-                <td class="right" data-ratio="0 5">0%</td>
+                <td class="right" data-ratio="0 7">0%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_7005a4ce5d73f943_scm_py.html">src/hatch_ci/scm.py</a></td>
                 <td>158</td>
                 <td>29</td>
                 <td>0</td>
-                <td>50</td>
+                <td>60</td>
                 <td>7</td>
-                <td class="right" data-ratio="166 208">80%</td>
+                <td class="right" data-ratio="176 218">81%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_7005a4ce5d73f943_tools_py.html">src/hatch_ci/tools.py</a></td>
                 <td>156</td>
                 <td>9</td>
                 <td>0</td>
-                <td>70</td>
+                <td>78</td>
                 <td>8</td>
-                <td class="right" data-ratio="205 226">91%</td>
+                <td class="right" data-ratio="213 234">91%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_7005a4ce5d73f943_version_hook_py.html">src/hatch_ci/version_hook.py</a></td>
                 <td>17</td>
                 <td>17</td>
                 <td>0</td>
                 <td>2</td>
@@ -131,29 +131,29 @@
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
                 <td>380</td>
                 <td>102</td>
                 <td>2</td>
-                <td>134</td>
+                <td>154</td>
                 <td>15</td>
-                <td class="right" data-ratio="373 514">73%</td>
+                <td class="right" data-ratio="391 534">73%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-28 04:31 +0000
+            created at 2023-07-28 08:08 +0000
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_version_hook_py.html"/>
         <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943___init___py.html"/>
         <button type="button" class="button_prev_file" data-shortcut="["/>
         <button type="button" class="button_next_file" data-shortcut="]"/>
```

#### html2text {}

```diff
@@ -2,23 +2,23 @@
 ****** Coverage report: 73% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 n s m x b p c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
-coverage.py_v7.2.7, created at 2023-07-28 04:31 +0000
+coverage.py_v7.2.7, created at 2023-07-28 08:08 +0000
 
 Module                   statements missing excluded branches partial coverage
 src/hatch_ci/__init__.py 2          0       0        0        0       100%
 src/hatch_ci/__main__.py 41         41      2        12       0       0%
 src/hatch_ci/common.py   1          1       0        0        0       0%
-src/hatch_ci/hooks.py    5          5       0        0        0       0%
-src/hatch_ci/scm.py      158        29      0        50       7       80%
-src/hatch_ci/tools.py    156        9       0        70       8       91%
+src/hatch_ci/hooks.py    5          5       0        2        0       0%
+src/hatch_ci/scm.py      158        29      0        60       7       81%
+src/hatch_ci/tools.py    156        9       0        78       8       91%
 src/hatch_ci/            17         17      0        2        0       0%
 version_hook.py
-Total                    380        102     2        134      15      73%
+Total                    380        102     2        154      15      73%
 No items found using the specified filter.
 
-coverage.py_v7.2.7, created at 2023-07-28 04:31 +0000
+coverage.py_v7.2.7, created at 2023-07-28 08:08 +0000
  ____
```

### Comparing `hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage/keybd_closed.png` & `hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/coverage/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage/keybd_open.png` & `hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/coverage/keybd_open.png`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage/status.json` & `hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/coverage/status.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8702215608465609%*

 * *Differences: {"'files'": "{'d_7005a4ce5d73f943_hooks_py': {'index': {'nums': {insert: [(5, 2), (7, 2)], delete: "*

 * *            "[6, 5]}}}, 'd_7005a4ce5d73f943_scm_py': {'hash': 'fa0955d167891059f2f305ff96579186', "*

 * *            "'index': {'nums': {insert: [(5, 60)], delete: [5]}}}, 'd_7005a4ce5d73f943_tools_py': "*

 * *            "{'hash': 'd26b99f9fdb0ce4b436056b8755ef082', 'index': {'nums': {insert: [(5, 78)], "*

 * *            'delete: [5]}}}}',*

 * * "'globals'": "'912672b4f90cb2ca057250700c241fab'"}*

```diff
@@ -57,49 +57,49 @@
                 "html_filename": "d_7005a4ce5d73f943_hooks_py.html",
                 "nums": [
                     0,
                     1,
                     5,
                     0,
                     5,
+                    2,
                     0,
-                    0,
-                    0
+                    2
                 ],
                 "relative_filename": "src/hatch_ci/hooks.py"
             }
         },
         "d_7005a4ce5d73f943_scm_py": {
-            "hash": "a4f2fed685312e935805cf98d5b2c117",
+            "hash": "fa0955d167891059f2f305ff96579186",
             "index": {
                 "html_filename": "d_7005a4ce5d73f943_scm_py.html",
                 "nums": [
                     0,
                     1,
                     158,
                     0,
                     29,
-                    50,
+                    60,
                     7,
                     13
                 ],
                 "relative_filename": "src/hatch_ci/scm.py"
             }
         },
         "d_7005a4ce5d73f943_tools_py": {
-            "hash": "ca1bca58e18972d11e2aafa63d0716ba",
+            "hash": "d26b99f9fdb0ce4b436056b8755ef082",
             "index": {
                 "html_filename": "d_7005a4ce5d73f943_tools_py.html",
                 "nums": [
                     0,
                     1,
                     156,
                     0,
                     9,
-                    70,
+                    78,
                     8,
                     12
                 ],
                 "relative_filename": "src/hatch_ci/tools.py"
             }
         },
         "d_7005a4ce5d73f943_version_hook_py": {
@@ -117,10 +117,10 @@
                     2
                 ],
                 "relative_filename": "src/hatch_ci/version_hook.py"
             }
         }
     },
     "format": 2,
-    "globals": "713f643547f0168a8ef127bf4ac63403",
+    "globals": "912672b4f90cb2ca057250700c241fab",
     "version": "7.2.7"
 }
```

### Comparing `hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage/style.css` & `hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/coverage/style.css`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/junit/junit.html` & `hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/junit/junit.html`

 * *Files 1% similar despite different names*

```diff
@@ -435,17 +435,17 @@
     const rows = findAll('.results-table-row').filter(isAllRowsHidden);
     const allRowsHidden = rows.length == 0 ? true : false;
     const notFoundMessage = document.getElementById('not-found-message');
     notFoundMessage.hidden = !allRowsHidden;
 }
 </script>
     <h1>junit.html</h1>
-    <p>Report generated on 28-Jul-2023 at 04:31:56 by <a href="https://pypi.python.org/pypi/pytest-html">pytest-html</a> v3.2.0</p>
+    <p>Report generated on 28-Jul-2023 at 08:08:28 by <a href="https://pypi.python.org/pypi/pytest-html">pytest-html</a> v3.2.0</p>
     <h2>Summary</h2>
-    <p>13 tests ran in 0.88 seconds. </p>
+    <p>13 tests ran in 0.89 seconds. </p>
     <p class="filter" hidden="true">(Un)check the boxes to filter the results.</p><input checked="true" class="filter" data-test-result="passed" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="passed">13 passed</span>, <input checked="true" class="filter" data-test-result="skipped" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="skipped">0 skipped</span>, <input checked="true" class="filter" data-test-result="failed" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="failed">0 failed</span>, <input checked="true" class="filter" data-test-result="error" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="error">0 errors</span>, <input checked="true" class="filter" data-test-result="xfailed" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="xfailed">0 expected failures</span>, <input checked="true" class="filter" data-test-result="xpassed" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="xpassed">0 unexpected passes</span>
     <h2>Results</h2>
     <table id="results-table">
       <thead id="results-table-head">
         <tr>
           <th class="sortable result initial-sort" col="result">Result</th>
           <th class="sortable" col="name">Test</th>
@@ -453,34 +453,34 @@
           <th class="sortable links" col="links">Links</th></tr>
         <tr hidden="true" id="not-found-message">
           <th colspan="4">No results found. Try to check the filters</th></tr></thead>
       <tbody class="passed results-table-row">
         <tr>
           <td class="col-result">Passed</td>
           <td class="col-name">tests/test_scm.py::test_lookup</td>
-          <td class="col-duration">0.03</td>
+          <td class="col-duration">0.02</td>
           <td class="col-links"></td></tr>
         <tr>
           <td class="extra" colspan="4">
             <div class="empty log">No log output captured.</div></td></tr></tbody>
       <tbody class="passed results-table-row">
         <tr>
           <td class="col-result">Passed</td>
           <td class="col-name">tests/test_scm.py::test_handle_remote_and_local_repos</td>
-          <td class="col-duration">0.25</td>
+          <td class="col-duration">0.22</td>
           <td class="col-links"></td></tr>
         <tr>
           <td class="extra" colspan="4">
             <div class="log"> ------------------------------Captured stderr call------------------------------ <br/>Switched to a new branch &#x27;beta/0.0.3&#x27;
 Switched to a new branch &#x27;beta/0.0.4&#x27;
 Switched to branch &#x27;master&#x27;
 Cloning into &#x27;/tmp/pytest-of-runner/pytest-0/test_handle_remote_and_local_r0/test_check_version-repo1&#x27;...
 done.
 Switched to a new branch &#x27;beta/0.0.2&#x27;
-Cloning into &#x27;/tmp/pytest-of-runner/pytest-0/test_handle_remote_and_local_r0/E8FJKT&#x27;...
+Cloning into &#x27;/tmp/pytest-of-runner/pytest-0/test_handle_remote_and_local_r0/LYDE23&#x27;...
 done.
 Switched to a new branch &#x27;beta/0.0.1&#x27;
 fatal: a branch named &#x27;master&#x27; already exists
 From /tmp/pytest-of-runner/pytest-0/test_handle_remote_and_local_r0/test_check_version-repo1
  * [new branch]      beta/0.0.2 -&gt; repo1/beta/0.0.2
  * [new branch]      master     -&gt; repo1/master
 <br/></div></td></tr></tbody>
@@ -565,27 +565,27 @@
         <tr>
           <td class="extra" colspan="4">
             <div class="empty log">No log output captured.</div></td></tr></tbody>
       <tbody class="passed results-table-row">
         <tr>
           <td class="col-result">Passed</td>
           <td class="col-name">tests/test_tools.py::test_update_version_beta</td>
-          <td class="col-duration">0.10</td>
+          <td class="col-duration">0.09</td>
           <td class="col-links"></td></tr>
         <tr>
           <td class="extra" colspan="4">
             <div class="log"> ------------------------------Captured stderr call------------------------------ <br/>Switched to a new branch &#x27;beta/0.0.4&#x27;
 Updated 1 path from the index
 Updated 1 path from the index
 Switched to a new branch &#x27;beta/0.0.2&#x27;
 <br/></div></td></tr></tbody>
       <tbody class="passed results-table-row">
         <tr>
           <td class="col-result">Passed</td>
           <td class="col-name">tests/test_tools.py::test_update_version_release</td>
-          <td class="col-duration">0.06</td>
+          <td class="col-duration">0.05</td>
           <td class="col-links"></td></tr>
         <tr>
           <td class="extra" colspan="4">
             <div class="log"> ------------------------------Captured stderr call------------------------------ <br/>Switched to a new branch &#x27;beta/0.0.3&#x27;
 Updated 1 path from the index
 <br/></div></td></tr></tbody></table></body></html>
```

#### html2text {}

```diff
@@ -1,28 +1,28 @@
 ****** junit.html ******
-Report generated on 28-Jul-2023 at 04:31:56 by pytest-html v3.2.0
+Report generated on 28-Jul-2023 at 08:08:28 by pytest-html v3.2.0
 ***** Summary *****
-13 tests ran in 0.88 seconds.
+13 tests ran in 0.89 seconds.
 (Un)check the boxes to filter the results.
 *13 passed, *0 skipped, *0 failed, *0 errors, *0 expected failures, *0
 unexpected passes
 ***** Results *****
 Result Test                                                  Duration Links
 No results found. Try to check the filters
-Passed tests/test_scm.py::test_lookup                        0.03
+Passed tests/test_scm.py::test_lookup                        0.02
 No log output captured.
-Passed tests/test_scm.py::test_handle_remote_and_local_repos 0.25
+Passed tests/test_scm.py::test_handle_remote_and_local_repos 0.22
 ------------------------------Captured stderr call--------------------------
 ----
 Switched to a new branch &#x27;beta/0.0.3&#x27; Switched to a new branch
 &#x27;beta/0.0.4&#x27; Switched to branch &#x27;master&#x27; Cloning into
 &#x27;/tmp/pytest-of-runner/pytest-0/test_handle_remote_and_local_r0/
 test_check_version-repo1&#x27;... done. Switched to a new branch &#x27;beta/
 0.0.2&#x27; Cloning into &#x27;/tmp/pytest-of-runner/pytest-0/
-test_handle_remote_and_local_r0/E8FJKT&#x27;... done. Switched to a new
+test_handle_remote_and_local_r0/LYDE23&#x27;... done. Switched to a new
 branch &#x27;beta/0.0.1&#x27; fatal: a branch named &#x27;master&#x27;
 already exists From /tmp/pytest-of-runner/pytest-0/
 test_handle_remote_and_local_r0/test_check_version-repo1 * [new branch]
 beta/0.0.2 -> repo1/beta/0.0.2 * [new branch] master -> repo1/master
 Passed tests/test_tools.py::test_abort_exception             0.00
 No log output captured.
 Passed tests/test_tools.py::test_urmtree                     0.00
@@ -37,18 +37,18 @@
 No log output captured.
 Passed tests/test_tools.py::test_set_module_var_empty_file   0.00
 No log output captured.
 Passed tests/test_tools.py::test_bump_version                0.00
 No log output captured.
 Passed tests/test_tools.py::test_update_version_master       0.04
 No log output captured.
-Passed tests/test_tools.py::test_update_version_beta         0.10
+Passed tests/test_tools.py::test_update_version_beta         0.09
 ------------------------------Captured stderr call--------------------------
 ----
 Switched to a new branch &#x27;beta/0.0.4&#x27; Updated 1 path from the
 index Updated 1 path from the index Switched to a new branch &#x27;beta/
 0.0.2&#x27;
-Passed tests/test_tools.py::test_update_version_release      0.06
+Passed tests/test_tools.py::test_update_version_release      0.05
 ------------------------------Captured stderr call--------------------------
 ----
 Switched to a new branch &#x27;beta/0.0.3&#x27; Updated 1 path from the
 index
```

### Comparing `hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/junit/junit.xml` & `hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/junit/junit.xml`

 * *Files 6% similar despite different names*

#### Comparing `hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/junit/junit.xml` & `hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/junit/junit.xml`

```diff
@@ -1,18 +1,18 @@
 <?xml version="1.0" encoding="utf-8"?>
 <testsuites>
-  <testsuite name="pytest" errors="0" failures="0" skipped="0" tests="13" time="0.873" timestamp="2023-07-28T04:31:55.534223" hostname="fv-az484-818">
-    <testcase classname="tests.test_scm" name="test_lookup" time="0.033"/>
-    <testcase classname="tests.test_scm" name="test_handle_remote_and_local_repos" time="0.258"/>
+  <testsuite name="pytest" errors="0" failures="0" skipped="0" tests="13" time="0.877" timestamp="2023-07-28T08:08:27.375965" hostname="fv-az166-351">
+    <testcase classname="tests.test_scm" name="test_lookup" time="0.029"/>
+    <testcase classname="tests.test_scm" name="test_handle_remote_and_local_repos" time="0.223"/>
     <testcase classname="tests.test_tools" name="test_abort_exception" time="0.001"/>
-    <testcase classname="tests.test_tools" name="test_urmtree" time="0.001"/>
+    <testcase classname="tests.test_tools" name="test_urmtree" time="0.002"/>
     <testcase classname="tests.test_tools" name="test_indent" time="0.001"/>
     <testcase classname="tests.test_tools" name="test_list_of_paths" time="0.001"/>
-    <testcase classname="tests.test_tools" name="test_get_module_var" time="0.002"/>
+    <testcase classname="tests.test_tools" name="test_get_module_var" time="0.003"/>
     <testcase classname="tests.test_tools" name="test_set_module_var" time="0.003"/>
     <testcase classname="tests.test_tools" name="test_set_module_var_empty_file" time="0.002"/>
     <testcase classname="tests.test_tools" name="test_bump_version" time="0.001"/>
-    <testcase classname="tests.test_tools" name="test_update_version_master" time="0.048"/>
-    <testcase classname="tests.test_tools" name="test_update_version_beta" time="0.107"/>
-    <testcase classname="tests.test_tools" name="test_update_version_release" time="0.064"/>
+    <testcase classname="tests.test_tools" name="test_update_version_master" time="0.044"/>
+    <testcase classname="tests.test_tools" name="test_update_version_beta" time="0.090"/>
+    <testcase classname="tests.test_tools" name="test_update_version_release" time="0.059"/>
   </testsuite>
 </testsuites>
```

### Comparing `hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/mypy/index.html` & `hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/mypy/index.html`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/mypy/mypy-html.css` & `hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/mypy/mypy-html.css`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/__init__.py.html` & `hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/mypy/html/src/hatch_ci/__init__.py.html`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/__main__.py.html` & `hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/mypy/html/src/hatch_ci/__main__.py.html`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/common.py.html` & `hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/mypy/html/src/hatch_ci/common.py.html`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/hooks.py.html` & `hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/mypy/html/src/hatch_ci/hooks.py.html`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/scm.py.html` & `hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/mypy/html/src/hatch_ci/scm.py.html`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/tools.py.html` & `hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/mypy/html/src/hatch_ci/tools.py.html`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/version_hook.py.html` & `hatch_ci-0.0.2b9/build/qa-3.11-ubuntu-latest/mypy/html/src/hatch_ci/version_hook.py.html`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.2b8/src/hatch_ci/__main__.py` & `hatch_ci-0.0.2b9/src/hatch_ci/__main__.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.2b8/src/hatch_ci/scm.py` & `hatch_ci-0.0.2b9/src/hatch_ci/scm.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.2b8/src/hatch_ci/tools.py` & `hatch_ci-0.0.2b9/src/hatch_ci/tools.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.2b8/src/hatch_ci/version_hook.py` & `hatch_ci-0.0.2b9/src/hatch_ci/version_hook.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.2b8/tests/conftest.py` & `hatch_ci-0.0.2b9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.2b8/tests/test_scm.py` & `hatch_ci-0.0.2b9/tests/test_scm.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.2b8/tests/test_tools.py` & `hatch_ci-0.0.2b9/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.2b8/LICENSE.txt` & `hatch_ci-0.0.2b9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.2b8/pyproject.toml` & `hatch_ci-0.0.2b9/pyproject.toml`

 * *Files identical despite different names*

