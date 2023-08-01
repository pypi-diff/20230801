# Comparing `tmp/alpaka-job-coverage-1.3.6.tar.gz` & `tmp/alpaka-job-coverage-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpaka-job-coverage-1.3.6.tar", last modified: Fri Jul 28 05:46:19 2023, max compression
+gzip compressed data, was "alpaka-job-coverage-1.4.0.tar", last modified: Tue Aug  1 10:25:32 2023, max compression
```

## Comparing `alpaka-job-coverage-1.3.6.tar` & `alpaka-job-coverage-1.4.0.tar`

### file list

```diff
@@ -1,31 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:46:19.740753 alpaka-job-coverage-1.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-28 05:46:00.000000 alpaka-job-coverage-1.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 05:46:00.000000 alpaka-job-coverage-1.3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-07-28 05:46:19.740753 alpaka-job-coverage-1.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-07-28 05:46:00.000000 alpaka-job-coverage-1.3.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-28 05:46:00.000000 alpaka-job-coverage-1.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 05:46:19.740753 alpaka-job-coverage-1.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-28 05:46:00.000000 alpaka-job-coverage-1.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:46:19.736753 alpaka-job-coverage-1.3.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:46:19.736753 alpaka-job-coverage-1.3.6/src/alpaka_job_coverage/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-28 05:46:00.000000 alpaka-job-coverage-1.3.6/src/alpaka_job_coverage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-07-28 05:46:00.000000 alpaka-job-coverage-1.3.6/src/alpaka_job_coverage/filter_backend_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-28 05:46:00.000000 alpaka-job-coverage-1.3.6/src/alpaka_job_coverage/filter_compiler_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-07-28 05:46:00.000000 alpaka-job-coverage-1.3.6/src/alpaka_job_coverage/filter_compiler_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-07-28 05:46:00.000000 alpaka-job-coverage-1.3.6/src/alpaka_job_coverage/filter_software_dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-28 05:46:00.000000 alpaka-job-coverage-1.3.6/src/alpaka_job_coverage/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-07-28 05:46:00.000000 alpaka-job-coverage-1.3.6/src/alpaka_job_coverage/main_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11681 2023-07-28 05:46:00.000000 alpaka-job-coverage-1.3.6/src/alpaka_job_coverage/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:46:19.736753 alpaka-job-coverage-1.3.6/src/alpaka_job_coverage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-07-28 05:46:19.000000 alpaka-job-coverage-1.3.6/src/alpaka_job_coverage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-28 05:46:19.000000 alpaka-job-coverage-1.3.6/src/alpaka_job_coverage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 05:46:19.000000 alpaka-job-coverage-1.3.6/src/alpaka_job_coverage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-28 05:46:19.000000 alpaka-job-coverage-1.3.6/src/alpaka_job_coverage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 05:46:19.000000 alpaka-job-coverage-1.3.6/src/alpaka_job_coverage.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:46:19.740753 alpaka-job-coverage-1.3.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-28 05:46:00.000000 alpaka-job-coverage-1.3.6/tests/test_compiler_names.py
--rw-r--r--   0 runner    (1001) docker     (123)    41676 2023-07-28 05:46:00.000000 alpaka-job-coverage-1.3.6/tests/test_cuda_sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)    12280 2023-07-28 05:46:00.000000 alpaka-job-coverage-1.3.6/tests/test_hipcc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-28 05:46:00.000000 alpaka-job-coverage-1.3.6/tests/test_single_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-07-28 05:46:00.000000 alpaka-job-coverage-1.3.6/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-28 05:46:00.000000 alpaka-job-coverage-1.3.6/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:25:32.847143 alpaka-job-coverage-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-08-01 10:25:13.000000 alpaka-job-coverage-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-01 10:25:13.000000 alpaka-job-coverage-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-08-01 10:25:32.843143 alpaka-job-coverage-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-08-01 10:25:13.000000 alpaka-job-coverage-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-01 10:25:13.000000 alpaka-job-coverage-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 10:25:32.847143 alpaka-job-coverage-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-08-01 10:25:13.000000 alpaka-job-coverage-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:25:32.835143 alpaka-job-coverage-1.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:25:32.843143 alpaka-job-coverage-1.4.0/src/alpaka_job_coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-01 10:25:13.000000 alpaka-job-coverage-1.4.0/src/alpaka_job_coverage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-08-01 10:25:13.000000 alpaka-job-coverage-1.4.0/src/alpaka_job_coverage/filter_backend_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-08-01 10:25:13.000000 alpaka-job-coverage-1.4.0/src/alpaka_job_coverage/filter_compiler_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7501 2023-08-01 10:25:13.000000 alpaka-job-coverage-1.4.0/src/alpaka_job_coverage/filter_compiler_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-08-01 10:25:13.000000 alpaka-job-coverage-1.4.0/src/alpaka_job_coverage/filter_software_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-08-01 10:25:13.000000 alpaka-job-coverage-1.4.0/src/alpaka_job_coverage/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-08-01 10:25:13.000000 alpaka-job-coverage-1.4.0/src/alpaka_job_coverage/main_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12216 2023-08-01 10:25:13.000000 alpaka-job-coverage-1.4.0/src/alpaka_job_coverage/util.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12111 2023-08-01 10:25:13.000000 alpaka-job-coverage-1.4.0/src/alpaka_job_coverage/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-08-01 10:25:13.000000 alpaka-job-coverage-1.4.0/src/alpaka_job_coverage/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:25:32.843143 alpaka-job-coverage-1.4.0/src/alpaka_job_coverage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-08-01 10:25:32.000000 alpaka-job-coverage-1.4.0/src/alpaka_job_coverage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-08-01 10:25:32.000000 alpaka-job-coverage-1.4.0/src/alpaka_job_coverage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 10:25:32.000000 alpaka-job-coverage-1.4.0/src/alpaka_job_coverage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-01 10:25:32.000000 alpaka-job-coverage-1.4.0/src/alpaka_job_coverage.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-01 10:25:32.000000 alpaka-job-coverage-1.4.0/src/alpaka_job_coverage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-01 10:25:32.000000 alpaka-job-coverage-1.4.0/src/alpaka_job_coverage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:25:32.843143 alpaka-job-coverage-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-08-01 10:25:13.000000 alpaka-job-coverage-1.4.0/tests/test_compiler_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41878 2023-08-01 10:25:13.000000 alpaka-job-coverage-1.4.0/tests/test_cuda_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12280 2023-08-01 10:25:13.000000 alpaka-job-coverage-1.4.0/tests/test_hipcc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-08-01 10:25:13.000000 alpaka-job-coverage-1.4.0/tests/test_single_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-08-01 10:25:13.000000 alpaka-job-coverage-1.4.0/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-08-01 10:25:13.000000 alpaka-job-coverage-1.4.0/tests/test_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 10:25:13.000000 alpaka-job-coverage-1.4.0/version.txt
```

### Comparing `alpaka-job-coverage-1.3.6/LICENSE` & `alpaka-job-coverage-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.3.6/PKG-INFO` & `alpaka-job-coverage-1.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaka-job-coverage
-Version: 1.3.6
+Version: 1.4.0
 Summary: The library provides everything needed to generate a sparse combination matrix for alpaca-based projects, including a set of general-purpose combination rules.
 Home-page: https://github.com/alpaka-group/alpaka-job-matrix-library
 Author: Simeon Ehrig
 Author-email: s.ehrig@hzdr.de
 Project-URL: Bug Tracker, https://github.com/alpaka-group/alpaka-job-matrix-library/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
@@ -51,22 +51,31 @@
 
 If you want to use a project-specific parameter, you can simply add it to the parameter list and the library will apply it. To limit the possible combinations of your new parameter, you need to add a new filter function. The `create_job_list()` function applies a chain of filter functions to each possible combination. Before and after each filter function is a function hook where you can insert your own filter function. The order is described in the doc string of `create_job_list()`. When you create a new filter rule, you must comply with the following rules:
 
 * The filter returns `True` if a combination is valid and `False` if not. All filters in the library follow the rule that every combination is valid until it is forbidden (blacklist).
 * The input of the filter is a combination of the values of the individual parameter fields, and the combination does not have to be complete. The list can contain at least 2 parameter fields up to all. You must check whether a parameter field is included in the current combination.
 * If a parameter field is not included in the current combination, it means that it can contain any possible value of this parameter. In practice, this means that if you only check for the presence of the parameter and return `False`, if the parameter is not present, no combination is possible.
 
+# ajc-validate
+
+`ajc-validate` is a tool which is installed together with the `alpaka-job-coverage` library. The tool allows to check whether a combination of parameters passes the different filters and displays the reason if not.
+
+![ajc-validate example](docs/images/ajc-validator-example.png)
+
+**Hint:** The source code of the tool is located in the file [validate.py](src/alpaka_job_coverage/validate.py).
+
 # Developing
 
 It is strongly recommended to use a Python environment for developing the code, such as `virtualenv` or a `conda` environment. The following code uses a `virtualenv`.
 
 1. Create the environment: `virtualenv -p python3 env`
 2. Activate the environment: `source env/bin/activate`
 3. Install the library: `python setup.py develop`
 4. Test the installation with the example: `python3 example/example.py 3.0`
+5. You can run the unit tests by going to the `test` directory and running `python -m unittest`
 
 If the example works correctly, a `job.yml` will be created in the current directory. You can also run `python3 example/example.py --help` to see additional options.
 
 Now the library is available in the environment. Therefore you can easily use the library in your own projects via `import alpaka_job_coverage as ajc`.
 
 ## Contribution
```

### Comparing `alpaka-job-coverage-1.3.6/README.md` & `alpaka-job-coverage-1.4.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -36,22 +36,31 @@
 
 If you want to use a project-specific parameter, you can simply add it to the parameter list and the library will apply it. To limit the possible combinations of your new parameter, you need to add a new filter function. The `create_job_list()` function applies a chain of filter functions to each possible combination. Before and after each filter function is a function hook where you can insert your own filter function. The order is described in the doc string of `create_job_list()`. When you create a new filter rule, you must comply with the following rules:
 
 * The filter returns `True` if a combination is valid and `False` if not. All filters in the library follow the rule that every combination is valid until it is forbidden (blacklist).
 * The input of the filter is a combination of the values of the individual parameter fields, and the combination does not have to be complete. The list can contain at least 2 parameter fields up to all. You must check whether a parameter field is included in the current combination.
 * If a parameter field is not included in the current combination, it means that it can contain any possible value of this parameter. In practice, this means that if you only check for the presence of the parameter and return `False`, if the parameter is not present, no combination is possible.
 
+# ajc-validate
+
+`ajc-validate` is a tool which is installed together with the `alpaka-job-coverage` library. The tool allows to check whether a combination of parameters passes the different filters and displays the reason if not.
+
+![ajc-validate example](docs/images/ajc-validator-example.png)
+
+**Hint:** The source code of the tool is located in the file [validate.py](src/alpaka_job_coverage/validate.py).
+
 # Developing
 
 It is strongly recommended to use a Python environment for developing the code, such as `virtualenv` or a `conda` environment. The following code uses a `virtualenv`.
 
 1. Create the environment: `virtualenv -p python3 env`
 2. Activate the environment: `source env/bin/activate`
 3. Install the library: `python setup.py develop`
 4. Test the installation with the example: `python3 example/example.py 3.0`
+5. You can run the unit tests by going to the `test` directory and running `python -m unittest`
 
 If the example works correctly, a `job.yml` will be created in the current directory. You can also run `python3 example/example.py --help` to see additional options.
 
 Now the library is available in the environment. Therefore you can easily use the library in your own projects via `import alpaka_job_coverage as ajc`.
 
 ## Contribution
```

### Comparing `alpaka-job-coverage-1.3.6/setup.py` & `alpaka-job-coverage-1.4.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,19 +26,21 @@
         "Bug Tracker": "https://github.com/alpaka-group/alpaka-job-matrix-library/issues",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
         "Operating System :: OS Independent",
     ],
-    packages=setuptools.find_packages('src'),
-    package_dir={'': 'src'},
+    packages=setuptools.find_packages("src"),
+    package_dir={"": "src"},
+    entry_points={
+        "console_scripts": ["ajc-validate=alpaka_job_coverage.validate:main"]
+    },
     python_requires=">=3.8",
     install_requires=[
         "allpairspy == 2.5.0",
         "typeguard",
         "pyaml",
         "types-PyYAML",
         "packaging",
-    ]
+    ],
 )
-
```

### Comparing `alpaka-job-coverage-1.3.6/src/alpaka_job_coverage/filter_compiler_name.py` & `alpaka-job-coverage-1.4.0/src/alpaka_job_coverage/filter_compiler_name.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,87 @@
 """Filter rules basing on host and device compiler names.
 """
 
+import io
+
 from alpaka_job_coverage.globals import *  # pylint: disable=wildcard-import,unused-wildcard-import
-from alpaka_job_coverage.util import row_check_name, is_in_row
-from typing import List, Tuple, Union
+from alpaka_job_coverage.util import row_check_name, is_in_row, reason
+from typing import List, Tuple, Union, Optional
 from typeguard import typechecked
 
 
+def get_required_parameter() -> List[str]:
+    """Returns a list of parameters which are required for using the filter defined by this module.
+    Returns:
+        List[str]: list of parameters
+    """
+    return [HOST_COMPILER, DEVICE_COMPILER]
+
+
 @typechecked
 def general_compiler_filter_typed(
-    row: List[Union[Tuple[str, str], List[Tuple[str, str]]]]
+    row: List[Union[Tuple[str, str], List[Tuple[str, str]]]],
+    output: Optional[Union[io.StringIO, io.TextIOWrapper]] = None,
 ) -> bool:
     """Type checked version of general_compiler_filter(). Should be only used for
     testing or tooling. The type check adds a big overhead, which slows down
     pair-wise generator by the factor 30.
 
     Args:
         row (List[Union[Tuple[str, str], List[Tuple[str, str]]]]): Combination
         to verify. The row can contain up to all combination fields and at least
-         two items.
+        two items.
+        output (Optional[Union[io.StringIO, io.TextIOWrapper]]): Write
+        additional information about filter decisions to the IO object
+        (io.SringIO, sys.stdout, sys.stderr). If it is None no information is
+        generated.
 
     Returns:
         bool: True, if combination is valid, otherwise False.
     """
-    return general_compiler_filter(row)
+    return general_compiler_filter(row, output)
 
 
-def general_compiler_filter(row: List) -> bool:
+def general_compiler_filter(
+    row: List, output: Optional[Union[io.StringIO, io.TextIOWrapper]] = None
+) -> bool:
     """Filter rules basing on host and device compiler names.
 
     Args:
         row (List): Combination to verify. The row can contain
         up to all combination fields and at least two items.
+        output (Optional[Union[io.StringIO, io.TextIOWrapper]]): Write
+        additional information about filter decisions to the IO object
+        (io.SringIO, sys.stdout, sys.stderr). If it is None no information is
+        generated.
 
     Returns:
         bool: True, if combination is valid, otherwise False.
     """
 
     # it is not allow to use the nvcc as host compiler
     if row_check_name(row, HOST_COMPILER, "==", NVCC):
+        reason(output, "nvcc is not allowed as host compiler")
         return False
 
     # only the nvcc allows to combine different host and device compiler
     if (
         is_in_row(row, HOST_COMPILER)
         and is_in_row(row, DEVICE_COMPILER)
         and (
             row[param_map[DEVICE_COMPILER]][NAME] != NVCC
             and row[param_map[HOST_COMPILER]][NAME]
             != row[param_map[DEVICE_COMPILER]][NAME]
         )
     ):
+        reason(output, "host and device compiler must be the same (except for nvcc)")
         return False
 
     # only clang and gcc are allowed as nvcc host compiler
     if row_check_name(row, DEVICE_COMPILER, "==", NVCC) and not (
         row_check_name(row, HOST_COMPILER, "==", GCC)
         or row_check_name(row, HOST_COMPILER, "==", CLANG)
     ):
+        reason(output, "only clang and gcc are allowed as nvcc host compilers")
         return False
 
     return True
```

### Comparing `alpaka-job-coverage-1.3.6/src/alpaka_job_coverage/filter_software_dependency.py` & `alpaka-job-coverage-1.4.0/src/alpaka_job_coverage/filter_backend_version.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,165 +1,204 @@
-"""Filter rules handling software dependencies and compiler settings.
+"""Filter rules basing on backend names and versions.
 """
 
+import io
+
 from alpaka_job_coverage.globals import *  # pylint: disable=wildcard-import,unused-wildcard-import
 from alpaka_job_coverage.util import (
-    row_check_backend_version,
     row_check_name,
     row_check_version,
-    is_in_row,
+    row_check_backend_version,
+    reason,
 )
-
-from packaging import version as pk_version
-from typing import List, Tuple, Union
+from typing import List, Tuple, Union, Optional
 from typeguard import typechecked
 
 
+def get_required_parameter() -> List[str]:
+    """Returns a list of parameters which are required for using the filter defined by this module.
+
+    Returns:
+        List[str]: list of parameters
+    """
+    return [DEVICE_COMPILER, BACKENDS]
+
+
 @typechecked
-def software_dependency_filter_typed(
-    row: List[Union[Tuple[str, str], List[Tuple[str, str]]]]
+def compiler_backend_filter_typed(
+    row: List[Union[Tuple[str, str], List[Tuple[str, str]]]],
+    output: Optional[Union[io.StringIO, io.TextIOWrapper]] = None,
 ) -> bool:
-    """Type checked version of software_dependency_filter(). Should be only used for
+    """Type checked version of compiler_backend_filter(). Should be only used for
     testing or tooling. The type check adds a big overhead, which slows down
     pair-wise generator by the factor 30.
 
     Args:
         row (List[Union[Tuple[str, str], List[Tuple[str, str]]]]): Combination
         to verify. The row can contain up to all combination fields and at least
-         two items.
+        two items.
+        output (Optional[Union[io.StringIO, io.TextIOWrapper]]): Write
+        additional information about filter decisions to the IO object
+        (io.SringIO, sys.stdout, sys.stderr). If it is None no information is
+        generated.
 
     Returns:
         bool: True, if combination is valid, otherwise False.
     """
-    return software_dependency_filter(row)
+    return compiler_backend_filter(row, output)
 
 
-def software_dependency_filter(row: List) -> bool:
-    """Filter rules handling software dependencies and compiler settings.
+def compiler_backend_filter(
+    row: List, output: Optional[Union[io.StringIO, io.TextIOWrapper]] = None
+) -> bool:
+    """Filter rules basing on backend names and versions.
 
     Args:
         row (List): Combination to verify. The row can contain
         up to all combination fields and at least two items.
+        output (Optional[Union[io.StringIO, io.TextIOWrapper]]): Write
+        additional information about filter decisions to the IO object
+        (io.SringIO, sys.stdout, sys.stderr). If it is None no information is
+        generated.
 
     Returns:
         bool: True, if combination is valid, otherwise False.
     """
+    ###########################
+    ## gcc device compiler
+    ###########################
+
+    if row_check_name(row, DEVICE_COMPILER, "==", GCC):
+        if row_check_backend_version(row, ALPAKA_ACC_GPU_CUDA_ENABLE, "!=", OFF_VER):
+            reason(
+                output,
+                "gcc as device compiler cannot compile with enabled alpaka_ACC_GPU_CUDA_ENABLE back-end",
+            )
+            return False
+
+        if row_check_backend_version(row, ALPAKA_ACC_GPU_HIP_ENABLE, "!=", OFF_VER):
+            reason(
+                output,
+                "gcc as device compiler cannot compile with enabled alpaka_ACC_GPU_HIP_ENABLE back-end",
+            )
+            return False
+
+    ###########################
+    ## clang device compiler
+    ###########################
+
+    if row_check_name(row, DEVICE_COMPILER, "==", CLANG):
+        if row_check_backend_version(row, ALPAKA_ACC_GPU_CUDA_ENABLE, "!=", OFF_VER):
+            reason(
+                output,
+                "clang as device compiler cannot compile with enabled alpaka_ACC_GPU_CUDA_ENABLE back-end (use clang-cuda instead)",
+            )
+            return False
+
+        # clang cannot compile with enabled HIP backend
+        if row_check_backend_version(row, ALPAKA_ACC_GPU_HIP_ENABLE, "!=", OFF_VER):
+            reason(
+                output,
+                "clang as device compiler cannot compile with enabled "
+                "alpaka_ACC_GPU_HIP_ENABLE back-end (use hipcc instead)",
+            )
+            return False
 
-    # GCC 6 and below is not available on Ubuntu 20.04
-    if row_check_version(row, UBUNTU, "==", "20.04"):
-        if (
-            row_check_name(row, HOST_COMPILER, "==", GCC)
-            and int(row[param_map[HOST_COMPILER]][VERSION]) <= 6
+    ###########################
+    ## nvcc device compiler
+    ###########################
+
+    if row_check_name(row, DEVICE_COMPILER, "==", NVCC):
+        # the nvcc compiler needs the same version, like the backend
+        if row_check_backend_version(
+            row,
+            ALPAKA_ACC_GPU_CUDA_ENABLE,
+            "!=",
+            row[param_map[DEVICE_COMPILER]][VERSION],
         ):
+            reason(
+                output,
+                "the nvcc compiler and the CUDA back-end must have the same version",
+            )
+            return False
+
+        # it is not allowed to enable the HIP and CUDA backend on the same time
+        if row_check_backend_version(row, ALPAKA_ACC_GPU_HIP_ENABLE, "!=", OFF_VER):
+            reason(
+                output,
+                "If nvcc is the device compiler and the CUDA back-end is enabled "
+                "it is not allowed to enable the HIP back-end",
+            )
             return False
 
-    # GCC 9 and older does not support -std=c++20
-    if (
-        row_check_version(row, CXX_STANDARD, ">=", "20")
-        and row_check_name(row, HOST_COMPILER, "==", GCC)
-        and row_check_version(row, HOST_COMPILER, "<=", "9")
-    ):
-        return False
-
-    if row_check_name(row, DEVICE_COMPILER, "==", NVCC) and is_in_row(
-        row, CXX_STANDARD
-    ):
-        parsed_nvcc_version = pk_version.parse(row[param_map[DEVICE_COMPILER]][VERSION])
-
-        # definition of the tuple values: if the nvcc version of the first
-        # tuple is older than the cxx standard of the second value, it is not supported
-        nvcc_cxx_versions = [
-            ("11.0", 17),  # NVCC versions older than 11.0 does not support C++ 17
-            ("12.0", 20),  # NVCC versions older than 12.0 does not support C++ 20
-            ("12.2", 23),  # NVCC 12.2 is not released yet, therefore we need to
-            # expect that it could support C++23
+    ###########################
+    ## clang-cuda device compiler
+    ###########################
+
+    if row_check_name(row, DEVICE_COMPILER, "==", CLANG_CUDA):
+        # the CUDA backend needs to be enabled
+        if row_check_backend_version(row, ALPAKA_ACC_GPU_CUDA_ENABLE, "==", OFF_VER):
+            reason(
+                output,
+                "when CLANG_CUDA is set as device compiler "
+                "the CUDA back-end must be enabled",
+            )
+            return False
+
+        # it is not allowed to enable the HIP and CUDA backend on the same time
+        if row_check_backend_version(row, ALPAKA_ACC_GPU_HIP_ENABLE, "!=", OFF_VER):
+            reason(
+                output,
+                "if clang-cuda is the device compiler and the CUDA back-end is enabled "
+                "it is not allowed to enable the HIP back-end",
+            )
+            return False
+
+        # check if clang-cuda supports the CUDA SDK version
+        clangcuda_cudasdk_versions = [
+            ("7", "9.2"),
+            ("8", "10.0"),
+            ("10", "10.1"),
+            ("12", "11.0"),
+            ("13", "11.2"),
+            ("16", "11.5"),
         ]
-        for nvcc_version, cxx_version in nvcc_cxx_versions:
-            if (
-                parsed_nvcc_version < pk_version.parse(nvcc_version)
-                and int(row[param_map[CXX_STANDARD]][VERSION]) >= cxx_version
+
+        for clang_cuda_version, cuda_sdk_version in clangcuda_cudasdk_versions:
+            if row_check_version(
+                row, DEVICE_COMPILER, "<=", clang_cuda_version
+            ) and row_check_backend_version(
+                row, ALPAKA_ACC_GPU_CUDA_ENABLE, ">", cuda_sdk_version
             ):
+                reason(
+                    output,
+                    f"clang-{clang_cuda_version} supports only up to CUDA {cuda_sdk_version}",
+                )
                 return False
 
-    # clang 11 and 12 are not available in the Ubuntu 18.04 ppa
-    if (
-        row_check_version(row, UBUNTU, "==", "18.04")
-        and (
-            row_check_name(
-                row,
-                HOST_COMPILER,
-                "==",
-                CLANG,
-            )
-            or row_check_name(
-                row,
-                HOST_COMPILER,
-                "==",
-                CLANG_CUDA,
-            )
-        )
-        and (
-            (
-                row_check_version(row, HOST_COMPILER, "==", "11")
-                or row_check_version(row, HOST_COMPILER, "==", "12")
-            )
-        )
-    ):
-        return False
-
-    # Clang 9 and older does not support -std=c++20
-    if row_check_version(row, CXX_STANDARD, ">=", "20"):
-        for compiler_name in [CLANG, CLANG_CUDA]:
-            if row_check_name(
-                row, HOST_COMPILER, "==", compiler_name
-            ) and row_check_version(row, HOST_COMPILER, "<=", "9"):
-                return False
+    ###########################
+    ## hipcc device compiler
+    ###########################
+
+    # the HIP backend needs to be enabled and has the same version number
+    if row_check_name(row, DEVICE_COMPILER, "==", HIPCC):
+        if row_check_backend_version(
+            row,
+            ALPAKA_ACC_GPU_HIP_ENABLE,
+            "!=",
+            row[param_map[DEVICE_COMPILER]][VERSION],
+        ):
+            reason(
+                output, "hipcc and the HIP back-end must have the same version number"
+            )
+            return False
 
-    # ubuntu 18.04 containers are not available for CUDA 11.0 and later
-    if (
-        row_check_version(row, UBUNTU, "==", "18.04")
-        and row_check_backend_version(row, ALPAKA_ACC_GPU_CUDA_ENABLE, "!=", OFF_VER)
-        and row_check_backend_version(row, ALPAKA_ACC_GPU_CUDA_ENABLE, ">=", "11.0")
-    ):
-        return False
-
-    # ubuntu 20.04 containers are not available for CUDA 10.2 and before
-    if (
-        row_check_version(row, UBUNTU, "==", "20.04")
-        and row_check_backend_version(row, ALPAKA_ACC_GPU_CUDA_ENABLE, "!=", OFF_VER)
-        and row_check_backend_version(row, ALPAKA_ACC_GPU_CUDA_ENABLE, "<", "11.0")
-    ):
-        return False
-
-    # all rocm images are Ubuntu 20.04 based
-    if (
-        row_check_version(row, UBUNTU, "!=", "20.04")
-        and row_check_name(row, DEVICE_COMPILER, "==", HIPCC)
-        and row_check_backend_version(row, ALPAKA_ACC_GPU_HIP_ENABLE, "!=", OFF_VER)
-    ):
-        return False
-
-    # a bug in CMAKE 3.18 avoids the correct usage of the variable CMAKE_CUDA_ARCHITECTURE if the
-    # CUDA compiler is Clang++
-    if row_check_name(row, DEVICE_COMPILER, "==", CLANG_CUDA) and row_check_version(
-        row, CMAKE, "<", "3.19"
-    ):
-        return False
-
-    # disable nvcc 11.0-11.3 + gcc 10 + Ubuntu 20.04
-    # Ubuntu 20.04 provides only gcc 10.3 and not 10.4 or 10.5
-    # this combination does not work: https://github.com/alpaka-group/alpaka/issues/1297
-    if (
-        row_check_name(row, DEVICE_COMPILER, "==", NVCC)
-        and (
-            row_check_version(row, DEVICE_COMPILER, "==", "11.0")
-            or row_check_version(row, DEVICE_COMPILER, "==", "11.1")
-            or row_check_version(row, DEVICE_COMPILER, "==", "11.2")
-            or row_check_version(row, DEVICE_COMPILER, "==", "11.3")
-        )
-        and row_check_name(row, HOST_COMPILER, "==", GCC)
-        and row_check_version(row, HOST_COMPILER, "==", "10")
-        and row_check_version(row, UBUNTU, "==", "20.04")
-    ):
-        return False
+        # it is not allowed to enable the HIP and CUDA backend on the same time
+        if row_check_backend_version(row, ALPAKA_ACC_GPU_CUDA_ENABLE, "!=", OFF_VER):
+            reason(
+                output,
+                "if hipcc is the device compiler and the HIP back-end is enabled, "
+                "it is not allowed to enable the CUDA back-end",
+            )
+            return False
 
     return True
```

### Comparing `alpaka-job-coverage-1.3.6/src/alpaka_job_coverage/globals.py` & `alpaka-job-coverage-1.4.0/src/alpaka_job_coverage/globals.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.3.6/src/alpaka_job_coverage/main_functions.py` & `alpaka-job-coverage-1.4.0/src/alpaka_job_coverage/main_functions.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.3.6/src/alpaka_job_coverage/util.py` & `alpaka-job-coverage-1.4.0/src/alpaka_job_coverage/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,16 @@
         ('alpaka_ACC_GPU_CUDA_ENABLE', '11.4'), 
         ('alpaka_ACC_GPU_HIP_ENABLE', '0.0.0')
     ], 
     ('cmake', '3.19.8'), ('boost', '1.66.0'), ('alpaka', '0.6.1'), 
     ('ubuntu', '20.04')]
 """
 
-import operator, re
-from typing import Any, List, Dict, Tuple
+import operator, re, io
+from typing import Any, List, Dict, Tuple, Optional, Union
 from typeguard import typechecked
 from packaging import version as pk_version
 
 
 from alpaka_job_coverage.globals import *  # pylint: disable=wildcard-import,unused-wildcard-import
 
 # maps strings to comparision operators
@@ -342,7 +342,24 @@
             support_versions[name][0]
         ) or parsed_version > pk_version.parse(support_versions[name][1]):
             if verbose:
                 print(warning_text(f"{name} {version} is not supported"))
             return False
 
     return True
+
+
+def reason(output: Optional[Union[io.StringIO, io.TextIOWrapper]], msg: str):
+    """Write the message to output if it is not None. This function is used
+    in filter functions to print additional information about filter decisions.
+
+    Args:
+        output (Optional[Union[io.StringIO, io.TextIOWrapper]]): IO object.
+        Can be io.StringIO, sys.stdout sys.stderr
+        msg (str): the message
+    """
+    if output:
+        print(
+            msg,
+            file=output,
+            end="",
+        )
```

### Comparing `alpaka-job-coverage-1.3.6/src/alpaka_job_coverage.egg-info/PKG-INFO` & `alpaka-job-coverage-1.4.0/src/alpaka_job_coverage.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaka-job-coverage
-Version: 1.3.6
+Version: 1.4.0
 Summary: The library provides everything needed to generate a sparse combination matrix for alpaca-based projects, including a set of general-purpose combination rules.
 Home-page: https://github.com/alpaka-group/alpaka-job-matrix-library
 Author: Simeon Ehrig
 Author-email: s.ehrig@hzdr.de
 Project-URL: Bug Tracker, https://github.com/alpaka-group/alpaka-job-matrix-library/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
@@ -51,22 +51,31 @@
 
 If you want to use a project-specific parameter, you can simply add it to the parameter list and the library will apply it. To limit the possible combinations of your new parameter, you need to add a new filter function. The `create_job_list()` function applies a chain of filter functions to each possible combination. Before and after each filter function is a function hook where you can insert your own filter function. The order is described in the doc string of `create_job_list()`. When you create a new filter rule, you must comply with the following rules:
 
 * The filter returns `True` if a combination is valid and `False` if not. All filters in the library follow the rule that every combination is valid until it is forbidden (blacklist).
 * The input of the filter is a combination of the values of the individual parameter fields, and the combination does not have to be complete. The list can contain at least 2 parameter fields up to all. You must check whether a parameter field is included in the current combination.
 * If a parameter field is not included in the current combination, it means that it can contain any possible value of this parameter. In practice, this means that if you only check for the presence of the parameter and return `False`, if the parameter is not present, no combination is possible.
 
+# ajc-validate
+
+`ajc-validate` is a tool which is installed together with the `alpaka-job-coverage` library. The tool allows to check whether a combination of parameters passes the different filters and displays the reason if not.
+
+![ajc-validate example](docs/images/ajc-validator-example.png)
+
+**Hint:** The source code of the tool is located in the file [validate.py](src/alpaka_job_coverage/validate.py).
+
 # Developing
 
 It is strongly recommended to use a Python environment for developing the code, such as `virtualenv` or a `conda` environment. The following code uses a `virtualenv`.
 
 1. Create the environment: `virtualenv -p python3 env`
 2. Activate the environment: `source env/bin/activate`
 3. Install the library: `python setup.py develop`
 4. Test the installation with the example: `python3 example/example.py 3.0`
+5. You can run the unit tests by going to the `test` directory and running `python -m unittest`
 
 If the example works correctly, a `job.yml` will be created in the current directory. You can also run `python3 example/example.py --help` to see additional options.
 
 Now the library is available in the environment. Therefore you can easily use the library in your own projects via `import alpaka_job_coverage as ajc`.
 
 ## Contribution
```

### Comparing `alpaka-job-coverage-1.3.6/src/alpaka_job_coverage.egg-info/SOURCES.txt` & `alpaka-job-coverage-1.4.0/src/alpaka_job_coverage.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -8,17 +8,21 @@
 src/alpaka_job_coverage/filter_backend_version.py
 src/alpaka_job_coverage/filter_compiler_name.py
 src/alpaka_job_coverage/filter_compiler_version.py
 src/alpaka_job_coverage/filter_software_dependency.py
 src/alpaka_job_coverage/globals.py
 src/alpaka_job_coverage/main_functions.py
 src/alpaka_job_coverage/util.py
+src/alpaka_job_coverage/validate.py
+src/alpaka_job_coverage/versions.py
 src/alpaka_job_coverage.egg-info/PKG-INFO
 src/alpaka_job_coverage.egg-info/SOURCES.txt
 src/alpaka_job_coverage.egg-info/dependency_links.txt
+src/alpaka_job_coverage.egg-info/entry_points.txt
 src/alpaka_job_coverage.egg-info/requires.txt
 src/alpaka_job_coverage.egg-info/top_level.txt
 tests/test_compiler_names.py
 tests/test_cuda_sdk.py
 tests/test_hipcc.py
 tests/test_single_rules.py
-tests/test_util.py
+tests/test_util.py
+tests/test_versions.py
```

### Comparing `alpaka-job-coverage-1.3.6/tests/test_compiler_names.py` & `alpaka-job-coverage-1.4.0/tests/test_compiler_names.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.3.6/tests/test_cuda_sdk.py` & `alpaka-job-coverage-1.4.0/tests/test_cuda_sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from alpaka_job_coverage.filter_compiler_name import general_compiler_filter_typed
 from alpaka_job_coverage.filter_compiler_version import compiler_version_filter_typed
 from alpaka_job_coverage.filter_backend_version import compiler_backend_filter_typed
 from alpaka_job_coverage.filter_software_dependency import (
     software_dependency_filter_typed,
 )
 from alpaka_job_coverage.globals import *
+from utils import manual_version_test
 
 
 def full_filter_chain(row) -> bool:
     return (
         general_compiler_filter_typed(row)
         and compiler_version_filter_typed(row)
         and compiler_backend_filter_typed(row)
@@ -386,15 +387,17 @@
     # This avoid behavior avoids, that valid combinations are silently disabled
     # if a new CUDA SDK version is released.
     def test_unknown_version(self):
         expected_results = [
             ("42.0", "45", True),
         ]
 
-        # TODO: add is_supported_sw_version to verify that our test version is not supported
+        # verify that our test version are not supported
+        manual_version_test(self, NVCC, [], ["42.0"])
+        manual_version_test(self, GCC, [], ["45"])
 
         for nvcc_version, gcc_version, expected_value in expected_results:
             self.assertEqual(
                 compiler_version_filter_typed(
                     [(NVCC, nvcc_version), (GCC, gcc_version)]
                 ),
                 expected_value,
@@ -464,15 +467,17 @@
     # This avoid behavior avoids, that valid combinations are silently disabled
     # if a new CUDA SDK version is released.
     def test_unknown_version(self):
         expected_results = [
             ("42.0", "45", True),
         ]
 
-        # TODO: add is_supported_sw_version to verify that our test version is not supported
+        # verify that our test version are not supported
+        manual_version_test(self, NVCC, [], ["42.0"])
+        manual_version_test(self, CLANG, [], ["45"])
 
         for nvcc_version, clang_version, expected_value in expected_results:
             self.assertEqual(
                 compiler_version_filter_typed(
                     [(NVCC, nvcc_version), (CLANG, clang_version)]
                 ),
                 expected_value,
@@ -496,26 +501,27 @@
         global param_map
         # reset param_map for following up tests
         param_map = {}
 
     # Test the combination of NVCC as device compiler an the C++ standard.
     # If SDK version is unknown, all C++ standards should be allowed.
     def test_nvcc_cxx(self):
-        # TODO: add is_supported_sw_version to verify that our test version is not supported
+        # verify that our test version are not supported
+        manual_version_test(self, NVCC, [], ["12.2, 45.0"])
 
         for nvcc_version, max_cxx in [
             ("11.0", 17),
             ("11.2", 17),
             ("11.8", 17),
             ("12.0", 20),
             ("12.1", 20),
             # not released version
             # therefore they should support all C++ versions
             ("12.2", 32),
-            ("13.0", 32),
+            ("45.0", 32),
         ]:
             for cxx_version in [11, 14, 17, 20, 23, 26, 29, 32]:
                 comb = [(NVCC, nvcc_version), (CXX_STANDARD, str(cxx_version))]
                 if cxx_version <= max_cxx:
                     self.assertTrue(
                         software_dependency_filter_typed(comb),
                         f"NVCC {nvcc_version} + CXX {cxx_version}",
```

### Comparing `alpaka-job-coverage-1.3.6/tests/test_hipcc.py` & `alpaka-job-coverage-1.4.0/tests/test_hipcc.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.3.6/tests/test_single_rules.py` & `alpaka-job-coverage-1.4.0/tests/test_single_rules.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.3.6/tests/test_util.py` & `alpaka-job-coverage-1.4.0/tests/test_util.py`

 * *Files identical despite different names*

