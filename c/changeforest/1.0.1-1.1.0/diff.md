# Comparing `tmp/changeforest-1.0.1.tar.gz` & `tmp/changeforest-1.1.0.tar.gz`

## Comparing `changeforest-1.0.1.tar` & `changeforest-1.1.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 changeforest-1.0.1/local_dependencies/changeforest/Cargo.toml
--rw-r--r--   0     1001      123     5182 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/CHANGELOG.md
--rw-r--r--   0     1001      123     1506 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/LICENSE
--rw-r--r--   0     1001      123    10533 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/README.md
--rw-r--r--   0     1001      123    44744 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/docs/py_cic_rf_binary_segmentation_result_plot.png
--rw-r--r--   0     1001      123    85452 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/docs/py_cic_rf_optimizer_result_plot.png
--rw-r--r--   0     1001      123    57577 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/docs/r_cic_rf_binary_segmentation_result_plot.png
--rw-r--r--   0     1001      123   164340 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/docs/r_cic_rf_optimizer_result_plot.png
--rw-r--r--   0     1001      123     7089 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/binary_segmentation.rs
--rw-r--r--   0     1001      123     3213 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/classifier/classifier.rs
--rw-r--r--   0     1001      123     6140 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/classifier/knn.rs
--rw-r--r--   0     1001      123      132 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/classifier/mod.rs
--rw-r--r--   0     1001      123     3489 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/classifier/random_forest.rs
--rw-r--r--   0     1001      123     4379 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/control.rs
--rw-r--r--   0     1001      123     5940 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/fmt.rs
--rw-r--r--   0     1001      123     3918 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/gain/change_in_mean.rs
--rw-r--r--   0     1001      123     7755 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/gain/classifier_gain.rs
--rw-r--r--   0     1001      123     4067 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/gain/gain.rs
--rw-r--r--   0     1001      123     3213 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/gain/gain_result.rs
--rw-r--r--   0     1001      123      276 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/gain/mod.rs
--rw-r--r--   0     1001      123      675 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/lib.rs
--rw-r--r--   0     1001      123      927 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/model_selection_result.rs
--rw-r--r--   0     1001      123     2421 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/optimizer/grid_search.rs
--rw-r--r--   0     1001      123      223 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/optimizer/mod.rs
--rw-r--r--   0     1001      123     1140 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/optimizer/optimizer.rs
--rw-r--r--   0     1001      123      660 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/optimizer/optimizer_result.rs
--rw-r--r--   0     1001      123     4938 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/optimizer/two_step_search.rs
--rw-r--r--   0     1001      123     8349 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/segmentation.rs
--rw-r--r--   0     1001      123     8543 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/testing.rs
--rw-r--r--   0     1001      123      387 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/utils.rs
--rw-r--r--   0     1001      123     3127 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/src/wrapper.rs
--rw-r--r--   0     1001      123     1792 2023-06-01 09:03:02.000000 changeforest-1.0.1/local_dependencies/changeforest/tests/test_integration.rs
--rw-r--r--   0        0        0      362 1970-01-01 00:00:00.000000 changeforest-1.0.1/Cargo.toml
--rw-r--r--   0     1001      123       35 2023-06-01 09:03:02.000000 changeforest-1.0.1/.gitignore
--rw-r--r--   0     1001      123     1506 2023-06-01 09:03:02.000000 changeforest-1.0.1/LICENSE
--rw-r--r--   0     1001      123     5416 2023-06-01 09:03:02.000000 changeforest-1.0.1/README.md
--rw-r--r--   0     1001      123      218 2023-06-01 09:03:02.000000 changeforest-1.0.1/changeforest/__init__.py
--rw-r--r--   0     1001      123     1780 2023-06-01 09:03:02.000000 changeforest-1.0.1/changeforest/control.py
--rw-r--r--   0     1001      123     6047 2023-06-01 09:03:02.000000 changeforest-1.0.1/changeforest/plotting.py
--rw-r--r--   0     1001      123      147 2023-06-01 09:03:02.000000 changeforest-1.0.1/environment.yml
--rw-r--r--   0     1001      123     1838 2023-06-01 09:03:02.000000 changeforest-1.0.1/pyproject.toml
--rw-r--r--   0     1001      123     5039 2023-06-01 09:03:02.000000 changeforest-1.0.1/src/control.rs
--rw-r--r--   0     1001      123     1180 2023-06-01 09:03:02.000000 changeforest-1.0.1/src/lib.rs
--rw-r--r--   0     1001      123     5789 2023-06-01 09:03:02.000000 changeforest-1.0.1/src/result.rs
--rw-r--r--   0     1001      123     1270 2023-06-01 09:03:02.000000 changeforest-1.0.1/tests/conftest.py
--rw-r--r--   0     1001      123      987 2023-06-01 09:03:02.000000 changeforest-1.0.1/tests/test_changeforest.py
--rw-r--r--   0     1001      123     4502 2023-06-01 09:03:02.000000 changeforest-1.0.1/tests/test_control.py
--rw-r--r--   0     1001      123      903 2023-06-01 09:03:02.000000 changeforest-1.0.1/tests/test_plotting.py
--rw-r--r--   0     1001      123    13024 2023-06-01 09:04:42.000000 changeforest-1.0.1/Cargo.lock
--rw-r--r--   0        0        0     5800 1970-01-01 00:00:00.000000 changeforest-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 changeforest-1.1.0/local_dependencies/changeforest/Cargo.toml
+-rw-r--r--   0     1001      123     5471 2023-08-01 15:49:27.000000 changeforest-1.1.0/local_dependencies/changeforest/CHANGELOG.md
+-rw-r--r--   0     1001      123     1506 2023-08-01 15:49:27.000000 changeforest-1.1.0/local_dependencies/changeforest/LICENSE
+-rw-r--r--   0     1001      123    10533 2023-08-01 15:49:27.000000 changeforest-1.1.0/local_dependencies/changeforest/README.md
+-rw-r--r--   0     1001      123    44744 2023-08-01 15:49:27.000000 changeforest-1.1.0/local_dependencies/changeforest/docs/py_cic_rf_binary_segmentation_result_plot.png
+-rw-r--r--   0     1001      123    85452 2023-08-01 15:49:27.000000 changeforest-1.1.0/local_dependencies/changeforest/docs/py_cic_rf_optimizer_result_plot.png
+-rw-r--r--   0     1001      123    57577 2023-08-01 15:49:27.000000 changeforest-1.1.0/local_dependencies/changeforest/docs/r_cic_rf_binary_segmentation_result_plot.png
+-rw-r--r--   0     1001      123   164340 2023-08-01 15:49:27.000000 changeforest-1.1.0/local_dependencies/changeforest/docs/r_cic_rf_optimizer_result_plot.png
+-rw-r--r--   0     1001      123     7089 2023-08-01 15:49:27.000000 changeforest-1.1.0/local_dependencies/changeforest/src/binary_segmentation.rs
+-rw-r--r--   0     1001      123     3213 2023-08-01 15:49:27.000000 changeforest-1.1.0/local_dependencies/changeforest/src/classifier/classifier.rs
+-rw-r--r--   0     1001      123     6140 2023-08-01 15:49:27.000000 changeforest-1.1.0/local_dependencies/changeforest/src/classifier/knn.rs
+-rw-r--r--   0     1001      123      132 2023-08-01 15:49:27.000000 changeforest-1.1.0/local_dependencies/changeforest/src/classifier/mod.rs
+-rw-r--r--   0     1001      123     3489 2023-08-01 15:49:27.000000 changeforest-1.1.0/local_dependencies/changeforest/src/classifier/random_forest.rs
+-rw-r--r--   0     1001      123     5078 2023-08-01 15:49:27.000000 changeforest-1.1.0/local_dependencies/changeforest/src/control.rs
+-rw-r--r--   0     1001      123     5940 2023-08-01 15:49:27.000000 changeforest-1.1.0/local_dependencies/changeforest/src/fmt.rs
+-rw-r--r--   0     1001      123     3918 2023-08-01 15:49:27.000000 changeforest-1.1.0/local_dependencies/changeforest/src/gain/change_in_mean.rs
+-rw-r--r--   0     1001      123     7755 2023-08-01 15:49:27.000000 changeforest-1.1.0/local_dependencies/changeforest/src/gain/classifier_gain.rs
+-rw-r--r--   0     1001      123     4067 2023-08-01 15:49:27.000000 changeforest-1.1.0/local_dependencies/changeforest/src/gain/gain.rs
+-rw-r--r--   0     1001      123     3213 2023-08-01 15:49:27.000000 changeforest-1.1.0/local_dependencies/changeforest/src/gain/gain_result.rs
+-rw-r--r--   0     1001      123      276 2023-08-01 15:49:27.000000 changeforest-1.1.0/local_dependencies/changeforest/src/gain/mod.rs
+-rw-r--r--   0     1001      123      675 2023-08-01 15:49:27.000000 changeforest-1.1.0/local_dependencies/changeforest/src/lib.rs
+-rw-r--r--   0     1001      123      927 2023-08-01 15:49:27.000000 changeforest-1.1.0/local_dependencies/changeforest/src/model_selection_result.rs
+-rw-r--r--   0     1001      123     3556 2023-08-01 15:49:27.000000 changeforest-1.1.0/local_dependencies/changeforest/src/optimizer/grid_search.rs
+-rw-r--r--   0     1001      123      223 2023-08-01 15:49:27.000000 changeforest-1.1.0/local_dependencies/changeforest/src/optimizer/mod.rs
+-rw-r--r--   0     1001      123     1707 2023-08-01 15:49:27.000000 changeforest-1.1.0/local_dependencies/changeforest/src/optimizer/optimizer.rs
+-rw-r--r--   0     1001      123      660 2023-08-01 15:49:27.000000 changeforest-1.1.0/local_dependencies/changeforest/src/optimizer/optimizer_result.rs
+-rw-r--r--   0     1001      123     6123 2023-08-01 15:49:27.000000 changeforest-1.1.0/local_dependencies/changeforest/src/optimizer/two_step_search.rs
+-rw-r--r--   0     1001      123     8442 2023-08-01 15:49:27.000000 changeforest-1.1.0/local_dependencies/changeforest/src/segmentation.rs
+-rw-r--r--   0     1001      123     8543 2023-08-01 15:49:27.000000 changeforest-1.1.0/local_dependencies/changeforest/src/testing.rs
+-rw-r--r--   0     1001      123      387 2023-08-01 15:49:27.000000 changeforest-1.1.0/local_dependencies/changeforest/src/utils.rs
+-rw-r--r--   0     1001      123     3127 2023-08-01 15:49:27.000000 changeforest-1.1.0/local_dependencies/changeforest/src/wrapper.rs
+-rw-r--r--   0     1001      123     1792 2023-08-01 15:49:27.000000 changeforest-1.1.0/local_dependencies/changeforest/tests/test_integration.rs
+-rw-r--r--   0        0        0      362 1970-01-01 00:00:00.000000 changeforest-1.1.0/Cargo.toml
+-rw-r--r--   0     1001      123       35 2023-08-01 15:49:27.000000 changeforest-1.1.0/.gitignore
+-rw-r--r--   0     1001      123     1506 2023-08-01 15:49:27.000000 changeforest-1.1.0/LICENSE
+-rw-r--r--   0     1001      123     5416 2023-08-01 15:49:27.000000 changeforest-1.1.0/README.md
+-rw-r--r--   0     1001      123      218 2023-08-01 15:49:27.000000 changeforest-1.1.0/changeforest/__init__.py
+-rw-r--r--   0     1001      123     2260 2023-08-01 15:49:27.000000 changeforest-1.1.0/changeforest/control.py
+-rw-r--r--   0     1001      123     6047 2023-08-01 15:49:27.000000 changeforest-1.1.0/changeforest/plotting.py
+-rw-r--r--   0     1001      123      147 2023-08-01 15:49:27.000000 changeforest-1.1.0/environment.yml
+-rw-r--r--   0     1001      123     1838 2023-08-01 15:49:27.000000 changeforest-1.1.0/pyproject.toml
+-rw-r--r--   0     1001      123     5284 2023-08-01 15:49:27.000000 changeforest-1.1.0/src/control.rs
+-rw-r--r--   0     1001      123     1180 2023-08-01 15:49:27.000000 changeforest-1.1.0/src/lib.rs
+-rw-r--r--   0     1001      123     5789 2023-08-01 15:49:27.000000 changeforest-1.1.0/src/result.rs
+-rw-r--r--   0     1001      123     1270 2023-08-01 15:49:27.000000 changeforest-1.1.0/tests/conftest.py
+-rw-r--r--   0     1001      123     2150 2023-08-01 15:49:27.000000 changeforest-1.1.0/tests/test_changeforest.py
+-rw-r--r--   0     1001      123     4885 2023-08-01 15:49:27.000000 changeforest-1.1.0/tests/test_control.py
+-rw-r--r--   0     1001      123      903 2023-08-01 15:49:27.000000 changeforest-1.1.0/tests/test_plotting.py
+-rw-r--r--   0     1001      123    12999 2023-08-01 15:49:35.000000 changeforest-1.1.0/Cargo.lock
+-rw-r--r--   0        0        0     5800 1970-01-01 00:00:00.000000 changeforest-1.1.0/PKG-INFO
```

### Comparing `changeforest-1.0.1/local_dependencies/changeforest/CHANGELOG.md` & `changeforest-1.1.0/local_dependencies/changeforest/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 
 # Changelog
 
+## 1.1.0 - (2023-08-01)
+
+**New features**:
+
+- New argument `forbidden_segments` (list or vector of 2-tuple) or `None` to `Control`. If not `None`, `changeforest` will not split on split points contained in segments `(a, b]` in `forbidden_segments` (rust and Python only). Thanks @enzbus!
+
 ## 1.0.1 - (2022-06-01)
 
 **Bug fixes:**
 
 - Python macos images are now again correctly built on GitHub runners.
 
 ## 1.0.0 - (2022-05-30)
```

### Comparing `changeforest-1.0.1/local_dependencies/changeforest/LICENSE` & `changeforest-1.1.0/local_dependencies/changeforest/LICENSE`

 * *Files identical despite different names*

### Comparing `changeforest-1.0.1/local_dependencies/changeforest/README.md` & `changeforest-1.1.0/local_dependencies/changeforest/README.md`

 * *Files identical despite different names*

### Comparing `changeforest-1.0.1/local_dependencies/changeforest/docs/py_cic_rf_binary_segmentation_result_plot.png` & `changeforest-1.1.0/local_dependencies/changeforest/docs/py_cic_rf_binary_segmentation_result_plot.png`

 * *Files identical despite different names*

### Comparing `changeforest-1.0.1/local_dependencies/changeforest/docs/py_cic_rf_optimizer_result_plot.png` & `changeforest-1.1.0/local_dependencies/changeforest/docs/py_cic_rf_optimizer_result_plot.png`

 * *Files identical despite different names*

### Comparing `changeforest-1.0.1/local_dependencies/changeforest/docs/r_cic_rf_binary_segmentation_result_plot.png` & `changeforest-1.1.0/local_dependencies/changeforest/docs/r_cic_rf_binary_segmentation_result_plot.png`

 * *Files identical despite different names*

### Comparing `changeforest-1.0.1/local_dependencies/changeforest/docs/r_cic_rf_optimizer_result_plot.png` & `changeforest-1.1.0/local_dependencies/changeforest/docs/r_cic_rf_optimizer_result_plot.png`

 * *Files identical despite different names*

### Comparing `changeforest-1.0.1/local_dependencies/changeforest/src/binary_segmentation.rs` & `changeforest-1.1.0/local_dependencies/changeforest/src/binary_segmentation.rs`

 * *Files identical despite different names*

### Comparing `changeforest-1.0.1/local_dependencies/changeforest/src/classifier/classifier.rs` & `changeforest-1.1.0/local_dependencies/changeforest/src/classifier/classifier.rs`

 * *Files identical despite different names*

### Comparing `changeforest-1.0.1/local_dependencies/changeforest/src/classifier/knn.rs` & `changeforest-1.1.0/local_dependencies/changeforest/src/classifier/knn.rs`

 * *Files identical despite different names*

### Comparing `changeforest-1.0.1/local_dependencies/changeforest/src/classifier/random_forest.rs` & `changeforest-1.1.0/local_dependencies/changeforest/src/classifier/random_forest.rs`

 * *Files identical despite different names*

### Comparing `changeforest-1.0.1/local_dependencies/changeforest/src/control.rs` & `changeforest-1.1.0/local_dependencies/changeforest/src/control.rs`

 * *Files 10% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     /// value close to 1 resulting in many segments. Corresponds to `\alpha` in
     /// https://arxiv.org/pdf/2002.06633.pdf.
     pub seeded_segments_alpha: f64,
     /// Seed used for segmentation.
     pub seed: u64,
     /// Hyperparameters for random forests.
     pub random_forest_parameters: RandomForestParameters,
+    /// Segments of indexes were no segmentation is allowed.
+    pub forbidden_segments: Option<Vec<(usize, usize)>>,
 }
 
 impl Control {
     #[allow(clippy::should_implement_trait)]
     pub fn default() -> Control {
         Control {
             minimal_relative_segment_length: 0.01,
@@ -41,14 +43,15 @@
             number_of_wild_segments: 100,
             seeded_segments_alpha: std::f64::consts::FRAC_1_SQRT_2, // 1 / sqrt(2)
             seed: 0,
             random_forest_parameters: RandomForestParameters::default()
                 .with_max_depth(Some(8))
                 .with_max_features(MaxFeatures::Sqrt)
                 .with_n_jobs(Some(-1)),
+            forbidden_segments: None,
         }
     }
 
     pub fn with_minimal_relative_segment_length(
         mut self,
         minimal_relative_segment_length: f64,
     ) -> Self {
@@ -107,8 +110,24 @@
     pub fn with_random_forest_parameters(
         mut self,
         random_forest_parameters: RandomForestParameters,
     ) -> Self {
         self.random_forest_parameters = random_forest_parameters;
         self
     }
+
+    pub fn with_forbidden_segments(
+        mut self,
+        forbidden_segments: Option<Vec<(usize, usize)>>,
+    ) -> Self {
+        // check that segments are well specified
+        if let Some(ref _forbidden_segments) = forbidden_segments {
+            for el in _forbidden_segments.iter() {
+                if el.0 > el.1 {
+                    panic!("Forbidden segments must be specified as [(a,b), ...] where a <= b!");
+                }
+            }
+        }
+        self.forbidden_segments = forbidden_segments;
+        self
+    }
 }
```

### Comparing `changeforest-1.0.1/local_dependencies/changeforest/src/fmt.rs` & `changeforest-1.1.0/local_dependencies/changeforest/src/fmt.rs`

 * *Files identical despite different names*

### Comparing `changeforest-1.0.1/local_dependencies/changeforest/src/gain/change_in_mean.rs` & `changeforest-1.1.0/local_dependencies/changeforest/src/gain/change_in_mean.rs`

 * *Files identical despite different names*

### Comparing `changeforest-1.0.1/local_dependencies/changeforest/src/gain/classifier_gain.rs` & `changeforest-1.1.0/local_dependencies/changeforest/src/gain/classifier_gain.rs`

 * *Files identical despite different names*

### Comparing `changeforest-1.0.1/local_dependencies/changeforest/src/gain/gain.rs` & `changeforest-1.1.0/local_dependencies/changeforest/src/gain/gain.rs`

 * *Files identical despite different names*

### Comparing `changeforest-1.0.1/local_dependencies/changeforest/src/gain/gain_result.rs` & `changeforest-1.1.0/local_dependencies/changeforest/src/gain/gain_result.rs`

 * *Files identical despite different names*

### Comparing `changeforest-1.0.1/local_dependencies/changeforest/src/lib.rs` & `changeforest-1.1.0/local_dependencies/changeforest/src/lib.rs`

 * *Files identical despite different names*

### Comparing `changeforest-1.0.1/local_dependencies/changeforest/src/model_selection_result.rs` & `changeforest-1.1.0/local_dependencies/changeforest/src/model_selection_result.rs`

 * *Files identical despite different names*

### Comparing `changeforest-1.0.1/local_dependencies/changeforest/src/optimizer/grid_search.rs` & `changeforest-1.1.0/local_dependencies/changeforest/src/optimizer/grid_search.rs`

 * *Files 22% similar despite different names*

```diff
@@ -89,8 +89,41 @@
         let gain = testing::ChangeInMean::new(&X_view, &control);
         let grid_search = GridSearch { gain };
         assert_eq!(
             grid_search.find_best_split(start, stop).unwrap().best_split,
             expected
         );
     }
+
+    #[rstest]
+    #[case(0, 10, Some(vec![(0, 3)]), 0.09, vec![4, 5, 6, 7, 8])]
+    #[case(1, 10, Some(vec![(6, 10)]), 0.15, vec![3, 4, 5, 6])]
+    #[case(0, 10, Some(vec![(2, 4), (5, 7)]), 0.09, vec![1, 2, 5, 8])]
+    #[case(1, 7, Some(vec![(2, 4), (5, 7)]), 0.09, vec![2, 5])]
+    fn test_split_candidates(
+        #[case] start: usize,
+        #[case] stop: usize,
+        #[case] forbidden_segments: Option<Vec<(usize, usize)>>,
+        #[case] delta: f64,
+        #[case] expected: Vec<usize>,
+    ) {
+        let X = ndarray::array![
+            [0.0],
+            [0.0],
+            [0.0],
+            [0.0],
+            [-0.0],
+            [-0.0],
+            [-0.0],
+            [-0.0],
+            [-0.0],
+            [-0.0]
+        ];
+        let X_view = X.view();
+        let control = Control::default()
+            .with_minimal_relative_segment_length(delta)
+            .with_forbidden_segments(forbidden_segments);
+        let gain = testing::ChangeInMean::new(&X_view, &control);
+        let grid_search = GridSearch { gain };
+        assert_eq!(grid_search.split_candidates(start, stop).unwrap(), expected);
+    }
 }
```

### Comparing `changeforest-1.0.1/local_dependencies/changeforest/src/optimizer/optimizer.rs` & `changeforest-1.1.0/local_dependencies/changeforest/src/optimizer/optimizer.rs`

 * *Files 26% similar despite different names*

```diff
@@ -19,11 +19,26 @@
     /// Vector with indices of allowed split points.
     fn split_candidates(&self, start: usize, stop: usize) -> Result<Vec<usize>, &str> {
         let minimal_segment_length =
             (self.control().minimal_relative_segment_length * (self.n() as f64)).ceil() as usize;
         if 2 * minimal_segment_length >= (stop - start) {
             Err("Segment too small.")
         } else {
-            Ok(((start + minimal_segment_length)..(stop - minimal_segment_length)).collect())
+            let mut split_candidates: Vec<usize> =
+                ((start + minimal_segment_length)..(stop - minimal_segment_length)).collect();
+
+            if let Some(forbidden_segments) = &self.control().forbidden_segments {
+                split_candidates.retain(|x| {
+                    forbidden_segments
+                        .iter()
+                        .all(|segment| x <= &segment.0 || x > &segment.1)
+                });
+            }
+
+            if split_candidates.is_empty() {
+                Err("No split_candidates left after filtering out forbidden_segments.")
+            } else {
+                Ok(split_candidates)
+            }
         }
     }
 }
```

### Comparing `changeforest-1.0.1/local_dependencies/changeforest/src/optimizer/optimizer_result.rs` & `changeforest-1.1.0/local_dependencies/changeforest/src/optimizer/optimizer_result.rs`

 * *Files identical despite different names*

### Comparing `changeforest-1.0.1/local_dependencies/changeforest/src/segmentation.rs` & `changeforest-1.1.0/local_dependencies/changeforest/src/segmentation.rs`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,17 @@
                     segment_step =
                         (optimizer.n() as f64 - segment_length) / (n_segments - 1) as f64; // s_k
                     for segment_id in 0..n_segments {
                         start = ((segment_id as f64 * segment_step) as f32) as usize;
                         // start + segment_length > n through floating point errors in
                         // n_segments, e.g. for n = 20'000, alpha_k = 1/sqrt(2), k=6
                         stop = (start + (segment_length as f32).ceil() as usize).min(optimizer.n());
-                        segments.push(optimizer.find_best_split(start, stop).unwrap());
+                        if let Ok(optimizer_result) = optimizer.find_best_split(start, stop) {
+                            segments.push(optimizer_result)
+                        }
                     }
                 }
             }
             SegmentationType::WBS => {
                 let mut rng = StdRng::seed_from_u64(optimizer.control().seed);
                 let dist = Uniform::from(0..(optimizer.n() + 1));
```

### Comparing `changeforest-1.0.1/local_dependencies/changeforest/src/testing.rs` & `changeforest-1.1.0/local_dependencies/changeforest/src/testing.rs`

 * *Files identical despite different names*

### Comparing `changeforest-1.0.1/local_dependencies/changeforest/src/wrapper.rs` & `changeforest-1.1.0/local_dependencies/changeforest/src/wrapper.rs`

 * *Files identical despite different names*

### Comparing `changeforest-1.0.1/local_dependencies/changeforest/tests/test_integration.rs` & `changeforest-1.1.0/local_dependencies/changeforest/tests/test_integration.rs`

 * *Files identical despite different names*

### Comparing `changeforest-1.0.1/LICENSE` & `changeforest-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `changeforest-1.0.1/README.md` & `changeforest-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `changeforest-1.0.1/changeforest/control.py` & `changeforest-1.1.0/changeforest/control.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,28 +14,30 @@
         number_of_wild_segments="default",
         seeded_segments_alpha="default",
         seed="default",
         random_forest_n_estimators="default",
         random_forest_max_depth="default",
         random_forest_max_features="default",
         random_forest_n_jobs="default",
+        forbidden_segments="default",
     ):
         self.minimal_relative_segment_length = _to_float(
             minimal_relative_segment_length
         )
         self.minimal_gain_to_split = _to_float(minimal_gain_to_split)
         self.model_selection_alpha = _to_float(model_selection_alpha)
         self.model_selection_n_permutations = _to_int(model_selection_n_permutations)
         self.number_of_wild_segments = _to_int(number_of_wild_segments)
         self.seeded_segments_alpha = _to_float(seeded_segments_alpha)
         self.seed = _to_int(seed)
         self.random_forest_n_estimators = _to_int(random_forest_n_estimators)
         self.random_forest_max_depth = _to_int(random_forest_max_depth)
         self.random_forest_max_features = _to_int(random_forest_max_features)
         self.random_forest_n_jobs = _to_int(random_forest_n_jobs)
+        self.forbidden_segments = _to_segments(forbidden_segments)
 
 
 def _to_float(value):
     if value is None:
         return None
     elif isinstance(value, str):
         return value
@@ -46,7 +48,20 @@
 def _to_int(value):
     if value is None:
         return None
     elif isinstance(value, str):
         return value
     else:
         return int(value)
+
+
+def _to_segments(value):
+    if (value is None) or isinstance(value, str):
+        return value
+    else:
+        try:
+            return [(int(el1), int(el2)) for (el1, el2) in value]
+        except Exception:
+            raise SyntaxError(
+                "forbidden_segments must be provided as [(a,b), ...] where a and b are "
+                "integers."
+            )
```

### Comparing `changeforest-1.0.1/changeforest/plotting.py` & `changeforest-1.1.0/changeforest/plotting.py`

 * *Files identical despite different names*

### Comparing `changeforest-1.0.1/pyproject.toml` & `changeforest-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "changeforest"
 description = "Random Forests for Change Point Detection"
 readme = "README.md"
-version = "1.0.1"
+version = "1.1.0"
 requires-python = ">=3.7"
 author = "Malte Londschien <malte@londschien.ch>"
 urls = {homepage = "https://github.com/mlondschien/changeforest/"}
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python"
 ]
```

### Comparing `changeforest-1.0.1/src/control.rs` & `changeforest-1.1.0/src/control.rs`

 * *Files 6% similar despite different names*

```diff
@@ -82,14 +82,20 @@
 
         if let Ok(pyvalue) = obj.getattr(py, "random_forest_n_jobs") {
             if let Ok(value) = pyvalue.extract::<Option<i32>>(py) {
                 control.random_forest_parameters =
                     control.random_forest_parameters.with_n_jobs(value);
             }
         };
+
+        if let Ok(pyvalue) = obj.getattr(py, "forbidden_segments") {
+            if let Ok(value) = pyvalue.extract::<Option<Vec<(usize, usize)>>>(py) {
+                control = control.with_forbidden_segments(value);
+            }
+        };
     }
 
     Ok(control)
 }
 
 #[pyclass(name = "MaxFeatures")]
 pub struct PyMaxFeatures {
```

### Comparing `changeforest-1.0.1/src/lib.rs` & `changeforest-1.1.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `changeforest-1.0.1/src/result.rs` & `changeforest-1.1.0/src/result.rs`

 * *Files identical despite different names*

### Comparing `changeforest-1.0.1/tests/conftest.py` & `changeforest-1.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `changeforest-1.0.1/tests/test_control.py` & `changeforest-1.1.0/tests/test_control.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,7 +125,26 @@
     )
     another_result = changeforest(
         iris_dataset, "random_forest", "bs", Control(**{key: another_value})
     )
 
     assert str(result) == str(default_result)
     assert str(result) != str(another_result)
+
+
+def test_control_segments():
+    with pytest.raises(SyntaxError):
+        Control(
+            forbidden_segments=[
+                (2),
+            ]
+        )
+
+    with pytest.raises(SyntaxError):
+        Control(
+            forbidden_segments=[
+                (2, 3, 4),
+            ]
+        )
+
+    with pytest.raises(SyntaxError):
+        Control(forbidden_segments=[2, 3])
```

### Comparing `changeforest-1.0.1/tests/test_plotting.py` & `changeforest-1.1.0/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `changeforest-1.0.1/Cargo.lock` & `changeforest-1.1.0/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -35,24 +35,24 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "changeforest"
-version = "1.0.1"
+version = "1.1.0"
 dependencies = [
  "biosphere",
  "ndarray",
  "rand",
 ]
 
 [[package]]
 name = "changeforest_py"
-version = "1.0.1"
+version = "1.1.0"
 dependencies = [
  "biosphere",
  "changeforest",
  "ndarray",
  "numpy",
  "pyo3",
 ]
@@ -76,59 +76,56 @@
  "cfg-if 1.0.0",
  "crossbeam-epoch",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-epoch"
-version = "0.9.14"
+version = "0.9.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46bd5f3f85273295a9d14aedfb86f6aadbff6d8f5295c4a9edb08e819dcf5695"
+checksum = "ae211234986c545741a7dc064309f67ee1e5ad243d0e48335adc0484d960bcc7"
 dependencies = [
  "autocfg",
  "cfg-if 1.0.0",
  "crossbeam-utils",
  "memoffset",
  "scopeguard",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.15"
+version = "0.8.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c063cd8cc95f5c377ed0d4b49a4b21f632396ff690e8470c29b3359b346984b"
+checksum = "5a22b2d63d4d1dc0b7f1b6b2747dd0088008a9be28b6ddf0b1e7d335e3037294"
 dependencies = [
  "cfg-if 1.0.0",
 ]
 
 [[package]]
 name = "either"
-version = "1.8.1"
+version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
+checksum = "a26ae43d7bcc3b814de94796a5e736d4029efb0ee900c12e2d54c993ad1a1e07"
 
 [[package]]
 name = "getrandom"
-version = "0.2.9"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
+checksum = "be4136b2a15dd319360be1c07d9933517ccf0be8f16bf62a3bee4f0d618df427"
 dependencies = [
  "cfg-if 1.0.0",
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "hermit-abi"
-version = "0.2.6"
+version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
-dependencies = [
- "libc",
-]
+checksum = "443144c8cdadd93ebf52ddb4056d257f5b52c04d3c804e657d19eb73fc33668b"
 
 [[package]]
 name = "indoc"
 version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "47741a8bc60fb26eb8d6e0238bbb26d8575ff623fdc97b1a2c00c050b9684ed8"
 dependencies = [
@@ -156,23 +153,23 @@
 checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
 dependencies = [
  "cfg-if 1.0.0",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.144"
+version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
+checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
 [[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "matrixmultiply"
@@ -182,17 +179,17 @@
 dependencies = [
  "autocfg",
  "rawpointer",
 ]
 
 [[package]]
 name = "memoffset"
-version = "0.8.0"
+version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
+checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "ndarray"
 version = "0.15.6"
@@ -223,26 +220,26 @@
 dependencies = [
  "autocfg",
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.15"
+version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
+checksum = "f30b0abd723be7e2ffca1272140fac1a2f084c77ec3e123c192b66af1ee9e6c2"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "num_cpus"
-version = "1.15.0"
+version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fac9e2da13b5eb447a6ce3d392f23a29d8694bff781bf03a16cd9ac8697593b"
+checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
 dependencies = [
  "hermit-abi",
  "libc",
 ]
 
 [[package]]
 name = "numpy"
@@ -256,17 +253,17 @@
  "num-complex",
  "num-traits",
  "pyo3",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.2"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9670a07f94779e00908f3e686eab508878ebb390ba6e604d3a284c00e8d0487b"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "parking_lot"
 version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7d17b78036a60663b797adeaee46f5c9dfebb86948d1255007a1d6be0271ff99"
 dependencies = [
@@ -318,17 +315,17 @@
 name = "proc-macro-hack"
 version = "0.5.20+deprecated"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc375e1527247fe1a97d8b7156678dfe7c1af2fc075c9a4db3690ecd2a148068"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.59"
+version = "1.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6aeca18b86b413c660b781aa319e4e2648a3e6f9eadc9b47e9038e6fe9f3451b"
+checksum = "18fb31db3f9bddb2ea821cde30a9f70117e3f119938b5ee630b7403aa6e2ead9"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.15.2"
@@ -375,17 +372,17 @@
  "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.28"
+version = "1.0.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
+checksum = "50f3b39ccfb720540debaa0164757101c08ecb8d326b15358ce76a62c7e85965"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -451,40 +448,40 @@
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "scopeguard"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
+checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "smallvec"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
+checksum = "62bb4feee49fdd9f707ef802e22365a35de4b7b299de4763d44bfea899442ff9"
 
 [[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.9"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
+checksum = "301abaae475aa91687eb82514b328ab47a211a533026cb25fc3e519b86adfc3c"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
```

### Comparing `changeforest-1.0.1/PKG-INFO` & `changeforest-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: changeforest
-Version: 1.0.1
+Version: 1.1.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 License-File: LICENSE
 Summary: Random Forests for Change Point Detection
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: homepage, https://github.com/mlondschien/changeforest/
```

