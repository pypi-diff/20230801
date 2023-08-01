# Comparing `tmp/moss_decoder-0.5.1.tar.gz` & `tmp/moss_decoder-0.5.2.tar.gz`

## Comparing `moss_decoder-0.5.1.tar` & `moss_decoder-0.5.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1057 1970-01-01 00:00:00.000000 moss_decoder-0.5.1/Cargo.toml
--rw-r--r--   0     1001      123      633 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/.CERN-gitlab-ci.yml
--rw-r--r--   0     1001      123     2835 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      373 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/.github/workflows/bench-py.yml
--rw-r--r--   0     1001      123      404 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/.github/workflows/rust.yml
--rw-r--r--   0     1001      123      715 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/.gitignore
--rw-r--r--   0     1001      123      757 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/.pre-commit-config.yaml
--rw-r--r--   0     1001      123     7642 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/README.md
--rw-r--r--   0     1001      123      360 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/benches/benchmark.rs
--rw-r--r--   0     1001      123      396 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/benches/decode_from_file_bench.rs
--rw-r--r--   0     1001      123      445 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/benches/decode_multiple_events_bench.rs
--rw-r--r--   0     1001      123      436 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/benches/decode_single_event_bench.rs
--rw-r--r--   0     1001      123      799 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/moss_decoder.pyi
--rw-r--r--   0     1001      123      641 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/pyproject.toml
--rw-r--r--   0     1001      123  4458776 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/python310.dll
--rw-r--r--   0     1001      123    14906 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/src/decode_hits_fsm.rs
--rw-r--r--   0     1001      123    11918 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/src/lib.rs
--rw-r--r--   0     1001      123     1880 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/src/moss_protocol/moss_hit.rs
--rw-r--r--   0     1001      123     1854 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/src/moss_protocol/moss_packet.rs
--rw-r--r--   0     1001      123     2847 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/src/moss_protocol/test_util.rs
--rw-r--r--   0     1001      123     2263 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/src/moss_protocol.rs
--rw-r--r--   0     1001      123     1321 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/src/parse_error.rs
--rw-r--r--   0     1001      123     3992 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/src/parse_util.rs
--rwxr-xr-x   0     1001      123      435 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/tests/bench_dev_vs_prod.sh
--rw-r--r--   0     1001      123     6433 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/tests/integration.py
--rw-r--r--   0     1001      123    11186 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/tests/integration_test.rs
--rw-r--r--   0     1001      123  9582576 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/tests/moss_noise.raw
--rw-r--r--   0     1001      123      500 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/tests/moss_noise_0-499b.raw
--rw-r--r--   0     1001      123      500 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/tests/moss_noise_500-999b.raw
--rwxr-xr-x   0     1001      123     1190 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/tests/performance_dev_py.sh
--rwxr-xr-x   0     1001      123      840 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/tests/performance_prod_py.sh
--rw-r--r--   0     1001      123      954 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/tests/utils.sh
--rw-r--r--   0     1001      123    24141 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/Cargo.lock
--rw-r--r--   0        0        0     8196 1970-01-01 00:00:00.000000 moss_decoder-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1057 1970-01-01 00:00:00.000000 moss_decoder-0.5.2/Cargo.toml
+-rw-r--r--   0     1000     1000      633 2023-07-27 11:40:06.000000 moss_decoder-0.5.2/.CERN-gitlab-ci.yml
+-rw-r--r--   0     1000     1000     2835 2023-07-26 12:17:40.000000 moss_decoder-0.5.2/.github/workflows/CI.yml
+-rw-r--r--   0     1000     1000      373 2023-07-26 12:32:27.000000 moss_decoder-0.5.2/.github/workflows/bench-py.yml
+-rw-r--r--   0     1000     1000      404 2023-07-26 12:23:44.000000 moss_decoder-0.5.2/.github/workflows/rust.yml
+-rw-r--r--   0     1000     1000      715 2023-08-01 13:34:35.000000 moss_decoder-0.5.2/.gitignore
+-rw-r--r--   0     1000     1000      757 2023-07-24 15:16:52.000000 moss_decoder-0.5.2/.pre-commit-config.yaml
+-rw-r--r--   0     1000     1000     7662 2023-08-01 13:48:11.000000 moss_decoder-0.5.2/README.md
+-rw-r--r--   0     1000     1000      360 2023-07-31 06:31:17.000000 moss_decoder-0.5.2/benches/benchmark.rs
+-rw-r--r--   0     1000     1000      396 2023-08-01 13:34:35.000000 moss_decoder-0.5.2/benches/decode_from_file_bench.rs
+-rw-r--r--   0     1000     1000      445 2023-08-01 13:34:35.000000 moss_decoder-0.5.2/benches/decode_multiple_events_bench.rs
+-rw-r--r--   0     1000     1000      436 2023-08-01 13:34:35.000000 moss_decoder-0.5.2/benches/decode_single_event_bench.rs
+-rw-r--r--   0     1000     1000      799 2023-08-01 13:34:35.000000 moss_decoder-0.5.2/moss_decoder.pyi
+-rw-r--r--   0     1000     1000      641 2023-07-24 12:33:32.000000 moss_decoder-0.5.2/pyproject.toml
+-rw-r--r--   0     1000     1000  4458776 2023-07-24 06:58:57.000000 moss_decoder-0.5.2/python310.dll
+-rw-r--r--   0     1000     1000    14999 2023-08-01 13:47:46.000000 moss_decoder-0.5.2/src/decode_hits_fsm.rs
+-rw-r--r--   0     1000     1000    11918 2023-08-01 13:34:35.000000 moss_decoder-0.5.2/src/lib.rs
+-rw-r--r--   0     1000     1000     1880 2023-07-25 14:37:04.000000 moss_decoder-0.5.2/src/moss_protocol/moss_hit.rs
+-rw-r--r--   0     1000     1000     1854 2023-07-31 06:31:17.000000 moss_decoder-0.5.2/src/moss_protocol/moss_packet.rs
+-rw-r--r--   0     1000     1000     2847 2023-08-01 13:34:35.000000 moss_decoder-0.5.2/src/moss_protocol/test_util.rs
+-rw-r--r--   0     1000     1000     2263 2023-08-01 13:34:35.000000 moss_decoder-0.5.2/src/moss_protocol.rs
+-rw-r--r--   0     1000     1000     1321 2023-08-01 13:34:35.000000 moss_decoder-0.5.2/src/parse_error.rs
+-rw-r--r--   0     1000     1000     3992 2023-08-01 13:34:35.000000 moss_decoder-0.5.2/src/parse_util.rs
+-rwxr-xr-x   0     1000     1000      435 2023-08-01 13:34:35.000000 moss_decoder-0.5.2/tests/bench_dev_vs_prod.sh
+-rw-r--r--   0     1000     1000     6433 2023-08-01 13:34:35.000000 moss_decoder-0.5.2/tests/integration.py
+-rw-r--r--   0     1000     1000    11186 2023-08-01 13:34:35.000000 moss_decoder-0.5.2/tests/integration_test.rs
+-rw-r--r--   0     1000     1000  9582576 2023-07-24 06:58:57.000000 moss_decoder-0.5.2/tests/moss_noise.raw
+-rw-r--r--   0     1000     1000      500 2023-08-01 13:34:35.000000 moss_decoder-0.5.2/tests/moss_noise_0-499b.raw
+-rw-r--r--   0     1000     1000      500 2023-08-01 13:34:35.000000 moss_decoder-0.5.2/tests/moss_noise_500-999b.raw
+-rwxr-xr-x   0     1000     1000     1190 2023-08-01 13:34:35.000000 moss_decoder-0.5.2/tests/performance_dev_py.sh
+-rwxr-xr-x   0     1000     1000      840 2023-08-01 13:34:35.000000 moss_decoder-0.5.2/tests/performance_prod_py.sh
+-rw-r--r--   0     1000     1000      954 2023-07-31 06:31:17.000000 moss_decoder-0.5.2/tests/utils.sh
+-rw-r--r--   0     1000     1000    24141 2023-08-01 13:49:06.000000 moss_decoder-0.5.2/Cargo.lock
+-rw-r--r--   0        0        0     8216 1970-01-01 00:00:00.000000 moss_decoder-0.5.2/PKG-INFO
```

### Comparing `moss_decoder-0.5.1/Cargo.toml` & `moss_decoder-0.5.2/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "moss_decoder"
-version = "0.5.1"
+version = "0.5.2"
 edition = "2021"
 authors = ["Marc Beck König <mbkj@tutamail.com>"]
 license = "MIT OR Apache-2.0"
 description = "Python module providing a decoder for the MOSS chip protocol."
 categories = ["python-module"]
```

### Comparing `moss_decoder-0.5.1/.CERN-gitlab-ci.yml` & `moss_decoder-0.5.2/.CERN-gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.1/.github/workflows/CI.yml` & `moss_decoder-0.5.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.1/.gitignore` & `moss_decoder-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.1/.pre-commit-config.yaml` & `moss_decoder-0.5.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.1/README.md` & `moss_decoder-0.5.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -180,14 +180,15 @@
 
     state DATA {
       [*] --> data_0
       data_0 --> data_1
       data_1 --> data_2
       data_2 --> data_0
       data_2 --> idle
+      idle --> idle
       idle --> [*]
       idle --> data_0
       data_2 --> [*]
 
     }
 
 ```
```

### Comparing `moss_decoder-0.5.1/moss_decoder.pyi` & `moss_decoder-0.5.2/moss_decoder.pyi`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.1/pyproject.toml` & `moss_decoder-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.1/python310.dll` & `moss_decoder-0.5.2/python310.dll`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.1/src/decode_hits_fsm.rs` & `moss_decoder-0.5.2/src/decode_hits_fsm.rs`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
             IDLE_ => DATA0_
             DATA0_ => DATA1_
             DATA1_ => DATA2_
         }
 
         _Idle {
             DATA2_ => IDLE_
+            IDLE_ => IDLE_
         }
 
         _RegionHeader0 {
             _UNIT_FRAME_HEADER_ => REGION_HEADER0_
         }
 
         _RegionHeader1 {
@@ -218,14 +219,15 @@
                     current_region = 2;
                     st.transition(_RegionHeader2).as_enum()
                 }
                 REGION_HEADER3 => {
                     current_region = 3;
                     st.transition(_RegionHeader3).as_enum()
                 }
+                MossWord::IDLE => st.transition(_Idle).as_enum(),
                 MossWord::UNIT_FRAME_TRAILER => {
                     is_trailer_seen = true;
                     break;
                 }
                 _ => {
                     return Err(ParseError::new(
                         ParseErrorKind::ProtocolError,
```

### Comparing `moss_decoder-0.5.1/src/lib.rs` & `moss_decoder-0.5.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.1/src/moss_protocol/moss_hit.rs` & `moss_decoder-0.5.2/src/moss_protocol/moss_hit.rs`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.1/src/moss_protocol/moss_packet.rs` & `moss_decoder-0.5.2/src/moss_protocol/moss_packet.rs`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.1/src/moss_protocol/test_util.rs` & `moss_decoder-0.5.2/src/moss_protocol/test_util.rs`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.1/src/moss_protocol.rs` & `moss_decoder-0.5.2/src/moss_protocol.rs`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.1/src/parse_error.rs` & `moss_decoder-0.5.2/src/parse_error.rs`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.1/src/parse_util.rs` & `moss_decoder-0.5.2/src/parse_util.rs`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.1/tests/integration.py` & `moss_decoder-0.5.2/tests/integration.py`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.1/tests/integration_test.rs` & `moss_decoder-0.5.2/tests/integration_test.rs`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.1/tests/moss_noise.raw` & `moss_decoder-0.5.2/tests/moss_noise.raw`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.1/tests/performance_dev_py.sh` & `moss_decoder-0.5.2/tests/performance_dev_py.sh`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.1/tests/performance_prod_py.sh` & `moss_decoder-0.5.2/tests/performance_prod_py.sh`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.1/tests/utils.sh` & `moss_decoder-0.5.2/tests/utils.sh`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.1/Cargo.lock` & `moss_decoder-0.5.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -323,15 +323,15 @@
 checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "moss_decoder"
-version = "0.5.1"
+version = "0.5.2"
 dependencies = [
  "criterion",
  "pretty_assertions",
  "pyo3",
  "sm",
 ]
```

### Comparing `moss_decoder-0.5.1/PKG-INFO` & `moss_decoder-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moss_decoder
-Version: 0.5.1
+Version: 0.5.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Python package implemented in Rust to decode MOSS readout data
 Author: Marc Beck König
 Author-email: marc.beck.konig@cern.ch
 Maintainer-email: Marc Beck König <marc.beck.konig@cern.ch>
@@ -194,14 +194,15 @@
 
     state DATA {
       [*] --> data_0
       data_0 --> data_1
       data_1 --> data_2
       data_2 --> data_0
       data_2 --> idle
+      idle --> idle
       idle --> [*]
       idle --> data_0
       data_2 --> [*]
 
     }
 
 ```
```

