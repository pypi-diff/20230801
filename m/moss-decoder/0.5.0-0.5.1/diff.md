# Comparing `tmp/moss_decoder-0.5.0.tar.gz` & `tmp/moss_decoder-0.5.1.tar.gz`

## Comparing `moss_decoder-0.5.0.tar` & `moss_decoder-0.5.1.tar`

### file list

```diff
@@ -1,30 +1,34 @@
--rw-r--r--   0        0        0     1057 1970-01-01 00:00:00.000000 moss_decoder-0.5.0/Cargo.toml
--rw-r--r--   0     1001      123      633 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/.CERN-gitlab-ci.yml
--rw-r--r--   0     1001      123     2835 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      373 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/.github/workflows/bench-py.yml
--rw-r--r--   0     1001      123      404 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/.github/workflows/rust.yml
--rw-r--r--   0     1001      123      714 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/.gitignore
--rw-r--r--   0     1001      123      757 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0     1001      123     7244 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/README.md
--rw-r--r--   0     1001      123      360 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/benches/benchmark.rs
--rw-r--r--   0     1001      123      555 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/benches/decode_from_file_bench.rs
--rw-r--r--   0     1001      123      859 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/benches/decode_multiple_events_bench.rs
--rw-r--r--   0     1001      123      839 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/benches/decode_single_event_bench.rs
--rw-r--r--   0     1001      123     1099 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/moss_decoder.pyi
--rw-r--r--   0     1001      123      641 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/pyproject.toml
--rw-r--r--   0     1001      123  4458776 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/python310.dll
--rw-r--r--   0     1001      123    20323 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/src/lib.rs
--rw-r--r--   0     1001      123     1880 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/src/moss_protocol/moss_hit.rs
--rw-r--r--   0     1001      123     1854 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/src/moss_protocol/moss_packet.rs
--rw-r--r--   0     1001      123     1762 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/src/moss_protocol.rs
--rw-r--r--   0     1001      123    10569 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/src/moss_protocol_fsm.rs
--rw-r--r--   0     1001      123    11217 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/src/moss_protocol_nested_fsm.rs
--rwxr-xr-x   0     1001      123      427 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/tests/bench_dev_vs_prod.sh
--rw-r--r--   0     1001      123     7400 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/tests/integration.py
--rw-r--r--   0     1001      123     9194 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/tests/integration_test.rs
--rw-r--r--   0     1001      123  9582576 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/tests/moss_noise.raw
--rwxr-xr-x   0     1001      123     1190 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/tests/performance_dev_py.sh
--rwxr-xr-x   0     1001      123      820 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/tests/performance_prod_py.sh
--rw-r--r--   0     1001      123      895 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/tests/utils.sh
--rw-r--r--   0     1001      123    24141 2023-07-30 08:49:32.000000 moss_decoder-0.5.0/Cargo.lock
--rw-r--r--   0        0        0     7798 1970-01-01 00:00:00.000000 moss_decoder-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1057 1970-01-01 00:00:00.000000 moss_decoder-0.5.1/Cargo.toml
+-rw-r--r--   0     1001      123      633 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/.CERN-gitlab-ci.yml
+-rw-r--r--   0     1001      123     2835 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      373 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/.github/workflows/bench-py.yml
+-rw-r--r--   0     1001      123      404 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/.github/workflows/rust.yml
+-rw-r--r--   0     1001      123      715 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/.gitignore
+-rw-r--r--   0     1001      123      757 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0     1001      123     7642 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/README.md
+-rw-r--r--   0     1001      123      360 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/benches/benchmark.rs
+-rw-r--r--   0     1001      123      396 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/benches/decode_from_file_bench.rs
+-rw-r--r--   0     1001      123      445 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/benches/decode_multiple_events_bench.rs
+-rw-r--r--   0     1001      123      436 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/benches/decode_single_event_bench.rs
+-rw-r--r--   0     1001      123      799 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/moss_decoder.pyi
+-rw-r--r--   0     1001      123      641 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/pyproject.toml
+-rw-r--r--   0     1001      123  4458776 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/python310.dll
+-rw-r--r--   0     1001      123    14906 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/src/decode_hits_fsm.rs
+-rw-r--r--   0     1001      123    11918 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/src/lib.rs
+-rw-r--r--   0     1001      123     1880 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/src/moss_protocol/moss_hit.rs
+-rw-r--r--   0     1001      123     1854 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/src/moss_protocol/moss_packet.rs
+-rw-r--r--   0     1001      123     2847 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/src/moss_protocol/test_util.rs
+-rw-r--r--   0     1001      123     2263 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/src/moss_protocol.rs
+-rw-r--r--   0     1001      123     1321 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/src/parse_error.rs
+-rw-r--r--   0     1001      123     3992 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/src/parse_util.rs
+-rwxr-xr-x   0     1001      123      435 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/tests/bench_dev_vs_prod.sh
+-rw-r--r--   0     1001      123     6433 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/tests/integration.py
+-rw-r--r--   0     1001      123    11186 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/tests/integration_test.rs
+-rw-r--r--   0     1001      123  9582576 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/tests/moss_noise.raw
+-rw-r--r--   0     1001      123      500 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/tests/moss_noise_0-499b.raw
+-rw-r--r--   0     1001      123      500 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/tests/moss_noise_500-999b.raw
+-rwxr-xr-x   0     1001      123     1190 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/tests/performance_dev_py.sh
+-rwxr-xr-x   0     1001      123      840 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/tests/performance_prod_py.sh
+-rw-r--r--   0     1001      123      954 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/tests/utils.sh
+-rw-r--r--   0     1001      123    24141 2023-08-01 13:36:44.000000 moss_decoder-0.5.1/Cargo.lock
+-rw-r--r--   0        0        0     8196 1970-01-01 00:00:00.000000 moss_decoder-0.5.1/PKG-INFO
```

### Comparing `moss_decoder-0.5.0/Cargo.toml` & `moss_decoder-0.5.1/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "moss_decoder"
-version = "0.5.0"
+version = "0.5.1"
 edition = "2021"
 authors = ["Marc Beck König <mbkj@tutamail.com>"]
 license = "MIT OR Apache-2.0"
 description = "Python module providing a decoder for the MOSS chip protocol."
 categories = ["python-module"]
```

### Comparing `moss_decoder-0.5.0/.CERN-gitlab-ci.yml` & `moss_decoder-0.5.1/.CERN-gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.0/.github/workflows/CI.yml` & `moss_decoder-0.5.1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.0/.gitignore` & `moss_decoder-0.5.1/.gitignore`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 /target
 dev-bench.md
 prod-bench.md
 
+
 # Byte-compiled / optimized / DLL files
 __pycache__/
 .pytest_cache/
 *.py[cod]
 
 # C extensions
 *.so
```

### Comparing `moss_decoder-0.5.0/.pre-commit-config.yaml` & `moss_decoder-0.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.0/README.md` & `moss_decoder-0.5.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # MOSS Decoder
 [![CI](https://github.com/CramBL/moss_decoder/actions/workflows/CI.yml/badge.svg)](https://github.com/CramBL/moss_decoder/actions/workflows/CI.yml)
+![PyPI - Version](https://img.shields.io/pypi/v/moss-decoder)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/moss-decoder)
+![PyPI - Implementation](https://img.shields.io/pypi/implementation/moss-decoder)
+
+![GitHub language count](https://img.shields.io/github/languages/count/crambl/moss_decoder)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/moss-decoder)
 ![GitHub commit activity (branch)](https://img.shields.io/github/commit-activity/m/crambl/moss_decoder)
 
 
-Python module implemented in Rust for high-performance decoding of readout data from the MOSS chip (Stitched Monolithic Pixel Sensor prototype).
+Python package implemented in Rust for high-performance decoding of readout data from the MOSS chip (Stitched Monolithic Pixel Sensor prototype).
 
 - [MOSS Decoder](#moss-decoder)
   - [Installation](#installation)
     - [Example](#example)
   - [Features](#features)
     - [3 types of functions are provided](#3-types-of-functions-are-provided)
   - [MOSS event data packet protocol FSM](#moss-event-data-packet-protocol-fsm)
@@ -40,87 +45,85 @@
 
 Two classes are provided: `MossPacket` & `MossHit`.
 
 ### 3 types of functions are provided
 ```python
 decode_event(arg: bytes)  -> tuple[MossPacket, int]: ...
 # allows decoding a single event from an iterable of bytes
-``` 
+```
 
 **Returns**: the decoded `MossPacket` and the index the *unit frame trailer* was found. Throws if no valid `MossPacket` is found.
-```python 
+```python
 decode_multiple_events(arg: bytes) -> tuple[list[MossPacket], int]: ...
-# returns as many `MossPacket`s as can be decoded from the bytes iterable. 
-# This is much more effecient than calling `decode_event` multiple times. 
-``` 
+# returns as many `MossPacket`s as can be decoded from the bytes iterable.
+# This is much more effecient than calling `decode_event` multiple times.
+```
 **Returns**: A list of `MossPacket`s and the index of the last observed *unit frame trailer*. Throws if no valid `MossPacket`s are found.
 
-```python 
+```python
 decode_from_file(arg: str | Path) -> list[MossPacket]: ...
-# takes a `Path` and returns as many `MossPacket` as can be decoded from file. 
+# takes a `Path` and returns as many `MossPacket` as can be decoded from file.
 # This is the most effecient way of decoding data from a file.
-``` 
+```
 **Returns**: A list of `MossPacket`s. Throws if the file is not found or no valid `MossPacket`s are found.
 
 
-Each function has a variant with a `_fsm`-suffix that uses an FSM based decoder, which is both faster and validates state transitions in the MOSS protocol. 
-
 ## MOSS event data packet protocol FSM
 The a MOSS half-unit event data packet follows the states seen in the FSM below. The region header state is simplified here.
 ```mermaid
 stateDiagram-v2
   frame_header : Unit Frame Header
   frame_trailer : Unit Frame Trailer
   region_header : Region Header
   data_0 : Data 0
   data_1 : Data 1
   data_2 : Data 2
   idle : Idle
 
     [*] --> frame_header
-    
+
     frame_header --> region_header
 
     region_header --> region_header
     region_header --> frame_trailer
     region_header --> DATA
 
     state DATA {
       direction LR
       [*] --> data_0
       data_0 --> data_1
       data_1 --> data_2
       data_2 --> data_0
       data_2 --> [*]
     }
-    
+
     DATA --> idle
     DATA --> region_header
     DATA --> frame_trailer
 
 
     idle --> DATA
     idle --> frame_trailer
 
     frame_trailer --> [*]
 
 ```
 
 ## MOSS event data packet decoder FSM
-The FSM based decoder uses the following FSM.
+The raw data is decoded using the following FSM.
 The `delimiter` is expected to be `0xFA`. The default `Idle` value `0xFF` is also assumed.
 
 ```mermaid
 stateDiagram-v2
 direction LR
   delimiter : Event Delimiter
   frame_header : Unit Frame Header
   frame_trailer : Unit Frame Trailer
 
-  
+
   [*] --> delimiter
   delimiter --> EVENT
   delimiter --> delimiter
 
   state EVENT {
 
     [*] --> frame_header
@@ -134,15 +137,15 @@
     HITS --> frame_trailer
 
     frame_trailer --> [*]
 
   }
 
 ```
-Decoding hits takes place with the FSM in the next section.
+The `EVENT` state is reached by finding decoding a Unit Frame Header and then the decoder enters the `HITS` substate which is depicted in the FSM in the next section.
 
 ## Event packet hit decoder FSM
 
 ```mermaid
 stateDiagram-v2
 
   region_header0 : Region Header 0
@@ -152,29 +155,34 @@
   data_0 : Data 0
   data_1 : Data 1
   data_2 : Data 2
   idle : Idle
 
   [*] --> region_header0
   region_header0 --> region_header1
+  region_header0 --> region_header2
+  region_header0 --> region_header3
   region_header0 --> DATA
+  region_header0 --> [*]
   DATA --> region_header1
   region_header1 --> region_header2
+  region_header1 --> region_header3
   region_header1 --> DATA
+  region_header1 --> [*]
   DATA --> region_header2
   region_header2 --> region_header3
   region_header2 --> DATA
+  region_header2 --> [*]
   DATA --> region_header3
   region_header3 --> DATA
   DATA --> [*]
   region_header3 --> [*]
 
-  
+
     state DATA {
-      direction LR
       [*] --> data_0
       data_0 --> data_1
       data_1 --> data_2
       data_2 --> data_0
       data_2 --> idle
       idle --> [*]
       idle --> data_0
```

### Comparing `moss_decoder-0.5.0/moss_decoder.pyi` & `moss_decoder-0.5.1/moss_decoder.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -21,14 +21,9 @@
     hits: list[MossHit]
 
     def __init__(self, unit_id: int) -> MossPacket:
         self.unit_id = unit_id
         self.hits = []
 
 def decode_event(raw_bytes: bytes) -> tuple[MossPacket, int]: ...
-def decode_event_noexcept(raw_bytes: bytes) -> tuple[MossPacket, int]: ...
 def decode_multiple_events(raw_bytes: bytes) -> tuple[list[MossPacket], int]: ...
 def decode_from_file(path: str | Path) -> list[MossPacket]: ...
-
-def decode_event_fsm(raw_bytes: bytes) -> tuple[MossPacket, int]: ...
-def decode_multiple_events_fsm(raw_bytes: bytes) -> tuple[list[MossPacket], int]: ...
-def decode_from_file_fsm(path: str | Path) -> list[MossPacket]: ...
```

### Comparing `moss_decoder-0.5.0/pyproject.toml` & `moss_decoder-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.0/python310.dll` & `moss_decoder-0.5.1/python310.dll`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.0/src/moss_protocol/moss_hit.rs` & `moss_decoder-0.5.1/src/moss_protocol/moss_hit.rs`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.0/src/moss_protocol/moss_packet.rs` & `moss_decoder-0.5.1/src/moss_protocol/moss_packet.rs`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.0/src/moss_protocol.rs` & `moss_decoder-0.5.1/src/moss_protocol.rs`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,17 @@
+#![allow(dead_code)]
 //! Module containing the MOSS readout protocol and basic structures to analyze the data.
 pub mod moss_hit;
 pub mod moss_packet;
+pub mod test_util;
 pub use moss_hit::MossHit;
 pub use moss_packet::MossPacket;
 
+use std::ops::RangeInclusive;
+
 #[derive(Debug, PartialEq)]
 pub(crate) enum MossWord {
     Idle,
     UnitFrameHeader,
     UnitFrameTrailer,
     RegionHeader,
     Data0,
@@ -15,29 +19,33 @@
     Data2,
     Delimiter,
     ProtocolError,
 }
 
 impl MossWord {
     pub(super) const IDLE: u8 = 0xFF; // 1111_1111 (default)
-    pub(super) const UNIT_FRAME_HEADER: u8 = 0b1101_0000; // 1101_<unit_id[3:0]>
+                                      // pub(super) const UNIT_FRAME_HEADER_LOWEST_ID: u8 = 0b1101_0001; // 1101_<unit_id[3:0]>
     pub(super) const UNIT_FRAME_TRAILER: u8 = 0b1110_0000; // 1110_0000
     pub(super) const REGION_HEADER: u8 = 0b1100_0000; // 1100_00_<region_id[1:0]>
     pub(super) const DATA_0: u8 = 0b0000_0000; // 00_<hit_row_pos[8:3]>
     pub(super) const DATA_1: u8 = 0b0100_0000; // 01_<hit_row_pos[2:0]>_<hit_col_pos[8:6]>
     pub(super) const DATA_2: u8 = 0b1000_0000; // 10_<hit_col_pos[5:0]>
     pub(super) const DELIMITER: u8 = 0xFA; // subject to change (FPGA implementation detail)
+    pub(crate) const UNIT_FRAME_HEADER_RANGE: RangeInclusive<u8> = 0xD1..=0xDA;
+    pub(crate) const DATA_0_RANGE: RangeInclusive<u8> = 0..=0b0010_1000; // Max is 320 pixel on bottom regions
+    pub(crate) const DATA_1_RANGE: RangeInclusive<u8> = 0b0100_0000..=0b0111_1101; // Max is 320 pixel on bottom regions
+    pub(crate) const DATA_2_RANGE: RangeInclusive<u8> = 0b1000_0000..=0b1011_1111;
 
     pub fn from_byte(b: u8) -> MossWord {
         match b {
             // Exact matches
             Self::IDLE => MossWord::Idle,
             Self::UNIT_FRAME_TRAILER => MossWord::UnitFrameTrailer,
             six_msb if six_msb & 0xFC == Self::REGION_HEADER => MossWord::RegionHeader,
-            four_msb if four_msb & 0xF0 == Self::UNIT_FRAME_HEADER => MossWord::UnitFrameHeader,
+            four_msb if four_msb & 0xF0 == 0b1101_0000 => MossWord::UnitFrameHeader,
             Self::DELIMITER => Self::Delimiter,
             two_msb if two_msb & 0b1100_0000 == Self::DATA_0 => MossWord::Data0,
             two_msb if two_msb & 0b1100_0000 == Self::DATA_1 => MossWord::Data1,
             two_msb if two_msb & 0b1100_0000 == Self::DATA_2 => MossWord::Data2,
             _ => MossWord::ProtocolError,
         }
     }
```

### Comparing `moss_decoder-0.5.0/src/moss_protocol_nested_fsm.rs` & `moss_decoder-0.5.1/src/decode_hits_fsm.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,77 +1,68 @@
 //! Contains an FSM implementation of the MOSS data readout protocol
 #![allow(non_camel_case_types)]
 
 use crate::moss_protocol::MossWord;
+use crate::parse_error::ParseError;
+use crate::parse_error::ParseErrorKind;
 use crate::MossHit;
-use crate::MossPacket;
-
-/// Advances the iterator until a Unit Frame Header is encountered, saves the unit ID,
-/// and extracts the hits with the [extract_hits] function, before returning a MossPacket if one is found.
-#[inline]
-pub(crate) fn extract_packet<'a>(
-    mut bytes: &mut impl Iterator<Item = &'a u8>,
-) -> Option<MossPacket> {
-    let mut unit_id: Option<u8> = None;
-    for b in &mut bytes {
-        if (0xD0..=0xD9).contains(b) {
-            unit_id = Some(b & 0xF);
-            break;
-        }
-    }
-
-    unit_id.map(|unit_id| MossPacket {
-        unit_id,
-        hits: extract_hits(bytes).unwrap_or_else(|| Vec::with_capacity(0)),
-    })
-}
 
 sm::sm! {
 
     MossDataFSM {
-        InitialStates { _REGION_HEADER0_ }
+        InitialStates { _UNIT_FRAME_HEADER_ }
 
         _Data {
-            _REGION_HEADER0_ => DATA0_
+            REGION_HEADER0_ => DATA0_
             REGION_HEADER1_ => DATA0_
             REGION_HEADER2_ => DATA0_
             REGION_HEADER3_ => DATA0_
             DATA2_ => DATA0_
             IDLE_ => DATA0_
             DATA0_ => DATA1_
             DATA1_ => DATA2_
         }
 
         _Idle {
             DATA2_ => IDLE_
         }
 
         _RegionHeader0 {
-            _REGION_HEADER0_ => _REGION_HEADER0_
+            _UNIT_FRAME_HEADER_ => REGION_HEADER0_
         }
 
         _RegionHeader1 {
-            _REGION_HEADER0_ => REGION_HEADER1_
+            _UNIT_FRAME_HEADER_ => REGION_HEADER1_
+            REGION_HEADER0_ => REGION_HEADER1_
             DATA2_ => REGION_HEADER1_
             IDLE_ => REGION_HEADER1_
         }
 
         _RegionHeader2 {
+            _UNIT_FRAME_HEADER_ => REGION_HEADER2_
+            REGION_HEADER0_ => REGION_HEADER2_
             REGION_HEADER1_ => REGION_HEADER2_
             DATA2_ => REGION_HEADER2_
             IDLE_ => REGION_HEADER2_
         }
 
         _RegionHeader3 {
+            _UNIT_FRAME_HEADER_ => REGION_HEADER3_
+            REGION_HEADER0_ => REGION_HEADER3_
+            REGION_HEADER1_ => REGION_HEADER3_
             REGION_HEADER2_ => REGION_HEADER3_
             DATA2_ => REGION_HEADER3_
             IDLE_ => REGION_HEADER3_
         }
 
         _FrameTrailer {
+            _UNIT_FRAME_HEADER_ => FRAME_TRAILER_
+            REGION_HEADER0_ => FRAME_TRAILER_
+            REGION_HEADER1_ => FRAME_TRAILER_
+            REGION_HEADER2_ => FRAME_TRAILER_
             REGION_HEADER3_ => FRAME_TRAILER_
             DATA2_ => FRAME_TRAILER_
             IDLE_ => FRAME_TRAILER_
         }
     }
 }
 
@@ -83,49 +74,114 @@
 const REGION_HEADER2: u8 = 0xC2;
 const REGION_HEADER3: u8 = 0xC3;
 
 /// Take an iterator that should be advanced to the position after a unit frame header.
 /// Advances the iterator and decodes any observed hits until a Unit Frame Trailer is encountered at which point the iteration stops.
 /// Returns all the decoded [MossHit]s if any.
 #[inline]
-pub(crate) fn extract_hits<'a>(bytes: &mut impl Iterator<Item = &'a u8>) -> Option<Vec<MossHit>> {
-    let mut sm = MossDataFSM::Machine::new(_REGION_HEADER0_).as_enum();
+pub(crate) fn extract_hits<'a>(
+    bytes: &mut (impl Iterator<Item = &'a u8>
+              + std::iter::DoubleEndedIterator
+              + std::iter::ExactSizeIterator),
+) -> Result<Vec<MossHit>, ParseError> {
+    let total_bytes = bytes.len();
+    let mut sm = MossDataFSM::Machine::new(_UNIT_FRAME_HEADER_).as_enum();
     let mut hits = Vec::<MossHit>::new();
 
+    let mut is_trailer_seen = false;
     let mut current_region = 0xff;
 
-    for b in bytes {
+    for (i, b) in bytes.enumerate() {
         sm = match sm {
-            Initial_REGION_HEADER0_(st) => match *b {
-                REGION_HEADER0 => st.transition(_RegionHeader0).as_enum(),
-                _ => unreachable!("Expected Region Header 0, got: {b:#X}"),
+            Initial_UNIT_FRAME_HEADER_(st) => match *b {
+                REGION_HEADER0 => {
+                    current_region = 0;
+                    st.transition(_RegionHeader0).as_enum()
+                }
+                REGION_HEADER1 => {
+                    current_region = 1;
+                    st.transition(_RegionHeader1).as_enum()
+                }
+                REGION_HEADER2 => {
+                    current_region = 2;
+                    st.transition(_RegionHeader2).as_enum()
+                }
+                REGION_HEADER3 => {
+                    current_region = 3;
+                    st.transition(_RegionHeader3).as_enum()
+                }
+                MossWord::UNIT_FRAME_TRAILER => {
+                    is_trailer_seen = true;
+                    break;
+                }
+                _ => {
+                    return Err(ParseError::new(
+                        ParseErrorKind::ProtocolError,
+                        "Expected REGION_HEADER_{1-3}/UNIT_FRAME_TRAILER",
+                        i,
+                    ))
+                }
             },
-            _REGION_HEADER0_By_RegionHeader0(st) => match *b {
+            REGION_HEADER0_By_RegionHeader0(st) => match *b {
                 REGION_HEADER1 => {
                     current_region = 1;
                     st.transition(_RegionHeader1).as_enum()
                 }
-                0..=0b0011_1111 => {
+                REGION_HEADER2 => {
+                    current_region = 2;
+                    st.transition(_RegionHeader2).as_enum()
+                }
+                REGION_HEADER3 => {
+                    current_region = 3;
+                    st.transition(_RegionHeader3).as_enum()
+                }
+                b if MossWord::DATA_0_RANGE.contains(&b) => {
                     current_region = 0;
-                    add_data0(&mut hits, *b, current_region);
+                    add_data0(&mut hits, b, current_region);
                     st.transition(_Data).as_enum()
                 }
-                _ => unreachable!("Expected Region Header 1 or DATA 0, got: {b:#X}"),
+                MossWord::UNIT_FRAME_TRAILER => {
+                    is_trailer_seen = true;
+                    break;
+                }
+                _ => {
+                    return Err(ParseError::new(
+                        ParseErrorKind::ProtocolError,
+                        "Expected REGION_HEADER_{1-3}/DATA_0/UNIT_FRAME_TRAILER",
+                        i,
+                    ))
+                }
             },
             DATA0_By_Data(st) => {
-                add_data1(&mut hits, *b);
-                st.transition(_Data).as_enum()
+                if MossWord::DATA_1_RANGE.contains(b) {
+                    add_data1(&mut hits, *b);
+                    st.transition(_Data).as_enum()
+                } else {
+                    return Err(ParseError::new(
+                        ParseErrorKind::ProtocolError,
+                        "Expected DATA_1",
+                        i,
+                    ));
+                }
             }
             DATA1_By_Data(st) => {
-                add_data2(&mut hits, *b);
-                st.transition(_Data).as_enum()
+                if MossWord::DATA_2_RANGE.contains(b) {
+                    add_data2(&mut hits, *b);
+                    st.transition(_Data).as_enum()
+                } else {
+                    return Err(ParseError::new(
+                        ParseErrorKind::ProtocolError,
+                        "Expected DATA_2",
+                        i,
+                    ));
+                }
             }
             DATA2_By_Data(st) => match *b {
-                0..=0b0011_1111 => {
-                    add_data0(&mut hits, *b, current_region);
+                b if MossWord::DATA_0_RANGE.contains(&b) => {
+                    add_data0(&mut hits, b, current_region);
                     st.transition(_Data).as_enum()
                 }
                 MossWord::IDLE => st.transition(_Idle).as_enum(),
                 REGION_HEADER1 => {
                     current_region = 1;
                     st.transition(_RegionHeader1).as_enum()
                 }
@@ -133,86 +189,139 @@
                     current_region = 2;
                     st.transition(_RegionHeader2).as_enum()
                 }
                 REGION_HEADER3 => {
                     current_region = 3;
                     st.transition(_RegionHeader3).as_enum()
                 }
-                MossWord::UNIT_FRAME_TRAILER => break,
-
+                MossWord::UNIT_FRAME_TRAILER => {
+                    is_trailer_seen = true;
+                    break;
+                }
                 _ => {
-                    unreachable!("Expected Region Header 1-3, DATA 0, or IDLE, got: {b:#X}")
+                    return Err(ParseError::new(
+                        ParseErrorKind::ProtocolError,
+                        "Expected REGION_HEADER_{1-3}/DATA_0/IDLE/UNIT_FRAME_TRAILER",
+                        i,
+                    ))
                 }
             },
             IDLE_By_Idle(st) => match *b {
-                0..=0b0011_1111 => {
-                    add_data0(&mut hits, *b, 0);
+                b if MossWord::DATA_0_RANGE.contains(&b) => {
+                    add_data0(&mut hits, b, 0);
                     st.transition(_Data).as_enum()
                 }
                 REGION_HEADER1 => {
                     current_region = 1;
                     st.transition(_RegionHeader1).as_enum()
                 }
                 REGION_HEADER2 => {
                     current_region = 2;
                     st.transition(_RegionHeader2).as_enum()
                 }
                 REGION_HEADER3 => {
                     current_region = 3;
                     st.transition(_RegionHeader3).as_enum()
                 }
-                MossWord::UNIT_FRAME_TRAILER => break,
-
+                MossWord::UNIT_FRAME_TRAILER => {
+                    is_trailer_seen = true;
+                    break;
+                }
                 _ => {
-                    unreachable!("Expected Region Header 1-3, DATA 0, or IDLE, got: {b:#X}")
+                    return Err(ParseError::new(
+                        ParseErrorKind::ProtocolError,
+                        "Expected REGION_HEADER_{1-3}/DATA_0/IDLE/UNIT_FRAME_TRAILER",
+                        i,
+                    ))
                 }
             },
             REGION_HEADER1_By_RegionHeader1(st) => match *b {
                 REGION_HEADER2 => {
                     current_region = 2;
                     st.transition(_RegionHeader2).as_enum()
                 }
-                0..=0b0011_1111 => {
+                REGION_HEADER3 => {
+                    current_region = 3;
+                    st.transition(_RegionHeader3).as_enum()
+                }
+                b if MossWord::DATA_0_RANGE.contains(&b) => {
                     current_region = 1;
-                    add_data0(&mut hits, *b, current_region);
+                    add_data0(&mut hits, b, current_region);
                     st.transition(_Data).as_enum()
                 }
-                _ => unreachable!("Expected Region Header 2 or DATA 0, got: {b:#X}"),
+                MossWord::UNIT_FRAME_TRAILER => {
+                    is_trailer_seen = true;
+                    break;
+                }
+                _ => {
+                    return Err(ParseError::new(
+                        ParseErrorKind::ProtocolError,
+                        "Expected REGION_HEADER_{2-3}/DATA_0/UNIT_FRAME_TRAILER",
+                        i,
+                    ))
+                }
             },
             REGION_HEADER2_By_RegionHeader2(st) => match *b {
                 REGION_HEADER3 => {
                     current_region = 3;
                     st.transition(_RegionHeader3).as_enum()
                 }
-                0..=0b0011_1111 => {
+                b if MossWord::DATA_0_RANGE.contains(&b) => {
                     current_region = 2;
-                    add_data0(&mut hits, *b, current_region);
+                    add_data0(&mut hits, b, current_region);
                     st.transition(_Data).as_enum()
                 }
-                _ => unreachable!("Expected Region Header 3 or DATA 0, got: {b:#X}"),
+                MossWord::UNIT_FRAME_TRAILER => {
+                    is_trailer_seen = true;
+                    break;
+                }
+                _ => {
+                    return Err(ParseError::new(
+                        ParseErrorKind::ProtocolError,
+                        "Expected REGION_HEADER_3/DATA_0/UNIT_FRAME_TRAILER",
+                        i,
+                    ))
+                }
             },
             REGION_HEADER3_By_RegionHeader3(st) => match *b {
-                MossWord::UNIT_FRAME_TRAILER => break,
-                0..=0b0011_1111 => {
+                b if MossWord::DATA_0_RANGE.contains(&b) => {
                     current_region = 3;
-                    add_data0(&mut hits, *b, current_region);
+                    add_data0(&mut hits, b, current_region);
                     st.transition(_Data).as_enum()
                 }
-                _ => unreachable!("Expected Unit Frame Trailer or DATA 0, got: {b:#X}"),
+                MossWord::UNIT_FRAME_TRAILER => {
+                    is_trailer_seen = true;
+                    break;
+                }
+                _ => {
+                    return Err(ParseError::new(
+                        ParseErrorKind::ProtocolError,
+                        "Expected UNIT_FRAME_TRAILER/DATA_0/UNIT_FRAME_TRAILER",
+                        i,
+                    ))
+                }
             },
             FRAME_TRAILER_By_FrameTrailer(_) => {
                 unreachable!("State machine should have already been used at this point")
             }
         };
     }
 
-    if hits.is_empty() {
-        None
+    if is_trailer_seen {
+        if hits.is_empty() {
+            Ok(Vec::with_capacity(0))
+        } else {
+            Ok(hits)
+        }
     } else {
-        Some(hits)
+        Err(ParseError::new(
+            ParseErrorKind::EndOfBufferNoTrailer,
+            "Reached end with no UNIT_FRAME_TRAILER",
+            total_bytes - 1,
+        ))
     }
 }
 
 #[inline]
 fn add_data0(moss_hits: &mut Vec<MossHit>, data0: u8, region: u8) {
     moss_hits.push(MossHit {
         region,                            // region id
@@ -237,71 +346,38 @@
 #[inline]
 fn add_data2(moss_hits: &mut [MossHit], data2: u8) {
     moss_hits.last_mut().unwrap().column |= (data2 & 0x3F) as u16;
 }
 
 #[cfg(test)]
 mod tests {
-    use pretty_assertions::assert_eq;
-
     use super::*;
-
-    const IDLE: u8 = 0xFF;
-    const UNIT_FRAME_TRAILER: u8 = 0xE0;
-    const UNIT_FRAME_HEADER_0: u8 = 0xD0;
-    const REGION_HEADER_0: u8 = 0xC0;
-    const REGION_HEADER_1: u8 = 0xC1;
-    const REGION_HEADER_2: u8 = 0xC2;
-    const REGION_HEADER_3: u8 = 0xC3;
-    fn fake_event_simple() -> Vec<u8> {
-        vec![
-            UNIT_FRAME_HEADER_0,
-            REGION_HEADER_0,
-            // Hit row 2, col 8
-            0x00,
-            0x50,
-            0x88,
-            IDLE,
-            0x01,
-            0x50,
-            0x88,
-            REGION_HEADER_1,
-            // Hit row 301, col 433
-            0x25,
-            0x6E,
-            0xB1,
-            REGION_HEADER_2,
-            REGION_HEADER_3,
-            // Hit row 2, col 8
-            0x00,
-            0x50,
-            0x88,
-            UNIT_FRAME_TRAILER,
-        ]
-    }
+    use crate::moss_protocol::test_util::*;
+    use crate::rust_only::extract_packet;
+    use pretty_assertions::assert_eq;
 
     #[test]
     fn test_fsm() {
         //
         let event_data_packet = fake_event_simple();
         let slice = &event_data_packet;
 
         let mut byte_iter = slice.iter();
         let byte_count = byte_iter.len();
 
         let unit_id = loop {
             if let Some(val) = byte_iter.next() {
-                if (0xD0..=0xD9).contains(val) {
+                if MossWord::UNIT_FRAME_HEADER_RANGE.contains(val) {
                     break val & 0xF;
                 }
             }
         };
 
-        if let Some(hits) = extract_hits(&mut byte_iter) {
-            assert_eq!(unit_id, 0);
+        if let Ok(hits) = extract_hits(&mut byte_iter) {
+            assert_eq!(unit_id, 1);
             assert_eq!(hits.len(), 4);
             assert_eq!(byte_count - byte_iter.len() - 1, 18);
         } else {
             panic!("Decoding failed")
         }
     }
 
@@ -313,49 +389,60 @@
         let slice = &event_data_packet;
 
         let mut byte_iter = slice.iter();
         let byte_count = byte_iter.len();
 
         let unit_id = loop {
             if let Some(val) = byte_iter.next() {
-                if (0xD0..=0xD9).contains(val) {
+                if MossWord::UNIT_FRAME_HEADER_RANGE.contains(val) {
                     break val & 0xF;
                 }
             }
         };
 
-        if let Some(hits) = extract_hits(&mut byte_iter) {
-            assert_eq!(unit_id, 0);
+        if let Ok(hits) = extract_hits(&mut byte_iter) {
+            assert_eq!(unit_id, 1);
             assert_eq!(hits.len(), 4);
             assert_eq!(byte_count - byte_iter.len() - 1, 18);
         } else {
             panic!("Decoding failed")
         }
 
         let unit_id = loop {
             if let Some(val) = byte_iter.next() {
-                if (0xD0..=0xD9).contains(val) {
+                if MossWord::UNIT_FRAME_HEADER_RANGE.contains(val) {
                     break val & 0xF;
                 }
             }
         };
 
-        if let Some(hits) = extract_hits(&mut byte_iter) {
-            assert_eq!(unit_id, 0);
+        if let Ok(hits) = extract_hits(&mut byte_iter) {
+            assert_eq!(unit_id, 1);
             assert_eq!(hits.len(), 4);
             assert_eq!(byte_count - byte_iter.len() - 1, 37);
         } else {
             panic!("Decoding failed")
         }
     }
 
     #[test]
     fn test_extract_packet() {
         let packet = fake_event_simple();
-        let slice = packet.as_slice();
-        let mut packet_iter = slice.iter();
-        let p = extract_packet(&mut packet_iter);
+        let p = extract_packet(&packet);
         println!("{p:?}");
-        assert!(p.is_some());
-        assert_eq!(p.unwrap().hits.len(), 4);
+        assert!(p.is_ok());
+        let (p, trailer_idx) = p.unwrap();
+        assert_eq!(p.hits.len(), 4);
+        assert_eq!(trailer_idx, 18);
+    }
+
+    #[test]
+    fn test_protocol_error() {
+        let packet = fake_event_protocol_error();
+
+        if let Err(e) = extract_packet(&packet) {
+            println!("{e:?}");
+        } else {
+            panic!("Expected error, got OK")
+        }
     }
 }
```

### Comparing `moss_decoder-0.5.0/tests/integration.py` & `moss_decoder-0.5.1/tests/integration.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Integration tests. Uses the `moss_decoder` package
 from python and allows benchmarks."""
 import sys  # Don't want to depend on `argparse`
 import time
 from pathlib import Path
 import moss_decoder
 from moss_decoder import MossPacket, MossHit
-from moss_decoder import decode_event, decode_event_noexcept
+from moss_decoder import decode_event
 
 FILE_PATH = Path("tests/moss_noise.raw")
 
 
 def read_bytes_from_file(file_path: Path) -> bytes:
     """Open file at `file_path` and read as binary, return `bytes`"""
     with open(file_path, "rb") as readout_file:
@@ -17,70 +17,60 @@
 
     return raw_bytes
 
 
 def make_simple_moss_event_packet() -> bytes:
     """Make a complete simple MOSS packet containing
     Unit 0 and 1 hit in region 1 row 2 col 8"""
-    unit_frame_header_0 = b"\xD0"
+    unit_frame_header_1 = b"\xD1"
     padding = b"\xFA"
     unit_frame_trailer = b"\xE0"
     region_header_0 = b"\xC0"
     region_header_1 = b"\xC1"
     region_header_2 = b"\xC2"
     region_header_3 = b"\xC3"
     data_0 = b"\x00"
     data_1 = b"\x50"  # row 2
     data_2 = b"\x88"  # col 8
 
     simple_packet = (
-        unit_frame_header_0
+        unit_frame_header_1
         + region_header_0
         + region_header_1
         + data_0
         + data_1
         + data_2
         + region_header_2
         + region_header_3
         + unit_frame_trailer
         + padding
     )
     return simple_packet
 
 
-def decode_multi_event(raw_bytes: bytes, fsm: bool = False) -> tuple[list["MossPacket"], int]:
+def decode_multi_event(raw_bytes: bytes) -> tuple[list["MossPacket"], int]:
     """Takes `bytes` and decodes it as `MossPacket`s.
     returns a tuple of `list[MossPackets]` and an int that indicates the
     index where the last MOSS trailer was seen
     """
-    if fsm is True:
-        packets, last_trailer_idx = moss_decoder.decode_multiple_events_fsm(
-        raw_bytes)
-    else:
-        packets, last_trailer_idx = moss_decoder.decode_multiple_events(
-        raw_bytes)
+    packets, last_trailer_idx = moss_decoder.decode_multiple_events(raw_bytes)
 
     return packets, last_trailer_idx
 
 
-def test_decode_multi_event(fsm: bool = False):
+def test_decode_multi_event():
     """Test that multiple events are correctly decoded from raw bytes"""
-    print(
-        (
-            "=== Test that multiple events"
-            "are correctly decoded from raw bytes ==="
-        )
-    )
+    print("=== Test multiple events are correctly decoded from raw bytes ===")
     raw_bytes = read_bytes_from_file(FILE_PATH)
     byte_count = len(raw_bytes)
     last_byte_idx = byte_count - 1
 
     print(f"Read {byte_count} bytes")
 
-    packets, last_trailer_idx = decode_multi_event(raw_bytes=raw_bytes, fsm=fsm)
+    packets, last_trailer_idx = decode_multi_event(raw_bytes=raw_bytes)
 
     print(f"Decoded {len(packets)} packets")
 
     print(f"Last trailer at index: {last_trailer_idx}/{last_byte_idx}")
     remainder_count = last_byte_idx - last_trailer_idx
     print(f"Remainder: {remainder_count} byte(s)")
 
@@ -112,56 +102,43 @@
         print(f"\t\tHit region: {hit.region}")
         print(f"\t\tHit row: {hit.row}")
         print(f"\t\tHit column: {hit.column}")
 
     print("==> Test OK\n\n")
 
 
-def test_100k_single_decodes(noexcept=False):
+def test_100k_single_decodes():
     """Tests 100k calls to decode_event (single event decoding)"""
 
-    if noexcept:
-        print(("=== Test 100k calls to decode_event with noexcept ==="))
-    else:
-        print(("=== Test 100k calls to decode_event ==="))
+    print(("=== Test 100k calls to decode_event ==="))
 
     raw_bytes = read_bytes_from_file(FILE_PATH)
     byte_count = len(raw_bytes)
     last_byte_idx = byte_count - 1
 
     print(f"Read {byte_count} bytes")
 
     packets = []
     last_trailer_idx = 0
 
-    if noexcept is False:
-        more_data = True
-        while more_data:
-            try:
-                pack, tmp_trailer_idx = moss_decoder.decode_event(
-                    raw_bytes[last_trailer_idx:]
-                )
-                packets.append(pack)
-                last_trailer_idx = last_trailer_idx + tmp_trailer_idx + 1
-            except ValueError as exc:
-                print(f"Decode event returned value error: {exc}")
-                more_data = False
-            except AssertionError as exc:
-                print(f"Decode event returned assertion error: {exc}")
-                more_data = False
-                raise exc
-
-    if noexcept is True:
-        res = 1
-        packets = []
-        while res != 0:
-            packet, res = decode_event_noexcept(raw_bytes[last_trailer_idx:])
-            if res != 0:
-                last_trailer_idx = last_trailer_idx + res + 1
-                packets.append(packet)
+    more_data = True
+    while more_data:
+        try:
+            pack, tmp_trailer_idx = moss_decoder.decode_event(
+                raw_bytes[last_trailer_idx:]
+            )
+            packets.append(pack)
+            last_trailer_idx = last_trailer_idx + tmp_trailer_idx + 1
+        except ValueError as exc:
+            print(f"Decode event returned value error: {exc}")
+            more_data = False
+        except AssertionError as exc:
+            print(f"Decode event returned assertion error: {exc}")
+            more_data = False
+            raise exc
 
     last_trailer_idx = last_trailer_idx - 1
 
     print(f"Decoded {len(packets)} packets")
     print(f"Last trailer at index: {last_trailer_idx}/{last_byte_idx}")
     remainder_count = last_byte_idx - last_trailer_idx
     print(f"Remainder: {remainder_count} byte(s)")
@@ -222,18 +199,13 @@
 
     test_fundamental_class_comparisons()
 
     start = time.time()
     test_decode_multi_event()
     print(f"Done in: {time.time()-start:.3f} s\n")
     start = time.time()
-    test_decode_multi_event(fsm=True)
-    print(f"Done in: {time.time()-start:.3f} s\n")
-    start = time.time()
     test_moss_packet_print()
     print(f"Done in: {time.time()-start:.3f} s\n")
     start = time.time()
     test_100k_single_decodes()
     print(f"Done in: {time.time()-start:.3f} s\n")
     start = time.time()
-    test_100k_single_decodes(noexcept=True)
-    print(f"Done in: {time.time()-start:.3f} s\n")
```

### Comparing `moss_decoder-0.5.0/tests/moss_noise.raw` & `moss_decoder-0.5.1/tests/moss_noise.raw`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.0/tests/performance_dev_py.sh` & `moss_decoder-0.5.1/tests/performance_dev_py.sh`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.0/tests/performance_prod_py.sh` & `moss_decoder-0.5.1/tests/performance_prod_py.sh`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     python -m pip install moss-decoder --upgrade --no-cache-dir --force-reinstall
 
     # Show installed packages
     python -m pip freeze
 
     cargo install hyperfine --locked
 
+    # Run benchmark
     hyperfine \
         "${BENCH_CMD}"\
         --warmup 3\
         --style full\
         --time-unit millisecond\
         --shell=bash\
         --export-markdown prod-bench.md
```

### Comparing `moss_decoder-0.5.0/tests/utils.sh` & `moss_decoder-0.5.1/tests/utils.sh`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/bin/bash
 
 export SCRIPT_PATH="tests/integration.py"
 export BENCH_CMD="python ${SCRIPT_PATH} benchmark"
+export BENCH_CMD_FSM="python ${SCRIPT_PATH} benchmark-fsm"
 
 export TXT_CLEAR="\e[0m"
 
 export TXT_YELLOW="\e[33m"
 function println_yellow {
     printf  "\e[33m%b\e[0m\n" "${1}"
 }
```

### Comparing `moss_decoder-0.5.0/Cargo.lock` & `moss_decoder-0.5.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -323,15 +323,15 @@
 checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "moss_decoder"
-version = "0.5.0"
+version = "0.5.1"
 dependencies = [
  "criterion",
  "pretty_assertions",
  "pyo3",
  "sm",
 ]
```

### Comparing `moss_decoder-0.5.0/PKG-INFO` & `moss_decoder-0.5.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 Metadata-Version: 2.1
 Name: moss_decoder
-Version: 0.5.0
+Version: 0.5.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Python package implemented in Rust to decode MOSS readout data
 Author: Marc Beck König
 Author-email: marc.beck.konig@cern.ch
 Maintainer-email: Marc Beck König <marc.beck.konig@cern.ch>
 License: MIT OR Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # MOSS Decoder
 [![CI](https://github.com/CramBL/moss_decoder/actions/workflows/CI.yml/badge.svg)](https://github.com/CramBL/moss_decoder/actions/workflows/CI.yml)
+![PyPI - Version](https://img.shields.io/pypi/v/moss-decoder)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/moss-decoder)
+![PyPI - Implementation](https://img.shields.io/pypi/implementation/moss-decoder)
+
+![GitHub language count](https://img.shields.io/github/languages/count/crambl/moss_decoder)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/moss-decoder)
 ![GitHub commit activity (branch)](https://img.shields.io/github/commit-activity/m/crambl/moss_decoder)
 
 
-Python module implemented in Rust for high-performance decoding of readout data from the MOSS chip (Stitched Monolithic Pixel Sensor prototype).
+Python package implemented in Rust for high-performance decoding of readout data from the MOSS chip (Stitched Monolithic Pixel Sensor prototype).
 
 - [MOSS Decoder](#moss-decoder)
   - [Installation](#installation)
     - [Example](#example)
   - [Features](#features)
     - [3 types of functions are provided](#3-types-of-functions-are-provided)
   - [MOSS event data packet protocol FSM](#moss-event-data-packet-protocol-fsm)
@@ -54,87 +59,85 @@
 
 Two classes are provided: `MossPacket` & `MossHit`.
 
 ### 3 types of functions are provided
 ```python
 decode_event(arg: bytes)  -> tuple[MossPacket, int]: ...
 # allows decoding a single event from an iterable of bytes
-``` 
+```
 
 **Returns**: the decoded `MossPacket` and the index the *unit frame trailer* was found. Throws if no valid `MossPacket` is found.
-```python 
+```python
 decode_multiple_events(arg: bytes) -> tuple[list[MossPacket], int]: ...
-# returns as many `MossPacket`s as can be decoded from the bytes iterable. 
-# This is much more effecient than calling `decode_event` multiple times. 
-``` 
+# returns as many `MossPacket`s as can be decoded from the bytes iterable.
+# This is much more effecient than calling `decode_event` multiple times.
+```
 **Returns**: A list of `MossPacket`s and the index of the last observed *unit frame trailer*. Throws if no valid `MossPacket`s are found.
 
-```python 
+```python
 decode_from_file(arg: str | Path) -> list[MossPacket]: ...
-# takes a `Path` and returns as many `MossPacket` as can be decoded from file. 
+# takes a `Path` and returns as many `MossPacket` as can be decoded from file.
 # This is the most effecient way of decoding data from a file.
-``` 
+```
 **Returns**: A list of `MossPacket`s. Throws if the file is not found or no valid `MossPacket`s are found.
 
 
-Each function has a variant with a `_fsm`-suffix that uses an FSM based decoder, which is both faster and validates state transitions in the MOSS protocol. 
-
 ## MOSS event data packet protocol FSM
 The a MOSS half-unit event data packet follows the states seen in the FSM below. The region header state is simplified here.
 ```mermaid
 stateDiagram-v2
   frame_header : Unit Frame Header
   frame_trailer : Unit Frame Trailer
   region_header : Region Header
   data_0 : Data 0
   data_1 : Data 1
   data_2 : Data 2
   idle : Idle
 
     [*] --> frame_header
-    
+
     frame_header --> region_header
 
     region_header --> region_header
     region_header --> frame_trailer
     region_header --> DATA
 
     state DATA {
       direction LR
       [*] --> data_0
       data_0 --> data_1
       data_1 --> data_2
       data_2 --> data_0
       data_2 --> [*]
     }
-    
+
     DATA --> idle
     DATA --> region_header
     DATA --> frame_trailer
 
 
     idle --> DATA
     idle --> frame_trailer
 
     frame_trailer --> [*]
 
 ```
 
 ## MOSS event data packet decoder FSM
-The FSM based decoder uses the following FSM.
+The raw data is decoded using the following FSM.
 The `delimiter` is expected to be `0xFA`. The default `Idle` value `0xFF` is also assumed.
 
 ```mermaid
 stateDiagram-v2
 direction LR
   delimiter : Event Delimiter
   frame_header : Unit Frame Header
   frame_trailer : Unit Frame Trailer
 
-  
+
   [*] --> delimiter
   delimiter --> EVENT
   delimiter --> delimiter
 
   state EVENT {
 
     [*] --> frame_header
@@ -148,15 +151,15 @@
     HITS --> frame_trailer
 
     frame_trailer --> [*]
 
   }
 
 ```
-Decoding hits takes place with the FSM in the next section.
+The `EVENT` state is reached by finding decoding a Unit Frame Header and then the decoder enters the `HITS` substate which is depicted in the FSM in the next section.
 
 ## Event packet hit decoder FSM
 
 ```mermaid
 stateDiagram-v2
 
   region_header0 : Region Header 0
@@ -166,29 +169,34 @@
   data_0 : Data 0
   data_1 : Data 1
   data_2 : Data 2
   idle : Idle
 
   [*] --> region_header0
   region_header0 --> region_header1
+  region_header0 --> region_header2
+  region_header0 --> region_header3
   region_header0 --> DATA
+  region_header0 --> [*]
   DATA --> region_header1
   region_header1 --> region_header2
+  region_header1 --> region_header3
   region_header1 --> DATA
+  region_header1 --> [*]
   DATA --> region_header2
   region_header2 --> region_header3
   region_header2 --> DATA
+  region_header2 --> [*]
   DATA --> region_header3
   region_header3 --> DATA
   DATA --> [*]
   region_header3 --> [*]
 
-  
+
     state DATA {
-      direction LR
       [*] --> data_0
       data_0 --> data_1
       data_1 --> data_2
       data_2 --> data_0
       data_2 --> idle
       idle --> [*]
       idle --> data_0
```

