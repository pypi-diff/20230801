# Comparing `tmp/TopologySuperpositionTheorem-0.0.1.tar.gz` & `tmp/TopologySuperpositionTheorem-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TopologySuperpositionTheorem-0.0.1.tar", last modified: Tue Aug  1 12:58:08 2023, max compression
+gzip compressed data, was "TopologySuperpositionTheorem-0.0.2.tar", last modified: Tue Aug  1 13:03:40 2023, max compression
```

## Comparing `TopologySuperpositionTheorem-0.0.1.tar` & `TopologySuperpositionTheorem-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 marotant (1774385106) marotant (1774385106)        0 2023-08-01 12:58:08.030832 TopologySuperpositionTheorem-0.0.1/
--rw-rw-r--   0 marotant (1774385106) marotant (1774385106)    16725 2023-08-01 12:55:04.000000 TopologySuperpositionTheorem-0.0.1/LICENSE.md
--rw-rw-r--   0 marotant (1774385106) marotant (1774385106)     2633 2023-08-01 12:58:08.030832 TopologySuperpositionTheorem-0.0.1/PKG-INFO
--rwxrwxrwx   0 marotant (1774385106) marotant (1774385106)     1233 2023-08-01 12:42:37.000000 TopologySuperpositionTheorem-0.0.1/README.md
-drwxrwxr-x   0 marotant (1774385106) marotant (1774385106)        0 2023-08-01 12:58:08.022832 TopologySuperpositionTheorem-0.0.1/TopologySuperpositionTheorem.egg-info/
--rw-rw-r--   0 marotant (1774385106) marotant (1774385106)     2633 2023-08-01 12:58:07.000000 TopologySuperpositionTheorem-0.0.1/TopologySuperpositionTheorem.egg-info/PKG-INFO
--rw-rw-r--   0 marotant (1774385106) marotant (1774385106)      935 2023-08-01 12:58:08.000000 TopologySuperpositionTheorem-0.0.1/TopologySuperpositionTheorem.egg-info/SOURCES.txt
--rw-rw-r--   0 marotant (1774385106) marotant (1774385106)        1 2023-08-01 12:58:07.000000 TopologySuperpositionTheorem-0.0.1/TopologySuperpositionTheorem.egg-info/dependency_links.txt
--rw-rw-r--   0 marotant (1774385106) marotant (1774385106)        1 2023-08-01 09:32:05.000000 TopologySuperpositionTheorem-0.0.1/TopologySuperpositionTheorem.egg-info/not-zip-safe
--rw-rw-r--   0 marotant (1774385106) marotant (1774385106)       32 2023-08-01 12:58:07.000000 TopologySuperpositionTheorem-0.0.1/TopologySuperpositionTheorem.egg-info/requires.txt
--rw-rw-r--   0 marotant (1774385106) marotant (1774385106)       22 2023-08-01 12:58:07.000000 TopologySuperpositionTheorem-0.0.1/TopologySuperpositionTheorem.egg-info/top_level.txt
--rw-rw-r--   0 marotant (1774385106) marotant (1774385106)      818 2023-08-01 12:58:08.030832 TopologySuperpositionTheorem-0.0.1/setup.cfg
--rw-rw-r--   0 marotant (1774385106) marotant (1774385106)     1314 2023-08-01 09:11:01.000000 TopologySuperpositionTheorem-0.0.1/setup.py
-drwxrwxr-x   0 marotant (1774385106) marotant (1774385106)        0 2023-08-01 12:58:08.022832 TopologySuperpositionTheorem-0.0.1/superposition_theorem/
--rw-rw-r--   0 marotant (1774385106) marotant (1774385106)        0 2023-08-01 07:18:03.000000 TopologySuperpositionTheorem-0.0.1/superposition_theorem/__init__.py
-drwxrwxr-x   0 marotant (1774385106) marotant (1774385106)        0 2023-08-01 12:58:08.026832 TopologySuperpositionTheorem-0.0.1/superposition_theorem/core/
--rw-rw-r--   0 marotant (1774385106) marotant (1774385106)        0 2023-08-01 07:18:03.000000 TopologySuperpositionTheorem-0.0.1/superposition_theorem/core/__init__.py
--rw-rw-r--   0 marotant (1774385106) marotant (1774385106)     6802 2023-08-01 09:33:39.000000 TopologySuperpositionTheorem-0.0.1/superposition_theorem/core/compute_beta_coefficients.py
--rw-rw-r--   0 marotant (1774385106) marotant (1774385106)    22168 2023-08-01 12:12:58.000000 TopologySuperpositionTheorem-0.0.1/superposition_theorem/core/compute_power_flows.py
--rw-rw-r--   0 marotant (1774385106) marotant (1774385106)     3482 2023-08-01 07:18:03.000000 TopologySuperpositionTheorem-0.0.1/superposition_theorem/main.py
-drwxrwxr-x   0 marotant (1774385106) marotant (1774385106)        0 2023-08-01 12:58:08.030832 TopologySuperpositionTheorem-0.0.1/superposition_theorem/tests/
--rw-rw-r--   0 marotant (1774385106) marotant (1774385106)        0 2023-08-01 07:18:03.000000 TopologySuperpositionTheorem-0.0.1/superposition_theorem/tests/__init__.py
--rw-rw-r--   0 marotant (1774385106) marotant (1774385106)    32055 2023-08-01 12:33:03.000000 TopologySuperpositionTheorem-0.0.1/superposition_theorem/tests/test_different_action_type_superposition.py
--rw-rw-r--   0 marotant (1774385106) marotant (1774385106)     5210 2023-08-01 08:47:35.000000 TopologySuperpositionTheorem-0.0.1/superposition_theorem/tests/test_line_disconnection_superposition.py
--rw-rw-r--   0 marotant (1774385106) marotant (1774385106)     7085 2023-08-01 08:47:30.000000 TopologySuperpositionTheorem-0.0.1/superposition_theorem/tests/test_line_reconnection_superposition.py
--rw-rw-r--   0 marotant (1774385106) marotant (1774385106)     8323 2023-08-01 08:47:24.000000 TopologySuperpositionTheorem-0.0.1/superposition_theorem/tests/test_node_merging_superposition.py
--rw-rw-r--   0 marotant (1774385106) marotant (1774385106)     7583 2023-08-01 11:38:40.000000 TopologySuperpositionTheorem-0.0.1/superposition_theorem/tests/test_node_splitting_superposition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:03:40.952002 TopologySuperpositionTheorem-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-08-01 13:03:28.000000 TopologySuperpositionTheorem-0.0.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-08-01 13:03:40.952002 TopologySuperpositionTheorem-0.0.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1233 2023-08-01 13:03:28.000000 TopologySuperpositionTheorem-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:03:40.952002 TopologySuperpositionTheorem-0.0.2/TopologySuperpositionTheorem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-08-01 13:03:40.000000 TopologySuperpositionTheorem-0.0.2/TopologySuperpositionTheorem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-08-01 13:03:40.000000 TopologySuperpositionTheorem-0.0.2/TopologySuperpositionTheorem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 13:03:40.000000 TopologySuperpositionTheorem-0.0.2/TopologySuperpositionTheorem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 13:03:40.000000 TopologySuperpositionTheorem-0.0.2/TopologySuperpositionTheorem.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-01 13:03:40.000000 TopologySuperpositionTheorem-0.0.2/TopologySuperpositionTheorem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 13:03:40.000000 TopologySuperpositionTheorem-0.0.2/TopologySuperpositionTheorem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-08-01 13:03:40.952002 TopologySuperpositionTheorem-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-01 13:03:28.000000 TopologySuperpositionTheorem-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:03:40.952002 TopologySuperpositionTheorem-0.0.2/superposition_theorem/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 13:03:28.000000 TopologySuperpositionTheorem-0.0.2/superposition_theorem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:03:40.952002 TopologySuperpositionTheorem-0.0.2/superposition_theorem/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 13:03:28.000000 TopologySuperpositionTheorem-0.0.2/superposition_theorem/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-08-01 13:03:28.000000 TopologySuperpositionTheorem-0.0.2/superposition_theorem/core/compute_beta_coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22168 2023-08-01 13:03:28.000000 TopologySuperpositionTheorem-0.0.2/superposition_theorem/core/compute_power_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-08-01 13:03:28.000000 TopologySuperpositionTheorem-0.0.2/superposition_theorem/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:03:40.952002 TopologySuperpositionTheorem-0.0.2/superposition_theorem/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 13:03:28.000000 TopologySuperpositionTheorem-0.0.2/superposition_theorem/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32055 2023-08-01 13:03:28.000000 TopologySuperpositionTheorem-0.0.2/superposition_theorem/tests/test_different_action_type_superposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-08-01 13:03:28.000000 TopologySuperpositionTheorem-0.0.2/superposition_theorem/tests/test_line_disconnection_superposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7085 2023-08-01 13:03:28.000000 TopologySuperpositionTheorem-0.0.2/superposition_theorem/tests/test_line_reconnection_superposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8323 2023-08-01 13:03:28.000000 TopologySuperpositionTheorem-0.0.2/superposition_theorem/tests/test_node_merging_superposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-08-01 13:03:28.000000 TopologySuperpositionTheorem-0.0.2/superposition_theorem/tests/test_node_splitting_superposition.py
```

### Comparing `TopologySuperpositionTheorem-0.0.1/LICENSE.md` & `TopologySuperpositionTheorem-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `TopologySuperpositionTheorem-0.0.1/PKG-INFO` & `TopologySuperpositionTheorem-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,15 @@
 Metadata-Version: 2.1
 Name: TopologySuperpositionTheorem
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for efficient combinatorial topological actions power flow computation based on the extended superposition theorem for powersystems
 Home-page: https://github.com/marota/Topology_Superposition_Theorem
 Author: Antoine MAROT
 License: Mozilla Public License 2.0 (MPL 2.0)
-Description: # Topology_Superposition_Theorem
-        
-        This is a package for efficient combinatorial topological actions power flow computation based on the extended superposition theorem for power systems.
-        
-        Here is the extended superposition theroem for topological changes. The resulting powerflows is a linear combination of unitary change power flows:
-        
-        𝑃𝐹(𝑇)=𝛼×𝑃𝐹(𝑇𝑟𝑒𝑓)+𝛽1×𝑃𝐹(𝑇𝑟𝑒𝑓∘𝜏1)+𝛽2×𝑃𝐹(𝑇𝑟𝑒𝑓∘𝜏2)
-        
-        with 𝑇=𝑇𝑟𝑒𝑓∘𝜏1∘𝜏2 and 𝛼=1−𝛽1−𝛽2
-        
-        We have 𝑇𝑟𝑒𝑓 as the reference topology from which we apply topological changes 𝜏1 and 𝜏2 in indifferent order to reach a target topology 𝑇. Finding the betas simply stems from solving a linear system of dimension the number of considered changes. Only minimal information from individual power flow state is needed for this, without knowledge of any underlying grid properties or complete adjacency matrix.
-        
-        For more information, see paper (under writing) and abstract in reference folder.
-        
-        # Get started
-        
-        you can install the package from pypi
-        ```
-        pip install topologysuperpositiontheorem
-        ```
-        
-        you can them run the getting started notebook to get familiar with the package
 Keywords: combinatorial powerflow topology power-systems
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
@@ -42,7 +19,31 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+# Topology_Superposition_Theorem
+
+This is a package for efficient combinatorial topological actions power flow computation based on the extended superposition theorem for power systems.
+
+Here is the extended superposition theroem for topological changes. The resulting powerflows is a linear combination of unitary change power flows:
+
+𝑃𝐹(𝑇)=𝛼×𝑃𝐹(𝑇𝑟𝑒𝑓)+𝛽1×𝑃𝐹(𝑇𝑟𝑒𝑓∘𝜏1)+𝛽2×𝑃𝐹(𝑇𝑟𝑒𝑓∘𝜏2)
+
+with 𝑇=𝑇𝑟𝑒𝑓∘𝜏1∘𝜏2 and 𝛼=1−𝛽1−𝛽2
+
+We have 𝑇𝑟𝑒𝑓 as the reference topology from which we apply topological changes 𝜏1 and 𝜏2 in indifferent order to reach a target topology 𝑇. Finding the betas simply stems from solving a linear system of dimension the number of considered changes. Only minimal information from individual power flow state is needed for this, without knowledge of any underlying grid properties or complete adjacency matrix.
+
+For more information, see paper (under writing) and abstract in reference folder.
+
+# Get started
+
+you can install the package from pypi
+```
+pip install topologysuperpositiontheorem
+```
+
+you can them run the getting started notebook to get familiar with the package
```

### Comparing `TopologySuperpositionTheorem-0.0.1/README.md` & `TopologySuperpositionTheorem-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `TopologySuperpositionTheorem-0.0.1/TopologySuperpositionTheorem.egg-info/PKG-INFO` & `TopologySuperpositionTheorem-0.0.2/TopologySuperpositionTheorem.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,15 @@
 Metadata-Version: 2.1
 Name: TopologySuperpositionTheorem
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for efficient combinatorial topological actions power flow computation based on the extended superposition theorem for powersystems
 Home-page: https://github.com/marota/Topology_Superposition_Theorem
 Author: Antoine MAROT
 License: Mozilla Public License 2.0 (MPL 2.0)
-Description: # Topology_Superposition_Theorem
-        
-        This is a package for efficient combinatorial topological actions power flow computation based on the extended superposition theorem for power systems.
-        
-        Here is the extended superposition theroem for topological changes. The resulting powerflows is a linear combination of unitary change power flows:
-        
-        𝑃𝐹(𝑇)=𝛼×𝑃𝐹(𝑇𝑟𝑒𝑓)+𝛽1×𝑃𝐹(𝑇𝑟𝑒𝑓∘𝜏1)+𝛽2×𝑃𝐹(𝑇𝑟𝑒𝑓∘𝜏2)
-        
-        with 𝑇=𝑇𝑟𝑒𝑓∘𝜏1∘𝜏2 and 𝛼=1−𝛽1−𝛽2
-        
-        We have 𝑇𝑟𝑒𝑓 as the reference topology from which we apply topological changes 𝜏1 and 𝜏2 in indifferent order to reach a target topology 𝑇. Finding the betas simply stems from solving a linear system of dimension the number of considered changes. Only minimal information from individual power flow state is needed for this, without knowledge of any underlying grid properties or complete adjacency matrix.
-        
-        For more information, see paper (under writing) and abstract in reference folder.
-        
-        # Get started
-        
-        you can install the package from pypi
-        ```
-        pip install topologysuperpositiontheorem
-        ```
-        
-        you can them run the getting started notebook to get familiar with the package
 Keywords: combinatorial powerflow topology power-systems
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
@@ -42,7 +19,31 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+# Topology_Superposition_Theorem
+
+This is a package for efficient combinatorial topological actions power flow computation based on the extended superposition theorem for power systems.
+
+Here is the extended superposition theroem for topological changes. The resulting powerflows is a linear combination of unitary change power flows:
+
+𝑃𝐹(𝑇)=𝛼×𝑃𝐹(𝑇𝑟𝑒𝑓)+𝛽1×𝑃𝐹(𝑇𝑟𝑒𝑓∘𝜏1)+𝛽2×𝑃𝐹(𝑇𝑟𝑒𝑓∘𝜏2)
+
+with 𝑇=𝑇𝑟𝑒𝑓∘𝜏1∘𝜏2 and 𝛼=1−𝛽1−𝛽2
+
+We have 𝑇𝑟𝑒𝑓 as the reference topology from which we apply topological changes 𝜏1 and 𝜏2 in indifferent order to reach a target topology 𝑇. Finding the betas simply stems from solving a linear system of dimension the number of considered changes. Only minimal information from individual power flow state is needed for this, without knowledge of any underlying grid properties or complete adjacency matrix.
+
+For more information, see paper (under writing) and abstract in reference folder.
+
+# Get started
+
+you can install the package from pypi
+```
+pip install topologysuperpositiontheorem
+```
+
+you can them run the getting started notebook to get familiar with the package
```

### Comparing `TopologySuperpositionTheorem-0.0.1/TopologySuperpositionTheorem.egg-info/SOURCES.txt` & `TopologySuperpositionTheorem-0.0.2/TopologySuperpositionTheorem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TopologySuperpositionTheorem-0.0.1/setup.cfg` & `TopologySuperpositionTheorem-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `TopologySuperpositionTheorem-0.0.1/setup.py` & `TopologySuperpositionTheorem-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,19 +18,19 @@
     "required": [
         "grid2op>=1.9",
         "lightsim2grid>=0.7"
     ]
 }
 
 setup(name='TopologySuperpositionTheorem',
-      version='0.0.1',
+      version='0.0.2',
       description='A package for efficient combinatorial topological actions power flow computation based on the extended superposition theorem for powersystems',
       long_description=long_description,
       long_description_content_type="text/markdown",
       author='Antoine MAROT',
       python_requires='>=3.8',
       url="https://github.com/marota/Topology_Superposition_Theorem",
       packages=setuptools.find_packages(),
       include_package_data=True,
       install_requires=pkgs["required"],
       zip_safe=False,
-      )
+      )
```

### Comparing `TopologySuperpositionTheorem-0.0.1/superposition_theorem/core/compute_beta_coefficients.py` & `TopologySuperpositionTheorem-0.0.2/superposition_theorem/core/compute_beta_coefficients.py`

 * *Files identical despite different names*

### Comparing `TopologySuperpositionTheorem-0.0.1/superposition_theorem/core/compute_power_flows.py` & `TopologySuperpositionTheorem-0.0.2/superposition_theorem/core/compute_power_flows.py`

 * *Files identical despite different names*

### Comparing `TopologySuperpositionTheorem-0.0.1/superposition_theorem/main.py` & `TopologySuperpositionTheorem-0.0.2/superposition_theorem/main.py`

 * *Files identical despite different names*

### Comparing `TopologySuperpositionTheorem-0.0.1/superposition_theorem/tests/test_different_action_type_superposition.py` & `TopologySuperpositionTheorem-0.0.2/superposition_theorem/tests/test_different_action_type_superposition.py`

 * *Files identical despite different names*

### Comparing `TopologySuperpositionTheorem-0.0.1/superposition_theorem/tests/test_line_disconnection_superposition.py` & `TopologySuperpositionTheorem-0.0.2/superposition_theorem/tests/test_line_disconnection_superposition.py`

 * *Files identical despite different names*

### Comparing `TopologySuperpositionTheorem-0.0.1/superposition_theorem/tests/test_line_reconnection_superposition.py` & `TopologySuperpositionTheorem-0.0.2/superposition_theorem/tests/test_line_reconnection_superposition.py`

 * *Files identical despite different names*

### Comparing `TopologySuperpositionTheorem-0.0.1/superposition_theorem/tests/test_node_merging_superposition.py` & `TopologySuperpositionTheorem-0.0.2/superposition_theorem/tests/test_node_merging_superposition.py`

 * *Files identical despite different names*

### Comparing `TopologySuperpositionTheorem-0.0.1/superposition_theorem/tests/test_node_splitting_superposition.py` & `TopologySuperpositionTheorem-0.0.2/superposition_theorem/tests/test_node_splitting_superposition.py`

 * *Files identical despite different names*

