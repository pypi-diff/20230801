# Comparing `tmp/typos-1.16.1.tar.gz` & `tmp/typos-1.16.2.tar.gz`

## Comparing `typos-1.16.1.tar` & `typos-1.16.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      704 1970-01-01 00:00:00.000000 typos-1.16.1/local_dependencies/typos/Cargo.toml
--rw-r--r--   0     1001      123     2794 2023-07-14 19:29:01.000000 typos-1.16.1/local_dependencies/typos/src/check.rs
--rw-r--r--   0     1001      123     2175 2023-07-14 19:29:01.000000 typos-1.16.1/local_dependencies/typos/src/dict.rs
--rw-r--r--   0     1001      123       74 2023-07-14 19:29:01.000000 typos-1.16.1/local_dependencies/typos/src/lib.rs
--rw-r--r--   0     1001      123    46000 2023-07-14 19:29:01.000000 typos-1.16.1/local_dependencies/typos/src/tokens.rs
--rw-r--r--   0        0        0      656 1970-01-01 00:00:00.000000 typos-1.16.1/local_dependencies/varcon-core/Cargo.toml
--rw-r--r--   0     1001      123     1488 2023-07-14 19:29:01.000000 typos-1.16.1/local_dependencies/varcon-core/src/borrowed.rs
--rw-r--r--   0     1001      123     2850 2023-07-14 19:29:01.000000 typos-1.16.1/local_dependencies/varcon-core/src/lib.rs
--rw-r--r--   0     1001      123    18950 2023-07-14 19:29:01.000000 typos-1.16.1/local_dependencies/varcon-core/src/parser.rs
--rw-r--r--   0        0        0      549 1970-01-01 00:00:00.000000 typos-1.16.1/local_dependencies/typos-dict/Cargo.toml
--rw-r--r--   0     1001      123  7035769 2023-07-14 19:29:01.000000 typos-1.16.1/local_dependencies/typos-dict/src/dict_codegen.rs
--rw-r--r--   0     1001      123       51 2023-07-14 19:29:01.000000 typos-1.16.1/local_dependencies/typos-dict/src/lib.rs
--rw-r--r--   0        0        0      761 1970-01-01 00:00:00.000000 typos-1.16.1/local_dependencies/dictgen/Cargo.toml
--rw-r--r--   0     1001      123      130 2023-07-14 19:29:01.000000 typos-1.16.1/local_dependencies/dictgen/src/lib.rs
--rw-r--r--   0     1001      123     2687 2023-07-14 19:29:01.000000 typos-1.16.1/local_dependencies/dictgen/src/map.rs
--rw-r--r--   0     1001      123     3726 2023-07-14 19:29:01.000000 typos-1.16.1/local_dependencies/dictgen/src/table.rs
--rw-r--r--   0     1001      123    10637 2023-07-14 19:29:01.000000 typos-1.16.1/local_dependencies/dictgen/src/trie.rs
--rw-r--r--   0        0        0      631 1970-01-01 00:00:00.000000 typos-1.16.1/local_dependencies/typos-vars/Cargo.toml
--rw-r--r--   0     1001      123      117 2023-07-14 19:29:01.000000 typos-1.16.1/local_dependencies/typos-vars/src/lib.rs
--rw-r--r--   0     1001      123  6086180 2023-07-14 19:29:01.000000 typos-1.16.1/local_dependencies/typos-vars/src/vars_codegen.rs
--rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 typos-1.16.1/pyproject.toml
--rw-r--r--   0        0        0     3037 1970-01-01 00:00:00.000000 typos-1.16.1/rust_src/typos-cli/Cargo.toml
--rw-r--r--   0     1001      123     2221 2023-07-14 19:29:01.000000 typos-1.16.1/rust_src/typos-cli/benches/checks.rs
--rw-r--r--   0     1001      123     4586 2023-07-14 19:29:01.000000 typos-1.16.1/rust_src/typos-cli/benches/corrections.rs
--rw-r--r--   0     1001      123     1347 2023-07-14 19:29:01.000000 typos-1.16.1/rust_src/typos-cli/benches/data.rs
--rw-r--r--   0     1001      123     3306 2023-07-14 19:29:01.000000 typos-1.16.1/rust_src/typos-cli/benches/tokenize.rs
--rw-r--r--   0     1001      123     8452 2023-07-14 19:29:01.000000 typos-1.16.1/rust_src/typos-cli/src/bin/typos-cli/args.rs
--rw-r--r--   0     1001      123     9824 2023-07-14 19:29:01.000000 typos-1.16.1/rust_src/typos-cli/src/bin/typos-cli/main.rs
--rw-r--r--   0     1001      123    12622 2023-07-14 19:29:01.000000 typos-1.16.1/rust_src/typos-cli/src/bin/typos-cli/report.rs
--rw-r--r--   0     1001      123    21859 2023-07-14 19:29:01.000000 typos-1.16.1/rust_src/typos-cli/src/config.rs
--rw-r--r--   0     1001      123    10240 2023-07-14 19:29:01.000000 typos-1.16.1/rust_src/typos-cli/src/default_types.rs
--rw-r--r--   0     1001      123    11574 2023-07-14 19:29:01.000000 typos-1.16.1/rust_src/typos-cli/src/dict.rs
--rw-r--r--   0     1001      123    32621 2023-07-14 19:29:01.000000 typos-1.16.1/rust_src/typos-cli/src/file.rs
--rw-r--r--   0     1001      123     6791 2023-07-14 19:29:01.000000 typos-1.16.1/rust_src/typos-cli/src/file_type.rs
--rw-r--r--   0     1001      123      299 2023-07-14 19:29:01.000000 typos-1.16.1/rust_src/typos-cli/src/lib.rs
--rw-r--r--   0     1001      123    17558 2023-07-14 19:29:01.000000 typos-1.16.1/rust_src/typos-cli/src/policy.rs
--rw-r--r--   0     1001      123     5561 2023-07-14 19:29:01.000000 typos-1.16.1/rust_src/typos-cli/src/report.rs
--rw-r--r--   0     1001      123      207 2023-07-14 19:29:01.000000 typos-1.16.1/rust_src/typos-cli/tests/cmd/false-positives.in/README.md
--rw-r--r--   0     1001      123    53691 2023-07-14 19:29:01.000000 typos-1.16.1/Cargo.lock
--rw-r--r--   0        0        0     5371 1970-01-01 00:00:00.000000 typos-1.16.1/PKG-INFO
+-rw-r--r--   0        0        0      631 1970-01-01 00:00:00.000000 typos-1.16.2/local_dependencies/typos-vars/Cargo.toml
+-rw-r--r--   0     1001      123      117 2023-08-01 15:48:27.000000 typos-1.16.2/local_dependencies/typos-vars/src/lib.rs
+-rw-r--r--   0     1001      123  6086180 2023-08-01 15:48:27.000000 typos-1.16.2/local_dependencies/typos-vars/src/vars_codegen.rs
+-rw-r--r--   0        0        0      761 1970-01-01 00:00:00.000000 typos-1.16.2/local_dependencies/dictgen/Cargo.toml
+-rw-r--r--   0     1001      123      130 2023-08-01 15:48:27.000000 typos-1.16.2/local_dependencies/dictgen/src/lib.rs
+-rw-r--r--   0     1001      123     2687 2023-08-01 15:48:27.000000 typos-1.16.2/local_dependencies/dictgen/src/map.rs
+-rw-r--r--   0     1001      123     3726 2023-08-01 15:48:27.000000 typos-1.16.2/local_dependencies/dictgen/src/table.rs
+-rw-r--r--   0     1001      123    10637 2023-08-01 15:48:27.000000 typos-1.16.2/local_dependencies/dictgen/src/trie.rs
+-rw-r--r--   0        0        0      656 1970-01-01 00:00:00.000000 typos-1.16.2/local_dependencies/varcon-core/Cargo.toml
+-rw-r--r--   0     1001      123     1488 2023-08-01 15:48:27.000000 typos-1.16.2/local_dependencies/varcon-core/src/borrowed.rs
+-rw-r--r--   0     1001      123     2850 2023-08-01 15:48:27.000000 typos-1.16.2/local_dependencies/varcon-core/src/lib.rs
+-rw-r--r--   0     1001      123    18950 2023-08-01 15:48:27.000000 typos-1.16.2/local_dependencies/varcon-core/src/parser.rs
+-rw-r--r--   0        0        0      704 1970-01-01 00:00:00.000000 typos-1.16.2/local_dependencies/typos/Cargo.toml
+-rw-r--r--   0     1001      123     2794 2023-08-01 15:48:27.000000 typos-1.16.2/local_dependencies/typos/src/check.rs
+-rw-r--r--   0     1001      123     2175 2023-08-01 15:48:27.000000 typos-1.16.2/local_dependencies/typos/src/dict.rs
+-rw-r--r--   0     1001      123       74 2023-08-01 15:48:27.000000 typos-1.16.2/local_dependencies/typos/src/lib.rs
+-rw-r--r--   0     1001      123    46000 2023-08-01 15:48:27.000000 typos-1.16.2/local_dependencies/typos/src/tokens.rs
+-rw-r--r--   0        0        0      549 1970-01-01 00:00:00.000000 typos-1.16.2/local_dependencies/typos-dict/Cargo.toml
+-rw-r--r--   0     1001      123  7038674 2023-08-01 15:48:27.000000 typos-1.16.2/local_dependencies/typos-dict/src/dict_codegen.rs
+-rw-r--r--   0     1001      123       51 2023-08-01 15:48:27.000000 typos-1.16.2/local_dependencies/typos-dict/src/lib.rs
+-rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 typos-1.16.2/pyproject.toml
+-rw-r--r--   0        0        0     3037 1970-01-01 00:00:00.000000 typos-1.16.2/rust_src/typos-cli/Cargo.toml
+-rw-r--r--   0     1001      123     2221 2023-08-01 15:48:27.000000 typos-1.16.2/rust_src/typos-cli/benches/checks.rs
+-rw-r--r--   0     1001      123     4586 2023-08-01 15:48:27.000000 typos-1.16.2/rust_src/typos-cli/benches/corrections.rs
+-rw-r--r--   0     1001      123     1347 2023-08-01 15:48:27.000000 typos-1.16.2/rust_src/typos-cli/benches/data.rs
+-rw-r--r--   0     1001      123     3306 2023-08-01 15:48:27.000000 typos-1.16.2/rust_src/typos-cli/benches/tokenize.rs
+-rw-r--r--   0     1001      123     8452 2023-08-01 15:48:27.000000 typos-1.16.2/rust_src/typos-cli/src/bin/typos-cli/args.rs
+-rw-r--r--   0     1001      123     9824 2023-08-01 15:48:27.000000 typos-1.16.2/rust_src/typos-cli/src/bin/typos-cli/main.rs
+-rw-r--r--   0     1001      123    12622 2023-08-01 15:48:27.000000 typos-1.16.2/rust_src/typos-cli/src/bin/typos-cli/report.rs
+-rw-r--r--   0     1001      123    21859 2023-08-01 15:48:27.000000 typos-1.16.2/rust_src/typos-cli/src/config.rs
+-rw-r--r--   0     1001      123    10240 2023-08-01 15:48:27.000000 typos-1.16.2/rust_src/typos-cli/src/default_types.rs
+-rw-r--r--   0     1001      123    11574 2023-08-01 15:48:27.000000 typos-1.16.2/rust_src/typos-cli/src/dict.rs
+-rw-r--r--   0     1001      123    32621 2023-08-01 15:48:27.000000 typos-1.16.2/rust_src/typos-cli/src/file.rs
+-rw-r--r--   0     1001      123     6791 2023-08-01 15:48:27.000000 typos-1.16.2/rust_src/typos-cli/src/file_type.rs
+-rw-r--r--   0     1001      123      299 2023-08-01 15:48:27.000000 typos-1.16.2/rust_src/typos-cli/src/lib.rs
+-rw-r--r--   0     1001      123    17558 2023-08-01 15:48:27.000000 typos-1.16.2/rust_src/typos-cli/src/policy.rs
+-rw-r--r--   0     1001      123     5561 2023-08-01 15:48:27.000000 typos-1.16.2/rust_src/typos-cli/src/report.rs
+-rw-r--r--   0     1001      123      207 2023-08-01 15:48:27.000000 typos-1.16.2/rust_src/typos-cli/tests/cmd/false-positives.in/README.md
+-rw-r--r--   0     1001      123    53691 2023-08-01 15:48:27.000000 typos-1.16.2/Cargo.lock
+-rw-r--r--   0        0        0     5436 1970-01-01 00:00:00.000000 typos-1.16.2/PKG-INFO
```

### Comparing `typos-1.16.1/local_dependencies/typos/Cargo.toml` & `typos-1.16.2/local_dependencies/typos/Cargo.toml`

 * *Files identical despite different names*

### Comparing `typos-1.16.1/local_dependencies/typos/src/check.rs` & `typos-1.16.2/local_dependencies/typos/src/check.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.1/local_dependencies/typos/src/dict.rs` & `typos-1.16.2/local_dependencies/typos/src/dict.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.1/local_dependencies/typos/src/tokens.rs` & `typos-1.16.2/local_dependencies/typos/src/tokens.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.1/local_dependencies/varcon-core/Cargo.toml` & `typos-1.16.2/local_dependencies/varcon-core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `typos-1.16.1/local_dependencies/varcon-core/src/borrowed.rs` & `typos-1.16.2/local_dependencies/varcon-core/src/borrowed.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.1/local_dependencies/varcon-core/src/lib.rs` & `typos-1.16.2/local_dependencies/varcon-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.1/local_dependencies/varcon-core/src/parser.rs` & `typos-1.16.2/local_dependencies/varcon-core/src/parser.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.1/local_dependencies/typos-dict/Cargo.toml` & `typos-1.16.2/local_dependencies/typos-dict/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "typos-dict"
-version = "0.10.7"
+version = "0.10.8"
 description = "Source Code Spelling Correction"
 readme = "../../README.md"
 categories = ["development-tools", "text-processing"]
 keywords = ["development", "spelling"]
 license= "MIT OR Apache-2.0"
 repository= "https://github.com/crate-ci/typos"
 edition= "2021"
```

### Comparing `typos-1.16.1/local_dependencies/typos-dict/src/dict_codegen.rs` & `typos-1.16.2/local_dependencies/typos-dict/src/dict_codegen.rs`

 * *Files 0% similar despite different names*

```diff
@@ -903,14 +903,15 @@
         dictgen::InsensitiveStr::Ascii("techetque"),
         dictgen::InsensitiveStr::Ascii("ted"),
         dictgen::InsensitiveStr::Ascii("teing"),
         dictgen::InsensitiveStr::Ascii("ten"),
         dictgen::InsensitiveStr::Ascii("tet"),
         dictgen::InsensitiveStr::Ascii("tewr"),
         dictgen::InsensitiveStr::Ascii("tingm"),
+        dictgen::InsensitiveStr::Ascii("tre"),
         dictgen::InsensitiveStr::Ascii("tte"),
         dictgen::InsensitiveStr::Ascii("tter"),
         dictgen::InsensitiveStr::Ascii("tters"),
         dictgen::InsensitiveStr::Ascii("ttin"),
         dictgen::InsensitiveStr::Ascii("tting"),
         dictgen::InsensitiveStr::Ascii("ttten"),
     ],
@@ -920,14 +921,15 @@
         &["writecheque"],
         &["wrote", "written", "write", "writer"],
         &["writing"],
         &["written"],
         &["writes"],
         &["writer"],
         &["writing"],
+        &["writer"],
         &["write", "written"],
         &["writer", "written"],
         &["writers"],
         &["written", "writing"],
         &["writing"],
         &["written"],
     ],
@@ -1201,17 +1203,20 @@
 
 static WORD_WORR_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_WORR_CHILDREN),
     value: None,
 };
 
 pub static WORD_WORR_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
-    keys: &[dictgen::InsensitiveStr::Ascii("ry")],
-    values: &[&["worry"]],
-    range: 2..=2,
+    keys: &[
+        dictgen::InsensitiveStr::Ascii("ing"),
+        dictgen::InsensitiveStr::Ascii("ry"),
+    ],
+    values: &[&["working"], &["worry"]],
+    range: 2..=3,
 };
 
 static WORD_WORN_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_WORN_CHILDREN),
     value: None,
 };
 
@@ -6260,28 +6265,30 @@
     keys: &[
         dictgen::InsensitiveStr::Ascii("age"),
         dictgen::InsensitiveStr::Ascii("aitm"),
         dictgen::InsensitiveStr::Ascii("aly"),
         dictgen::InsensitiveStr::Ascii("atium"),
         dictgen::InsensitiveStr::Ascii("atum"),
         dictgen::InsensitiveStr::Ascii("oase"),
+        dictgen::InsensitiveStr::Ascii("ode"),
         dictgen::InsensitiveStr::Ascii("ous"),
         dictgen::InsensitiveStr::Ascii("ouse"),
         dictgen::InsensitiveStr::Ascii("ously"),
         dictgen::InsensitiveStr::Ascii("se"),
     ],
     values: &[
         &["verbiage"],
         &["verbatim"],
         &["verbally"],
         &["verbatim"],
         &["verbatim"],
         &["verbose"],
         &["verbose"],
         &["verbose"],
+        &["verbose"],
         &["verbosely"],
         &["verbose"],
     ],
     range: 2..=5,
 };
 
 static WORD_VERA_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
@@ -6574,14 +6581,16 @@
         dictgen::InsensitiveStr::Ascii("hiles"),
         dictgen::InsensitiveStr::Ascii("otor"),
         dictgen::InsensitiveStr::Ascii("otr"),
         dictgen::InsensitiveStr::Ascii("otrs"),
         dictgen::InsensitiveStr::Ascii("tices"),
         dictgen::InsensitiveStr::Ascii("tore"),
         dictgen::InsensitiveStr::Ascii("tores"),
+        dictgen::InsensitiveStr::Ascii("torr"),
+        dictgen::InsensitiveStr::Ascii("torrs"),
         dictgen::InsensitiveStr::Ascii("torss"),
         dictgen::InsensitiveStr::Ascii("tror"),
         dictgen::InsensitiveStr::Ascii("trors"),
         dictgen::InsensitiveStr::Ascii("tros"),
         dictgen::InsensitiveStr::Ascii("vtor"),
         dictgen::InsensitiveStr::Ascii("vtors"),
     ],
@@ -6589,14 +6598,16 @@
         &["vehicles"],
         &["vector"],
         &["vector"],
         &["vectors"],
         &["vertices"],
         &["vector"],
         &["vectors"],
+        &["vector"],
+        &["vectors"],
         &["vectors"],
         &["vector"],
         &["vectors"],
         &["vectors"],
         &["vector"],
         &["vectors"],
     ],
@@ -11038,28 +11049,32 @@
 
 pub static WORD_UNIF_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
         dictgen::InsensitiveStr::Ascii("form"),
         dictgen::InsensitiveStr::Ascii("forms"),
         dictgen::InsensitiveStr::Ascii("iy"),
         dictgen::InsensitiveStr::Ascii("nished"),
+        dictgen::InsensitiveStr::Ascii("om"),
+        dictgen::InsensitiveStr::Ascii("omly"),
         dictgen::InsensitiveStr::Ascii("omtity"),
         dictgen::InsensitiveStr::Ascii("ormely"),
         dictgen::InsensitiveStr::Ascii("ormes"),
         dictgen::InsensitiveStr::Ascii("ormy"),
         dictgen::InsensitiveStr::Ascii("rom"),
         dictgen::InsensitiveStr::Ascii("romed"),
         dictgen::InsensitiveStr::Ascii("romity"),
         dictgen::InsensitiveStr::Ascii("roms"),
     ],
     values: &[
         &["uniform"],
         &["uniforms"],
         &["unify"],
         &["unfinished"],
+        &["uniform"],
+        &["uniformly"],
         &["uniformity"],
         &["uniformly"],
         &["uniforms"],
         &["uniformly", "uniform"],
         &["uniform"],
         &["uniformed"],
         &["uniformity"],
@@ -17118,14 +17133,15 @@
         dictgen::InsensitiveStr::Ascii("endant"),
         dictgen::InsensitiveStr::Ascii("endentational"),
         dictgen::InsensitiveStr::Ascii("evier"),
         dictgen::InsensitiveStr::Ascii("iever"),
         dictgen::InsensitiveStr::Ascii("ievers"),
         dictgen::InsensitiveStr::Ascii("iprt"),
         dictgen::InsensitiveStr::Ascii("irpt"),
+        dictgen::InsensitiveStr::Ascii("iver"),
         dictgen::InsensitiveStr::Ascii("luent"),
         dictgen::InsensitiveStr::Ascii("ocde"),
         dictgen::InsensitiveStr::Ascii("ocded"),
         dictgen::InsensitiveStr::Ascii("ocder"),
         dictgen::InsensitiveStr::Ascii("ocders"),
         dictgen::InsensitiveStr::Ascii("ocdes"),
         dictgen::InsensitiveStr::Ascii("ocding"),
@@ -17169,14 +17185,15 @@
         &["transcendent"],
         &["transcendental"],
         &["transceiver"],
         &["transceiver"],
         &["transceivers"],
         &["transcripts"],
         &["transcripts"],
+        &["transceiver"],
         &["translucent"],
         &["transcode"],
         &["transcoded"],
         &["transcoder"],
         &["transcoders"],
         &["transcodes"],
         &["transcoding"],
@@ -21497,14 +21514,15 @@
         dictgen::InsensitiveStr::Ascii("ats"),
         dictgen::InsensitiveStr::Ascii("eos"),
         dictgen::InsensitiveStr::Ascii("ers"),
         dictgen::InsensitiveStr::Ascii("ete"),
         dictgen::InsensitiveStr::Ascii("eted"),
         dictgen::InsensitiveStr::Ascii("etes"),
         dictgen::InsensitiveStr::Ascii("eting"),
+        dictgen::InsensitiveStr::Ascii("tes"),
     ],
     values: &[
         &["templated"],
         &["templates"],
         &["templating"],
         &["template"],
         &["templars"],
@@ -21517,14 +21535,15 @@
         &["templates"],
         &["temples"],
         &["temples"],
         &["template"],
         &["templated"],
         &["templates"],
         &["templating"],
+        &["templates"],
     ],
     range: 2..=5,
 };
 
 static WORD_TEMPE_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_TEMPE_CHILDREN),
     value: None,
@@ -24838,15 +24857,15 @@
         &["substrate"],
     ],
     range: 5..=9,
 };
 
 static WORD_SUR_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Nested(&WORD_SUR_CHILDREN),
-    value: None,
+    value: Some(&["sure"]),
 };
 
 static WORD_SUR_CHILDREN: [Option<&dictgen::DictTrieNode<&'static [&'static str]>>; 26] = [
     None,
     Some(&WORD_SURB_NODE),
     None,
     None,
@@ -34642,14 +34661,15 @@
         dictgen::InsensitiveStr::Ascii("etries"),
         dictgen::InsensitiveStr::Ascii("igles"),
         dictgen::InsensitiveStr::Ascii("ipet"),
         dictgen::InsensitiveStr::Ascii("ipets"),
         dictgen::InsensitiveStr::Ascii("ippent"),
         dictgen::InsensitiveStr::Ascii("ippert"),
         dictgen::InsensitiveStr::Ascii("ippes"),
+        dictgen::InsensitiveStr::Ascii("ippests"),
         dictgen::InsensitiveStr::Ascii("ippetts"),
         dictgen::InsensitiveStr::Ascii("odwen"),
         dictgen::InsensitiveStr::Ascii("owbaling"),
         dictgen::InsensitiveStr::Ascii("owballes"),
         dictgen::InsensitiveStr::Ascii("owballling"),
         dictgen::InsensitiveStr::Ascii("owballls"),
         dictgen::InsensitiveStr::Ascii("owbals"),
@@ -34691,14 +34711,15 @@
         &["singles"],
         &["snippet"],
         &["snippets"],
         &["snippet"],
         &["snippet"],
         &["snippets"],
         &["snippets"],
+        &["snippets"],
         &["snowden"],
         &["snowballing"],
         &["snowballs"],
         &["snowballing"],
         &["snowballs"],
         &["snowballs"],
         &["snowboarding"],
@@ -40436,14 +40457,15 @@
         dictgen::InsensitiveStr::Ascii("mentaion"),
         dictgen::InsensitiveStr::Ascii("mente"),
         dictgen::InsensitiveStr::Ascii("mentes"),
         dictgen::InsensitiveStr::Ascii("metn"),
         dictgen::InsensitiveStr::Ascii("metned"),
         dictgen::InsensitiveStr::Ascii("metns"),
         dictgen::InsensitiveStr::Ascii("mnet"),
+        dictgen::InsensitiveStr::Ascii("mnets"),
         dictgen::InsensitiveStr::Ascii("ragated"),
         dictgen::InsensitiveStr::Ascii("ragation"),
         dictgen::InsensitiveStr::Ascii("regacion"),
         dictgen::InsensitiveStr::Ascii("regaded"),
         dictgen::InsensitiveStr::Ascii("regatie"),
         dictgen::InsensitiveStr::Ascii("retated"),
         dictgen::InsensitiveStr::Ascii("retation"),
@@ -40483,14 +40505,15 @@
         &["segmentation"],
         &["segment"],
         &["segments"],
         &["segment"],
         &["segmented"],
         &["segments"],
         &["segment"],
+        &["segments"],
         &["segregated"],
         &["segregation"],
         &["segregation"],
         &["segregated"],
         &["segregated"],
         &["segregated"],
         &["segregation"],
@@ -56091,14 +56114,15 @@
         dictgen::InsensitiveStr::Ascii("locaitons"),
         dictgen::InsensitiveStr::Ascii("oded"),
         dictgen::InsensitiveStr::Ascii("oding"),
         dictgen::InsensitiveStr::Ascii("sie"),
         dictgen::InsensitiveStr::Ascii("sied"),
         dictgen::InsensitiveStr::Ascii("sim"),
         dictgen::InsensitiveStr::Ascii("sitic"),
+        dictgen::InsensitiveStr::Ascii("stic"),
         dictgen::InsensitiveStr::Ascii("table"),
         dictgen::InsensitiveStr::Ascii("ted"),
         dictgen::InsensitiveStr::Ascii("tes"),
         dictgen::InsensitiveStr::Ascii("tion"),
         dictgen::InsensitiveStr::Ascii("tions"),
         dictgen::InsensitiveStr::Ascii("tionships"),
         dictgen::InsensitiveStr::Ascii("tive"),
@@ -56151,14 +56175,15 @@
         &["reallocations"],
         &["reloaded"],
         &["reloading"],
         &["realise"],
         &["realised"],
         &["realism"],
         &["realistic"],
+        &["realistic"],
         &["relatable"],
         &["related"],
         &["relates"],
         &["relation", "reaction"],
         &["relations", "reactions"],
         &["relationships"],
         &["relative", "reactive"],
@@ -56767,14 +56792,16 @@
         dictgen::InsensitiveStr::Ascii("ioactice"),
         dictgen::InsensitiveStr::Ascii("ioactief"),
         dictgen::InsensitiveStr::Ascii("ioactieve"),
         dictgen::InsensitiveStr::Ascii("ioaktive"),
         dictgen::InsensitiveStr::Ascii("iobuttion"),
         dictgen::InsensitiveStr::Ascii("iocative"),
         dictgen::InsensitiveStr::Ascii("is"),
+        dictgen::InsensitiveStr::Ascii("uis"),
+        dictgen::InsensitiveStr::Ascii("us"),
         dictgen::InsensitiveStr::Ascii("y"),
     ],
     values: &[
         &["radiance"],
         &["radiant"],
         &["radiation"],
         &["read", "raid"],
@@ -56796,14 +56823,16 @@
         &["radioactive"],
         &["radioactive"],
         &["radioactive"],
         &["radioactive"],
         &["radiobutton"],
         &["radioactive"],
         &["radix"],
+        &["radius"],
+        &["radius"],
         &["ready"],
     ],
     range: 1..=9,
 };
 
 static WORD_RAC_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_RAC_CHILDREN),
@@ -63073,14 +63102,15 @@
         dictgen::InsensitiveStr::Ascii("entivo"),
         dictgen::InsensitiveStr::Ascii("entors"),
         dictgen::InsensitiveStr::Ascii("erse"),
         dictgen::InsensitiveStr::Ascii("erses"),
         dictgen::InsensitiveStr::Ascii("ert"),
         dictgen::InsensitiveStr::Ascii("erve"),
         dictgen::InsensitiveStr::Ascii("erved"),
+        dictgen::InsensitiveStr::Ascii("et"),
         dictgen::InsensitiveStr::Ascii("ew"),
         dictgen::InsensitiveStr::Ascii("ews"),
         dictgen::InsensitiveStr::Ascii("ial"),
         dictgen::InsensitiveStr::Ascii("ialing"),
         dictgen::InsensitiveStr::Ascii("ies"),
         dictgen::InsensitiveStr::Ascii("iewd"),
         dictgen::InsensitiveStr::Ascii("iious"),
@@ -63136,14 +63166,15 @@
         &["prevention"],
         &["prevents"],
         &["perverse"],
         &["preserves"],
         &["pervert"],
         &["preserve"],
         &["preserved"],
+        &["prevent"],
         &["preview"],
         &["previews"],
         &["prevail"],
         &["prevailing"],
         &["previews"],
         &["previewed"],
         &["previous"],
@@ -67683,14 +67714,15 @@
         dictgen::InsensitiveStr::Ascii("ofms"),
         dictgen::InsensitiveStr::Ascii("ofmss"),
         dictgen::InsensitiveStr::Ascii("oform"),
         dictgen::InsensitiveStr::Ascii("oforms"),
         dictgen::InsensitiveStr::Ascii("ofrm"),
         dictgen::InsensitiveStr::Ascii("ofrmer"),
         dictgen::InsensitiveStr::Ascii("ofrms"),
+        dictgen::InsensitiveStr::Ascii("orm"),
         dictgen::InsensitiveStr::Ascii("tform"),
         dictgen::InsensitiveStr::Ascii("tforms"),
         dictgen::InsensitiveStr::Ascii("toe"),
         dictgen::InsensitiveStr::Ascii("toes"),
     ],
     values: &[
         &["plateau"],
@@ -67729,14 +67761,15 @@
         &["platforms"],
         &["platform"],
         &["platforms"],
         &["platform"],
         &["platformer"],
         &["platforms"],
         &["platform"],
+        &["platform"],
         &["platforms"],
         &["plateau"],
         &["plateaus"],
     ],
     range: 2..=7,
 };
 
@@ -69776,14 +69809,16 @@
         dictgen::InsensitiveStr::Ascii("stens"),
         dictgen::InsensitiveStr::Ascii("stense"),
         dictgen::InsensitiveStr::Ascii("stente"),
         dictgen::InsensitiveStr::Ascii("stented"),
         dictgen::InsensitiveStr::Ascii("stes"),
         dictgen::InsensitiveStr::Ascii("ted"),
         dictgen::InsensitiveStr::Ascii("tent"),
+        dictgen::InsensitiveStr::Ascii("tentely"),
+        dictgen::InsensitiveStr::Ascii("tently"),
         dictgen::InsensitiveStr::Ascii("ts"),
     ],
     values: &[
         &["persecuted"],
         &["persecution"],
         &["persist"],
         &["persisted"],
@@ -69795,14 +69830,16 @@
         &["persists"],
         &["persistence"],
         &["persistence"],
         &["persisted"],
         &["persists"],
         &["persisted"],
         &["persistent"],
+        &["persistently"],
+        &["persistently"],
         &["persist"],
     ],
     range: 2..=7,
 };
 
 static WORD_PERSH_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_PERSH_CHILDREN),
@@ -73810,34 +73847,36 @@
 static WORD_PARAS_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_PARAS_CHILDREN),
     value: None,
 };
 
 pub static WORD_PARAS_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
+        dictgen::InsensitiveStr::Ascii("er"),
         dictgen::InsensitiveStr::Ascii("ide"),
         dictgen::InsensitiveStr::Ascii("itisme"),
         dictgen::InsensitiveStr::Ascii("its"),
         dictgen::InsensitiveStr::Ascii("itter"),
         dictgen::InsensitiveStr::Ascii("tic"),
         dictgen::InsensitiveStr::Ascii("tics"),
         dictgen::InsensitiveStr::Ascii("tie"),
         dictgen::InsensitiveStr::Ascii("ties"),
     ],
     values: &[
+        &["parser"],
         &["paradise"],
         &["parasites"],
         &["parasites"],
         &["parasite"],
         &["parasitic"],
         &["parasitics"],
         &["parasite"],
         &["parasites"],
     ],
-    range: 3..=6,
+    range: 2..=6,
 };
 
 static WORD_PARAR_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_PARAR_CHILDREN),
     value: None,
 };
 
@@ -74679,17 +74718,18 @@
     value: None,
 };
 
 pub static WORD_PAE_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
         dictgen::InsensitiveStr::Ascii("rmission"),
         dictgen::InsensitiveStr::Ascii("rmissions"),
+        dictgen::InsensitiveStr::Ascii("rnt"),
         dictgen::InsensitiveStr::Ascii("th"),
     ],
-    values: &[&["permission"], &["permissions"], &["path"]],
+    values: &[&["permission"], &["permissions"], &["parent"], &["path"]],
     range: 2..=9,
 };
 
 static WORD_PAD_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_PAD_CHILDREN),
     value: None,
 };
@@ -78458,14 +78498,15 @@
 static WORD_OPI_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_OPI_CHILDREN),
     value: None,
 };
 
 pub static WORD_OPI_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
+        dictgen::InsensitiveStr::Ascii("mized"),
         dictgen::InsensitiveStr::Ascii("niones"),
         dictgen::InsensitiveStr::Ascii("noins"),
         dictgen::InsensitiveStr::Ascii("nyon"),
         dictgen::InsensitiveStr::Ascii("nyonable"),
         dictgen::InsensitiveStr::Ascii("nyonaire"),
         dictgen::InsensitiveStr::Ascii("nyonal"),
         dictgen::InsensitiveStr::Ascii("nyonate"),
@@ -78486,14 +78527,15 @@
         dictgen::InsensitiveStr::Ascii("tional"),
         dictgen::InsensitiveStr::Ascii("tionally"),
         dictgen::InsensitiveStr::Ascii("tmal"),
         dictgen::InsensitiveStr::Ascii("ton"),
         dictgen::InsensitiveStr::Ascii("tons"),
     ],
     values: &[
+        &["optimized"],
         &["opinions"],
         &["opinions"],
         &["opinion"],
         &["opinionable"],
         &["opinionnaire"],
         &["opinional"],
         &["opinionated"],
@@ -79783,15 +79825,15 @@
         dictgen::InsensitiveStr::Ascii("er"),
         dictgen::InsensitiveStr::Ascii("ly"),
         dictgen::InsensitiveStr::Ascii("y"),
     ],
     values: &[
         &["odyssey"],
         &["odysseys"],
-        &["order", "odor"],
+        &["order", "odor", "older"],
         &["oddly"],
         &["body"],
     ],
     range: 1..=5,
 };
 
 static WORD_OC_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
@@ -94878,14 +94920,15 @@
         dictgen::InsensitiveStr::Ascii("aer"),
         dictgen::InsensitiveStr::Ascii("aers"),
         dictgen::InsensitiveStr::Ascii("ager"),
         dictgen::InsensitiveStr::Ascii("agers"),
         dictgen::InsensitiveStr::Ascii("eld"),
         dictgen::InsensitiveStr::Ascii("ement"),
         dictgen::InsensitiveStr::Ascii("ementt"),
+        dictgen::InsensitiveStr::Ascii("es"),
         dictgen::InsensitiveStr::Ascii("esium"),
         dictgen::InsensitiveStr::Ascii("etic"),
         dictgen::InsensitiveStr::Ascii("ets"),
         dictgen::InsensitiveStr::Ascii("itude"),
         dictgen::InsensitiveStr::Ascii("lade"),
     ],
     values: &[
@@ -94894,21 +94937,22 @@
         &["manager", "manger"],
         &["managers", "mangers"],
         &["manager"],
         &["managers"],
         &["mangled"],
         &["management"],
         &["management"],
+        &["manages"],
         &["magnesium"],
         &["magnetic"],
         &["magnets"],
         &["magnitude"],
         &["mangled"],
     ],
-    range: 3..=6,
+    range: 2..=6,
 };
 
 static WORD_MANF_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_MANF_CHILDREN),
     value: None,
 };
 
@@ -102434,14 +102478,15 @@
         dictgen::InsensitiveStr::Ascii("sibillity"),
         dictgen::InsensitiveStr::Ascii("sibiltiy"),
         dictgen::InsensitiveStr::Ascii("sibily"),
         dictgen::InsensitiveStr::Ascii("silibity"),
         dictgen::InsensitiveStr::Ascii("sivble"),
         dictgen::InsensitiveStr::Ascii("sivility"),
         dictgen::InsensitiveStr::Ascii("tacion"),
+        dictgen::InsensitiveStr::Ascii("taion"),
         dictgen::InsensitiveStr::Ascii("tating"),
         dictgen::InsensitiveStr::Ascii("tato"),
     ],
     values: &[
         &["invitation"],
         &["invisibility"],
         &["invincible"],
@@ -102472,14 +102517,15 @@
         &["invisibility"],
         &["invisibility"],
         &["invisible"],
         &["invisibility"],
         &["invitation"],
         &["invitation"],
         &["invitation"],
+        &["invitation"],
     ],
     range: 4..=9,
 };
 
 static WORD_INVE_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Nested(&WORD_INVE_CHILDREN),
     value: None,
@@ -103205,14 +103251,15 @@
         dictgen::InsensitiveStr::Ascii("guied"),
         dictgen::InsensitiveStr::Ascii("gured"),
         dictgen::InsensitiveStr::Ascii("nisc"),
         dictgen::InsensitiveStr::Ascii("niscally"),
         dictgen::InsensitiveStr::Ascii("nsecally"),
         dictgen::InsensitiveStr::Ascii("nseci"),
         dictgen::InsensitiveStr::Ascii("nsicaly"),
+        dictgen::InsensitiveStr::Ascii("nsict"),
         dictgen::InsensitiveStr::Ascii("nsinc"),
         dictgen::InsensitiveStr::Ascii("nsisch"),
         dictgen::InsensitiveStr::Ascii("quing"),
         dictgen::InsensitiveStr::Ascii("sinc"),
         dictgen::InsensitiveStr::Ascii("sincally"),
         dictgen::InsensitiveStr::Ascii("sincs"),
         dictgen::InsensitiveStr::Ascii("snic"),
@@ -103235,14 +103282,15 @@
         &["intrinsic"],
         &["intrinsically"],
         &["intrinsically"],
         &["intrinsic"],
         &["intrinsically"],
         &["intrinsic"],
         &["intrinsic"],
+        &["intrinsic"],
         &["intriguing"],
         &["intrinsic"],
         &["intrinsically"],
         &["intrinsics"],
         &["intrinsic"],
         &["intrinsically"],
         &["intrigue"],
@@ -107171,14 +107219,15 @@
         dictgen::InsensitiveStr::Ascii("ecting"),
         dictgen::InsensitiveStr::Ascii("ection"),
         dictgen::InsensitiveStr::Ascii("ections"),
         dictgen::InsensitiveStr::Ascii("ending"),
         dictgen::InsensitiveStr::Ascii("enetrable"),
         dictgen::InsensitiveStr::Ascii("erfections"),
         dictgen::InsensitiveStr::Ascii("ersonating"),
+        dictgen::InsensitiveStr::Ascii("ired"),
         dictgen::InsensitiveStr::Ascii("lementation"),
         dictgen::InsensitiveStr::Ascii("lementations"),
         dictgen::InsensitiveStr::Ascii("lemented"),
         dictgen::InsensitiveStr::Ascii("lementing"),
         dictgen::InsensitiveStr::Ascii("lications"),
         dictgen::InsensitiveStr::Ascii("licit"),
         dictgen::InsensitiveStr::Ascii("licitly"),
@@ -107230,14 +107279,15 @@
         &["inspecting"],
         &["inception", "inspection"],
         &["inspections"],
         &["impending"],
         &["impenetrable"],
         &["imperfections"],
         &["impersonating"],
+        &["inspired"],
         &["implementation"],
         &["implementations"],
         &["implemented"],
         &["implementing"],
         &["implications"],
         &["implicit"],
         &["implicitly"],
@@ -108929,14 +108979,15 @@
         dictgen::InsensitiveStr::Ascii("grahpic"),
         dictgen::InsensitiveStr::Ascii("grapgic"),
         dictgen::InsensitiveStr::Ascii("grapic"),
         dictgen::InsensitiveStr::Ascii("grpahic"),
         dictgen::InsensitiveStr::Ascii("grpahics"),
         dictgen::InsensitiveStr::Ascii("mation"),
         dictgen::InsensitiveStr::Ascii("mational"),
+        dictgen::InsensitiveStr::Ascii("matrion"),
         dictgen::InsensitiveStr::Ascii("med"),
         dictgen::InsensitiveStr::Ascii("mer"),
         dictgen::InsensitiveStr::Ascii("mration"),
         dictgen::InsensitiveStr::Ascii("ms"),
         dictgen::InsensitiveStr::Ascii("r"),
         dictgen::InsensitiveStr::Ascii("ramtion"),
         dictgen::InsensitiveStr::Ascii("ration"),
@@ -108987,14 +109038,15 @@
         &["infographic"],
         &["infographic"],
         &["infographic"],
         &["infographic"],
         &["infographic"],
         &["information"],
         &["informational"],
+        &["information"],
         &["informed"],
         &["informer"],
         &["information"],
         &["informs"],
         &["info"],
         &["information"],
         &["information"],
@@ -118611,22 +118663,26 @@
 static WORD_HED_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_HED_CHILDREN),
     value: None,
 };
 
 pub static WORD_HED_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
+        dictgen::InsensitiveStr::Ascii("aer"),
+        dictgen::InsensitiveStr::Ascii("aers"),
         dictgen::InsensitiveStr::Ascii("eghog"),
         dictgen::InsensitiveStr::Ascii("er"),
         dictgen::InsensitiveStr::Ascii("ers"),
         dictgen::InsensitiveStr::Ascii("gehodge"),
         dictgen::InsensitiveStr::Ascii("gehoog"),
         dictgen::InsensitiveStr::Ascii("gehorg"),
     ],
     values: &[
+        &["header"],
+        &["headers"],
         &["hedgehog"],
         &["header"],
         &["headers"],
         &["hedgehog"],
         &["hedgehog"],
         &["hedgehog"],
     ],
@@ -128338,16 +128394,19 @@
 
 static WORD_FIB_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_FIB_CHILDREN),
     value: None,
 };
 
 pub static WORD_FIB_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
-    keys: &[dictgen::InsensitiveStr::Ascii("onaacci")],
-    values: &[&["fibonacci"]],
+    keys: &[
+        dictgen::InsensitiveStr::Ascii("onaacci"),
+        dictgen::InsensitiveStr::Ascii("onnacci"),
+    ],
+    values: &[&["fibonacci"], &["fibonacci"]],
     range: 7..=7,
 };
 
 static WORD_FIA_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_FIA_CHILDREN),
     value: None,
 };
@@ -130013,20 +130072,22 @@
 
 pub static WORD_EXTRI_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
         dictgen::InsensitiveStr::Ascii("me"),
         dictgen::InsensitiveStr::Ascii("mely"),
         dictgen::InsensitiveStr::Ascii("mists"),
         dictgen::InsensitiveStr::Ascii("mly"),
+        dictgen::InsensitiveStr::Ascii("nsict"),
     ],
     values: &[
         &["extreme"],
         &["extremely"],
         &["extremists"],
         &["extremely"],
+        &["extrinsic"],
     ],
     range: 2..=5,
 };
 
 static WORD_EXTRE_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_EXTRE_CHILDREN),
     value: None,
@@ -136918,14 +136979,15 @@
         dictgen::InsensitiveStr::Ascii("ecialy"),
         dictgen::InsensitiveStr::Ascii("ecialyl"),
         dictgen::InsensitiveStr::Ascii("ecifically"),
         dictgen::InsensitiveStr::Ascii("eciially"),
         dictgen::InsensitiveStr::Ascii("ect"),
         dictgen::InsensitiveStr::Ascii("eically"),
         dictgen::InsensitiveStr::Ascii("erate"),
+        dictgen::InsensitiveStr::Ascii("escially"),
         dictgen::InsensitiveStr::Ascii("ianoge"),
         dictgen::InsensitiveStr::Ascii("inoage"),
         dictgen::InsensitiveStr::Ascii("isode"),
         dictgen::InsensitiveStr::Ascii("isodes"),
         dictgen::InsensitiveStr::Ascii("isodic"),
         dictgen::InsensitiveStr::Ascii("isodical"),
         dictgen::InsensitiveStr::Ascii("isodically"),
@@ -136953,14 +137015,15 @@
         &["especially"],
         &["especially"],
         &["specifically", "especially"],
         &["especially"],
         &["expect"],
         &["especially"],
         &["separate"],
+        &["especially"],
         &["espionage"],
         &["espionage"],
         &["episode"],
         &["episodes"],
         &["episodic"],
         &["episodical"],
         &["episodically"],
@@ -139990,14 +140053,15 @@
 pub static WORD_ENA_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
         dictgen::InsensitiveStr::Ascii("able"),
         dictgen::InsensitiveStr::Ascii("be"),
         dictgen::InsensitiveStr::Ascii("bel"),
         dictgen::InsensitiveStr::Ascii("beled"),
         dictgen::InsensitiveStr::Ascii("beling"),
+        dictgen::InsensitiveStr::Ascii("bels"),
         dictgen::InsensitiveStr::Ascii("bing"),
         dictgen::InsensitiveStr::Ascii("bledi"),
         dictgen::InsensitiveStr::Ascii("bleing"),
         dictgen::InsensitiveStr::Ascii("blen"),
         dictgen::InsensitiveStr::Ascii("hnces"),
         dictgen::InsensitiveStr::Ascii("hncing"),
         dictgen::InsensitiveStr::Ascii("lbe"),
@@ -140008,14 +140072,15 @@
     ],
     values: &[
         &["enable"],
         &["enable"],
         &["enable"],
         &["enabled"],
         &["enabling"],
+        &["enables"],
         &["enabling"],
         &["enabled"],
         &["enabling"],
         &["enabled"],
         &["enhances"],
         &["enhancing"],
         &["enable"],
@@ -151940,14 +152005,15 @@
         dictgen::InsensitiveStr::Ascii("te"),
         dictgen::InsensitiveStr::Ascii("tected"),
         dictgen::InsensitiveStr::Ascii("tes"),
         dictgen::InsensitiveStr::Ascii("tetd"),
         dictgen::InsensitiveStr::Ascii("tie"),
         dictgen::InsensitiveStr::Ascii("tiona"),
         dictgen::InsensitiveStr::Ascii("tionn"),
+        dictgen::InsensitiveStr::Ascii("tionns"),
         dictgen::InsensitiveStr::Ascii("tivs"),
         dictgen::InsensitiveStr::Ascii("toare"),
         dictgen::InsensitiveStr::Ascii("tsion"),
         dictgen::InsensitiveStr::Ascii("tsions"),
         dictgen::InsensitiveStr::Ascii("tt"),
     ],
     values: &[
@@ -151964,14 +152030,15 @@
         &["detected", "detect", "detects"],
         &["detected"],
         &["detects"],
         &["detected"],
         &["detectives"],
         &["detection", "detections"],
         &["detection"],
+        &["detections"],
         &["detectives"],
         &["detector"],
         &["detection"],
         &["detections"],
         &["detect"],
     ],
     range: 1..=6,
@@ -156338,22 +156405,24 @@
 pub static WORD_DEFN_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
         dictgen::InsensitiveStr::Ascii("ed"),
         dictgen::InsensitiveStr::Ascii("iately"),
         dictgen::InsensitiveStr::Ascii("ietly"),
         dictgen::InsensitiveStr::Ascii("inition"),
         dictgen::InsensitiveStr::Ascii("initions"),
+        dictgen::InsensitiveStr::Ascii("itely"),
         dictgen::InsensitiveStr::Ascii("itions"),
     ],
     values: &[
         &["defend", "defined"],
         &["definitely"],
         &["definitely"],
         &["definition"],
         &["definitions"],
+        &["definitely"],
         &["definitions"],
     ],
     range: 2..=8,
 };
 
 static WORD_DEFL_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_DEFL_CHILDREN),
@@ -177951,17 +178020,20 @@
 
 static WORD_CIRR_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_CIRR_CHILDREN),
     value: None,
 };
 
 pub static WORD_CIRR_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
-    keys: &[dictgen::InsensitiveStr::Ascii("uculum")],
-    values: &[&["curriculum"]],
-    range: 6..=6,
+    keys: &[
+        dictgen::InsensitiveStr::Ascii("ently"),
+        dictgen::InsensitiveStr::Ascii("uculum"),
+    ],
+    values: &[&["currently"], &["curriculum"]],
+    range: 5..=6,
 };
 
 static WORD_CIRL_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_CIRL_CHILDREN),
     value: None,
 };
 
@@ -182027,14 +182099,15 @@
     value: None,
 };
 
 pub static WORD_CC_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
         dictgen::InsensitiveStr::Ascii("ahe"),
         dictgen::InsensitiveStr::Ascii("ale"),
+        dictgen::InsensitiveStr::Ascii("annot"),
         dictgen::InsensitiveStr::Ascii("ertificate"),
         dictgen::InsensitiveStr::Ascii("ertificated"),
         dictgen::InsensitiveStr::Ascii("ertificates"),
         dictgen::InsensitiveStr::Ascii("ertification"),
         dictgen::InsensitiveStr::Ascii("essible"),
         dictgen::InsensitiveStr::Ascii("he"),
         dictgen::InsensitiveStr::Ascii("onfiguration"),
@@ -182046,14 +182119,15 @@
         dictgen::InsensitiveStr::Ascii("urred"),
         dictgen::InsensitiveStr::Ascii("ustom"),
         dictgen::InsensitiveStr::Ascii("ustoms"),
     ],
     values: &[
         &["cache"],
         &["scale"],
+        &["cannot"],
         &["certificate"],
         &["certificated"],
         &["certificates"],
         &["certification"],
         &["accessible"],
         &["cache"],
         &["configuration"],
@@ -187929,17 +188003,20 @@
 
 static WORD_BOI_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_BOI_CHILDREN),
     value: None,
 };
 
 pub static WORD_BOI_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
-    keys: &[dictgen::InsensitiveStr::Ascii("nter")],
-    values: &[&["pointer"]],
-    range: 4..=4,
+    keys: &[
+        dictgen::InsensitiveStr::Ascii("lerplatte"),
+        dictgen::InsensitiveStr::Ascii("nter"),
+    ],
+    values: &[&["boilerplate"], &["pointer"]],
+    range: 4..=9,
 };
 
 static WORD_BOG_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_BOG_CHILDREN),
     value: None,
 };
 
@@ -195877,14 +195954,15 @@
         dictgen::InsensitiveStr::Ascii("ieated"),
         dictgen::InsensitiveStr::Ascii("ieates"),
         dictgen::InsensitiveStr::Ascii("ieating"),
         dictgen::InsensitiveStr::Ascii("ieation"),
         dictgen::InsensitiveStr::Ascii("ieations"),
         dictgen::InsensitiveStr::Ascii("ieted"),
         dictgen::InsensitiveStr::Ascii("isted"),
+        dictgen::InsensitiveStr::Ascii("itated"),
         dictgen::InsensitiveStr::Ascii("ite"),
         dictgen::InsensitiveStr::Ascii("ited"),
         dictgen::InsensitiveStr::Ascii("ites"),
         dictgen::InsensitiveStr::Ascii("iting"),
         dictgen::InsensitiveStr::Ascii("ition"),
         dictgen::InsensitiveStr::Ascii("itions"),
         dictgen::InsensitiveStr::Ascii("itive"),
@@ -195926,14 +196004,15 @@
         &["associated"],
         &["associates"],
         &["associating"],
         &["association"],
         &["associations"],
         &["associated"],
         &["associates"],
+        &["associated"],
         &["associate"],
         &["associated"],
         &["associates"],
         &["associating"],
         &["association"],
         &["associations"],
         &["associative"],
@@ -201096,22 +201175,24 @@
 
 pub static WORD_ANOU_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
         dictgen::InsensitiveStr::Ascii("nce"),
         dictgen::InsensitiveStr::Ascii("nced"),
         dictgen::InsensitiveStr::Ascii("ncement"),
         dictgen::InsensitiveStr::Ascii("nt"),
+        dictgen::InsensitiveStr::Ascii("t"),
     ],
     values: &[
         &["announce"],
         &["announced"],
         &["announcement"],
         &["amount"],
+        &["about"],
     ],
-    range: 2..=7,
+    range: 1..=7,
 };
 
 static WORD_ANOT_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_ANOT_CHILDREN),
     value: None,
 };
 
@@ -210015,14 +210096,15 @@
 static WORD_ACCES_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_ACCES_CHILDREN),
     value: Some(&["access"]),
 };
 
 pub static WORD_ACCES_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
+        dictgen::InsensitiveStr::Ascii("able"),
         dictgen::InsensitiveStr::Ascii("ed"),
         dictgen::InsensitiveStr::Ascii("es"),
         dictgen::InsensitiveStr::Ascii("ibility"),
         dictgen::InsensitiveStr::Ascii("ible"),
         dictgen::InsensitiveStr::Ascii("iblity"),
         dictgen::InsensitiveStr::Ascii("iibility"),
         dictgen::InsensitiveStr::Ascii("iiblity"),
@@ -210066,14 +210148,15 @@
         dictgen::InsensitiveStr::Ascii("ssing"),
         dictgen::InsensitiveStr::Ascii("ssor"),
         dictgen::InsensitiveStr::Ascii("ssors"),
         dictgen::InsensitiveStr::Ascii("tor"),
         dictgen::InsensitiveStr::Ascii("tors"),
     ],
     values: &[
+        &["accessible"],
         &["accessed"],
         &["accesses"],
         &["accessibility"],
         &["accessible"],
         &["accessibility"],
         &["accessibility"],
         &["accessibility"],
```

### Comparing `typos-1.16.1/local_dependencies/dictgen/Cargo.toml` & `typos-1.16.2/local_dependencies/dictgen/Cargo.toml`

 * *Files identical despite different names*

### Comparing `typos-1.16.1/local_dependencies/dictgen/src/map.rs` & `typos-1.16.2/local_dependencies/dictgen/src/map.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.1/local_dependencies/dictgen/src/table.rs` & `typos-1.16.2/local_dependencies/dictgen/src/table.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.1/local_dependencies/dictgen/src/trie.rs` & `typos-1.16.2/local_dependencies/dictgen/src/trie.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.1/local_dependencies/typos-vars/Cargo.toml` & `typos-1.16.2/local_dependencies/typos-vars/Cargo.toml`

 * *Files identical despite different names*

### Comparing `typos-1.16.1/local_dependencies/typos-vars/src/vars_codegen.rs` & `typos-1.16.2/local_dependencies/typos-vars/src/vars_codegen.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.1/rust_src/typos-cli/Cargo.toml` & `typos-1.16.2/rust_src/typos-cli/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "typos-cli"
-version = "1.16.1"
+version = "1.16.2"
 description = "Source Code Spelling Correction"
 readme = "../../README.md"
 categories = ["development-tools", "text-processing"]
 keywords = ["development", "spelling"]
 license= "MIT OR Apache-2.0"
 repository= "https://github.com/crate-ci/typos"
 edition= "2021"
```

### Comparing `typos-1.16.1/rust_src/typos-cli/benches/checks.rs` & `typos-1.16.2/rust_src/typos-cli/benches/checks.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.1/rust_src/typos-cli/benches/corrections.rs` & `typos-1.16.2/rust_src/typos-cli/benches/corrections.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.1/rust_src/typos-cli/benches/data.rs` & `typos-1.16.2/rust_src/typos-cli/benches/data.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.1/rust_src/typos-cli/benches/tokenize.rs` & `typos-1.16.2/rust_src/typos-cli/benches/tokenize.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.1/rust_src/typos-cli/src/bin/typos-cli/args.rs` & `typos-1.16.2/rust_src/typos-cli/src/bin/typos-cli/args.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.1/rust_src/typos-cli/src/bin/typos-cli/main.rs` & `typos-1.16.2/rust_src/typos-cli/src/bin/typos-cli/main.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.1/rust_src/typos-cli/src/bin/typos-cli/report.rs` & `typos-1.16.2/rust_src/typos-cli/src/bin/typos-cli/report.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.1/rust_src/typos-cli/src/config.rs` & `typos-1.16.2/rust_src/typos-cli/src/config.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.1/rust_src/typos-cli/src/default_types.rs` & `typos-1.16.2/rust_src/typos-cli/src/default_types.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.1/rust_src/typos-cli/src/dict.rs` & `typos-1.16.2/rust_src/typos-cli/src/dict.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.1/rust_src/typos-cli/src/file.rs` & `typos-1.16.2/rust_src/typos-cli/src/file.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.1/rust_src/typos-cli/src/file_type.rs` & `typos-1.16.2/rust_src/typos-cli/src/file_type.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.1/rust_src/typos-cli/src/policy.rs` & `typos-1.16.2/rust_src/typos-cli/src/policy.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.1/rust_src/typos-cli/src/report.rs` & `typos-1.16.2/rust_src/typos-cli/src/report.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.1/Cargo.lock` & `typos-1.16.2/Cargo.lock`

 * *Files identical despite different names*

```diff
@@ -1649,15 +1649,15 @@
  "unicode-segmentation",
  "unicode-xid",
  "winnow 0.5.0",
 ]
 
 [[package]]
 name = "typos-cli"
-version = "1.16.1"
+version = "1.16.2"
 dependencies = [
  "ahash",
  "anstream",
  "anstyle",
  "anyhow",
  "assert_fs",
  "atty",
@@ -1697,15 +1697,15 @@
  "unicode-segmentation",
  "unicode-width",
  "varcon-core",
 ]
 
 [[package]]
 name = "typos-dict"
-version = "0.10.7"
+version = "0.10.8"
 dependencies = [
  "codegenrs",
  "csv",
  "dictgen",
  "edit-distance",
  "indexmap 2.0.0",
  "itertools",
```

### Comparing `typos-1.16.1/PKG-INFO` & `typos-1.16.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typos
-Version: 1.16.1
+Version: 1.16.2
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Source Code Spelling Correction
 Keywords: development,spelling
@@ -119,14 +119,15 @@
 ```
 
 ### Integrations
 
 - [GitHub Actions](docs/github-action.md)
 - [pre-commit](docs/pre-commit.md)
 - [🐊Putout Processor](https://github.com/putoutjs/putout-processor-typos)
+- [Visual Studio Code](https://github.com/tekumara/typos-vscode)
 
 #### Custom
 
 `typos` provides several building blocks for custom native integrations
 - `-` reads from `stdin`, `--write-changes` will be written to `stdout`
 - `--diff` to provide a diff
 - `--format json` to get jsonlines with exit code 0 on no errors, code 2 on typos, anything else is an error.
```

