# Comparing `tmp/myqlm_simulators-1.7.1-py3-none-any.whl.zip` & `tmp/myqlm_simulators-1.9.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 19442 bytes, number of entries: 12
--rw-r--r--  2.0 unx      890 b- defN 22-Nov-04 21:33 qat/pylinalg/__init__.py
--rw-r--r--  2.0 unx     8263 b- defN 22-Nov-04 21:33 qat/pylinalg/service.py
--rw-r--r--  2.0 unx    16753 b- defN 22-Nov-04 21:33 qat/pylinalg/simulator.py
--rw-r--r--  2.0 unx      933 b- defN 22-Nov-04 21:33 qat/qpus/hook_pylinalg.py
--rw-r--r--  2.0 unx      983 b- defN 22-Nov-04 21:33 qat/simulated_annealing/__init__.py
--rw-r--r--  2.0 unx     9892 b- defN 22-Nov-04 21:33 qat/simulated_annealing/service.py
--rw-r--r--  2.0 unx    11340 b- defN 22-Nov-04 21:33 myqlm_simulators-1.7.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      983 b- defN 22-Nov-04 21:33 myqlm_simulators-1.7.1.dist-info/METADATA
--rw-r--r--  2.0 unx      161 b- defN 22-Nov-04 21:33 myqlm_simulators-1.7.1.dist-info/NOTICE
--rw-r--r--  2.0 unx       92 b- defN 22-Nov-04 21:33 myqlm_simulators-1.7.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 22-Nov-04 21:33 myqlm_simulators-1.7.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1031 b- defN 22-Nov-04 21:33 myqlm_simulators-1.7.1.dist-info/RECORD
-12 files, 51325 bytes uncompressed, 17690 bytes compressed:  65.5%
+Zip file size: 19462 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      890 b- defN 23-Jul-31 22:46 qat/pylinalg/__init__.py
+-rw-r--r--  2.0 unx     8259 b- defN 23-Jul-31 22:46 qat/pylinalg/service.py
+-rw-r--r--  2.0 unx    16753 b- defN 23-Jul-31 22:46 qat/pylinalg/simulator.py
+-rw-r--r--  2.0 unx     1022 b- defN 23-Jul-31 22:46 qat/qpus/hook_pylinalg.py
+-rw-r--r--  2.0 unx      983 b- defN 23-Jul-31 22:46 qat/simulated_annealing/__init__.py
+-rw-r--r--  2.0 unx     9804 b- defN 23-Jul-31 22:46 qat/simulated_annealing/service.py
+-rw-r--r--  2.0 unx    11340 b- defN 23-Jul-31 22:46 myqlm_simulators-1.9.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      983 b- defN 23-Jul-31 22:46 myqlm_simulators-1.9.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      161 b- defN 23-Jul-31 22:46 myqlm_simulators-1.9.1.dist-info/NOTICE
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-31 22:46 myqlm_simulators-1.9.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 23-Jul-31 22:46 myqlm_simulators-1.9.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1032 b- defN 23-Jul-31 22:46 myqlm_simulators-1.9.1.dist-info/RECORD
+12 files, 51323 bytes uncompressed, 17710 bytes compressed:  65.5%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: qat/simulated_annealing/__init__.py
 Comment: 
 
 Filename: qat/simulated_annealing/service.py
 Comment: 
 
-Filename: myqlm_simulators-1.7.1.dist-info/LICENSE
+Filename: myqlm_simulators-1.9.1.dist-info/LICENSE
 Comment: 
 
-Filename: myqlm_simulators-1.7.1.dist-info/METADATA
+Filename: myqlm_simulators-1.9.1.dist-info/METADATA
 Comment: 
 
-Filename: myqlm_simulators-1.7.1.dist-info/NOTICE
+Filename: myqlm_simulators-1.9.1.dist-info/NOTICE
 Comment: 
 
-Filename: myqlm_simulators-1.7.1.dist-info/WHEEL
+Filename: myqlm_simulators-1.9.1.dist-info/WHEEL
 Comment: 
 
-Filename: myqlm_simulators-1.7.1.dist-info/top_level.txt
+Filename: myqlm_simulators-1.9.1.dist-info/top_level.txt
 Comment: 
 
-Filename: myqlm_simulators-1.7.1.dist-info/RECORD
+Filename: myqlm_simulators-1.9.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qat/pylinalg/service.py

```diff
@@ -32,15 +32,15 @@
 from .simulator import simulate, measure, compute_observable_average
 
 
 class PyLinalg(QPUHandler):
     """
     Simple linalg simulator plugin.
 
-    Inherits :func:`serve` and :func:`submit` method from :class:`qat.core.qpu.QPUHandler`
+    Inherits :func:`serve` and :func:`submit` method from :class:`qat.qpus.QPUHandler`
     Only the :func:`submit_job` method is simulator-specific and defined here.
 
     """
 
     def __init__(self):
         super(PyLinalg, self).__init__() # calls QPUHandler __init__()
```

## qat/qpus/hook_pylinalg.py

```diff
@@ -15,10 +15,12 @@
     software distributed under the License is distributed on an
     "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 """
 
-from qat.pylinalg import PyLinalg
-from qat.simulated_annealing import SimulatedAnnealing
-
+# Declare QPUs available in this package
+__qlm_importables__ = {
+    "PyLinalg": "qat.pylinalg:PyLinalg",
+    "SimulatedAnnealing": "qat.simulated_annealing:SimulatedAnnealing"
+}
```

## qat/simulated_annealing/service.py

```diff
@@ -29,16 +29,15 @@
 from qat.core.variables import ArithExpression
 from qat.core.wrappers.result import Sample, Result, aggregate_data
 from qat.lang.AQASM.bits import QRegister
 
 
 class SimulatedAnnealing(QPUHandler):
     """
-    A Simulated Annealing solver interfaced as a Quantum Processing Unit (QPU).
-    which implements the :func:`submit_job` method of :class:`qat.core.qpu.QPUHandler`
+    A Simulated Annealing solver interfaced as a Quantum Processing Unit (QPU)
 
     Args:
         temp_t (:class:`~qat.core.variables.ArithExpression`): temperature-time dependence. It needs to be specified using
             a variable :code:`t` instantiated with the class :class:`~qat.core.Variable`.
         n_steps (int): number of annealing time steps in Temp(t) evolution.
         seed (int, optional): Randomness seed.
     """
```

## Comparing `myqlm_simulators-1.7.1.dist-info/LICENSE` & `myqlm_simulators-1.9.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `myqlm_simulators-1.7.1.dist-info/METADATA` & `myqlm_simulators-1.9.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myqlm-simulators
-Version: 1.7.1
+Version: 1.9.1
 Summary: myQLM-simulators package
 Home-page: https://atos.net/en/lp/myqlm
 Author: Atos Quantum Lab
 License: Atos myQLM EULA
 Project-URL: Documentation, https://myqlm.github.io
 Project-URL: Bug Tracker, https://github.com/myQLM/myqlm-issues/issues
 Project-URL: Community, https://myqlmworkspace.slack.com
```

