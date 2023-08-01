# Comparing `tmp/pyqtorch-0.4.1.tar.gz` & `tmp/pyqtorch-0.4.2.tar.gz`

## Comparing `pyqtorch-0.4.1.tar` & `pyqtorch-0.4.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/CONTRIBUTING.md
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/README.md
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/mkdocs.yml
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/readthedocs.yml
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/setup.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/.github/workflows/run-tests-and-mypy.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/docs/CODE_OF_CONDUCT.md -> ../CODE_OF_CONDUCT.md
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/docs/CONTRIBUTING.md -> ../CONTRIBUTING.md
--rw-r--r--   0        0        0    57645 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/docs/QAOA.ipynb
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/docs/circuit.md
--rw-r--r--   0        0        0     6493 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/docs/essentials.ipynb
--rw-r--r--   0        0        0   154246 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/docs/fit_function.ipynb
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/docs/gate_composition.ipynb
--rw-r--r--   0        0        0     4634 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/docs/hamevo.md
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/docs/index.md
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/docs/matrices.md
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/docs/parametric.md
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/docs/primitive.md
--rw-r--r--   0        0        0    46162 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/docs/deprecated/QAOA.ipynb
--rw-r--r--   0        0        0    19339 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/docs/deprecated/bench.py
--rw-r--r--   0        0        0    74042 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/docs/deprecated/fit_function.ipynb
--rw-r--r--   0        0        0    74062 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/docs/deprecated/getting_started.ipynb
--rw-r--r--   0        0        0   121176 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/docs/deprecated/ham_evol_comparison.ipynb
--rw-r--r--   0        0        0     6459 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/docs/deprecated/state_evolution.ipynb
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/__init__.py
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/ansatz.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/embedding.py
--rw-r--r--   0        0        0     4939 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/matrices.py
--rw-r--r--   0        0        0     6255 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/matrices_sparse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/converters/__init__.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/converters/store_ops.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/converters/to_qiskit.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/core/__init__.py
--rw-r--r--   0        0        0    24532 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/core/batched_operation.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/core/circuit.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/core/measurement.py
--rw-r--r--   0        0        0    23548 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/core/operation.py
--rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/core/utils.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/modules/__init__.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/modules/abstract.py
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/modules/apply.py
--rw-r--r--   0        0        0     6904 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/modules/circuit.py
--rw-r--r--   0        0        0    12217 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/modules/hamevo.py
--rw-r--r--   0        0        0    15727 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/modules/parametric.py
--rw-r--r--   0        0        0    13235 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/modules/primitive.py
--rw-r--r--   0        0        0     5393 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/modules/utils.py
--rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/tests/conftest.py
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/tests/test_batched_operations.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/tests/test_circ_matrices.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/tests/test_converters.py
--rw-r--r--   0        0        0     8146 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/tests/test_module_hamevo.py
--rw-r--r--   0        0        0    11404 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/tests/test_modules.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/tests/test_notebooks.py
--rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/tests/test_operations.py
--rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/tests/test_operations_hamevo.py
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/tests/test_sparse_modules.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/LICENSE
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/README.md
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/mkdocs.yml
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/readthedocs.yml
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/setup.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/.github/workflows/run-tests-and-mypy.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/docs/CODE_OF_CONDUCT.md -> ../CODE_OF_CONDUCT.md
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/docs/CONTRIBUTING.md -> ../CONTRIBUTING.md
+-rw-r--r--   0        0        0    57645 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/docs/QAOA.ipynb
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/docs/circuit.md
+-rw-r--r--   0        0        0     6493 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/docs/essentials.ipynb
+-rw-r--r--   0        0        0   154246 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/docs/fit_function.ipynb
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/docs/gate_composition.ipynb
+-rw-r--r--   0        0        0     4634 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/docs/hamevo.md
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/docs/index.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/docs/matrices.md
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/docs/parametric.md
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/docs/primitive.md
+-rw-r--r--   0        0        0    46162 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/docs/deprecated/QAOA.ipynb
+-rw-r--r--   0        0        0    19339 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/docs/deprecated/bench.py
+-rw-r--r--   0        0        0    74042 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/docs/deprecated/fit_function.ipynb
+-rw-r--r--   0        0        0    74062 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/docs/deprecated/getting_started.ipynb
+-rw-r--r--   0        0        0   121176 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/docs/deprecated/ham_evol_comparison.ipynb
+-rw-r--r--   0        0        0     6459 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/docs/deprecated/state_evolution.ipynb
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/pyqtorch/__init__.py
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/pyqtorch/ansatz.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/pyqtorch/embedding.py
+-rw-r--r--   0        0        0     4939 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/pyqtorch/matrices.py
+-rw-r--r--   0        0        0     6255 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/pyqtorch/matrices_sparse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/pyqtorch/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/pyqtorch/converters/__init__.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/pyqtorch/converters/store_ops.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/pyqtorch/converters/to_qiskit.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/pyqtorch/core/__init__.py
+-rw-r--r--   0        0        0    24532 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/pyqtorch/core/batched_operation.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/pyqtorch/core/circuit.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/pyqtorch/core/measurement.py
+-rw-r--r--   0        0        0    23669 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/pyqtorch/core/operation.py
+-rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/pyqtorch/core/utils.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/pyqtorch/modules/__init__.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/pyqtorch/modules/abstract.py
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/pyqtorch/modules/apply.py
+-rw-r--r--   0        0        0     6904 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/pyqtorch/modules/circuit.py
+-rw-r--r--   0        0        0    12217 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/pyqtorch/modules/hamevo.py
+-rw-r--r--   0        0        0    15727 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/pyqtorch/modules/parametric.py
+-rw-r--r--   0        0        0    14512 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/pyqtorch/modules/primitive.py
+-rw-r--r--   0        0        0     5393 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/pyqtorch/modules/utils.py
+-rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/tests/conftest.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/tests/test_batched_operations.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/tests/test_circ_matrices.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/tests/test_converters.py
+-rw-r--r--   0        0        0     8146 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/tests/test_module_hamevo.py
+-rw-r--r--   0        0        0    12198 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/tests/test_modules.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/tests/test_notebooks.py
+-rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/tests/test_operations.py
+-rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/tests/test_operations_hamevo.py
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/tests/test_sparse_modules.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/LICENSE
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 pyqtorch-0.4.2/PKG-INFO
```

### Comparing `pyqtorch-0.4.1/.pre-commit-config.yaml` & `pyqtorch-0.4.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/CODE_OF_CONDUCT.md` & `pyqtorch-0.4.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/CONTRIBUTING.md` & `pyqtorch-0.4.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/mkdocs.yml` & `pyqtorch-0.4.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/.github/workflows/run-tests-and-mypy.yml` & `pyqtorch-0.4.2/.github/workflows/run-tests-and-mypy.yml`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/docs/QAOA.ipynb` & `pyqtorch-0.4.2/docs/QAOA.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/docs/essentials.ipynb` & `pyqtorch-0.4.2/docs/essentials.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/docs/fit_function.ipynb` & `pyqtorch-0.4.2/docs/fit_function.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/docs/gate_composition.ipynb` & `pyqtorch-0.4.2/docs/gate_composition.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/docs/hamevo.md` & `pyqtorch-0.4.2/docs/hamevo.md`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/docs/deprecated/QAOA.ipynb` & `pyqtorch-0.4.2/docs/deprecated/QAOA.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/docs/deprecated/bench.py` & `pyqtorch-0.4.2/docs/deprecated/bench.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/docs/deprecated/fit_function.ipynb` & `pyqtorch-0.4.2/docs/deprecated/fit_function.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/docs/deprecated/getting_started.ipynb` & `pyqtorch-0.4.2/docs/deprecated/getting_started.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/docs/deprecated/ham_evol_comparison.ipynb` & `pyqtorch-0.4.2/docs/deprecated/ham_evol_comparison.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/docs/deprecated/state_evolution.ipynb` & `pyqtorch-0.4.2/docs/deprecated/state_evolution.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/pyqtorch/__init__.py` & `pyqtorch-0.4.2/pyqtorch/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/pyqtorch/ansatz.py` & `pyqtorch-0.4.2/pyqtorch/ansatz.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/pyqtorch/embedding.py` & `pyqtorch-0.4.2/pyqtorch/embedding.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/pyqtorch/matrices.py` & `pyqtorch-0.4.2/pyqtorch/matrices.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/pyqtorch/matrices_sparse.py` & `pyqtorch-0.4.2/pyqtorch/matrices_sparse.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/pyqtorch/converters/store_ops.py` & `pyqtorch-0.4.2/pyqtorch/converters/store_ops.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/pyqtorch/converters/to_qiskit.py` & `pyqtorch-0.4.2/pyqtorch/converters/to_qiskit.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/pyqtorch/core/__init__.py` & `pyqtorch-0.4.2/pyqtorch/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/pyqtorch/core/batched_operation.py` & `pyqtorch-0.4.2/pyqtorch/core/batched_operation.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/pyqtorch/core/circuit.py` & `pyqtorch-0.4.2/pyqtorch/core/circuit.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/pyqtorch/core/measurement.py` & `pyqtorch-0.4.2/pyqtorch/core/measurement.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/pyqtorch/core/operation.py` & `pyqtorch-0.4.2/pyqtorch/core/operation.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,28 +36,30 @@
     """
     return OPERATIONS_DICT["I"] * torch.cos(theta / 2) - 1j * OPERATIONS_DICT[
         operation_type
     ] * torch.sin(theta / 2)
 
 
 def create_controlled_matrix_from_operation(
-    operation_matrix: torch.Tensor,
+    operation_matrix: torch.Tensor, n_control_qubits: int = 1
 ) -> torch.Tensor:
-    """Method which takes a 2x2 torch.Tensor and transforms it into a Controlled Operation Gate
+    """Method which takes a torch.Tensor and transforms it into a Controlled Operation Gate
 
     Args:
 
-        operation_matrix (torch.Tensor): the type of operation which should be performed (RX,RY,RZ)
+        operation_matrix: (torch.Tensor): the type of operation which should be
+        performed (RX,RY,RZ,SWAP)
+        n_control_qubits: (int): The number of control qubits used
 
     Returns:
 
         torch.Tensor: the resulting controlled gate populated by operation_matrix
     """
     mat_size = len(operation_matrix)
-    controlled_mat: torch.Tensor = torch.eye(2 * mat_size, dtype=torch.cdouble)
+    controlled_mat: torch.Tensor = torch.eye(2**n_control_qubits * mat_size, dtype=torch.cdouble)
     controlled_mat[-mat_size:, -mat_size:] = operation_matrix
     return controlled_mat
 
 
 def RX(theta: torch.Tensor, state: torch.Tensor, qubits: ArrayLike, N_qubits: int) -> torch.Tensor:
     """Parametrized single-qubit RX rotation
```

### Comparing `pyqtorch-0.4.1/pyqtorch/core/utils.py` & `pyqtorch-0.4.2/pyqtorch/core/utils.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/pyqtorch/modules/abstract.py` & `pyqtorch-0.4.2/pyqtorch/modules/abstract.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/pyqtorch/modules/apply.py` & `pyqtorch-0.4.2/pyqtorch/modules/apply.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/pyqtorch/modules/circuit.py` & `pyqtorch-0.4.2/pyqtorch/modules/circuit.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/pyqtorch/modules/hamevo.py` & `pyqtorch-0.4.2/pyqtorch/modules/hamevo.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/pyqtorch/modules/parametric.py` & `pyqtorch-0.4.2/pyqtorch/modules/parametric.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/pyqtorch/modules/primitive.py` & `pyqtorch-0.4.2/pyqtorch/modules/primitive.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 
+import math
+
 import torch
 from numpy.typing import ArrayLike
 
 from pyqtorch.core.operation import _apply_gate, create_controlled_matrix_from_operation
 from pyqtorch.core.utils import OPERATIONS_DICT
 from pyqtorch.modules.abstract import AbstractGate
 
@@ -291,15 +293,20 @@
 
 
 class ControlledOperationGate(AbstractGate):
     def __init__(self, gate: str, qubits: ArrayLike, n_qubits: int):
         super().__init__(qubits, n_qubits)
         self.gate = gate
         mat = OPERATIONS_DICT[gate]
-        self.register_buffer("matrix", create_controlled_matrix_from_operation(mat))
+        self.register_buffer(
+            "matrix",
+            create_controlled_matrix_from_operation(
+                mat, n_control_qubits=len(qubits) - (int)(math.log2(mat.shape[0]))
+            ),
+        )
 
     def matrices(self, _: torch.Tensor) -> torch.Tensor:
         return self.matrix
 
     def apply(self, matrix: torch.Tensor, state: torch.Tensor) -> torch.Tensor:
         return _apply_gate(state, matrix, self.qubits, self.n_qubits)
 
@@ -423,7 +430,36 @@
         swap_state = pyq.zero_state(n_qubits=3)
 
         # Apply the CSWAP gate to the zero state
         result = cswap_gate(swap_state)
         print(result)
         """
         super().__init__("SWAP", qubits, n_qubits)
+
+
+class Toffoli(ControlledOperationGate):
+    def __init__(self, qubits: ArrayLike, n_qubits: int):
+        """
+        Represents a multi qubit controlled toffoli gate in a quantum circuit.
+        This gate performs a NOT operation only if all the control qubits are in state 1.
+        Arguments:
+            qubits (ArrayLike): The first n-1 qubits will be considered as the control
+                                qubits and the last one will be the target qubit of the
+                                Toffoli gate.
+
+        Examples:
+        ```python exec="on" source="above" result="json"
+        import torch
+        import pyqtorch.modules as pyq
+
+        # Create a Toffoli gate with 2 control qubits.
+        toffoli_gate = pyq.Toffoli(qubits=[0, 1, 2], n_qubits=3)
+
+        # Create a one state
+        state_1111 = pyq.X(qubits=[0], n_qubits=3)(pyq.X(qubits=[1], n_qubits=3)
+        (pyq.X(qubits=[2], n_qubits=3)(pyq.zero_state(n_qubits=3)))
+
+        # Apply the Toffoli gate to the zero state
+        result = toffoli_gate(toffoli_state)
+        print(result)
+        """
+        super().__init__("X", qubits, n_qubits)
```

### Comparing `pyqtorch-0.4.1/pyqtorch/modules/utils.py` & `pyqtorch-0.4.2/pyqtorch/modules/utils.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/tests/conftest.py` & `pyqtorch-0.4.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/tests/test_batched_operations.py` & `pyqtorch-0.4.2/tests/test_batched_operations.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/tests/test_circ_matrices.py` & `pyqtorch-0.4.2/tests/test_circ_matrices.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/tests/test_converters.py` & `pyqtorch-0.4.2/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/tests/test_module_hamevo.py` & `pyqtorch-0.4.2/tests/test_module_hamevo.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/tests/test_modules.py` & `pyqtorch-0.4.2/tests/test_modules.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,41 @@
 from __future__ import annotations
 
 from typing import Callable
 
 import pytest
 import torch
+from torch import Tensor
 
 import pyqtorch.core as func_pyq
 import pyqtorch.modules as pyq
 from pyqtorch.core.utils import OPERATIONS_DICT
 from pyqtorch.modules.abstract import AbstractGate
 
 DEVICE = "cuda" if torch.cuda.is_available() else "cpu"
 DTYPE = torch.cdouble
 
 state_000 = pyq.zero_state(3, device=DEVICE, dtype=DTYPE)
 state_001 = pyq.X(qubits=[2], n_qubits=3)(state_000)
 state_100 = pyq.X(qubits=[0], n_qubits=3)(state_000)
 state_101 = pyq.X(qubits=[2], n_qubits=3)(pyq.X(qubits=[0], n_qubits=3)(state_000))
 state_110 = pyq.X(qubits=[1], n_qubits=3)(pyq.X(qubits=[0], n_qubits=3)(state_000))
+state_111 = pyq.X(qubits=[2], n_qubits=3)(
+    pyq.X(qubits=[1], n_qubits=3)(pyq.X(qubits=[0], n_qubits=3)(state_000))
+)
+
+state_0000 = pyq.zero_state(4, device=DEVICE, dtype=DTYPE)
+state_1110 = pyq.X(qubits=[0], n_qubits=4)(
+    pyq.X(qubits=[1], n_qubits=4)(pyq.X(qubits=[2], n_qubits=4)(state_0000))
+)
+state_1111 = pyq.X(qubits=[0], n_qubits=4)(
+    pyq.X(qubits=[1], n_qubits=4)(
+        pyq.X(qubits=[2], n_qubits=4)(pyq.X(qubits=[3], n_qubits=4)(state_0000))
+    )
+)
 
 
 @pytest.mark.parametrize("batch_size", [i for i in range(1, 2, 10)])
 @pytest.mark.parametrize("n_qubits", [i for i in range(1, 6)])
 @pytest.mark.parametrize("gate", ["X", "Y", "Z", "H", "I", "S", "T", "Sdagger"])
 def test_constant_gates(batch_size: int, n_qubits: int, gate: str) -> None:
     dtype = torch.cdouble
@@ -210,42 +224,52 @@
     circ = pyq.QuantumCircuit(1, [pyq.X([0], 1), pyq.Y([0], 1)]) * pyq.QuantumCircuit(
         n_qubits, [rx, pyq.RY([0], 1)]
     )
     truth = pyq.QuantumCircuit(n_qubits, [pyq.X([0], 1), pyq.Y([0], 1), rx, pyq.RY([0], 1)])
     assert circ == truth
 
 
-def test_CSWAP_state000_controlqubit_0() -> None:
-    n_qubits = 3
-    cswap = pyq.CSWAP([0, 1, 2], n_qubits)
-    assert torch.allclose(cswap(state_000), state_000)
-
-
-def test_CSWAP_state001_controlqubit_0() -> None:
-    n_qubits = 3
-    cswap = pyq.CSWAP([0, 1, 2], n_qubits)
-    assert torch.allclose(cswap(state_001), state_001)
-
-
-def test_CSWAP_state100_controlqubit_0() -> None:
+@pytest.mark.parametrize(
+    "initial_state,expected_state",
+    [
+        (state_000, state_000),
+        (state_001, state_001),
+        (state_100, state_100),
+        (state_101, state_110),
+        (state_110, state_101),
+    ],
+)
+def test_CSWAP_controlqubits0(initial_state: Tensor, expected_state: Tensor) -> None:
+    print(initial_state.shape)
+    print(expected_state.shape)
     n_qubits = 3
     cswap = pyq.CSWAP([0, 1, 2], n_qubits)
-    assert torch.allclose(cswap(state_100), state_100)
+    assert torch.allclose(cswap(initial_state), expected_state)
 
 
-def test_CSWAP_state101_controlqubit_0() -> None:
+@pytest.mark.parametrize(
+    "initial_state,expected_state",
+    [
+        (state_000, state_000),
+        (state_001, state_001),
+        (state_100, state_100),
+        (state_101, state_101),
+        (state_110, state_111),
+    ],
+)
+def test_Toffoli_controlqubits0(initial_state: Tensor, expected_state: Tensor) -> None:
     n_qubits = 3
-    cswap = pyq.CSWAP([0, 1, 2], n_qubits)
-    assert torch.allclose(cswap(state_101), state_110)
+    toffoli = pyq.Toffoli([0, 1, 2], n_qubits)
+    assert torch.allclose(toffoli(initial_state), expected_state)
 
 
-def test_CSWAP_state110_controlqubit_0() -> None:
-    n_qubits = 3
-    cswap = pyq.CSWAP([0, 1, 2], n_qubits)
-    assert torch.allclose(cswap(state_110), state_101)
+def test_4qubit_Toffoli() -> None:
+    n_qubits = 4
+    toffoli = pyq.Toffoli([0, 1, 2, 3], n_qubits)
+    assert torch.allclose(toffoli(state_1110), state_1111)
 
 
 @pytest.mark.parametrize("state_fn", [pyq.random_state, pyq.zero_state, pyq.uniform_state])
 @pytest.mark.parametrize("n_qubits", [i for i in range(1, 8)])
 @pytest.mark.parametrize("batch_size", [i for i in range(1, 8)])
 def test_isnormalized_states(state_fn: Callable, n_qubits: int, batch_size: int) -> None:
     state = state_fn(n_qubits, batch_size, device=DEVICE, dtype=DTYPE)
```

### Comparing `pyqtorch-0.4.1/tests/test_notebooks.py` & `pyqtorch-0.4.2/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/tests/test_operations.py` & `pyqtorch-0.4.2/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/tests/test_operations_hamevo.py` & `pyqtorch-0.4.2/tests/test_operations_hamevo.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/tests/test_sparse_modules.py` & `pyqtorch-0.4.2/tests/test_sparse_modules.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/.gitignore` & `pyqtorch-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/LICENSE` & `pyqtorch-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.1/pyproject.toml` & `pyqtorch-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     { name = "Aleksander Wennersteen", email = "aleksander.wennersteen@pasqal.com" },
     { name = "Mario Dagrada", email = "mario.dagrada@pasqal.com" },
     { name = "Dominik Seitz", email = "dominik.seitz@pasqal.com" },
     { name = "Niklas Heim", email = "niklas.heim@pasqal.com" },
 ]
 requires-python = ">=3.8,<3.12"
 license = {text = "Proprietary"}
-version = "0.4.1"
+version = "0.4.2"
 classifiers=[
     "License :: Other/Proprietary License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
```

### Comparing `pyqtorch-0.4.1/PKG-INFO` & `pyqtorch-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqtorch
-Version: 0.4.1
+Version: 0.4.2
 Summary: An efficient, large-scale emulator designed for quantum machine learning, seamlessly integrated with a PyTorch backend. Please refer to https://pyqtorch.readthedocs.io/en/latest/ for setup and usage info, along with the full documentation.
 Author-email: Slimane Thabet <slimane.thabet@pasqal.com>, Aleksander Wennersteen <aleksander.wennersteen@pasqal.com>, Mario Dagrada <mario.dagrada@pasqal.com>, Dominik Seitz <dominik.seitz@pasqal.com>, Niklas Heim <niklas.heim@pasqal.com>
 License: Proprietary
 License-File: LICENSE
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

