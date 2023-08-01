# Comparing `tmp/mlforecast-0.8.1.tar.gz` & `tmp/mlforecast-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlforecast-0.8.1.tar", last modified: Fri Jul 21 02:46:31 2023, max compression
+gzip compressed data, was "mlforecast-0.9.0.tar", last modified: Tue Aug  1 03:06:06 2023, max compression
```

## Comparing `mlforecast-0.8.1.tar` & `mlforecast-0.9.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:46:31.589855 mlforecast-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-07-21 02:46:18.000000 mlforecast-0.8.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11336 2023-07-21 02:46:18.000000 mlforecast-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-21 02:46:18.000000 mlforecast-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12470 2023-07-21 02:46:31.589855 mlforecast-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11575 2023-07-21 02:46:18.000000 mlforecast-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:46:31.585855 mlforecast-0.8.1/mlforecast/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-21 02:46:18.000000 mlforecast-0.8.1/mlforecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30980 2023-07-21 02:46:18.000000 mlforecast-0.8.1/mlforecast/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (123)    23264 2023-07-21 02:46:18.000000 mlforecast-0.8.1/mlforecast/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:46:31.585855 mlforecast-0.8.1/mlforecast/distributed/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-21 02:46:18.000000 mlforecast-0.8.1/mlforecast/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25805 2023-07-21 02:46:18.000000 mlforecast-0.8.1/mlforecast/distributed/forecast.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:46:31.585855 mlforecast-0.8.1/mlforecast/distributed/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 02:46:18.000000 mlforecast-0.8.1/mlforecast/distributed/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:46:31.589855 mlforecast-0.8.1/mlforecast/distributed/models/dask/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 02:46:18.000000 mlforecast-0.8.1/mlforecast/distributed/models/dask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-21 02:46:18.000000 mlforecast-0.8.1/mlforecast/distributed/models/dask/lgb.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-21 02:46:18.000000 mlforecast-0.8.1/mlforecast/distributed/models/dask/xgb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:46:31.589855 mlforecast-0.8.1/mlforecast/distributed/models/ray/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 02:46:18.000000 mlforecast-0.8.1/mlforecast/distributed/models/ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-21 02:46:18.000000 mlforecast-0.8.1/mlforecast/distributed/models/ray/lgb.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-21 02:46:18.000000 mlforecast-0.8.1/mlforecast/distributed/models/ray/xgb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:46:31.589855 mlforecast-0.8.1/mlforecast/distributed/models/spark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 02:46:18.000000 mlforecast-0.8.1/mlforecast/distributed/models/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-21 02:46:18.000000 mlforecast-0.8.1/mlforecast/distributed/models/spark/lgb.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-21 02:46:18.000000 mlforecast-0.8.1/mlforecast/distributed/models/spark/xgb.py
--rw-r--r--   0 runner    (1001) docker     (123)    29454 2023-07-21 02:46:18.000000 mlforecast-0.8.1/mlforecast/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)     7357 2023-07-21 02:46:18.000000 mlforecast-0.8.1/mlforecast/grouped_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    22365 2023-07-21 02:46:18.000000 mlforecast-0.8.1/mlforecast/lgb_cv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-21 02:46:18.000000 mlforecast-0.8.1/mlforecast/target_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-07-21 02:46:18.000000 mlforecast-0.8.1/mlforecast/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:46:31.585855 mlforecast-0.8.1/mlforecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12470 2023-07-21 02:46:31.000000 mlforecast-0.8.1/mlforecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-21 02:46:31.000000 mlforecast-0.8.1/mlforecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 02:46:31.000000 mlforecast-0.8.1/mlforecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 02:46:31.000000 mlforecast-0.8.1/mlforecast.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-21 02:46:31.000000 mlforecast-0.8.1/mlforecast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-21 02:46:31.000000 mlforecast-0.8.1/mlforecast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-21 02:46:18.000000 mlforecast-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-21 02:46:18.000000 mlforecast-0.8.1/settings.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 02:46:31.589855 mlforecast-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-21 02:46:18.000000 mlforecast-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:06:06.455897 mlforecast-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-08-01 03:05:53.000000 mlforecast-0.9.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11336 2023-08-01 03:05:53.000000 mlforecast-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-01 03:05:53.000000 mlforecast-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12470 2023-08-01 03:06:06.455897 mlforecast-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11575 2023-08-01 03:05:53.000000 mlforecast-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:06:06.451897 mlforecast-0.9.0/mlforecast/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-01 03:05:53.000000 mlforecast-0.9.0/mlforecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30980 2023-08-01 03:05:53.000000 mlforecast-0.9.0/mlforecast/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24526 2023-08-01 03:05:53.000000 mlforecast-0.9.0/mlforecast/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:06:06.451897 mlforecast-0.9.0/mlforecast/distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-01 03:05:53.000000 mlforecast-0.9.0/mlforecast/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25805 2023-08-01 03:05:53.000000 mlforecast-0.9.0/mlforecast/distributed/forecast.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:06:06.451897 mlforecast-0.9.0/mlforecast/distributed/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 03:05:53.000000 mlforecast-0.9.0/mlforecast/distributed/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:06:06.451897 mlforecast-0.9.0/mlforecast/distributed/models/dask/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 03:05:53.000000 mlforecast-0.9.0/mlforecast/distributed/models/dask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-08-01 03:05:53.000000 mlforecast-0.9.0/mlforecast/distributed/models/dask/lgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-01 03:05:53.000000 mlforecast-0.9.0/mlforecast/distributed/models/dask/xgb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:06:06.455897 mlforecast-0.9.0/mlforecast/distributed/models/ray/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 03:05:53.000000 mlforecast-0.9.0/mlforecast/distributed/models/ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-01 03:05:53.000000 mlforecast-0.9.0/mlforecast/distributed/models/ray/lgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-08-01 03:05:53.000000 mlforecast-0.9.0/mlforecast/distributed/models/ray/xgb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:06:06.455897 mlforecast-0.9.0/mlforecast/distributed/models/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 03:05:53.000000 mlforecast-0.9.0/mlforecast/distributed/models/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-01 03:05:53.000000 mlforecast-0.9.0/mlforecast/distributed/models/spark/lgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-08-01 03:05:53.000000 mlforecast-0.9.0/mlforecast/distributed/models/spark/xgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29946 2023-08-01 03:05:53.000000 mlforecast-0.9.0/mlforecast/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-08-01 03:05:53.000000 mlforecast-0.9.0/mlforecast/grouped_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22522 2023-08-01 03:05:53.000000 mlforecast-0.9.0/mlforecast/lgb_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-08-01 03:05:53.000000 mlforecast-0.9.0/mlforecast/target_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-08-01 03:05:53.000000 mlforecast-0.9.0/mlforecast/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:06:06.451897 mlforecast-0.9.0/mlforecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12470 2023-08-01 03:06:06.000000 mlforecast-0.9.0/mlforecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-08-01 03:06:06.000000 mlforecast-0.9.0/mlforecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 03:06:06.000000 mlforecast-0.9.0/mlforecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 03:06:06.000000 mlforecast-0.9.0/mlforecast.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-08-01 03:06:06.000000 mlforecast-0.9.0/mlforecast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-01 03:06:06.000000 mlforecast-0.9.0/mlforecast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-01 03:05:53.000000 mlforecast-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-08-01 03:05:53.000000 mlforecast-0.9.0/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 03:06:06.455897 mlforecast-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-08-01 03:05:53.000000 mlforecast-0.9.0/setup.py
```

### Comparing `mlforecast-0.8.1/CONTRIBUTING.md` & `mlforecast-0.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mlforecast-0.8.1/LICENSE` & `mlforecast-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mlforecast-0.8.1/PKG-INFO` & `mlforecast-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlforecast
-Version: 0.8.1
+Version: 0.9.0
 Summary: Scalable machine learning based time series forecasting
 Home-page: https://github.com/Nixtla/mlforecast
 Author: José Morales
 Author-email: jmoralz92@gmail.com
 License: Apache Software License 2.0
 Keywords: python forecast forecasting machine-learning dask
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mlforecast-0.8.1/README.md` & `mlforecast-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `mlforecast-0.8.1/mlforecast/_modidx.py` & `mlforecast-0.9.0/mlforecast/_modidx.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.8.1/mlforecast/core.py` & `mlforecast-0.9.0/mlforecast/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -219,44 +219,38 @@
                 self.freq = 1
         else:
             raise ValueError(f"{time_col} must be either timestamp or integer.")
         self.id_col = id_col
         self.target_col = target_col
         self.time_col = time_col
         self.keep_last_n = keep_last_n
-        to_drop = [id_col, time_col, target_col]
         self.static_features = static_features
-        if static_features is None:
-            static_features = df.columns.drop([time_col, target_col]).tolist()
-        elif id_col not in static_features:
-            static_features = [id_col] + static_features
-        else:  # static_features defined and contain id_col
-            to_drop = [time_col, target_col]
-        self.static_features_ = (
-            df[static_features]
-            .groupby(id_col, observed=True)
-            .head(1)
-            .sort_values(id_col)
-            .reset_index(drop=True)
-        )
         sort_idxs = pd.core.sorting.lexsort_indexer([df[id_col], df[time_col]])
         self.restore_idxs = np.empty(df.shape[0], dtype=np.int32)
         self.restore_idxs[sort_idxs] = np.arange(df.shape[0])
         sorted_df = df[[id_col, time_col, target_col]].iloc[sort_idxs]
         if self.target_transforms is not None:
             for tfm in self.target_transforms:
                 tfm.set_column_names(id_col, time_col, target_col)
                 sorted_df = tfm.fit_transform(sorted_df)
-        sorted_df = sorted_df.set_index([id_col, time_col])
-        self.uids = sorted_df.index.unique(level=0)
         self.ga = GroupedArray.from_sorted_df(sorted_df, id_col, target_col)
         self._ga = GroupedArray(self.ga.data, self.ga.indptr)
-        self.last_dates = sorted_df.index.get_level_values(self.time_col)[
-            self.ga.indptr[1:] - 1
-        ]
+        last_idxs_per_serie = self.ga.indptr[1:] - 1
+        self.uids = pd.Index(sorted_df[id_col].iloc[last_idxs_per_serie])
+        self.last_dates = pd.Index(sorted_df[time_col].iloc[last_idxs_per_serie])
+        to_drop = [id_col, time_col, target_col]
+        if static_features is None:
+            static_features = df.columns.drop([time_col, target_col]).tolist()
+        elif id_col not in static_features:
+            static_features = [id_col] + static_features
+        else:  # static_features defined and contain id_col
+            to_drop = [time_col, target_col]
+        self.static_features_ = df.iloc[sort_idxs[last_idxs_per_serie]][
+            static_features
+        ].reset_index(drop=True)
         self.features_order_ = df.columns.drop(to_drop).tolist() + self.features
         return self
 
     def _apply_transforms(self, updates_only: bool = False) -> Dict[str, np.ndarray]:
         """Apply the transformations using the main process.
 
         If `updates_only` then only the updates are returned.
@@ -323,66 +317,64 @@
         dropna: bool = True,
         max_horizon: Optional[int] = None,
         return_X_y: bool = False,
     ) -> pd.DataFrame:
         """Add the features to `df`.
 
         if `dropna=True` then all the null rows are dropped."""
-        modifies_target = bool(self.target_transforms)
-        df = df.copy(deep=modifies_target and not return_X_y)
-        self.features_ = self._compute_transforms()
-
-        # lag transforms
-        for feat in self.transforms.keys():
-            df[feat] = self.features_[feat][self.restore_idxs]
-
-        # date features
-        dates = df[self.time_col]
-        if not np.issubdtype(dates.dtype.type, np.integer):
-            dates = pd.DatetimeIndex(dates)
-        for feature in self.date_features:
-            feat_name, feat_vals = self._compute_date_feature(dates, feature)
-            df[feat_name] = feat_vals
+        features = {
+            k: v[self.restore_idxs] for k, v in self._compute_transforms().items()
+        }
 
         # target
         self.max_horizon = max_horizon
         if max_horizon is None:
-            if modifies_target:
-                target = pd.Series(self.ga.data[self.restore_idxs], index=df.index)
-            else:
-                target = df[self.target_col]
+            target = self.ga.data[self.restore_idxs]
         else:
-            target = pd.DataFrame(
-                self.ga.expand_target(max_horizon)[self.restore_idxs],
-                index=df.index,
-                columns=[f"{self.target_col}{i}" for i in range(max_horizon)],
-            )
+            target = self.ga.expand_target(max_horizon)[self.restore_idxs]
 
         # determine rows to keep
         if dropna:
-            feature_nulls = df[self.features].isnull().any(axis=1)
-            target_nulls = target.isnull()
+            feature_nulls = np.full(df.shape[0], False)
+            for feature_vals in features.values():
+                feature_nulls |= np.isnan(feature_vals)
+            target_nulls = np.isnan(target)
             if target_nulls.ndim == 2:
                 # target nulls for each horizon are dropped in MLForecast.fit_models
                 # we just drop rows here for which all the target values are null
                 target_nulls = target_nulls.all(axis=1)
-            keep_rows = ~(feature_nulls | target_nulls).values
+            keep_rows = ~(feature_nulls | target_nulls)
+            df = df[keep_rows].copy(deep=False)
+            target = target[keep_rows]
         else:
             keep_rows = np.full(df.shape[0], True)
+            df = df.copy(deep=False)
+
+        # lag transforms
+        for feat in self.transforms.keys():
+            df[feat] = features[feat][keep_rows]
+
+        # date features
+        if self.date_features:
+            dates = df[self.time_col]
+            if not np.issubdtype(dates.dtype.type, np.integer):
+                dates = pd.DatetimeIndex(dates)
+            for feature in self.date_features:
+                feat_name, feat_vals = self._compute_date_feature(dates, feature)
+                df[feat_name] = feat_vals
 
         # assemble return
-        xs = df.columns.drop(self.target_col)
         if return_X_y:
-            return df.loc[keep_rows, xs], target.loc[keep_rows]
-        if max_horizon is None:
-            if modifies_target:
-                df[self.target_col] = target
+            return df, target
+        if max_horizon is not None:
+            for i in range(max_horizon):
+                df[f"{self.target_col}{i}"] = target[:, i]
         else:
-            df = pd.concat([df[xs], target], axis=1)
-        return df.loc[keep_rows]
+            df[self.target_col] = target
+        return df
 
     def fit_transform(
         self,
         data: pd.DataFrame,
         id_col: str,
         time_col: str,
         target_col: str,
@@ -458,41 +450,48 @@
     def _predict_setup(self) -> None:
         self.curr_dates = self.last_dates.copy()
         self.test_dates = []
         self.y_pred = []
         self.ga = GroupedArray(self._ga.data, self._ga.indptr)
         if self.keep_last_n is not None:
             self.ga = self.ga.take_from_groups(slice(-self.keep_last_n, None))
+        self._h = 0
 
-    def _get_features_for_next_step(self, dynamic_dfs):
+    def _get_features_for_next_step(self, dynamic_dfs, X_df=None):
         new_x = self._update_features()
         if dynamic_dfs:
             for df in dynamic_dfs:
                 new_x = new_x.merge(df, how="left")
             new_x = new_x.sort_values(self.id_col)
+        if X_df is not None:
+            n_series = self.uids.size
+            X = X_df.iloc[self._h * n_series : (self._h + 1) * n_series]
+            new_x = pd.concat([new_x, X.reset_index(drop=True)], axis=1)
         nulls = new_x.isnull().any()
         if any(nulls):
             warnings.warn(f'Found null values in {", ".join(nulls[nulls].index)}.')
+        self._h += 1
         return new_x[self.features_order_]
 
     def _predict_recursive(
         self,
         models: Dict[str, BaseEstimator],
         horizon: int,
         dynamic_dfs: Optional[List[pd.DataFrame]] = None,
         before_predict_callback: Optional[Callable] = None,
         after_predict_callback: Optional[Callable] = None,
+        X_df: Optional[pd.DataFrame] = None,
     ) -> pd.DataFrame:
         """Use `model` to predict the next `horizon` timesteps."""
         if dynamic_dfs is None:
             dynamic_dfs = []
         for i, (name, model) in enumerate(models.items()):
             self._predict_setup()
             for _ in range(horizon):
-                new_x = self._get_features_for_next_step(dynamic_dfs)
+                new_x = self._get_features_for_next_step(dynamic_dfs, X_df)
                 if before_predict_callback is not None:
                     new_x = before_predict_callback(new_x)
                 predictions = model.predict(new_x)
                 if after_predict_callback is not None:
                     predictions_serie = pd.Series(predictions, index=self.uids)
                     predictions = after_predict_callback(predictions_serie).values
                 self._update_y(predictions)
@@ -507,14 +506,15 @@
 
     def _predict_multi(
         self,
         models: Dict[str, BaseEstimator],
         horizon: int,
         dynamic_dfs: Optional[List[pd.DataFrame]] = None,
         before_predict_callback: Optional[Callable] = None,
+        X_df: Optional[pd.DataFrame] = None,
     ) -> pd.DataFrame:
         assert self.max_horizon is not None
         if horizon > self.max_horizon:
             raise ValueError(
                 f"horizon must be at most max_horizon ({self.max_horizon})"
             )
         if dynamic_dfs is None:
@@ -526,15 +526,15 @@
                 for date in self.last_dates
                 for i in range(horizon)
             ]
         )
         result = pd.DataFrame({self.id_col: uids, self.time_col: dates})
         for name, model in models.items():
             self._predict_setup()
-            new_x = self._get_features_for_next_step(dynamic_dfs)
+            new_x = self._get_features_for_next_step(dynamic_dfs, X_df)
             if before_predict_callback is not None:
                 new_x = before_predict_callback(new_x)
             predictions = np.empty((new_x.shape[0], horizon))
             for i in range(horizon):
                 predictions[:, i] = model[i].predict(new_x)
             raw_preds = predictions.ravel()
             result[name] = raw_preds
@@ -543,29 +543,54 @@
     def predict(
         self,
         models: Dict[str, Union[BaseEstimator, List[BaseEstimator]]],
         horizon: int,
         dynamic_dfs: Optional[List[pd.DataFrame]] = None,
         before_predict_callback: Optional[Callable] = None,
         after_predict_callback: Optional[Callable] = None,
+        X_df: Optional[pd.DataFrame] = None,
     ) -> pd.DataFrame:
+        if X_df is not None:
+            if self.id_col not in X_df or self.time_col not in X_df:
+                raise ValueError(
+                    f"X_df must have '{self.id_col}' and '{self.time_col}' columns."
+                )
+            dates_validation = pd.DataFrame(
+                {
+                    self.id_col: self.uids,
+                    "_start": self.last_dates + self.freq,
+                    "_end": self.last_dates + horizon * self.freq,
+                }
+            )
+            X_df = X_df.merge(dates_validation, on=[self.id_col])
+            X_df = X_df[X_df[self.time_col].between(X_df["_start"], X_df["_end"])]
+            if X_df.shape[0] != self.uids.size * horizon:
+                raise ValueError(
+                    "Found missing inputs in X_df. "
+                    "It should have one row per id and date for the complete forecasting horizon"
+                )
+            X_df = X_df.sort_values([self.id_col, self.time_col]).drop(
+                columns=[self.id_col, self.time_col, "_start", "_end"]
+            )
         if getattr(self, "max_horizon", None) is None:
             preds = self._predict_recursive(
                 models,
                 horizon,
                 dynamic_dfs,
                 before_predict_callback,
                 after_predict_callback,
+                X_df,
             )
         else:
             preds = self._predict_multi(
                 models,
                 horizon,
                 dynamic_dfs,
                 before_predict_callback,
+                X_df,
             )
         if self.target_transforms is not None:
             for tfm in self.target_transforms[::-1]:
                 preds = tfm.inverse_transform(preds)
         return preds
 
     def update(self, df: pd.DataFrame) -> None:
```

### Comparing `mlforecast-0.8.1/mlforecast/distributed/forecast.py` & `mlforecast-0.9.0/mlforecast/distributed/forecast.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.8.1/mlforecast/distributed/models/dask/lgb.py` & `mlforecast-0.9.0/mlforecast/distributed/models/dask/lgb.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.8.1/mlforecast/distributed/models/dask/xgb.py` & `mlforecast-0.9.0/mlforecast/distributed/models/dask/xgb.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.8.1/mlforecast/distributed/models/ray/xgb.py` & `mlforecast-0.9.0/mlforecast/distributed/models/ray/xgb.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.8.1/mlforecast/distributed/models/spark/lgb.py` & `mlforecast-0.9.0/mlforecast/distributed/models/spark/lgb.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.8.1/mlforecast/distributed/models/spark/xgb.py` & `mlforecast-0.9.0/mlforecast/distributed/models/spark/xgb.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.8.1/mlforecast/forecast.py` & `mlforecast-0.9.0/mlforecast/forecast.py`

 * *Files 1% similar despite different names*

```diff
@@ -269,18 +269,18 @@
         self : MLForecast
             Forecast object with trained models.
         """
         self.models_: Dict[str, Union[BaseEstimator, List[BaseEstimator]]] = {}
         for name, model in self.models.items():
             if y.ndim == 2 and y.shape[1] > 1:
                 self.models_[name] = []
-                for col in y:
-                    keep = y[col].notnull()
+                for col in range(y.shape[1]):
+                    keep = ~np.isnan(y[:, col])
                     self.models_[name].append(
-                        clone(model).fit(X.loc[keep], y.loc[keep, col])
+                        clone(model).fit(X.loc[keep], y[keep, col])
                     )
             else:
                 self.models_[name] = clone(model).fit(X, y)
         return self
 
     def _conformity_scores(
         self,
@@ -403,14 +403,15 @@
         self,
         h: int,
         dynamic_dfs: Optional[List[pd.DataFrame]] = None,
         before_predict_callback: Optional[Callable] = None,
         after_predict_callback: Optional[Callable] = None,
         new_df: Optional[pd.DataFrame] = None,
         level: Optional[List[Union[int, float]]] = None,
+        X_df: Optional[pd.DataFrame] = None,
         *,
         horizon: Optional[int] = None,  # noqa: ARG002
         new_data: Optional[pd.DataFrame] = None,  # noqa: ARG002
     ) -> pd.DataFrame:
         """Compute the predictions for the next `horizon` steps.
 
         Parameters
@@ -429,14 +430,16 @@
                 The series identifier is on the index.
         new_df : pandas DataFrame, optional (default=None)
             Series data of new observations for which forecasts are to be generated.
                 This dataframe should have the same structure as the one used to fit the model, including any features and time series data.
                 If `new_df` is not None, the method will generate forecasts for the new observations.
         level : list of ints or floats, optional (default=None)
             Confidence levels between 0 and 100 for prediction intervals.
+        X_df : pandas DataFrame, optional (default=None)
+            Dataframe with the future exogenous features. Should have the id column and the time column.
         horizon : int
             Number of periods to predict. This argument has been replaced by h and will be removed in a later release.
         new_data : pandas DataFrame, optional (default=None)
             Series data of new observations for which forecasts are to be generated.
                 This dataframe should have the same structure as the one used to fit the model, including any features and time series data.
                 If `new_data` is not None, the method will generate forecasts for the new observations.
 
@@ -451,14 +454,19 @@
             )
         if new_data is not None:
             warnings.warn(
                 "`new_data` has been deprecated, please use `new_df` instead.",
                 DeprecationWarning,
             )
             new_df = new_data
+        if dynamic_dfs is not None:
+            warnings.warn(
+                "`dynamic_dfs` has been deprecated, please use `X_df` instead",
+                DeprecationWarning,
+            )
 
         if new_df is not None:
             new_ts = TimeSeries(
                 freq=self.ts.freq,
                 lags=self.ts.lags,
                 lag_transforms=self.ts.lag_transforms,
                 date_features=self.ts.date_features,
@@ -480,14 +488,15 @@
 
         forecasts = ts.predict(
             self.models_,
             h,
             dynamic_dfs,
             before_predict_callback,
             after_predict_callback,
+            X_df,
         )
         if level is not None:
             if self._cs_df is None:
                 warn_msg = (
                     "Please rerun the `fit` method passing a proper value "
                     "to prediction intervals to compute them."
                 )
@@ -626,18 +635,14 @@
             h=h,
             id_col=id_col,
             time_col=time_col,
             freq=freq,
             step_size=step_size,
             input_size=input_size,
         )
-        ex_cols_to_drop = [id_col, time_col, target_col]
-        if static_features is not None:
-            ex_cols_to_drop.extend(static_features)
-        has_ex = not df.columns.drop(ex_cols_to_drop).empty
         self.cv_fitted_values_ = []
         for i_window, (cutoffs, train, valid) in enumerate(splits):
             if refit or i_window == 0:
                 self.fit(
                     train,
                     id_col=id_col,
                     time_col=time_col,
@@ -667,22 +672,27 @@
                     insample_results[name] = model.predict(trainX)  # type: ignore[union-attr]
                 if self.ts.target_transforms is not None:
                     for tfm in self.ts.target_transforms[::-1]:
                         insample_results = tfm.inverse_transform(insample_results)
                 insample_results["fold"] = i_window
                 insample_results[target_col] = train[target_col].values
                 self.cv_fitted_values_.append(insample_results)
-            dynamic_dfs = [valid.drop(columns=[target_col])] if has_ex else None
+            static = self.ts.static_features_.columns.drop(id_col).tolist()
+            dynamic = valid.columns.drop(static + [id_col, time_col, target_col])
+            if not dynamic.empty:
+                X_df = valid.drop(columns=static + [target_col])
+            else:
+                X_df = None
             y_pred = self.predict(
                 h,
-                dynamic_dfs,
-                before_predict_callback,
-                after_predict_callback,
+                before_predict_callback=before_predict_callback,
+                after_predict_callback=after_predict_callback,
                 new_df=train if not refit else None,
                 level=level,
+                X_df=X_df,
             )
             y_pred = y_pred.merge(cutoffs, on=id_col, how="left")
             result = valid[[id_col, time_col, target_col]].merge(
                 y_pred, on=[id_col, time_col]
             )
             if result.shape[0] < valid.shape[0]:
                 raise ValueError(
```

### Comparing `mlforecast-0.8.1/mlforecast/grouped_array.py` & `mlforecast-0.9.0/mlforecast/grouped_array.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,18 +153,17 @@
             raise ValueError(f"vals must be of size {self[idx].size}")
         self[idx][:] = vals
 
     @classmethod
     def from_sorted_df(
         cls, df: "pd.DataFrame", id_col: str, target_col: str
     ) -> "GroupedArray":
-        grouped = df.groupby(id_col, observed=True)
-        sizes = grouped.size().values
+        sizes = df.groupby(id_col, observed=True).size().values
         indptr = np.append(0, sizes.cumsum())
-        data = df[target_col].values
+        data = df[target_col].values.copy()
         if data.dtype not in (np.float32, np.float64):
             # since all transformations generate nulls, we need a float dtype
             data = data.astype(np.float32)
         return cls(data, indptr)
 
     def transform_series(
         self, updates_only: bool, lag: int, func: Callable, *args
```

### Comparing `mlforecast-0.8.1/mlforecast/lgb_cv.py` & `mlforecast-0.9.0/mlforecast/lgb_cv.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,27 +40,27 @@
 
 def _update(bst, n):
     for _ in range(n):
         bst.update()
 
 
 def _predict(ts, bst, valid, h, before_predict_callback, after_predict_callback):
-    ex_cols_to_drop = [ts.id_col, ts.time_col, ts.target_col]
-    static_features = ts.static_features_.columns.drop(ts.id_col).tolist()
-    ex_cols_to_drop.extend(static_features)
-    has_ex = not valid.columns.drop(ex_cols_to_drop).empty
-    dynamic_dfs = (
-        [valid.drop(columns=static_features + [ts.target_col])] if has_ex else None
-    )
+    static = ts.static_features_.columns.drop(ts.id_col).tolist()
+    dynamic = valid.columns.drop(static + [ts.id_col, ts.time_col, ts.target_col])
+    if not dynamic.empty:
+        X_df = valid.drop(columns=static + [ts.target_col])
+    else:
+        X_df = None
     preds = ts.predict(
         {"Booster": bst},
         h,
-        dynamic_dfs,
+        None,
         before_predict_callback,
         after_predict_callback,
+        X_df=X_df,
     )
     return valid.merge(preds, on=[ts.id_col, ts.time_col], how="left")
 
 
 def _update_and_predict(
     ts, bst, valid, n, h, before_predict_callback, after_predict_callback
 ):
@@ -508,14 +508,15 @@
     @old_kw_to_pos(["horizon"], [1])
     def predict(
         self,
         h: int,
         dynamic_dfs: Optional[List[pd.DataFrame]] = None,
         before_predict_callback: Optional[Callable] = None,
         after_predict_callback: Optional[Callable] = None,
+        X_df: Optional[pd.DataFrame] = None,
         *,
         horizon: Optional[int] = None,  # noqa: ARG002
     ) -> pd.DataFrame:
         """Compute predictions with each of the trained boosters.
 
         Parameters
         ----------
@@ -527,22 +528,25 @@
             Function to call on the features before computing the predictions.
                 This function will take the input dataframe that will be passed to the model for predicting and should return a dataframe with the same structure.
                 The series identifier is on the index.
         after_predict_callback : callable, optional (default=None)
             Function to call on the predictions before updating the targets.
                 This function will take a pandas Series with the predictions and should return another one with the same structure.
                 The series identifier is on the index.
+        X_df : pandas DataFrame, optional (default=None)
+            Dataframe with the future exogenous features. Should have the id column and the time column.
         horizon : int
             Forecast horizon. This argument has been replaced by h and will be removed in a later release.
 
         Returns
         -------
         result : pandas DataFrame
             Predictions for each serie and timestep, with one column per window.
         """
         return self.ts.predict(
             self.cv_models_,
             h,
             dynamic_dfs,
             before_predict_callback,
             after_predict_callback,
+            X_df=X_df,
         )
```

### Comparing `mlforecast-0.8.1/mlforecast/target_transforms.py` & `mlforecast-0.9.0/mlforecast/target_transforms.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.8.1/mlforecast/utils.py` & `mlforecast-0.9.0/mlforecast/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,23 +76,21 @@
 def generate_prices_for_series(
     series: pd.DataFrame, horizon: int = 7, seed: int = 0
 ) -> pd.DataFrame:
     rng = np.random.RandomState(seed)
     unique_last_dates = series.groupby("unique_id")["ds"].max().nunique()
     if unique_last_dates > 1:
         raise ValueError("series must have equal ends.")
-    if "product_id" not in series:
-        raise ValueError("series must have a product_id column.")
     day_offset = pd.tseries.frequencies.Day()
-    starts_ends = series.groupby("product_id")["ds"].agg([min, max])
+    starts_ends = series.groupby("unique_id")["ds"].agg([min, max])
     dfs = []
     for idx, (start, end) in starts_ends.iterrows():
         product_df = pd.DataFrame(
             {
-                "product_id": idx,
+                "unique_id": idx,
                 "price": rng.rand((end - start).days + 1 + horizon),
             },
             index=pd.date_range(start, end + horizon * day_offset, name="ds"),
         )
         dfs.append(product_df)
     prices_catalog = pd.concat(dfs).reset_index()
     return prices_catalog
```

### Comparing `mlforecast-0.8.1/mlforecast.egg-info/PKG-INFO` & `mlforecast-0.9.0/mlforecast.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlforecast
-Version: 0.8.1
+Version: 0.9.0
 Summary: Scalable machine learning based time series forecasting
 Home-page: https://github.com/Nixtla/mlforecast
 Author: José Morales
 Author-email: jmoralz92@gmail.com
 License: Apache Software License 2.0
 Keywords: python forecast forecasting machine-learning dask
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mlforecast-0.8.1/mlforecast.egg-info/SOURCES.txt` & `mlforecast-0.9.0/mlforecast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlforecast-0.8.1/settings.ini` & `mlforecast-0.9.0/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 user = Nixtla
 description = Scalable machine learning based time series forecasting
 keywords = python forecast forecasting machine-learning dask
 author = José Morales
 author_email = jmoralz92@gmail.com
 copyright = Nixtla
 branch = main
-version = 0.8.1
+version = 0.9.0
 min_python = 3.6
 audience = Developers
 language = English
 custom_sidebar = True
 license = apache2
 status = 3
 requirements = numba pandas scikit-learn window-ops
```

### Comparing `mlforecast-0.8.1/setup.py` & `mlforecast-0.9.0/setup.py`

 * *Files identical despite different names*

