# Comparing `tmp/dataframe_api_compat-0.1.0.tar.gz` & `tmp/dataframe_api_compat-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataframe_api_compat-0.1.0.tar", last modified: Wed Jun 28 15:17:22 2023, max compression
+gzip compressed data, was "dataframe_api_compat-0.1.1.tar", last modified: Tue Aug  1 14:36:56 2023, max compression
```

## Comparing `dataframe_api_compat-0.1.0.tar` & `dataframe_api_compat-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-06-28 15:17:22.970803 dataframe_api_compat-0.1.0/
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     1071 2023-05-05 10:36:05.000000 dataframe_api_compat-0.1.0/LICENSE
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     3133 2023-06-28 15:17:22.970803 dataframe_api_compat-0.1.0/PKG-INFO
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     2510 2023-06-28 15:12:14.000000 dataframe_api_compat-0.1.0/README.md
-drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-06-28 15:17:22.970803 dataframe_api_compat-0.1.0/dataframe_api_compat/
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-06-28 15:01:51.000000 dataframe_api_compat-0.1.0/dataframe_api_compat/__init__.py
-drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-06-28 15:17:22.970803 dataframe_api_compat-0.1.0/dataframe_api_compat/pandas_standard/
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     1957 2023-06-28 15:06:40.000000 dataframe_api_compat-0.1.0/dataframe_api_compat/pandas_standard/__init__.py
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)    25069 2023-06-28 15:04:35.000000 dataframe_api_compat-0.1.0/dataframe_api_compat/pandas_standard/pandas_standard.py
-drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-06-28 15:17:22.970803 dataframe_api_compat-0.1.0/dataframe_api_compat/polars_standard/
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     1510 2023-06-28 15:06:40.000000 dataframe_api_compat-0.1.0/dataframe_api_compat/polars_standard/__init__.py
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)    19468 2023-06-28 15:07:33.000000 dataframe_api_compat-0.1.0/dataframe_api_compat/polars_standard/polars_standard.py
-drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-06-28 15:17:22.970803 dataframe_api_compat-0.1.0/dataframe_api_compat.egg-info/
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     3133 2023-06-28 15:17:22.000000 dataframe_api_compat-0.1.0/dataframe_api_compat.egg-info/PKG-INFO
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)      455 2023-06-28 15:17:22.000000 dataframe_api_compat-0.1.0/dataframe_api_compat.egg-info/SOURCES.txt
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)        1 2023-06-28 15:17:22.000000 dataframe_api_compat-0.1.0/dataframe_api_compat.egg-info/dependency_links.txt
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)       26 2023-06-28 15:17:22.000000 dataframe_api_compat-0.1.0/dataframe_api_compat.egg-info/top_level.txt
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)      828 2023-06-28 15:17:22.970803 dataframe_api_compat-0.1.0/setup.cfg
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)       38 2023-05-05 10:36:12.000000 dataframe_api_compat-0.1.0/setup.py
+drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-01 14:36:56.694927 dataframe_api_compat-0.1.1/
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     1071 2023-05-05 10:36:05.000000 dataframe_api_compat-0.1.1/LICENSE
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     2365 2023-08-01 14:36:56.694927 dataframe_api_compat-0.1.1/PKG-INFO
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     1731 2023-08-01 13:22:30.000000 dataframe_api_compat-0.1.1/README.md
+drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-01 14:36:56.694927 dataframe_api_compat-0.1.1/dataframe_api_compat/
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-06-28 15:01:51.000000 dataframe_api_compat-0.1.1/dataframe_api_compat/__init__.py
+drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-01 14:36:56.694927 dataframe_api_compat-0.1.1/dataframe_api_compat/pandas_standard/
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     3707 2023-08-01 14:35:35.000000 dataframe_api_compat-0.1.1/dataframe_api_compat/pandas_standard/__init__.py
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)    28727 2023-08-01 14:33:46.000000 dataframe_api_compat-0.1.1/dataframe_api_compat/pandas_standard/pandas_standard.py
+drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-01 14:36:56.694927 dataframe_api_compat-0.1.1/dataframe_api_compat/polars_standard/
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     3074 2023-08-01 14:35:34.000000 dataframe_api_compat-0.1.1/dataframe_api_compat/polars_standard/__init__.py
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)    25104 2023-08-01 14:35:35.000000 dataframe_api_compat-0.1.1/dataframe_api_compat/polars_standard/polars_standard.py
+drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-01 14:36:56.694927 dataframe_api_compat-0.1.1/dataframe_api_compat.egg-info/
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     2365 2023-08-01 14:36:56.000000 dataframe_api_compat-0.1.1/dataframe_api_compat.egg-info/PKG-INFO
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)      470 2023-08-01 14:36:56.000000 dataframe_api_compat-0.1.1/dataframe_api_compat.egg-info/SOURCES.txt
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)        1 2023-08-01 14:36:56.000000 dataframe_api_compat-0.1.1/dataframe_api_compat.egg-info/dependency_links.txt
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)       21 2023-08-01 14:36:56.000000 dataframe_api_compat-0.1.1/dataframe_api_compat.egg-info/top_level.txt
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)      440 2023-08-01 13:41:52.000000 dataframe_api_compat-0.1.1/pyproject.toml
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)      835 2023-08-01 14:36:56.694927 dataframe_api_compat-0.1.1/setup.cfg
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)       38 2023-05-05 10:36:12.000000 dataframe_api_compat-0.1.1/setup.py
```

### Comparing `dataframe_api_compat-0.1.0/LICENSE` & `dataframe_api_compat-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dataframe_api_compat-0.1.0/PKG-INFO` & `dataframe_api_compat-0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: dataframe_api_compat
-Version: 0.1.0
-Summary: Draft implementation of the DataFrame Standard for pandas and polars
-Home-page: https://github.com/MarcoGorelli/dataframe-api-compat
+Version: 0.1.1
+Summary: Implementation of the DataFrame Standard for pandas and polars
+Home-page: https://github.com/data-apis/dataframe-api-compat
 Author: Marco Gorelli
 License: MIT
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Build Status](https://github.com/MarcoGorelli/dataframe-api-compat/workflows/tox/badge.svg)](https://github.com/MarcoGorelli/dataframe-api-compat/actions?workflow=tox)
-[![Coverage](https://codecov.io/gh/MarcoGorelli/cython-lint/branch/main/graph/badge.svg)](https://codecov.io/gh/MarcoGorelli/dataframe-api-compat)
+[![Build Status](https://github.com/data-apis/dataframe-api-compat/workflows/tox/badge.svg)](https://github.com/data-apis/dataframe-api-compat/actions?workflow=tox)
+[![Coverage](https://codecov.io/gh/MarcoGorelli/cython-lint/branch/main/graph/badge.svg)](https://codecov.io/gh/data-apis/dataframe-api-compat)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/MarcoGorelli/dataframe-api-compat/main.svg)](https://results.pre-commit.ci/latest/github/MarcoGorelli/dataframe-api-compat/main)
 
-# DataFrame Standard POC
+# DataFrame API Compat
 
 <h1 align="center">
 	<img
 		width="400"
 		alt="standard-compliant DataFrame"
-		src="https://github.com/MarcoGorelli/dataframe-api-compat/assets/33491632/fb4bc907-2b85-4ad7-8d13-c2b9912b97f5">
+		src="https://github.com/data-apis/dataframe-api-compat/assets/33491632/fb4bc907-2b85-4ad7-8d13-c2b9912b97f5">
 </h1>
 
-Work-in-progress POC of what the [DataFrame Standard](https://data-apis.org/dataframe-api/draft/index.html)
-might look like for pandas and polars.
+Implementation of the [DataFrame Standard](https://data-apis.org/dataframe-api/draft/index.html)
+for pandas and polars.
 
 What's this?
 ------------
 Please read our blog post! https://data-apis.org/blog/dataframe_standard_rfc/.
 
 How to try this out
 -------------------
@@ -55,37 +56,11 @@
 df_std = convert_to_standard_compliant_dataframe(df)
 ```
 The object `df_std` is a Standard-compliant DataFrame.
 
 Installation
 ------------
 ```
-pip install git+https://github.com/MarcoGorelli/dataframe-api-compat
+pip install dataframe-api-compat
 ```
 
-Testing
--------
-```
-pytest --cov=dataframe_api_compat --cov=test_standard --cov-fail-under=100
-```
-100% branch coverage isn't the objective - it's the bare minimum.
-
-Linting
--------
-```
-pre-commit run --all-files
-```
 
-Type Checking
--------------
-
-First, clone the [dataframe_standard](https://github.com/data-apis/dataframe-api) to some
-local path. Then, run:
-```console
-MYPYPATH=<path to dataframe-api/spec/API_specification> mypy dataframe_api_compat
-MYPYPATH=<path to dataframe-api/spec/API_specification> mypy polars_standard.py
-```
-
-For example, if you cloned both repos in the same place, this could be:
-```console
-MYPYPATH=../dataframe-api/spec/API_specification/ mypy dataframe_api_compat
-```
```

### Comparing `dataframe_api_compat-0.1.0/README.md` & `dataframe_api_compat-0.1.1/dataframe_api_compat.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,39 @@
-[![Build Status](https://github.com/MarcoGorelli/dataframe-api-compat/workflows/tox/badge.svg)](https://github.com/MarcoGorelli/dataframe-api-compat/actions?workflow=tox)
-[![Coverage](https://codecov.io/gh/MarcoGorelli/cython-lint/branch/main/graph/badge.svg)](https://codecov.io/gh/MarcoGorelli/dataframe-api-compat)
+Metadata-Version: 2.1
+Name: dataframe-api-compat
+Version: 0.1.1
+Summary: Implementation of the DataFrame Standard for pandas and polars
+Home-page: https://github.com/data-apis/dataframe-api-compat
+Author: Marco Gorelli
+License: MIT
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![Build Status](https://github.com/data-apis/dataframe-api-compat/workflows/tox/badge.svg)](https://github.com/data-apis/dataframe-api-compat/actions?workflow=tox)
+[![Coverage](https://codecov.io/gh/MarcoGorelli/cython-lint/branch/main/graph/badge.svg)](https://codecov.io/gh/data-apis/dataframe-api-compat)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/MarcoGorelli/dataframe-api-compat/main.svg)](https://results.pre-commit.ci/latest/github/MarcoGorelli/dataframe-api-compat/main)
 
-# DataFrame Standard POC
+# DataFrame API Compat
 
 <h1 align="center">
 	<img
 		width="400"
 		alt="standard-compliant DataFrame"
-		src="https://github.com/MarcoGorelli/dataframe-api-compat/assets/33491632/fb4bc907-2b85-4ad7-8d13-c2b9912b97f5">
+		src="https://github.com/data-apis/dataframe-api-compat/assets/33491632/fb4bc907-2b85-4ad7-8d13-c2b9912b97f5">
 </h1>
 
-Work-in-progress POC of what the [DataFrame Standard](https://data-apis.org/dataframe-api/draft/index.html)
-might look like for pandas and polars.
+Implementation of the [DataFrame Standard](https://data-apis.org/dataframe-api/draft/index.html)
+for pandas and polars.
 
 What's this?
 ------------
 Please read our blog post! https://data-apis.org/blog/dataframe_standard_rfc/.
 
 How to try this out
 -------------------
@@ -39,37 +56,11 @@
 df_std = convert_to_standard_compliant_dataframe(df)
 ```
 The object `df_std` is a Standard-compliant DataFrame.
 
 Installation
 ------------
 ```
-pip install git+https://github.com/MarcoGorelli/dataframe-api-compat
-```
-
-Testing
--------
-```
-pytest --cov=dataframe_api_compat --cov=test_standard --cov-fail-under=100
-```
-100% branch coverage isn't the objective - it's the bare minimum.
-
-Linting
--------
-```
-pre-commit run --all-files
+pip install dataframe-api-compat
 ```
 
-Type Checking
--------------
 
-First, clone the [dataframe_standard](https://github.com/data-apis/dataframe-api) to some
-local path. Then, run:
-```console
-MYPYPATH=<path to dataframe-api/spec/API_specification> mypy dataframe_api_compat
-MYPYPATH=<path to dataframe-api/spec/API_specification> mypy polars_standard.py
-```
-
-For example, if you cloned both repos in the same place, this could be:
-```console
-MYPYPATH=../dataframe-api/spec/API_specification/ mypy dataframe_api_compat
-```
```

### Comparing `dataframe_api_compat-0.1.0/dataframe_api_compat/pandas_standard/pandas_standard.py` & `dataframe_api_compat-0.1.1/dataframe_api_compat/pandas_standard/pandas_standard.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,117 +1,158 @@
 from __future__ import annotations
-import dataframe_api_compat.pandas_standard
-import numpy as np
 
-import pandas as pd
-from pandas.api.types import is_extension_array_dtype
 import collections
 from typing import (
-    Any,
-    Sequence,
-    Mapping,
-    NoReturn,
-    cast,
-    Literal,
     TYPE_CHECKING,
+    Any,
     Generic,
+    Literal,
+    NoReturn,
     TypeVar,
+    cast,
+)
+
+import numpy as np
+import pandas as pd
+from pandas.api.types import is_extension_array_dtype
+
+import dataframe_api_compat.pandas_standard
+
+DType = TypeVar("DType")
+
+_ARRAY_API_DTYPES = frozenset(
+    (
+        "bool",
+        "int8",
+        "int16",
+        "int32",
+        "int64",
+        "uint8",
+        "uint16",
+        "uint32",
+        "uint64",
+        "float32",
+        "float64",
+    )
 )
 
 if TYPE_CHECKING:
+    from collections.abc import Mapping, Sequence
+
     from dataframe_api import (
-        DataFrame,
-        DTypeT,
-        IntDType,
         Bool,
         Column,
-        DType,
-        Scalar,
+        DataFrame,
         GroupBy,
     )
 else:
-    DTypeT = TypeVar("DTypeT")
 
-    class DataFrame(Generic[DTypeT]):
+    class DataFrame(Generic[DType]):
         ...
 
-    class Column(Generic[DTypeT]):
+    class Column(Generic[DType]):
         ...
 
     class GroupBy:
         ...
 
 
-class PandasColumn(Column[DTypeT]):
+class PandasColumn(Column[DType]):
     # private, not technically part of the standard
-    def __init__(self, column: pd.Series) -> None:  # type: ignore[type-arg]
+    def __init__(
+        self, column: pd.Series, *, name: str | None = None  # type: ignore[type-arg]
+    ) -> None:
         if (
             isinstance(column.index, pd.RangeIndex)
             and column.index.start == 0  # type: ignore[comparison-overlap]
             and column.index.step == 1  # type: ignore[comparison-overlap]
             and (column.index.stop == len(column))  # type: ignore[comparison-overlap]
         ):
             self._series = column
         else:
             self._series = column.reset_index(drop=True)
+        self._name = name
+
+    def _validate_index(self, index: pd.Index) -> None:
+        pd.testing.assert_index_equal(self.column.index, index)
 
     # In the standard
     def __column_namespace__(self, *, api_version: str | None = None) -> Any:
         return dataframe_api_compat.pandas_standard
 
     @property
+    def name(self) -> str | None:
+        return self._name
+
+    @property
     def column(self) -> pd.Series[Any]:
         return self._series
 
     def __len__(self) -> int:
         return len(self.column)
 
     def __iter__(self) -> NoReturn:
         raise NotImplementedError()
 
     @property
-    def dtype(self) -> DType:
+    def dtype(self) -> Any:
         return dataframe_api_compat.pandas_standard.DTYPE_MAP[self.column.dtype.name]
 
-    def get_rows(self, indices: Column[IntDType]) -> PandasColumn[DTypeT]:
+    def get_rows(self, indices: Column[Any]) -> PandasColumn[DType]:
         return PandasColumn(self.column.iloc[indices.column.to_numpy()])
 
-    def get_value(self, row: int) -> Scalar:
-        return self.column.iloc[row]  # type: ignore[no-any-return]
+    def slice_rows(
+        self, start: int | None, stop: int | None, step: int | None
+    ) -> PandasColumn[DType]:
+        if start is None:
+            start = 0
+        if stop is None:
+            stop = len(self.column)
+        if step is None:
+            step = 1
+        return PandasColumn(self.column.iloc[start:stop:step])
+
+    def get_rows_by_mask(self, mask: Column[Bool]) -> PandasColumn[DType]:
+        series = mask.column
+        self._validate_index(series.index)
+        return PandasColumn(self.column.loc[series])
+
+    def get_value(self, row: int) -> Any:
+        return self.column.iloc[row]
 
     def __eq__(  # type: ignore[override]
-        self, other: PandasColumn[DTypeT] | Scalar
+        self, other: PandasColumn[DType] | Any
     ) -> PandasColumn[Bool]:
         if isinstance(other, PandasColumn):
             return PandasColumn(self.column == other.column)
         return PandasColumn(self.column == other)
 
     def __ne__(  # type: ignore[override]
-        self, other: Column[DTypeT]
+        self, other: Column[DType]
     ) -> PandasColumn[Bool]:
         if isinstance(other, PandasColumn):
             return PandasColumn(self.column != other.column)
         return PandasColumn(self.column != other)
 
-    def __ge__(self, other: Column[DTypeT] | Scalar) -> PandasColumn[Bool]:
+    def __ge__(self, other: Column[DType] | Any) -> PandasColumn[Bool]:
         if isinstance(other, PandasColumn):
             return PandasColumn(self.column >= other.column)
         return PandasColumn(self.column >= other)
 
-    def __gt__(self, other: Column[DTypeT] | Scalar) -> PandasColumn[Bool]:
+    def __gt__(self, other: Column[DType] | Any) -> PandasColumn[Bool]:
         if isinstance(other, PandasColumn):
             return PandasColumn(self.column > other.column)
         return PandasColumn(self.column > other)
 
-    def __le__(self, other: Column[DTypeT] | Scalar) -> PandasColumn[Bool]:
+    def __le__(self, other: Column[DType] | Any) -> PandasColumn[Bool]:
         if isinstance(other, PandasColumn):
             return PandasColumn(self.column <= other.column)
         return PandasColumn(self.column <= other)
 
-    def __lt__(self, other: Column[DTypeT] | Scalar) -> PandasColumn[Bool]:
+    def __lt__(self, other: Column[DType] | Any) -> PandasColumn[Bool]:
         if isinstance(other, PandasColumn):
             return PandasColumn(self.column < other.column)
         return PandasColumn(self.column < other)
 
     def __and__(self, other: Column[Bool] | bool) -> PandasColumn[Bool]:
         if isinstance(other, PandasColumn):
             return PandasColumn(self.column & other.column)
@@ -119,51 +160,51 @@
         return PandasColumn(result)
 
     def __or__(self, other: Column[Bool] | bool) -> PandasColumn[Bool]:
         if isinstance(other, PandasColumn):
             return PandasColumn(self.column | other.column)
         return PandasColumn(self.column | other)  # type: ignore[operator]
 
-    def __add__(self, other: Column[DTypeT] | Scalar) -> PandasColumn[DTypeT]:
+    def __add__(self, other: Column[DType] | Any) -> PandasColumn[DType]:
         if isinstance(other, PandasColumn):
             return PandasColumn(self.column + other.column)
         return PandasColumn(self.column + other)  # type: ignore[operator]
 
-    def __sub__(self, other: Column[DTypeT] | Scalar) -> PandasColumn[DTypeT]:
+    def __sub__(self, other: Column[DType] | Any) -> PandasColumn[DType]:
         if isinstance(other, PandasColumn):
             return PandasColumn(self.column - other.column)
         return PandasColumn(self.column - other)  # type: ignore[operator]
 
-    def __mul__(self, other: Column[DTypeT] | Scalar) -> PandasColumn[Any]:
+    def __mul__(self, other: Column[DType] | Any) -> PandasColumn[Any]:
         if isinstance(other, PandasColumn):
             return PandasColumn(self.column * other.column)
         return PandasColumn(self.column * other)  # type: ignore[operator]
 
-    def __truediv__(self, other: Column[DTypeT] | Scalar) -> PandasColumn[Any]:
+    def __truediv__(self, other: Column[DType] | Any) -> PandasColumn[Any]:
         if isinstance(other, PandasColumn):
             return PandasColumn(self.column / other.column)
         return PandasColumn(self.column / other)  # type: ignore[operator]
 
-    def __floordiv__(self, other: Column[DTypeT] | Scalar) -> PandasColumn[Any]:
+    def __floordiv__(self, other: Column[DType] | Any) -> PandasColumn[Any]:
         if isinstance(other, PandasColumn):
             return PandasColumn(self.column // other.column)
         return PandasColumn(self.column // other)  # type: ignore[operator]
 
-    def __pow__(self, other: Column[DTypeT] | Scalar) -> PandasColumn[Any]:
+    def __pow__(self, other: Column[DType] | Any) -> PandasColumn[Any]:
         if isinstance(other, PandasColumn):
             return PandasColumn(self.column**other.column)
         return PandasColumn(self.column**other)  # type: ignore[operator]
 
-    def __mod__(self, other: Column[DTypeT] | Scalar) -> PandasColumn[Any]:
+    def __mod__(self, other: Column[DType] | Any) -> PandasColumn[Any]:
         if isinstance(other, PandasColumn):
             return PandasColumn(self.column % other.column)
         return PandasColumn(self.column % other)  # type: ignore[operator]
 
     def __divmod__(
-        self, other: Column[DTypeT] | Scalar
+        self, other: Column[DType] | Any
     ) -> tuple[PandasColumn[Any], PandasColumn[Any]]:
         if isinstance(other, PandasColumn):
             quotient, remainder = self.column.__divmod__(other.column)
         else:
             quotient, remainder = self.column.__divmod__(other)
         return PandasColumn(quotient), PandasColumn(remainder)
 
@@ -172,69 +213,100 @@
 
     def any(self, *, skip_nulls: bool = True) -> bool:
         return self.column.any()
 
     def all(self, *, skip_nulls: bool = True) -> bool:
         return self.column.all()
 
-    def min(self, *, skip_nulls: bool = True) -> Scalar:
-        return self.column.min()  # type: ignore[no-any-return]
+    def min(self, *, skip_nulls: bool = True) -> Any:
+        return self.column.min()
 
-    def max(self, *, skip_nulls: bool = True) -> Scalar:
-        return self.column.max()  # type: ignore[no-any-return]
+    def max(self, *, skip_nulls: bool = True) -> Any:
+        return self.column.max()
 
-    def sum(self, *, skip_nulls: bool = True) -> Scalar:
-        return self.column.sum()  # type: ignore[no-any-return]
+    def sum(self, *, skip_nulls: bool = True) -> Any:
+        return self.column.sum()
 
-    def prod(self, *, skip_nulls: bool = True) -> Scalar:
-        return self.column.prod()  # type: ignore[return-value]
+    def prod(self, *, skip_nulls: bool = True) -> Any:
+        return self.column.prod()
 
-    def median(self, *, skip_nulls: bool = True) -> Scalar:
-        return self.column.median()  # type: ignore[return-value]
+    def median(self, *, skip_nulls: bool = True) -> Any:
+        return self.column.median()
 
-    def mean(self, *, skip_nulls: bool = True) -> Scalar:
-        return self.column.mean()  # type: ignore[return-value]
+    def mean(self, *, skip_nulls: bool = True) -> Any:
+        return self.column.mean()
 
-    def std(self, *, skip_nulls: bool = True) -> Scalar:
-        return self.column.std()  # type: ignore[return-value]
+    def std(self, *, correction: int | float = 1.0, skip_nulls: bool = True) -> Any:
+        return self.column.std()
 
-    def var(self, *, skip_nulls: bool = True) -> Scalar:
-        return self.column.var()  # type: ignore[return-value]
+    def var(self, *, correction: int | float = 1.0, skip_nulls: bool = True) -> Any:
+        return self.column.var()
 
     def is_null(self) -> PandasColumn[Bool]:
         if is_extension_array_dtype(self.column.dtype):
             return PandasColumn(self.column.isnull())
         else:
             return PandasColumn(pd.Series(np.array([False] * len(self))))
 
     def is_nan(self) -> PandasColumn[Bool]:
         if is_extension_array_dtype(self.column.dtype):
             return PandasColumn(np.isnan(self.column).replace(pd.NA, False).astype(bool))
         return PandasColumn(self.column.isna())
 
     def sorted_indices(
         self, *, ascending: bool = True, nulls_position: Literal["first", "last"] = "last"
-    ) -> PandasColumn[IntDType]:
-        return PandasColumn(pd.Series(self.column.argsort()))
+    ) -> PandasColumn[Any]:
+        if ascending:
+            return PandasColumn(pd.Series(self.column.argsort()))
+        return PandasColumn(pd.Series(self.column.argsort()[::-1]))
 
-    def is_in(self, values: Column[DTypeT]) -> PandasColumn[Bool]:
+    def is_in(self, values: Column[DType]) -> PandasColumn[Bool]:
         if values.dtype != self.dtype:
             raise ValueError(f"`value` has dtype {values.dtype}, expected {self.dtype}")
         return PandasColumn(self.column.isin(values.column))
 
-    def unique_indices(self, *, skip_nulls: bool = True) -> PandasColumn[IntDType]:
+    def unique_indices(self, *, skip_nulls: bool = True) -> PandasColumn[Any]:
         return PandasColumn(self.column.drop_duplicates().index.to_series())
 
     def fill_nan(
         self, value: float | pd.NAType  # type: ignore[name-defined]
-    ) -> PandasColumn[DTypeT]:
+    ) -> PandasColumn[DType]:
         ser = self.column.copy()
         ser[cast("pd.Series[bool]", np.isnan(ser)).fillna(False).to_numpy(bool)] = value
         return PandasColumn(ser)
 
+    def fill_null(
+        self,
+        value: Any,
+    ) -> PandasColumn[DType]:
+        ser = self.column.copy()
+        ser = np.where(
+            np.isnan(ser).fillna(False), ser, ser.fillna(value)
+        )  # type: ignore[assignment]
+        return PandasColumn(pd.Series(ser))
+
+    def cumulative_sum(self, *, skip_nulls: bool = True) -> PandasColumn[DType]:
+        return PandasColumn(self.column.cumsum())
+
+    def cumulative_prod(self, *, skip_nulls: bool = True) -> PandasColumn[DType]:
+        return PandasColumn(self.column.cumprod())
+
+    def cumulative_max(self, *, skip_nulls: bool = True) -> PandasColumn[DType]:
+        return PandasColumn(self.column.cummax())
+
+    def cumulative_min(self, *, skip_nulls: bool = True) -> PandasColumn[DType]:
+        return PandasColumn(self.column.cummin())
+
+    def to_array_object(self, dtype: str) -> Any:
+        if dtype not in _ARRAY_API_DTYPES:
+            raise ValueError(
+                f"Invalid dtype {dtype}. Expected one of {_ARRAY_API_DTYPES}"
+            )
+        return self.column.to_numpy(dtype=dtype)
+
 
 class PandasGroupBy(GroupBy):
     def __init__(self, df: pd.DataFrame, keys: Sequence[str]) -> None:
         self.df = df
         self.grouped = df.groupby(list(keys), sort=False, as_index=False)
         self.keys = list(keys)
 
@@ -252,15 +324,15 @@
         return PandasDataFrame(self.grouped.size())  # type: ignore[arg-type]
 
     def _validate_booleanness(self) -> None:
         if not (
             (self.df.drop(columns=self.keys).dtypes == "bool")
             | (self.df.drop(columns=self.keys).dtypes == "boolean")
         ).all():
-            raise NotImplementedError(
+            raise ValueError(
                 "'function' can only be called on DataFrame "
                 "where all dtypes are 'bool'"
             )
 
     def any(self, *, skip_nulls: bool = True) -> PandasDataFrame:
         self._validate_booleanness()
         result = self.grouped.any()
@@ -299,20 +371,24 @@
         return PandasDataFrame(result)
 
     def mean(self, *, skip_nulls: bool = True) -> PandasDataFrame:
         result = self.grouped.mean()
         self._validate_result(result)
         return PandasDataFrame(result)
 
-    def std(self, *, skip_nulls: bool = True) -> PandasDataFrame:
+    def std(
+        self, *, correction: int | float = 1.0, skip_nulls: bool = True
+    ) -> PandasDataFrame:
         result = self.grouped.std()
         self._validate_result(result)
         return PandasDataFrame(result)
 
-    def var(self, *, skip_nulls: bool = True) -> PandasDataFrame:
+    def var(
+        self, *, correction: int | float = 1.0, skip_nulls: bool = True
+    ) -> PandasDataFrame:
         result = self.grouped.var()
         self._validate_result(result)
         return PandasDataFrame(result)
 
 
 class PandasDataFrame(DataFrame):
     # Not technically part of the standard
@@ -384,26 +460,26 @@
         if isinstance(keys, str):
             raise TypeError("Expected sequence of strings, got: str")
         for key in keys:
             if key not in self.get_column_names():
                 raise KeyError(f"key {key} not present in DataFrame's columns")
         return PandasGroupBy(self.dataframe, keys)
 
-    def get_column_by_name(self, name: str) -> PandasColumn[DTypeT]:
+    def get_column_by_name(self, name: str) -> PandasColumn[DType]:
         if not isinstance(name, str):
             raise ValueError(f"Expected str, got: {type(name)}")
         return PandasColumn(self.dataframe.loc[:, name])
 
     def get_columns_by_name(self, names: Sequence[str]) -> PandasDataFrame:
         if isinstance(names, str):
             raise TypeError(f"Expected sequence of str, got {type(names)}")
         self._validate_columns(names)
         return PandasDataFrame(self.dataframe.loc[:, list(names)])
 
-    def get_rows(self, indices: Column[IntDType]) -> PandasDataFrame:
+    def get_rows(self, indices: Column[Any]) -> PandasDataFrame:
         return PandasDataFrame(self.dataframe.iloc[indices.column, :])
 
     def slice_rows(
         self, start: int | None, stop: int | None, step: int | None
     ) -> PandasDataFrame:
         if start is None:
             start = 0
@@ -437,107 +513,127 @@
         return PandasDataFrame(self.dataframe.rename(columns=mapping))
 
     def get_column_names(self) -> Sequence[str]:
         return self.dataframe.columns.tolist()
 
     def sorted_indices(
         self,
-        keys: Sequence[str],
+        keys: Sequence[str] | None = None,
         *,
         ascending: Sequence[bool] | bool = True,
         nulls_position: Literal["first", "last"] = "last",
-    ) -> PandasColumn[IntDType]:
+    ) -> PandasColumn[Any]:
+        if keys is None:
+            keys = self.dataframe.columns.tolist()
         df = self.dataframe.loc[:, list(keys)]
-        return PandasColumn(df.sort_values(keys).index.to_series())
+        if ascending:
+            return PandasColumn(df.sort_values(keys).index.to_series())
+        return PandasColumn(df.sort_values(keys).index.to_series()[::-1])
 
-    def __eq__(  # type: ignore[override]
-        self, other: DataFrame | Scalar
-    ) -> PandasDataFrame:
+    def unique_indices(
+        self,
+        keys: Sequence[str] | None = None,
+        *,
+        skip_nulls: bool = True,
+    ) -> PandasColumn[Any]:
+        return PandasColumn(self.dataframe.drop_duplicates(subset=keys).index.to_series())
+
+    def __eq__(self, other: DataFrame | Any) -> PandasDataFrame:  # type: ignore[override]
         if isinstance(other, PandasDataFrame):
             self._validate_comparand(other)
             return PandasDataFrame(self.dataframe.__eq__(other.dataframe))
         return PandasDataFrame(self.dataframe.__eq__(other))
 
-    def __ne__(  # type: ignore[override]
-        self, other: DataFrame | Scalar
-    ) -> PandasDataFrame:
+    def __ne__(self, other: DataFrame | Any) -> PandasDataFrame:  # type: ignore[override]
+        if isinstance(other, PandasDataFrame):
+            self._validate_comparand(other)
+            return PandasDataFrame(self.dataframe.__ne__(other.dataframe))
+        return PandasDataFrame(self.dataframe.__ne__(other))
+
+    def __ge__(self, other: DataFrame | Any) -> PandasDataFrame:
+        if isinstance(other, PandasDataFrame):
+            self._validate_comparand(other)
+            return PandasDataFrame(self.dataframe.__ge__(other.dataframe))
+        return PandasDataFrame(self.dataframe.__ge__(other))
+
+    def __gt__(self, other: DataFrame | Any) -> PandasDataFrame:
         if isinstance(other, PandasDataFrame):
             self._validate_comparand(other)
-            return PandasDataFrame((self.dataframe.__ne__(other.dataframe)))
-        return PandasDataFrame((self.dataframe.__ne__(other)))
+            return PandasDataFrame(self.dataframe.__gt__(other.dataframe))
+        return PandasDataFrame(self.dataframe.__gt__(other))
 
-    def __ge__(self, other: DataFrame | Scalar) -> PandasDataFrame:
+    def __le__(self, other: DataFrame | Any) -> PandasDataFrame:
         if isinstance(other, PandasDataFrame):
             self._validate_comparand(other)
-            return PandasDataFrame((self.dataframe.__ge__(other.dataframe)))
-        return PandasDataFrame((self.dataframe.__ge__(other)))
+            return PandasDataFrame(self.dataframe.__le__(other.dataframe))
+        return PandasDataFrame(self.dataframe.__le__(other))
 
-    def __gt__(self, other: DataFrame | Scalar) -> PandasDataFrame:
+    def __lt__(self, other: DataFrame | Any) -> PandasDataFrame:
         if isinstance(other, PandasDataFrame):
             self._validate_comparand(other)
-            return PandasDataFrame((self.dataframe.__gt__(other.dataframe)))
-        return PandasDataFrame((self.dataframe.__gt__(other)))
+            return PandasDataFrame(self.dataframe.__lt__(other.dataframe))
+        return PandasDataFrame(self.dataframe.__lt__(other))
 
-    def __le__(self, other: DataFrame | Scalar) -> PandasDataFrame:
+    def __and__(self, other: DataFrame | Any) -> PandasDataFrame:
         if isinstance(other, PandasDataFrame):
             self._validate_comparand(other)
-            return PandasDataFrame((self.dataframe.__le__(other.dataframe)))
-        return PandasDataFrame((self.dataframe.__le__(other)))
+            return PandasDataFrame(self.dataframe.__and__(other.dataframe))
+        return PandasDataFrame(self.dataframe.__and__(other))
 
-    def __lt__(self, other: DataFrame | Scalar) -> PandasDataFrame:
+    def __or__(self, other: DataFrame | Any) -> PandasDataFrame:
         if isinstance(other, PandasDataFrame):
             self._validate_comparand(other)
-            return PandasDataFrame((self.dataframe.__lt__(other.dataframe)))
-        return PandasDataFrame((self.dataframe.__lt__(other)))
+            return PandasDataFrame(self.dataframe.__or__(other.dataframe))
+        return PandasDataFrame(self.dataframe.__or__(other))
 
-    def __add__(self, other: DataFrame | Scalar) -> PandasDataFrame:
+    def __add__(self, other: DataFrame | Any) -> PandasDataFrame:
         if isinstance(other, PandasDataFrame):
             self._validate_comparand(other)
-            return PandasDataFrame((self.dataframe.__add__(other.dataframe)))
-        return PandasDataFrame((self.dataframe.__add__(other)))
+            return PandasDataFrame(self.dataframe.__add__(other.dataframe))
+        return PandasDataFrame(self.dataframe.__add__(other))
 
-    def __sub__(self, other: DataFrame | Scalar) -> PandasDataFrame:
+    def __sub__(self, other: DataFrame | Any) -> PandasDataFrame:
         if isinstance(other, PandasDataFrame):
             self._validate_comparand(other)
-            return PandasDataFrame((self.dataframe.__sub__(other.dataframe)))
-        return PandasDataFrame((self.dataframe.__sub__(other)))
+            return PandasDataFrame(self.dataframe.__sub__(other.dataframe))
+        return PandasDataFrame(self.dataframe.__sub__(other))
 
-    def __mul__(self, other: DataFrame | Scalar) -> PandasDataFrame:
+    def __mul__(self, other: DataFrame | Any) -> PandasDataFrame:
         if isinstance(other, PandasDataFrame):
             self._validate_comparand(other)
-            return PandasDataFrame((self.dataframe.__mul__(other.dataframe)))
-        return PandasDataFrame((self.dataframe.__mul__(other)))
+            return PandasDataFrame(self.dataframe.__mul__(other.dataframe))
+        return PandasDataFrame(self.dataframe.__mul__(other))
 
-    def __truediv__(self, other: DataFrame | Scalar) -> PandasDataFrame:
+    def __truediv__(self, other: DataFrame | Any) -> PandasDataFrame:
         if isinstance(other, PandasDataFrame):
             self._validate_comparand(other)
-            return PandasDataFrame((self.dataframe.__truediv__(other.dataframe)))
-        return PandasDataFrame((self.dataframe.__truediv__(other)))
+            return PandasDataFrame(self.dataframe.__truediv__(other.dataframe))
+        return PandasDataFrame(self.dataframe.__truediv__(other))
 
-    def __floordiv__(self, other: DataFrame | Scalar) -> PandasDataFrame:
+    def __floordiv__(self, other: DataFrame | Any) -> PandasDataFrame:
         if isinstance(other, PandasDataFrame):
             self._validate_comparand(other)
-            return PandasDataFrame((self.dataframe.__floordiv__(other.dataframe)))
-        return PandasDataFrame((self.dataframe.__floordiv__(other)))
+            return PandasDataFrame(self.dataframe.__floordiv__(other.dataframe))
+        return PandasDataFrame(self.dataframe.__floordiv__(other))
 
-    def __pow__(self, other: DataFrame | Scalar) -> PandasDataFrame:
+    def __pow__(self, other: DataFrame | Any) -> PandasDataFrame:
         if isinstance(other, PandasDataFrame):
             self._validate_comparand(other)
-            return PandasDataFrame((self.dataframe.__pow__(other.dataframe)))
-        return PandasDataFrame((self.dataframe.__pow__(other)))
+            return PandasDataFrame(self.dataframe.__pow__(other.dataframe))
+        return PandasDataFrame(self.dataframe.__pow__(other))
 
-    def __mod__(self, other: DataFrame | Scalar) -> PandasDataFrame:
+    def __mod__(self, other: DataFrame | Any) -> PandasDataFrame:
         if isinstance(other, PandasDataFrame):
             self._validate_comparand(other)
-            return PandasDataFrame((self.dataframe.__mod__(other.dataframe)))
-        return PandasDataFrame((self.dataframe.__mod__(other)))
+            return PandasDataFrame(self.dataframe.__mod__(other.dataframe))
+        return PandasDataFrame(self.dataframe.__mod__(other))
 
     def __divmod__(
         self,
-        other: DataFrame | Scalar,
+        other: DataFrame | Any,
     ) -> tuple[PandasDataFrame, PandasDataFrame]:
         if isinstance(other, PandasDataFrame):
             self._validate_comparand(other)
             quotient, remainder = self.dataframe.__divmod__(other.dataframe)
         else:
             quotient, remainder = self.dataframe.__divmod__(other)
         return PandasDataFrame(quotient), PandasDataFrame(remainder)
@@ -579,18 +675,22 @@
 
     def median(self, *, skip_nulls: bool = True) -> PandasDataFrame:
         return PandasDataFrame(self.dataframe.median().to_frame().T)
 
     def mean(self, *, skip_nulls: bool = True) -> PandasDataFrame:
         return PandasDataFrame(self.dataframe.mean().to_frame().T)
 
-    def std(self, *, skip_nulls: bool = True) -> PandasDataFrame:
+    def std(
+        self, *, correction: int | float = 1.0, skip_nulls: bool = True
+    ) -> PandasDataFrame:
         return PandasDataFrame(self.dataframe.std().to_frame().T)
 
-    def var(self, *, skip_nulls: bool = True) -> PandasDataFrame:
+    def var(
+        self, *, correction: int | float = 1.0, skip_nulls: bool = True
+    ) -> PandasDataFrame:
         return PandasDataFrame(self.dataframe.var().to_frame().T)
 
     def is_null(self, *, skip_nulls: bool = True) -> PandasDataFrame:
         result = []
         for column in self.dataframe.columns:
             if is_extension_array_dtype(self.dataframe[column].dtype):
                 result.append(self.dataframe[column].isnull())
@@ -612,10 +712,30 @@
     def fill_nan(
         self, value: float | pd.NAType  # type: ignore[name-defined]
     ) -> PandasDataFrame:
         df = self.dataframe.copy()
         df[cast(pd.DataFrame, np.isnan(df)).fillna(False).to_numpy(bool)] = value
         return PandasDataFrame(df)
 
+    def fill_null(
+        self,
+        value: Any,
+        *,
+        column_names: list[str] | None = None,
+    ) -> PandasDataFrame:
+        if column_names is None:
+            column_names = self.dataframe.columns.tolist()
+        df = self.dataframe.copy()
+        for column in column_names:
+            col = df[column]
+            col = np.where(
+                np.isnan(col).fillna(False), col, col.fillna(value)
+            )  # type: ignore[assignment]
+            df[column] = col
+        return PandasDataFrame(df)
 
-# missing: min, max, prod, etc...
-# ok, break, then do that?
+    def to_array_object(self, dtype: str) -> Any:
+        if dtype not in _ARRAY_API_DTYPES:
+            raise ValueError(
+                f"Invalid dtype {dtype}. Expected one of {_ARRAY_API_DTYPES}"
+            )
+        return self.dataframe.to_numpy(dtype=dtype)
```

### Comparing `dataframe_api_compat-0.1.0/dataframe_api_compat/polars_standard/polars_standard.py` & `dataframe_api_compat-0.1.1/dataframe_api_compat/polars_standard/polars_standard.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,186 +1,251 @@
 from __future__ import annotations
-import dataframe_api_compat.polars_standard
-import collections
 
+import collections
 from typing import (
-    Any,
-    Sequence,
-    Mapping,
-    NoReturn,
     TYPE_CHECKING,
+    Any,
     Generic,
-    TypeVar,
     Literal,
+    NoReturn,
+    TypeVar,
 )
+
 import polars as pl
 
+import dataframe_api_compat.polars_standard
+
+_ARRAY_API_DTYPES = frozenset(
+    (
+        "bool",
+        "int8",
+        "int16",
+        "int32",
+        "int64",
+        "uint8",
+        "uint16",
+        "uint32",
+        "uint64",
+        "float32",
+        "float64",
+    )
+)
+DType = TypeVar("DType")
+
 if TYPE_CHECKING:
+    from collections.abc import Mapping, Sequence
+
     from dataframe_api import (
-        DataFrame,
-        DTypeT,
-        IntDType,
         Bool,
         Column,
-        Scalar,
+        DataFrame,
         GroupBy,
-        null,
-        DType,
     )
 else:
-    DTypeT = TypeVar("DTypeT")
 
-    class DataFrame(Generic[DTypeT]):
+    class DataFrame(Generic[DType]):
         ...
 
-    class Column(Generic[DTypeT]):
+    class Column(Generic[DType]):
         ...
 
     class GroupBy:
         ...
 
 
-class PolarsColumn(Column[DTypeT]):
-    def __init__(self, column: pl.Series) -> None:
+null = None
+NullType = type[None]
+
+
+def _is_integer_dtype(dtype: Any) -> bool:
+    return any(
+        dtype is _dtype
+        for _dtype in (
+            pl.Int64,
+            pl.Int32,
+            pl.Int16,
+            pl.Int8,
+            pl.UInt64,
+            pl.UInt32,
+            pl.UInt16,
+            pl.UInt8,
+        )
+    )
+
+
+class PolarsColumn(Column[DType]):
+    def __init__(self, column: pl.Series, *, name: str | None = None) -> None:
         self._series = column
+        self._name = name
 
     # In the standard
     def __column_namespace__(self, *, api_version: str | None = None) -> Any:
         return dataframe_api_compat.polars_standard
 
     @property
+    def name(self) -> str | None:
+        return self._name
+
+    @property
     def column(self) -> pl.Series:
         return self._series
 
     def __len__(self) -> int:
         return len(self.column)
 
     @property
-    def dtype(self) -> DType:
-        return dataframe_api_compat.polars_standard.DTYPE_MAP[  # type: ignore[index]
-            self.column.dtype
+    def dtype(self) -> Any:
+        return dataframe_api_compat.polars_standard.DTYPE_MAP[
+            self.column.dtype  # type: ignore[index]
         ]
 
-    def get_rows(self, indices: Column[IntDType]) -> PolarsColumn[DTypeT]:
+    def get_rows(self, indices: Column[Any]) -> PolarsColumn[DType]:
         return PolarsColumn(self.column.take(indices.column))
 
-    def get_value(self, row: int) -> Scalar:
-        return self.column[row]  # type: ignore[no-any-return]
+    def slice_rows(
+        self, start: int | None, stop: int | None, step: int | None
+    ) -> PolarsColumn[DType]:
+        if start is None:
+            start = 0
+        if stop is None:
+            stop = len(self.column)
+        if step is None:
+            step = 1
+        return PolarsColumn(self.column[start:stop:step])
+
+    def get_rows_by_mask(self, mask: Column[Bool]) -> PolarsColumn[DType]:
+        name = self.column.name
+        return PolarsColumn(self.column.to_frame().filter(mask.column)[name])
+
+    def get_value(self, row: int) -> Any:
+        return self.column[row]
 
     def __iter__(self) -> NoReturn:
         raise NotImplementedError()
 
-    def is_in(self, values: Column[DTypeT]) -> PolarsColumn[Bool]:
+    def is_in(self, values: Column[DType]) -> PolarsColumn[Bool]:
         if values.dtype != self.dtype:
             raise ValueError(f"`value` has dtype {values.dtype}, expected {self.dtype}")
         return PolarsColumn(self.column.is_in(values.column))
 
-    def unique_indices(self, *, skip_nulls: bool = True) -> PolarsColumn[IntDType]:
+    def unique_indices(self, *, skip_nulls: bool = True) -> PolarsColumn[Any]:
         df = self.column.to_frame()
         keys = df.columns
         return PolarsColumn(df.with_row_count().unique(keys)["row_nr"])
 
     def is_null(self) -> PolarsColumn[Bool]:
         return PolarsColumn(self.column.is_null())
 
     def is_nan(self) -> PolarsColumn[Bool]:
         return PolarsColumn(self.column.is_nan())
 
-    def any(self, *, skip_nulls: bool = True) -> bool:
+    def any(self, *, skip_nulls: bool = True) -> bool | None:
+        # todo: this is wrong!
         return self.column.any()
 
-    def all(self, *, skip_nulls: bool = True) -> bool:
+    def all(self, *, skip_nulls: bool = True) -> bool | None:
         return self.column.all()
 
-    def min(self, *, skip_nulls: bool = True) -> Scalar:
-        return self.column.min()  # type: ignore[return-value]
+    def min(self, *, skip_nulls: bool = True) -> Any:
+        return self.column.min()
 
-    def max(self, *, skip_nulls: bool = True) -> Scalar:
-        return self.column.max()  # type: ignore[return-value]
+    def max(self, *, skip_nulls: bool = True) -> Any:
+        return self.column.max()
 
-    def sum(self, *, skip_nulls: bool = True) -> Scalar:
-        return self.column.sum()  # type: ignore[return-value]
+    def sum(self, *, skip_nulls: bool = True) -> Any:
+        return self.column.sum()
 
-    def prod(self, *, skip_nulls: bool = True) -> Scalar:
-        return self.column.product()  # type: ignore[return-value]
+    def prod(self, *, skip_nulls: bool = True) -> Any:
+        return self.column.product()
 
-    def mean(self, *, skip_nulls: bool = True) -> Scalar:
-        return self.column.mean()  # type: ignore[return-value]
+    def mean(self, *, skip_nulls: bool = True) -> Any:
+        return self.column.mean()
 
-    def median(self, *, skip_nulls: bool = True) -> Scalar:
-        return self.column.median()  # type: ignore[return-value]
+    def median(self, *, skip_nulls: bool = True) -> Any:
+        return self.column.median()
 
-    def std(self, *, skip_nulls: bool = True) -> Scalar:
-        return self.column.std()  # type: ignore[return-value]
+    def std(self, *, correction: int | float = 1.0, skip_nulls: bool = True) -> Any:
+        return self.column.std()
 
-    def var(self, *, skip_nulls: bool = True) -> Scalar:
-        return self.column.var()  # type: ignore[return-value]
+    def var(self, *, correction: int | float = 1.0, skip_nulls: bool = True) -> Any:
+        return self.column.var()
 
     def __eq__(  # type: ignore[override]
-        self, other: Column[DTypeT] | Scalar
+        self, other: Column[DType] | Any
     ) -> PolarsColumn[Bool]:
         if isinstance(other, PolarsColumn):
             return PolarsColumn(self.column == other.column)
         return PolarsColumn(self.column == other)
 
     def __ne__(  # type: ignore[override]
-        self, other: Column[DTypeT] | Scalar
+        self, other: Column[DType] | Any
     ) -> PolarsColumn[Bool]:
         if isinstance(other, PolarsColumn):
             return PolarsColumn(self.column != other.column)
         return PolarsColumn(self.column != other)
 
-    def __ge__(self, other: Column[DTypeT] | Scalar) -> PolarsColumn[Bool]:
+    def __ge__(self, other: Column[DType] | Any) -> PolarsColumn[Bool]:
         if isinstance(other, PolarsColumn):
             return PolarsColumn(self.column >= other.column)
         return PolarsColumn(self.column >= other)
 
-    def __gt__(self, other: Column[DTypeT] | Scalar) -> PolarsColumn[Bool]:
+    def __gt__(self, other: Column[DType] | Any) -> PolarsColumn[Bool]:
         if isinstance(other, PolarsColumn):
             return PolarsColumn(self.column > other.column)
         return PolarsColumn(self.column > other)
 
-    def __le__(self, other: Column[DTypeT] | Scalar) -> PolarsColumn[Bool]:
+    def __le__(self, other: Column[DType] | Any) -> PolarsColumn[Bool]:
         if isinstance(other, PolarsColumn):
             return PolarsColumn(self.column <= other.column)
         return PolarsColumn(self.column <= other)
 
-    def __lt__(self, other: Column[DTypeT] | Scalar) -> PolarsColumn[Bool]:
+    def __lt__(self, other: Column[DType] | Any) -> PolarsColumn[Bool]:
         if isinstance(other, PolarsColumn):
             return PolarsColumn(self.column < other.column)
         return PolarsColumn(self.column < other)
 
-    def __mul__(self, other: Column[DTypeT] | Scalar) -> PolarsColumn[Any]:
+    def __mul__(self, other: Column[DType] | Any) -> PolarsColumn[Any]:
         if isinstance(other, PolarsColumn):
             return PolarsColumn(self.column * other.column)
         return PolarsColumn(self.column * other)
 
-    def __floordiv__(self, other: Column[DTypeT] | Scalar) -> PolarsColumn[Any]:
+    def __floordiv__(self, other: Column[DType] | Any) -> PolarsColumn[Any]:
         if isinstance(other, PolarsColumn):
             return PolarsColumn(self.column // other.column)
         return PolarsColumn(self.column // other)
 
-    def __truediv__(self, other: Column[DTypeT] | Scalar) -> PolarsColumn[Any]:
+    def __truediv__(self, other: Column[DType] | Any) -> PolarsColumn[Any]:
         if isinstance(other, PolarsColumn):
             return PolarsColumn(self.column / other.column)
         return PolarsColumn(self.column / other)
 
-    def __pow__(self, other: Column[DTypeT] | Scalar) -> PolarsColumn[Any]:
+    def __pow__(self, other: Column[DType] | Any) -> PolarsColumn[Any]:
+        original_type = self.column.dtype
         if isinstance(other, PolarsColumn):
-            return PolarsColumn(self.column.pow(other.column))
-        return PolarsColumn(self.column.pow(other))  # type: ignore[arg-type]
+            ret = self.column.pow(other.column)
+            if _is_integer_dtype(original_type) and _is_integer_dtype(other.column.dtype):
+                if (other.column < 0).any():
+                    raise ValueError("Cannot raise integer to negative power")
+                ret = ret.cast(original_type)
+        else:
+            ret = self.column.pow(other)  # type: ignore[arg-type]
+            if _is_integer_dtype(original_type) and isinstance(other, int):
+                if other < 0:
+                    raise ValueError("Cannot raise integer to negative power")
+                ret = ret.cast(original_type)
+        return PolarsColumn(ret)
 
-    def __mod__(self, other: Column[DTypeT] | Scalar) -> PolarsColumn[Any]:
+    def __mod__(self, other: Column[DType] | Any) -> PolarsColumn[Any]:
         if isinstance(other, PolarsColumn):
             return PolarsColumn(self.column % other.column)
         return PolarsColumn(self.column % other)
 
     def __divmod__(
         self,
-        other: Column[DTypeT] | Scalar,
+        other: Column[DType] | Any,
     ) -> tuple[PolarsColumn[Any], PolarsColumn[Any]]:
         quotient = self // other
         remainder = self - quotient * other
         return quotient, remainder
 
     def __and__(self, other: Column[Bool] | bool) -> PolarsColumn[Bool]:
         if isinstance(other, PolarsColumn):
@@ -191,34 +256,62 @@
         if isinstance(other, PolarsColumn):
             return PolarsColumn(self.column | other.column)
         return PolarsColumn(self.column | other)  # type: ignore[operator]
 
     def __invert__(self) -> PolarsColumn[Bool]:
         return PolarsColumn(~self.column)
 
-    def __add__(self, other: Column[Any] | Scalar) -> PolarsColumn[Any]:
+    def __add__(self, other: Column[Any] | Any) -> PolarsColumn[Any]:
         if isinstance(other, PolarsColumn):
             return PolarsColumn(self.column + other.column)
         return PolarsColumn(self.column + other)
 
-    def __sub__(self, other: Column[Any] | Scalar) -> PolarsColumn[Any]:
+    def __sub__(self, other: Column[Any] | Any) -> PolarsColumn[Any]:
         if isinstance(other, PolarsColumn):
             return PolarsColumn(self.column - other.column)
         return PolarsColumn(self.column - other)
 
     def sorted_indices(
         self, *, ascending: bool = True, nulls_position: Literal["first", "last"] = "last"
-    ) -> PolarsColumn[IntDType]:
+    ) -> PolarsColumn[Any]:
         df = self.column.to_frame()
         keys = df.columns
-        return PolarsColumn(df.with_row_count().sort(keys, descending=False)["row_nr"])
+        if ascending:
+            return PolarsColumn(
+                df.with_row_count().sort(keys, descending=False)["row_nr"]
+            )
+        return PolarsColumn(
+            df.with_row_count().sort(keys, descending=False)["row_nr"][::-1]
+        )
 
-    def fill_nan(self, value: float | null) -> PolarsColumn[DTypeT]:
+    def fill_nan(self, value: float | NullType) -> PolarsColumn[DType]:
         return PolarsColumn(self.column.fill_nan(value))  # type: ignore[arg-type]
 
+    def fill_null(self, value: Any) -> PolarsColumn[DType]:
+        return PolarsColumn(self.column.fill_null(value))
+
+    def cumulative_sum(self, *, skip_nulls: bool = True) -> PolarsColumn[DType]:
+        return PolarsColumn(self.column.cumsum())
+
+    def cumulative_prod(self, *, skip_nulls: bool = True) -> PolarsColumn[DType]:
+        return PolarsColumn(self.column.cumprod())
+
+    def cumulative_max(self, *, skip_nulls: bool = True) -> PolarsColumn[DType]:
+        return PolarsColumn(self.column.cummax())
+
+    def cumulative_min(self, *, skip_nulls: bool = True) -> PolarsColumn[DType]:
+        return PolarsColumn(self.column.cummin())
+
+    def to_array_object(self, dtype: str) -> Any:
+        if dtype not in _ARRAY_API_DTYPES:
+            raise ValueError(
+                f"Invalid dtype {dtype}. Expected one of {_ARRAY_API_DTYPES}"
+            )
+        return self.column.to_numpy().astype(dtype)
+
 
 class PolarsGroupBy(GroupBy):
     def __init__(self, df: pl.DataFrame, keys: Sequence[str]) -> None:
         for key in keys:
             if key not in df.columns:
                 raise KeyError(f"key {key} not present in DataFrame's columns")
         self.df = df
@@ -256,19 +349,23 @@
         result = self.df.groupby(self.keys).agg(pl.col("*").median())
         return PolarsDataFrame(result)
 
     def mean(self, skip_nulls: bool = True) -> PolarsDataFrame:
         result = self.df.groupby(self.keys).agg(pl.col("*").mean())
         return PolarsDataFrame(result)
 
-    def std(self, skip_nulls: bool = True) -> PolarsDataFrame:
+    def std(
+        self, correction: int | float = 1.0, skip_nulls: bool = True
+    ) -> PolarsDataFrame:
         result = self.df.groupby(self.keys).agg(pl.col("*").std())
         return PolarsDataFrame(result)
 
-    def var(self, skip_nulls: bool = True) -> PolarsDataFrame:
+    def var(
+        self, correction: int | float = 1.0, skip_nulls: bool = True
+    ) -> PolarsDataFrame:
         result = self.df.groupby(self.keys).agg(pl.col("*").var())
         return PolarsDataFrame(result)
 
 
 class PolarsDataFrame(DataFrame):
     def __init__(self, df: pl.DataFrame) -> None:
         # columns already have to be strings, and duplicates aren't
@@ -284,39 +381,35 @@
 
     def shape(self) -> tuple[int, int]:
         return self.df.shape
 
     def groupby(self, keys: Sequence[str]) -> PolarsGroupBy:
         return PolarsGroupBy(self.df, keys)
 
-    def get_column_by_name(self, name: str) -> PolarsColumn[DTypeT]:
+    def get_column_by_name(self, name: str) -> PolarsColumn[DType]:
         return PolarsColumn(self.df[name])
 
     def get_columns_by_name(self, names: Sequence[str]) -> PolarsDataFrame:
         if isinstance(names, str):
             raise TypeError(f"Expected sequence of str, got {type(names)}")
         return PolarsDataFrame(self.df.select(names))
 
-    def get_rows(self, indices: Column[IntDType]) -> PolarsDataFrame:
+    def get_rows(self, indices: Column[Any]) -> PolarsDataFrame:
         return PolarsDataFrame(self.dataframe[indices.column])
 
     def slice_rows(
         self, start: int | None, stop: int | None, step: int | None
     ) -> PolarsDataFrame:
         if start is None:
             start = 0
         if stop is None:
             stop = len(self.dataframe)
         if step is None:
             step = 1
-        return PolarsDataFrame(
-            self.df.with_row_count("idx")
-            .filter(pl.col("idx").is_in(range(start, stop, step)))
-            .drop("idx")
-        )
+        return PolarsDataFrame(self.df[start:stop:step])
 
     def get_rows_by_mask(self, mask: Column[Bool]) -> PolarsDataFrame:
         return PolarsDataFrame(self.df.filter(mask.column))
 
     def insert(self, loc: int, label: str, value: Column[Any]) -> PolarsDataFrame:
         df = self.df.clone()
         df.insert_at_idx(loc, pl.Series(label, value.column))
@@ -333,102 +426,142 @@
         return PolarsDataFrame(self.dataframe.rename(dict(mapping)))
 
     def get_column_names(self) -> Sequence[str]:
         return self.dataframe.columns
 
     def __eq__(  # type: ignore[override]
         self,
-        other: DataFrame | Scalar,
+        other: DataFrame | Any,
     ) -> PolarsDataFrame:
         if isinstance(other, PolarsDataFrame):
             return PolarsDataFrame(self.dataframe.__eq__(other.dataframe))
         return PolarsDataFrame(self.dataframe.__eq__(other))
 
     def __ne__(  # type: ignore[override]
         self,
         other: DataFrame,
     ) -> PolarsDataFrame:
         if isinstance(other, PolarsDataFrame):
             return PolarsDataFrame(self.dataframe.__ne__(other.dataframe))
         return PolarsDataFrame(self.dataframe.__ne__(other))
 
-    def __ge__(self, other: DataFrame | Scalar) -> PolarsDataFrame:
+    def __ge__(self, other: DataFrame | Any) -> PolarsDataFrame:
         if isinstance(other, PolarsDataFrame):
             return PolarsDataFrame(self.dataframe.__ge__(other.dataframe))
         return PolarsDataFrame(self.dataframe.__ge__(other))
 
-    def __gt__(self, other: DataFrame | Scalar) -> PolarsDataFrame:
+    def __gt__(self, other: DataFrame | Any) -> PolarsDataFrame:
         if isinstance(other, PolarsDataFrame):
             return PolarsDataFrame(self.dataframe.__gt__(other.dataframe))
         return PolarsDataFrame(self.dataframe.__gt__(other))
 
-    def __le__(self, other: DataFrame | Scalar) -> PolarsDataFrame:
+    def __le__(self, other: DataFrame | Any) -> PolarsDataFrame:
         if isinstance(other, PolarsDataFrame):
             return PolarsDataFrame(self.dataframe.__le__(other.dataframe))
         return PolarsDataFrame(self.dataframe.__le__(other))
 
-    def __lt__(self, other: DataFrame | Scalar) -> PolarsDataFrame:
+    def __lt__(self, other: DataFrame | Any) -> PolarsDataFrame:
         if isinstance(other, PolarsDataFrame):
             return PolarsDataFrame(self.dataframe.__lt__(other.dataframe))
         return PolarsDataFrame(self.dataframe.__lt__(other))
 
-    def __add__(self, other: DataFrame | Scalar) -> PolarsDataFrame:
+    def __and__(self, other: DataFrame | Any) -> PolarsDataFrame:
+        if isinstance(other, PolarsDataFrame):
+            return PolarsDataFrame(
+                self.dataframe.with_columns(
+                    self.dataframe[col] & other.dataframe[col]
+                    for col in self.dataframe.columns
+                )
+            )
+        return PolarsDataFrame(
+            self.dataframe.with_columns(
+                self.dataframe[col] & other  # type: ignore[operator]
+                for col in self.dataframe.columns
+            )
+        )
+
+    def __or__(self, other: DataFrame | Any) -> PolarsDataFrame:
+        if isinstance(other, PolarsDataFrame):
+            return PolarsDataFrame(
+                self.dataframe.with_columns(
+                    self.dataframe[col] | other.dataframe[col]
+                    for col in self.dataframe.columns
+                )
+            )
+        return PolarsDataFrame(
+            self.dataframe.with_columns(
+                self.dataframe[col] | other  # type: ignore[operator]
+                for col in self.dataframe.columns
+            )
+        )
+
+    def __add__(self, other: DataFrame | Any) -> PolarsDataFrame:
         if isinstance(other, PolarsDataFrame):
             return PolarsDataFrame(self.dataframe.__add__(other.dataframe))
         return PolarsDataFrame(self.dataframe.__add__(other))  # type: ignore[operator]
 
-    def __sub__(self, other: DataFrame | Scalar) -> PolarsDataFrame:
+    def __sub__(self, other: DataFrame | Any) -> PolarsDataFrame:
         if isinstance(other, PolarsDataFrame):
             return PolarsDataFrame(self.dataframe.__sub__(other.dataframe))
         return PolarsDataFrame(self.dataframe.__sub__(other))  # type: ignore[operator]
 
-    def __mul__(self, other: DataFrame | Scalar) -> PolarsDataFrame:
+    def __mul__(self, other: DataFrame | Any) -> PolarsDataFrame:
         if isinstance(other, PolarsDataFrame):
             return PolarsDataFrame(self.dataframe.__mul__(other.dataframe))
         return PolarsDataFrame(self.dataframe.__mul__(other))  # type: ignore[operator]
 
-    def __truediv__(self, other: DataFrame | Scalar) -> PolarsDataFrame:
+    def __truediv__(self, other: DataFrame | Any) -> PolarsDataFrame:
         if isinstance(other, PolarsDataFrame):
             return PolarsDataFrame(self.dataframe.__truediv__(other.dataframe))
         return PolarsDataFrame(
             self.dataframe.__truediv__(other)  # type: ignore[operator]
         )
 
-    def __floordiv__(self, other: DataFrame | Scalar) -> PolarsDataFrame:
+    def __floordiv__(self, other: DataFrame | Any) -> PolarsDataFrame:
         if isinstance(other, PolarsDataFrame):
             return PolarsDataFrame(self.dataframe.__floordiv__(other.dataframe))
         return PolarsDataFrame(
             self.dataframe.__floordiv__(other)  # type: ignore[operator]
         )
 
-    def __pow__(self, other: DataFrame | Scalar) -> PolarsDataFrame:
+    def __pow__(self, other: DataFrame | Any) -> PolarsDataFrame:
+        original_type = self.dataframe.schema
         if isinstance(other, PolarsDataFrame):
-            return PolarsDataFrame(
-                self.dataframe.select(
-                    [
-                        pl.col(col).pow(other.dataframe[col])
-                        for col in self.get_column_names()
-                    ]
-                )
+            ret = self.dataframe.select(
+                [pl.col(col).pow(other.dataframe[col]) for col in self.get_column_names()]
             )
-        return PolarsDataFrame(
-            self.dataframe.select(
-                pl.col(col).pow(other)  # type: ignore[arg-type]
-                for col in self.get_column_names()
+            for column in self.dataframe.columns:
+                if _is_integer_dtype(original_type[column]) and _is_integer_dtype(
+                    other.dataframe[column].dtype
+                ):
+                    if (other.dataframe[column] < 0).any():
+                        raise ValueError("Cannot raise integer to negative power")
+                    ret = ret.with_columns(pl.col(column).cast(original_type[column]))
+        else:
+            ret = self.dataframe.select(
+                [
+                    pl.col(col).pow(other)  # type: ignore[arg-type]
+                    for col in self.get_column_names()
+                ]
             )
-        )
+            for column in self.dataframe.columns:
+                if _is_integer_dtype(original_type[column]) and isinstance(other, int):
+                    if other < 0:
+                        raise ValueError("Cannot raise integer to negative power")
+                    ret = ret.with_columns(pl.col(column).cast(original_type[column]))
+        return PolarsDataFrame(ret)
 
-    def __mod__(self, other: DataFrame | Scalar) -> PolarsDataFrame:
+    def __mod__(self, other: DataFrame | Any) -> PolarsDataFrame:
         if isinstance(other, PolarsDataFrame):
             return PolarsDataFrame(self.dataframe.__mod__(other.dataframe))
         return PolarsDataFrame(self.dataframe.__mod__(other))  # type: ignore[operator]
 
     def __divmod__(
         self,
-        other: DataFrame | Scalar,
+        other: DataFrame | Any,
     ) -> tuple[PolarsDataFrame, PolarsDataFrame]:
         quotient = self // other
         remainder = self - quotient * other
         return quotient, remainder
 
     def __invert__(self) -> PolarsDataFrame:
         return PolarsDataFrame(self.dataframe.select(~pl.col("*")))
@@ -451,18 +584,18 @@
     def any(self, *, skip_nulls: bool = True) -> PolarsDataFrame:
         return PolarsDataFrame(self.dataframe.select(pl.col("*").any()))
 
     def all(self, *, skip_nulls: bool = True) -> PolarsDataFrame:
         return PolarsDataFrame(self.dataframe.select(pl.col("*").all()))
 
     def any_rowwise(self, *, skip_nulls: bool = True) -> PolarsColumn[Bool]:
-        return PolarsColumn(self.dataframe.select(pl.any(pl.col("*")))["any"])
+        return PolarsColumn(self.dataframe.select(pl.any_horizontal(pl.col("*")))["any"])
 
     def all_rowwise(self, *, skip_nulls: bool = True) -> PolarsColumn[Bool]:
-        return PolarsColumn(self.dataframe.select(pl.all(pl.col("*")))["all"])
+        return PolarsColumn(self.dataframe.select(pl.all_horizontal(pl.col("*")))["all"])
 
     def min(self, *, skip_nulls: bool = True) -> PolarsDataFrame:
         return PolarsDataFrame(self.dataframe.select(pl.col("*").min()))
 
     def max(self, *, skip_nulls: bool = True) -> PolarsDataFrame:
         return PolarsDataFrame(self.dataframe.select(pl.col("*").max()))
 
@@ -474,28 +607,68 @@
 
     def mean(self, *, skip_nulls: bool = True) -> PolarsDataFrame:
         return PolarsDataFrame(self.dataframe.select(pl.col("*").mean()))
 
     def median(self, *, skip_nulls: bool = True) -> PolarsDataFrame:
         return PolarsDataFrame(self.dataframe.select(pl.col("*").median()))
 
-    def std(self, *, skip_nulls: bool = True) -> PolarsDataFrame:
+    def std(
+        self, *, correction: int | float = 1.0, skip_nulls: bool = True
+    ) -> PolarsDataFrame:
         return PolarsDataFrame(self.dataframe.select(pl.col("*").std()))
 
-    def var(self, *, skip_nulls: bool = True) -> PolarsDataFrame:
+    def var(
+        self, *, correction: int | float = 1.0, skip_nulls: bool = True
+    ) -> PolarsDataFrame:
         return PolarsDataFrame(self.dataframe.select(pl.col("*").var()))
 
     def sorted_indices(
         self,
-        keys: Sequence[Any],
+        keys: Sequence[Any] | None = None,
         *,
         ascending: Sequence[bool] | bool = True,
         nulls_position: Literal["first", "last"] = "last",
-    ) -> PolarsColumn[IntDType]:
+    ) -> PolarsColumn[Any]:
+        if keys is None:
+            keys = self.dataframe.columns
         df = self.dataframe.select(keys)
-        return PolarsColumn(df.with_row_count().sort(keys, descending=False)["row_nr"])
+        if ascending:
+            return PolarsColumn(
+                df.with_row_count().sort(keys, descending=False)["row_nr"]
+            )
+        return PolarsColumn(
+            df.with_row_count().sort(keys, descending=False)["row_nr"][::-1]
+        )
+
+    def unique_indices(
+        self, keys: Sequence[str] | None = None, *, skip_nulls: bool = True
+    ) -> PolarsColumn[Any]:
+        df = self.dataframe
+        if keys is None:
+            keys = df.columns
+        return PolarsColumn(df.with_row_count().unique(keys)["row_nr"])
 
     def fill_nan(
         self,
-        value: float | null,
+        value: float | NullType,
     ) -> PolarsDataFrame:
         return PolarsDataFrame(self.dataframe.fill_nan(value))  # type: ignore[arg-type]
+
+    def fill_null(
+        self,
+        value: Any,
+        *,
+        column_names: list[str] | None = None,
+    ) -> PolarsDataFrame:
+        if column_names is None:
+            column_names = self.dataframe.columns
+        df = self.dataframe.with_columns(
+            pl.col(col).fill_null(value) for col in column_names
+        )
+        return PolarsDataFrame(df)
+
+    def to_array_object(self, dtype: str) -> Any:
+        if dtype not in _ARRAY_API_DTYPES:
+            raise ValueError(
+                f"Invalid dtype {dtype}. Expected one of {_ARRAY_API_DTYPES}"
+            )
+        return self.dataframe.to_numpy().astype(dtype)
```

### Comparing `dataframe_api_compat-0.1.0/setup.cfg` & `dataframe_api_compat-0.1.1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [metadata]
 name = dataframe_api_compat
-version = 0.1.0
-description = Draft implementation of the DataFrame Standard for pandas and polars
+version = 0.1.1
+description = Implementation of the DataFrame Standard for pandas and polars
 long_description = file: README.md
 long_description_content_type = text/markdown
-url = https://github.com/MarcoGorelli/dataframe-api-compat
+url = https://github.com/data-apis/dataframe-api-compat
 author = Marco Gorelli
 license = MIT
 license_files = LICENSE
 classifiers = 
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 
 [options]
 packages = find:
-py_modules = nbqa
+py_modules = dataframe_api_compat
 python_requires = >=3.8
 
 [options.packages.find]
 exclude = 
 	tests*
 	testing*
```

