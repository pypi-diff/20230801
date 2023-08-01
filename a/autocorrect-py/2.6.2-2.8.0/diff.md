# Comparing `tmp/autocorrect_py-2.6.2.tar.gz` & `tmp/autocorrect_py-2.8.0.tar.gz`

## Comparing `autocorrect_py-2.6.2.tar` & `autocorrect_py-2.8.0.tar`

### file list

```diff
@@ -1,107 +1,109 @@
--rw-r--r--   0        0        0      451 1970-01-01 00:00:00.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect-derive/Cargo.toml
--rw-r--r--   0      501       20     1153 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect-derive/src/lib.rs
--rw-r--r--   0        0        0     1142 1970-01-01 00:00:00.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/Cargo.toml
--rw-r--r--   0      501       20     2399 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/.autocorrectrc.default
--rw-r--r--   0      501       20     1066 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/LICENSE
--rw-r--r--   0      501       20     5214 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/README.md
--rw-r--r--   0      501       20     6828 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/benches/example.rs
--rw-r--r--   0      501       20     1906 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/benches/fixtures/example.html
--rw-r--r--   0      501       20      893 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/benches/fixtures/example.js
--rw-r--r--   0      501       20      279 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/benches/fixtures/example.json
--rw-r--r--   0      501       20     5194 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/benches/fixtures/example.md
--rw-r--r--   0      501       20     3094 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/benches/fixtures/example.yml
--rw-r--r--   0      501       20    97501 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/benches/fixtures/large.json
--rw-r--r--   0      501       20     1728 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/asciidoc.pest
--rw-r--r--   0      501       20      431 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/c.pest
--rw-r--r--   0      501       20      267 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/conf.pest
--rw-r--r--   0      501       20      542 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/csharp.pest
--rw-r--r--   0      501       20      269 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/css.pest
--rw-r--r--   0      501       20      557 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/dart.pest
--rw-r--r--   0      501       20      699 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/elixir.pest
--rw-r--r--   0      501       20      703 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/gettext.pest
--rw-r--r--   0      501       20      696 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/go.pest
--rw-r--r--   0      501       20     5039 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/html.pest
--rw-r--r--   0      501       20      529 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/java.pest
--rw-r--r--   0      501       20     1096 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/javascript.pest
--rw-r--r--   0      501       20     1224 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/json.pest
--rw-r--r--   0      501       20     1125 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/jupyter.pest
--rw-r--r--   0      501       20      536 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/kotlin.pest
--rw-r--r--   0      501       20      493 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/latex.pest
--rw-r--r--   0      501       20     4077 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/markdown.pest
--rw-r--r--   0      501       20      583 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/objective_c.pest
--rw-r--r--   0      501       20      658 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/php.pest
--rw-r--r--   0      501       20      643 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/python.pest
--rw-r--r--   0      501       20      567 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/ruby.pest
--rw-r--r--   0      501       20      500 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/rust.pest
--rw-r--r--   0      501       20      584 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/scala.pest
--rw-r--r--   0      501       20      367 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/sql.pest
--rw-r--r--   0      501       20      463 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/strings.pest
--rw-r--r--   0      501       20      712 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/swift.pest
--rw-r--r--   0      501       20      502 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/xml.pest
--rw-r--r--   0      501       20      627 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/yaml.pest
--rw-r--r--   0      501       20       89 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/release.toml
--rw-r--r--   0      501       20     3533 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/asciidoc.rs
--rw-r--r--   0      501       20     1482 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/c.rs
--rw-r--r--   0      501       20    12808 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/code.rs
--rw-r--r--   0      501       20      987 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/conf.rs
--rw-r--r--   0      501       20     1563 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/csharp.rs
--rw-r--r--   0      501       20     1315 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/css.rs
--rw-r--r--   0      501       20     1639 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/dart.rs
--rw-r--r--   0      501       20     1717 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/elixir.rs
--rw-r--r--   0      501       20     1528 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/gettext.rs
--rw-r--r--   0      501       20     1716 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/go.rs
--rw-r--r--   0      501       20     9557 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/html.rs
--rw-r--r--   0      501       20     1628 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/java.rs
--rw-r--r--   0      501       20     7364 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/javascript.rs
--rw-r--r--   0      501       20     1649 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/json.rs
--rw-r--r--   0      501       20    11585 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/jupyter.rs
--rw-r--r--   0      501       20     1446 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/kotlin.rs
--rw-r--r--   0      501       20     4600 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/latex.rs
--rw-r--r--   0      501       20    12553 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/markdown.rs
--rw-r--r--   0      501       20     4458 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/mod.rs
--rw-r--r--   0      501       20     1453 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/objective_c.rs
--rw-r--r--   0      501       20     1723 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/php.rs
--rw-r--r--   0      501       20     1598 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/python.rs
--rw-r--r--   0      501       20     1174 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/ruby.rs
--rw-r--r--   0      501       20     2502 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/rust.rs
--rw-r--r--   0      501       20     1627 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/scala.rs
--rw-r--r--   0      501       20     1294 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/sql.rs
--rw-r--r--   0      501       20     1318 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/strings.rs
--rw-r--r--   0      501       20     1796 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/swift.rs
--rw-r--r--   0      501       20     4816 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/types.rs
--rw-r--r--   0      501       20     1253 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/xml.rs
--rw-r--r--   0      501       20     1077 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/yaml.rs
--rw-r--r--   0      501       20    13723 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/config/mod.rs
--rw-r--r--   0      501       20     3000 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/config/severity.rs
--rw-r--r--   0      501       20     2136 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/config/spellcheck.rs
--rw-r--r--   0      501       20      392 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/config/toggle.pest
--rw-r--r--   0      501       20     8865 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/config/toggle.rs
--rw-r--r--   0      501       20     6309 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/diff.rs
--rw-r--r--   0      501       20    19238 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/format.rs
--rw-r--r--   0      501       20     1592 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/ignorer.rs
--rw-r--r--   0      501       20     4668 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/lib.rs
--rw-r--r--   0      501       20     8743 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/result.rs
--rw-r--r--   0      501       20     4766 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/rule/fullwidth.rs
--rw-r--r--   0      501       20    13453 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/rule/halfwidth.rs
--rw-r--r--   0      501       20    10177 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/rule/mod.rs
--rw-r--r--   0      501       20     2733 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/rule/rule.rs
--rw-r--r--   0      501       20     3967 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/rule/spellcheck.rs
--rw-r--r--   0      501       20     2192 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/rule/strategery.rs
--rw-r--r--   0      501       20     2968 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/rule/word.rs
--rw-r--r--   0      501       20     1563 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/serde_any/de.rs
--rw-r--r--   0      501       20      713 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/serde_any/error.rs
--rw-r--r--   0      501       20       52 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/src/serde_any/mod.rs
--rw-r--r--   0      501       20      369 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/tests/.autocorrectrc.test
--rw-r--r--   0      501       20     7914 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/tests/fixtures/jupyter.expected.json
--rw-r--r--   0      501       20    16656 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/tests/fixtures/jupyter.expected.txt
--rw-r--r--   0      501       20    16591 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/tests/fixtures/jupyter.ipynb
--rw-r--r--   0      501       20      849 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/tests/fixtures/jupyter.sm.ipynb
--rw-r--r--   0      501       20      644 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/local_dependencies/autocorrect/tests/format.rs
--rw-r--r--   0        0        0      685 1970-01-01 00:00:00.000000 autocorrect_py-2.6.2/Cargo.toml
--rw-r--r--   0      501       20     3078 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/.gitignore
--rw-r--r--   0      501       20     1603 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/README.md
--rw-r--r--   0      501       20      601 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/autocorrect_py.pyi
--rw-r--r--   0      501       20       76 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/pyproject.toml
--rw-r--r--   0      501       20     3660 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/src/lib.rs
--rw-r--r--   0      501       20     1461 2023-02-08 16:14:29.000000 autocorrect_py-2.6.2/test_autocorrect_py.py
--rw-r--r--   0        0        0     2007 1970-01-01 00:00:00.000000 autocorrect_py-2.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1161 1970-01-01 00:00:00.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/Cargo.toml
+-rw-r--r--   0      501       20     2482 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/.autocorrectrc.default
+-rw-r--r--   0      501       20     1066 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/LICENSE
+-rw-r--r--   0      501       20     5214 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/README.md
+-rw-r--r--   0      501       20     6828 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/benches/example.rs
+-rw-r--r--   0      501       20     1906 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/benches/fixtures/example.html
+-rw-r--r--   0      501       20      893 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/benches/fixtures/example.js
+-rw-r--r--   0      501       20      279 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/benches/fixtures/example.json
+-rw-r--r--   0      501       20     5194 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/benches/fixtures/example.md
+-rw-r--r--   0      501       20     3094 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/benches/fixtures/example.yml
+-rw-r--r--   0      501       20    97501 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/benches/fixtures/large.json
+-rw-r--r--   0      501       20     1892 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/asciidoc.pest
+-rw-r--r--   0      501       20      502 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/c.pest
+-rw-r--r--   0      501       20      295 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/conf.pest
+-rw-r--r--   0      501       20      603 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/csharp.pest
+-rw-r--r--   0      501       20      342 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/css.pest
+-rw-r--r--   0      501       20      618 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/dart.pest
+-rw-r--r--   0      501       20      768 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/elixir.pest
+-rw-r--r--   0      501       20      798 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/gettext.pest
+-rw-r--r--   0      501       20      793 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/go.pest
+-rw-r--r--   0      501       20     5199 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/html.pest
+-rw-r--r--   0      501       20      600 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/java.pest
+-rw-r--r--   0      501       20     1286 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/javascript.pest
+-rw-r--r--   0      501       20     1326 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/json.pest
+-rw-r--r--   0      501       20     1193 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/jupyter.pest
+-rw-r--r--   0      501       20      611 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/kotlin.pest
+-rw-r--r--   0      501       20      600 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/latex.pest
+-rw-r--r--   0      501       20     4224 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/markdown.pest
+-rw-r--r--   0      501       20      670 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/objective_c.pest
+-rw-r--r--   0      501       20      763 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/php.pest
+-rw-r--r--   0      501       20      721 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/python.pest
+-rw-r--r--   0      501       20      647 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/ruby.pest
+-rw-r--r--   0      501       20      579 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/rust.pest
+-rw-r--r--   0      501       20      664 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/scala.pest
+-rw-r--r--   0      501       20      420 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/sql.pest
+-rw-r--r--   0      501       20      594 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/strings.pest
+-rw-r--r--   0      501       20      794 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/swift.pest
+-rw-r--r--   0      501       20      589 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/xml.pest
+-rw-r--r--   0      501       20      696 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/yaml.pest
+-rw-r--r--   0      501       20       89 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/release.toml
+-rw-r--r--   0      501       20     3533 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/asciidoc.rs
+-rw-r--r--   0      501       20     1482 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/c.rs
+-rw-r--r--   0      501       20    12808 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/code.rs
+-rw-r--r--   0      501       20      987 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/conf.rs
+-rw-r--r--   0      501       20     1563 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/csharp.rs
+-rw-r--r--   0      501       20     1315 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/css.rs
+-rw-r--r--   0      501       20     1639 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/dart.rs
+-rw-r--r--   0      501       20     1717 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/elixir.rs
+-rw-r--r--   0      501       20     1528 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/gettext.rs
+-rw-r--r--   0      501       20     1716 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/go.rs
+-rw-r--r--   0      501       20     9557 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/html.rs
+-rw-r--r--   0      501       20     1628 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/java.rs
+-rw-r--r--   0      501       20     7364 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/javascript.rs
+-rw-r--r--   0      501       20     1649 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/json.rs
+-rw-r--r--   0      501       20    11585 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/jupyter.rs
+-rw-r--r--   0      501       20     1446 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/kotlin.rs
+-rw-r--r--   0      501       20     4600 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/latex.rs
+-rw-r--r--   0      501       20    12553 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/markdown.rs
+-rw-r--r--   0      501       20     4458 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/mod.rs
+-rw-r--r--   0      501       20     1453 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/objective_c.rs
+-rw-r--r--   0      501       20     1723 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/php.rs
+-rw-r--r--   0      501       20     1598 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/python.rs
+-rw-r--r--   0      501       20     1174 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/ruby.rs
+-rw-r--r--   0      501       20     2502 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/rust.rs
+-rw-r--r--   0      501       20     1627 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/scala.rs
+-rw-r--r--   0      501       20     1294 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/sql.rs
+-rw-r--r--   0      501       20     1318 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/strings.rs
+-rw-r--r--   0      501       20     1796 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/swift.rs
+-rw-r--r--   0      501       20     4816 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/types.rs
+-rw-r--r--   0      501       20     1253 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/xml.rs
+-rw-r--r--   0      501       20     1077 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/yaml.rs
+-rw-r--r--   0      501       20    13723 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/config/mod.rs
+-rw-r--r--   0      501       20     3000 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/config/severity.rs
+-rw-r--r--   0      501       20     2136 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/config/spellcheck.rs
+-rw-r--r--   0      501       20      407 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/config/toggle.pest
+-rw-r--r--   0      501       20     8865 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/config/toggle.rs
+-rw-r--r--   0      501       20     6309 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/diff.rs
+-rw-r--r--   0      501       20    19238 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/format.rs
+-rw-r--r--   0      501       20     1592 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/ignorer.rs
+-rw-r--r--   0      501       20     4682 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/lib.rs
+-rw-r--r--   0      501       20     1609 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/result/json.rs
+-rw-r--r--   0      501       20     8773 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/result/mod.rs
+-rw-r--r--   0      501       20     4670 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/result/rdjson.rs
+-rw-r--r--   0      501       20     4766 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/rule/fullwidth.rs
+-rw-r--r--   0      501       20    13453 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/rule/halfwidth.rs
+-rw-r--r--   0      501       20    10177 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/rule/mod.rs
+-rw-r--r--   0      501       20     2733 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/rule/rule.rs
+-rw-r--r--   0      501       20     3967 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/rule/spellcheck.rs
+-rw-r--r--   0      501       20     2192 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/rule/strategery.rs
+-rw-r--r--   0      501       20     2968 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/rule/word.rs
+-rw-r--r--   0      501       20     1563 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/serde_any/de.rs
+-rw-r--r--   0      501       20      713 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/serde_any/error.rs
+-rw-r--r--   0      501       20       52 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/src/serde_any/mod.rs
+-rw-r--r--   0      501       20      453 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/tests/.autocorrectrc.test
+-rw-r--r--   0      501       20     7914 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/tests/fixtures/jupyter.expected.json
+-rw-r--r--   0      501       20    16656 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/tests/fixtures/jupyter.expected.txt
+-rw-r--r--   0      501       20    16591 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/tests/fixtures/jupyter.ipynb
+-rw-r--r--   0      501       20      849 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/tests/fixtures/jupyter.sm.ipynb
+-rw-r--r--   0      501       20      644 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect/tests/format.rs
+-rw-r--r--   0        0        0      451 1970-01-01 00:00:00.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect-derive/Cargo.toml
+-rw-r--r--   0      501       20     1153 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/local_dependencies/autocorrect-derive/src/lib.rs
+-rw-r--r--   0        0        0      685 1970-01-01 00:00:00.000000 autocorrect_py-2.8.0/Cargo.toml
+-rw-r--r--   0      501       20     3078 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/.gitignore
+-rw-r--r--   0      501       20     1603 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/README.md
+-rw-r--r--   0      501       20      601 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/autocorrect_py.pyi
+-rw-r--r--   0      501       20       76 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/pyproject.toml
+-rw-r--r--   0      501       20     3660 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/src/lib.rs
+-rw-r--r--   0      501       20     1461 2023-08-01 09:02:27.000000 autocorrect_py-2.8.0/test_autocorrect_py.py
+-rw-r--r--   0        0        0     2007 1970-01-01 00:00:00.000000 autocorrect_py-2.8.0/PKG-INFO
```

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect-derive/src/lib.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect-derive/src/lib.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/Cargo.toml` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/Cargo.toml`

 * *Files 13% similar despite different names*

```diff
@@ -4,36 +4,36 @@
 edition = "2021"
 homepage = "https://github.com/huacnlee/autocorrect"
 keywords = ["autocorrect", "lint", "format"]
 license = "MIT"
 name = "autocorrect"
 readme = "../README.md"
 repository = "https://github.com/huacnlee/autocorrect"
-version = "2.6.2"
+version = "2.8.0"
 
 [lib]
 name = "autocorrect"
 path = "src/lib.rs"
 
 [dependencies]
-autocorrect-derive = {path = "../autocorrect-derive" }
+autocorrect-derive = {version = "0.3.0", path = "../autocorrect-derive" }
 diff = "0.1.13"
 ignore = "0.4"
 lazy_static = "1.4.0"
 owo-colors = "3"
-pest = "2.5.5"
-pest_derive = "2.5.5"
+pest = "2.6.1"
+pest_derive = "2.6.1"
 regex = "1"
 serde = {version = "1", features = ["derive"]}
 serde_json = "1.0.83"
 serde_repr = "0.1"
 serde_yaml = "0.9.9"
 
 [dev-dependencies]
-criterion = "0.3"
+criterion = "0.5"
 indoc = "1.0"
 pretty_assertions = "1.0.0"
 
 [build-dependencies]
 regex = "1"
 
 [profile.release]
```

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/.autocorrectrc.default` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/.autocorrectrc.default`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# yaml-language-server: $schema=https://huacnlee.github.io/autocorrect/schema.json
 rules:
   # Auto add spacing between CJK (Chinese, Japanese, Korean) and English words.
   # 0 - off, 1 - error, 2 - warning
   space-word: 1
   # Add space between some punctuations.
   space-punctuation: 1
   # Add space between brackets (), [] when near the CJK.
```

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/LICENSE` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/LICENSE`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/README.md` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/README.md`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/benches/example.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/benches/example.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/benches/fixtures/example.html` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/benches/fixtures/example.html`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/benches/fixtures/example.js` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/benches/fixtures/example.js`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/benches/fixtures/example.md` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/benches/fixtures/example.md`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/benches/fixtures/example.yml` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/benches/fixtures/example.yml`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/benches/fixtures/large.json` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/benches/fixtures/large.json`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/asciidoc.pest` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/asciidoc.pest`

 * *Files 17% similar despite different names*

```diff
@@ -1,57 +1,65 @@
-
-// https://docs.asciidoctor.org/asciidoc/latest
+//! Asciidoc Parser
+//! https://docs.asciidoctor.org/asciidoc/latest
 item = _{ SOI ~ line* ~ EOI }
 line = _{ expr }
 expr = _{ block | inline }
 
-block = ${ heading | codeblock | td_tag | paragraph }
+/// Block and Inline
+block  = ${ heading | codeblock | td_tag | paragraph }
 inline = _{ img | link | code | mark }
 
-string = ${ (!(inline | NEWLINE) ~ ANY)+ }
-paragraph = { (string | inline)+ }
+/// string and text
+string    = ${ (!(inline | NEWLINE) ~ ANY)+ }
+paragraph =  { (string | inline)+ }
 
+/// Whitespace
 WHITESPACE = { " " | "\t" | NEWLINE }
 
-codeblock = ${ 
-  codeblock_filename* ~ codeblock_meta* ~ 
-  PUSH("----" | "....") ~ codeblock_lang ~ codeblock_code ~ PUSH("----" | "....")
+/// Codeblock
+codeblock          = ${
+    codeblock_filename* ~ codeblock_meta* ~ PUSH("----" | "....") ~ codeblock_lang ~ codeblock_code ~ PUSH("----" | "....")
 }
 codeblock_filename = @{ "." ~ (!NEWLINE ~ ANY)+ ~ NEWLINE }
-codeblock_meta = @{ "[" ~ (!"]" ~ ANY)+ ~ "]" ~ NEWLINE  }
-codeblock_lang = { ASCII_ALPHA* }
-codeblock_code = { (!(PEEK) ~ ANY)* }
+codeblock_meta     = @{ "[" ~ (!"]" ~ ANY)+ ~ "]" ~ NEWLINE }
+codeblock_lang     =  { ASCII_ALPHA* }
+codeblock_code     =  { (!(PEEK) ~ ANY)* }
 
+/// Table TD
 td_tag = @{ "|" }
 
+/// Image
 img_start = @{ "!" }
-img = ${ img_start ~ link }
+img       = ${ img_start ~ link }
+
+/// Link
+link        = ${ link_string ~ href }
+link_string =  { "[" ~ (!("]" | NEWLINE) ~ ANY)* ~ "]" }
+href        =  { "(" ~ (!(")" | NEWLINE) ~ ANY)* ~ ")" }
+
+/// Inline marks
+open_mark   = @{
+    "**" // https://docs.asciidoctor.org/asciidoc/latest/text/bold/
+
+  | "*" // Italic https://docs.asciidoctor.org/asciidoc/latest/text/italic/
+
+  | "_" // Highlight https://docs.asciidoctor.org/asciidoc/latest/text/highlight/
+
+  | "#" // Subscript https://docs.asciidoctor.org/asciidoc/latest/text/subscript-and-superscript/
+
+  | "~" // Superscript
 
-link = ${ link_string ~ href }
-link_string = { "[" ~ (!("]" | NEWLINE) ~ ANY)* ~ "]" } 
-href = { "(" ~ (!(")" | NEWLINE) ~ ANY)* ~ ")" }
-
-open_mark = @{
-  // Bold https://docs.asciidoctor.org/asciidoc/latest/text/bold/
-  "**"
-  // https://docs.asciidoctor.org/asciidoc/latest/text/bold/
-  | "*"
-  // Italic https://docs.asciidoctor.org/asciidoc/latest/text/italic/
-  | "_"
-  // Highlight https://docs.asciidoctor.org/asciidoc/latest/text/highlight/
-  | "#"
-  // Subscript https://docs.asciidoctor.org/asciidoc/latest/text/subscript-and-superscript/
-  | "~"
-  // Superscript
   | "^"
 }
-close_mark = @{ POP }
-mark = ${ PUSH(open_mark) ~ (mark | mark_string) ~ close_mark }
-mark_string = { (!(PEEK | NEWLINE | inline) ~ ANY)* }
-
-code = ${ PUSH(open_code) ~ inner_code ~ close_code }
-open_code = @{ "`" }
+close_mark  = @{ POP }
+mark        = ${ PUSH(open_mark) ~ (mark | mark_string) ~ close_mark }
+mark_string =  { (!(PEEK | NEWLINE | inline) ~ ANY)* }
+
+/// Inline code
+code       = ${ PUSH(open_code) ~ inner_code ~ close_code }
+open_code  = @{ "`" }
 close_code = @{ POP }
-inner_code = @{ (!(NEWLINE | PEEK) ~ ANY)*  }
+inner_code = @{ (!(NEWLINE | PEEK) ~ ANY)* }
 
+/// Heading
 heading_tag = @{ ("======" | "=====" | "====" | "===" | "==" | "=") ~ " "* }
-heading = ${ PUSH(heading_tag) ~ string }
+heading     = ${ PUSH(heading_tag) ~ string }
```

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/csharp.pest` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/scala.pest`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,24 @@
-item = _{ SOI ~ line* ~ EOI } 
-line = _{ regexp | string | other }
+//! Scala Parser
+item       = _{ SOI ~ line* ~ EOI }
+line       = _{ regexp | string_literal | string | other }
+other      = ${ !(string) ~ ANY }
+WHITESPACE =  { " " | "\t" | NEWLINE }
 
-other = ${ !(string) ~ ANY }
-
-WHITESPACE = { " " | "\t" | NEWLINE }
-
-line_comment  = _{ "//" ~ (!(NEWLINE) ~ ANY)* }
-block_comment = _{ "/*" ~ (!("*/") ~ ANY)* ~ "*/"}
+/// Comment
 COMMENT       = ${ line_comment | block_comment }
+line_comment  = _{ "//" ~ (!(NEWLINE) ~ ANY)* }
+block_comment = _{ "/*" ~ (!("*/") ~ ANY)* ~ "*/" }
 
-string       = ${ inner_string }
-inner_string = _{ 
-  ("@\"" ~ (!("\"") ~ ANY)* ~ "\"") 
-  | ("\"" ~ (!(NEWLINE | "\"") ~ ANY)* ~ "\"") 
-  | ("$\"" ~ (!(NEWLINE | "\"") ~ ANY)* ~ "\"") 
+/// String
+string         = ${ inner_string }
+inner_string   = _{
+    ("\"\"\"" ~ (!("\"\"\"") ~ ANY)* ~ "\"\"\"")
+  | ("\"" ~ (!(NEWLINE | "\"") ~ ANY)* ~ "\"")
 }
+string_literal = ${ "s" ~ inner_string }
 
-regexp = ${ "Regex(" ~ " "* ~ inner_string ~ (!")" ~ ANY)* ~ ")" }
+/// Regexp
+regexp = ${
+    ("Regex(" ~ " "* ~ inner_string ~ (!")" ~ ANY)* ~ ")")
+  | (inner_string ~ ".r")
+}
```

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/dart.pest` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/elixir.pest`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,27 @@
-item = _{ SOI ~ line* ~ EOI } 
-line = _{ regexp | string | other }
+//! Elixir Parser
+item       = _{ SOI ~ line* ~ EOI }
+line       = _{ regexp | string | other }
+other      = ${ !(string) ~ ANY }
+WHITESPACE =  { " " | "\t" | NEWLINE }
 
-other = ${ !(string) ~ ANY }
-
-WHITESPACE = { " " | "\t" | NEWLINE }
-
-line_comment  = _{ "//" ~ (!(NEWLINE) ~ ANY)* }
-block_comment = _{ "/*" ~ (!("*/") ~ ANY)* ~ "*/" }
+/// Comment
+line_comment  = _{ "#" ~ (!(NEWLINE) ~ ANY)* }
+block_comment = _{ "\"\"\"" ~ (!("\"\"\"") ~ ANY)* ~ "\"\"\"" }
 COMMENT       = ${ line_comment | block_comment }
 
-string       = ${ inner_string }
-inner_string = _{ 
-  ("'''" ~ (!("'''") ~ ANY)* ~ "'''") 
-  | ("'" ~ (!("'" | NEWLINE) ~ ANY)* ~ "'") 
-  | ("\"\"\"" ~ (!("\"\"\"") ~ ANY)* ~ "\"\"\"") 
-  | ("\"" ~ (!("\"" | NEWLINE) ~ ANY)* ~ "\"") 
+/// String
+string       = ${
+    inner_string
+  | ("\"\"\"" ~ (!("\"\"\"") ~ ANY)* ~ "\"\"\"")
+  | ("~" ~ ("s" | "c") ~ "(" ~ (!(NEWLINE | ")") ~ ANY)* ~ ")")
+}
+inner_string = _{
+    ("'" ~ (!(inner_string | "'") ~ ANY)* ~ "'")
+  | ("\"" ~ (!(inner_string | "\"") ~ ANY)* ~ "\"")
 }
 
-regexp = ${ "r" ~ inner_string }
+/// Regex
+regexp = ${
+    ("~r/" ~ (!(inner_string | "/") ~ ANY)* ~ "/")
+  | ("Regex.compile(" ~ " "* ~ inner_string ~ (!")" ~ ANY)* ~ ")")
+}
```

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/elixir.pest` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/python.pest`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-item = _{ SOI ~ line* ~ EOI } 
-line = _{ regexp | string | other }
+//! Python Parser
+item       = _{ SOI ~ line* ~ EOI }
+line       = _{ regexp | string | other }
+other      = ${ !(string) ~ ANY }
+WHITESPACE =  { " " | "\t" | NEWLINE }
 
-other = ${ !(string) ~ ANY }
-
-WHITESPACE = { " " | "\t" | NEWLINE }
-
-line_comment  = _{ "#" ~ (!(NEWLINE) ~ ANY)* }
-block_comment = _{ "\"\"\"" ~ (!("\"\"\"") ~ ANY)* ~ "\"\"\"" }
+/// Comment
 COMMENT       = ${ line_comment | block_comment }
+line_comment  = _{ "#" ~ (!(NEWLINE) ~ ANY)* }
+block_comment = _{ "'''" ~ (!("'''") ~ ANY)* ~ "'''" }
 
-string = ${ 
-  inner_string 
-  | ("\"\"\"" ~ (!("\"\"\"") ~ ANY)* ~ "\"\"\"") 
-  | ("~" ~ ("s" | "c") ~ "(" ~ (!(NEWLINE | ")") ~ ANY)* ~ ")") 
-}
+/// String
+string       = ${ inner_string }
 inner_string = _{
-  ("'" ~ (!(inner_string | "'") ~ ANY)* ~ "'") 
-  | ("\"" ~ (!(inner_string | "\"") ~ ANY)* ~ "\"") 
+    ("'" ~ (!(NEWLINE | "'") ~ ANY)* ~ "'")
+  | ("\"\"\"" ~ (!("\"\"\"") ~ ANY)* ~ "\"\"\""+)
+  | ("\"" ~ (!(NEWLINE | "\"") ~ ANY)* ~ "\"")
 }
 
+/// Regexp
 regexp = ${
-  ( "~r/" ~ (!(inner_string | "/") ~ ANY)* ~ "/" )
-  | ("Regex.compile(" ~ " "* ~ inner_string ~  (!")" ~ ANY)* ~ ")")
+    ("r'" ~ (!(NEWLINE | "'") ~ ANY)* ~ "'")
+  | ("r\"\"\"" ~ (!("\"\"\"") ~ ANY)* ~ "\"\"\"")
+  | ("compile(" ~ " "* ~ inner_string ~ (!")" ~ ANY)* ~ ")")
 }
```

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/gettext.pest` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/gettext.pest`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,29 @@
-item = _{ SOI ~ line* ~ EOI } 
-line = _{ pair | key | value | string | refrence | other }
-
-other = ${ !(string) ~ ANY }
-
-WHITESPACE = { " " | "\t" | NEWLINE }
-
-refrence = ${ "#:" ~ (!(NEWLINE) ~ ANY)* }
+//! Gettext Parser
+item       = _{ SOI ~ line* ~ EOI }
+line       = _{ pair | key | value | string | refrence | other }
+other      = ${ !(string) ~ ANY }
+WHITESPACE =  { " " | "\t" | NEWLINE }
 
+/// Comment
 line_comment  = _{ "#" ~ (!(NEWLINE) ~ ANY)* }
 block_comment = _{ "/*" ~ (!("*/") ~ ANY)* ~ "*/" }
 COMMENT       = ${ line_comment | block_comment }
 
-key_func   = @{ "msgid" | "msgid_plural" | "msgctxt" }
-value_func = @{ "msgstr" }
+/// refrence
+refrence = ${ "#:" ~ (!(NEWLINE) ~ ANY)* }
 
-string = @{ inner_string }
+/// string
+string       = @{ inner_string }
 inner_string = @{
-  ("'" ~ (!(NEWLINE | "'") ~ ANY)* ~ "'") 
-  | ("\"" ~ (!(NEWLINE | "\"") ~ ANY)* ~ "\"") 
+    ("'" ~ (!(NEWLINE | "'") ~ ANY)* ~ "'")
+  | ("\"" ~ (!(NEWLINE | "\"") ~ ANY)* ~ "\"")
 }
 
-pair  = _{ key ~ NEWLINE+ ~ value } 
-key   = ${ key_func ~ other* ~ inner_string } 
+/// pair
+pair  = _{ key ~ NEWLINE+ ~ value }
+key   = ${ key_func ~ other* ~ inner_string }
 value = ${ value_func ~ other* ~ string }
 
+/// key value
+key_func   = @{ "msgid" | "msgid_plural" | "msgctxt" }
+value_func = @{ "msgstr" }
```

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/go.pest` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/go.pest`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-item = _{ SOI ~ line* ~ EOI } 
-line = _{ regexp | timeparse | string | other }
-
-other = ${ !(string) ~ ANY }
-
-WHITESPACE = { " " | "\t" | NEWLINE }
+//! Go Parser
+item       = _{ SOI ~ line* ~ EOI }
+line       = _{ regexp | timeparse | string | other }
+other      = ${ !(string) ~ ANY }
+WHITESPACE =  { " " | "\t" | NEWLINE }
 
+/// Comment
 line_comment  = _{ "//" ~ (!(NEWLINE) ~ ANY)* }
-block_comment = _{ "/*" ~ (!("*/") ~ ANY)* ~ "*/"}
+block_comment = _{ "/*" ~ (!("*/") ~ ANY)* ~ "*/" }
 COMMENT       = ${ line_comment | block_comment }
 
+/// String
 string       = ${ inner_string }
 inner_string = _{
-  ("`" ~ (!("`" | string_verb) ~ ANY)* ~ "`") 
-  | ("\"" ~ (!(NEWLINE | "\"" | string_verb) ~ ANY)* ~ "\"") 
+    ("`" ~ (!("`" | string_verb) ~ ANY)* ~ "`")
+  | ("\"" ~ (!(NEWLINE | "\"" | string_verb) ~ ANY)* ~ "\"")
 }
-string_verb  = { "%" ~ ("s" | "q" | "v") }
+string_verb  =  { "%" ~ ("s" | "q" | "v") }
 
-regexp = ${
-  ("regexp." ~ (ASCII_ALPHA)+ ~ "(" ~ " "* ~ inner_string ~ (!")" ~ ANY)* ~ ")")
+/// Regex and other special function
+regexp    = ${
+    ("regexp." ~ (ASCII_ALPHA)+ ~ "(" ~ " "* ~ inner_string ~ (!")" ~ ANY)* ~ ")")
 }
 timeparse = ${
-  ("time." ~ (ASCII_ALPHA)+ ~ "(" ~ " "* ~ inner_string ~ (!")" ~ ANY)* ~ ")")
-}
+    ("time." ~ (ASCII_ALPHA)+ ~ "(" ~ " "* ~ inner_string ~ (!")" ~ ANY)* ~ ")")
+}
```

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/html.pest` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/html.pest`

 * *Files 26% similar despite different names*

```diff
@@ -1,163 +1,142 @@
-//
-// HTML
-//
-// Fork from:
-// https://github.com/mathiversen/html-parser/blob/v0.6.3/src/grammar/rules.pest
-//
+//! HTML Parser
+//!
+//! Fork from:
+//! https://github.com/mathiversen/html-parser/blob/v0.6.3/src/grammar/rules.pest
 item = _{
-    SOI
-    ~ comment*
-    ~ doctype?
-    ~ node*
-    ~ EOI
+    SOI ~ comment* ~ doctype? ~ node* ~ EOI
 }
-
 // Other
-other = { !(comment | node_element | server | text) ~ ANY }
-
+other      = { !(comment | node_element | server | text) ~ ANY }
 WHITESPACE = { " " | "\t" | NEWLINE }
 
-// Code
+/// Code
 code = ${ "<code>" ~ (!"</code>" ~ ANY)* ~ "</code>" }
 
-//
-// DOCTYPE
-//
-doctype = { chevron_left_bang ~ doctype_name ~ attr* ~ chevron_right_normal }
+/// DOCTYPE
+doctype      =  { chevron_left_bang ~ doctype_name ~ attr* ~ chevron_right_normal }
 doctype_name = @{ ^"doctype" }
 
-//
-// SERVER CODE
-//
-server = ${ chevron_left_server ~ server_code ~ chevron_right_server }
-server_code = { (!chevron_right_server ~ ANY)* }
-chevron_left_server = { "<%" }
-chevron_right_server = { "%>" }
-
-//
-// NODES
-//
-node = _{ code | server | comment | node_element | text | other }
-comment = { comment_if | comment_normal }
-text = ${ (!(chevron_left_normal | comment_tag_start ) ~ ANY)+ } // NOTE: Should we be able to write < in text? ^^
+/// SERVER CODE
+server               = ${ chevron_left_server ~ server_code ~ chevron_right_server }
+server_code          =  { (!chevron_right_server ~ ANY)* }
+chevron_left_server  =  { "<%" }
+chevron_right_server =  { "%>" }
+
+/// NODES
+node    = _{ code | server | comment | node_element | text | other }
+comment =  { comment_if | comment_normal }
+text    = ${ (!(chevron_left_normal | comment_tag_start) ~ ANY)+ }
+// NOTE: Should we be able to write < in text? ^^
 node_element = { el_void | el_void_xml | el_process_instruct | javascript_text | style_text | el_raw_text | el_normal | el_dangling }
 
-//
-// COMMENTS
-//
-comment_normal = _{ comment_tag_start ~ (!comment_tag_end ~ ANY)* ~ comment_tag_end }
+/// COMMENTS
+comment_normal    = _{ comment_tag_start ~ (!comment_tag_end ~ ANY)* ~ comment_tag_end }
 comment_tag_start = _{ chevron_left_bang ~ "--" }
-comment_tag_end = _{ "--" ~ chevron_right_normal }
+comment_tag_end   = _{ "--" ~ chevron_right_normal }
 
-// Compatability with old IE browsers... This is not necessary for newer browsers
-comment_if = _{ comment_if_start ~ (!comment_if_end ~ ANY)* ~ comment_if_end }
+/// Compatability with old IE browsers... This is not necessary for newer browsers
+comment_if       = _{ comment_if_start ~ (!comment_if_end ~ ANY)* ~ comment_if_end }
 comment_if_start = _{ comment_tag_start ~ "[" ~ ^"if" }
-comment_if_end = _{ chevron_left_bang ~ "[" ~ ^"endif" ~ "]" ~ comment_tag_end }
+comment_if_end   = _{ chevron_left_bang ~ "[" ~ ^"endif" ~ "]" ~ comment_tag_end }
 
-//
-// ATTRIBUTES
-//
-attr = { attr_key ~ (equal ~ (attr_non_quoted | attr_quoted ))? }
-attr_quoted =  { PUSH(quote) ~ attr_value ~ PUSH(quote) }
+/// ATTRIBUTES
+attr            =  { attr_key ~ (equal ~ (attr_non_quoted | attr_quoted))? }
+attr_quoted     =  { PUSH(quote) ~ attr_value ~ end_attr_quoted }
+end_attr_quoted = { POP }
 attr_non_quoted = @{ !quote ~ (!(WHITESPACE | chevron_right) ~ ANY)* }
-attr_key = ${ !WHITESPACE ~ (":" | "@" | "#" | ".")? ~ ASCII_ALPHA ~ text_chars* }
-attr_value = ${ WHITESPACE* ~ (!PEEK ~ ANY)* ~ WHITESPACE* }
+attr_key        = ${ !WHITESPACE ~ (":" | "@" | "#" | ".")? ~ ASCII_ALPHA ~ text_chars* }
+attr_value      = ${ WHITESPACE* ~ (!PEEK ~ ANY)* ~ WHITESPACE* }
 
-//
-// ELEMENTS
-//
+/// ELEMENTS
 el_name = @{ ASCII_ALPHA ~ text_chars* }
 
-// Void element aka self-closing element
-// Ex: <hr>
+/// Void element aka self-closing element
+/// Ex: <hr>
 el_void_name_html = @{
     ^"area"
-    | ^"base"
-    | ^"br"
-    | ^"col"
-    | ^"command"
-    | ^"embed"
-    | ^"hr"
-    | ^"img"
-    | ^"input"
-    | ^"keygen"
-    | ^"link"
-    | ^"meta"
-    | ^"param"
-    | ^"source"
-    | ^"track"
-    | ^"wbr"
-    | ^"meta"
+  | ^"base"
+  | ^"br"
+  | ^"col"
+  | ^"command"
+  | ^"embed"
+  | ^"hr"
+  | ^"img"
+  | ^"input"
+  | ^"keygen"
+  | ^"link"
+  | ^"meta"
+  | ^"param"
+  | ^"source"
+  | ^"track"
+  | ^"wbr"
+  | ^"meta"
 }
 // NOTE: This should not have to be a rule, but people doesn't know what void elements are...
 el_void_name_svg = @{
     ^"path"
-    | ^"polygon"
-    | ^"rect"
-    | ^"circle"
+  | ^"polygon"
+  | ^"rect"
+  | ^"circle"
 }
-el_void_name = @{ el_void_name_html | el_void_name_svg }
-el_void = _{ chevron_left_normal ~ el_void_name ~ attr* ~ (chevron_right_normal | chevron_right_closed) }
-el_void_xml = _{ chevron_left_normal ~ el_name ~ attr* ~ chevron_right_closed }
-
-// Open elements are default element that can take children 
-// and have both a start tag and an end tag
-// Ex: <html lang="en"></html>
-el_normal = _{ el_normal_start ~ (!el_normal_end ~ node)* ~ el_normal_end }
-el_normal_start = _{ chevron_left_normal ~ PUSH(el_name) ~ attr* ~ chevron_right_normal}
-el_normal_end = _{ chevron_left_closed ~ PUSH(el_name) ~ chevron_right_normal}
-
-// Raw text elements are elements with text/script content that
-// might interfere with the normal html syntax
-el_raw_text_name = {
+el_void_name     = @{ el_void_name_html | el_void_name_svg }
+el_void          = _{ chevron_left_normal ~ el_void_name ~ attr* ~ (chevron_right_normal | chevron_right_closed) }
+el_void_xml      = _{ chevron_left_normal ~ el_name ~ attr* ~ chevron_right_closed }
+
+/// Open elements are default element that can take children
+/// and have both a start tag and an end tag
+/// Ex: <html lang="en"></html>
+el_normal       = _{ el_normal_start ~ (!el_normal_end ~ node)* ~ el_normal_end }
+el_normal_start = _{ chevron_left_normal ~ PUSH(el_name) ~ attr* ~ chevron_right_normal }
+el_normal_end   = _{ chevron_left_closed ~ PUSH(el_name) ~ chevron_right_normal }
+
+/// Raw text elements are elements with text/script content that
+/// might interfere with the normal html syntax
+el_raw_text_name    =  {
     ^"title"
-    | ^"textarea"
+  | ^"textarea"
 }
 el_raw_text_content = ${ (!el_raw_text_end ~ ANY)* }
-el_raw_text = _{ el_raw_text_start ~ el_raw_text_content ~ el_raw_text_end }
-el_raw_text_start = _{ chevron_left_normal ~ PUSH(el_raw_text_name) ~ attr* ~ chevron_right_normal}
-el_raw_text_end = { chevron_left_closed ~ PUSH(el_raw_text_name) ~ chevron_right_normal}
-
-inline_javascript = ${ (!javascript_end ~ ANY)* }
-javascript_text = _{ javascript_start ~ inline_javascript ~ javascript_end }
-el_javascript_name = @{ ^"script" }
-javascript_start = _{ chevron_left_normal ~ PUSH(el_javascript_name) ~ attr* ~ chevron_right_normal}
-javascript_end = { chevron_left_closed ~ PUSH(el_javascript_name) ~ chevron_right_normal}
-
-inline_style = ${ (!style_end ~ ANY)* }
-el_style_name = @{ ^"style" }
-style_text = _{ style_start ~ inline_style ~ style_end }
-style_start = _{ chevron_left_normal ~ PUSH(el_style_name) ~ attr* ~ chevron_right_normal}
-style_end = { chevron_left_closed ~ PUSH(el_style_name) ~ chevron_right_normal}
+el_raw_text         = _{ el_raw_text_start ~ el_raw_text_content ~ el_raw_text_end }
+el_raw_text_start   = _{ chevron_left_normal ~ PUSH(el_raw_text_name) ~ attr* ~ chevron_right_normal }
+el_raw_text_end     =  { chevron_left_closed ~ PUSH(el_raw_text_name) ~ chevron_right_normal }
+inline_javascript   = ${ (!javascript_end ~ ANY)* }
+javascript_text     = _{ javascript_start ~ inline_javascript ~ javascript_end }
+el_javascript_name  = @{ ^"script" }
+javascript_start    = _{ chevron_left_normal ~ PUSH(el_javascript_name) ~ attr* ~ chevron_right_normal }
+javascript_end      =  { chevron_left_closed ~ PUSH(el_javascript_name) ~ chevron_right_normal }
+inline_style        = ${ (!style_end ~ ANY)* }
+el_style_name       = @{ ^"style" }
+style_text          = _{ style_start ~ inline_style ~ style_end }
+style_start         = _{ chevron_left_normal ~ PUSH(el_style_name) ~ attr* ~ chevron_right_normal }
+style_end           =  { chevron_left_closed ~ PUSH(el_style_name) ~ chevron_right_normal }
 
-// XML processing instruction
-// Ex: <?xml version="1.0" ?>
+/// XML processing instruction
+/// Ex: <?xml version="1.0" ?>
 el_process_instruct = { chevron_left_question ~ el_name? ~ attr* ~ chevron_right_question }
 
-// Catch dangling elements
-// Ex: <div/></div>
-el_dangling = { chevron_left_closed ~ el_name ~ chevron_right_normal}
-
-//
-// SYMBOLS / CHARACTERS
-//
-text_chars = _{'a'..'z' | 'A'..'Z' | "_" | "-" | ":" |'0'..'9'}
-
-chevron_left_normal = { "<"}
-chevron_left_closed = { "</" }
-chevron_left_bang = { "<!" }
+/// Catch dangling elements
+/// Ex: <div/></div>
+el_dangling = { chevron_left_closed ~ el_name ~ chevron_right_normal }
+
+/// SYMBOLS / CHARACTERS
+text_chars = _{ 'a'..'z' | 'A'..'Z' | "_" | "-" | ":" | '0'..'9' }
+
+/// tag left
+chevron_left_normal   = { "<" }
+chevron_left_closed   = { "</" }
+chevron_left_bang     = { "<!" }
 chevron_left_question = { "<?" }
 
-chevron_right_normal = { ">" }
-chevron_right_closed = { "/>" }
-chevron_right_question = { "?>" }
-chevron_right = _{
+/// tag right
+chevron_right_normal   =  { ">" }
+chevron_right_closed   =  { "/>" }
+chevron_right_question =  { "?>" }
+chevron_right          = _{
     chevron_right_normal
-    | chevron_right_closed
-    | chevron_right_question
+  | chevron_right_closed
+  | chevron_right_question
 }
 
-equal = { "=" }
-quote_dubble = { "\"" }
-quote_single = { "'" }
-quote = _{ quote_dubble | quote_single }
+/// other
+equal        = @{ "=" }
+quote        = @{ "\"" | "'" }
```

#### html2text {}

```diff
@@ -1,69 +1,69 @@
-// // HTML // // Fork from: // https://github.com/mathiversen/html-parser/blob/
-v0.6.3/src/grammar/rules.pest // item = _{ SOI ~ comment* ~ doctype? ~ node* ~
-EOI } // Other other = { !(comment | node_element | server | text) ~ ANY }
-WHITESPACE = { " " | "\t" | NEWLINE } // Code code = ${ "" ~ (!"" ~ ANY)* ~ "
-" } // // DOCTYPE // doctype = { chevron_left_bang ~ doctype_name ~ attr* ~
-chevron_right_normal } doctype_name = @{ ^"doctype" } // // SERVER CODE /
-/ server = ${ chevron_left_server ~ server_code ~ chevron_right_server }
-server_code = { (!chevron_right_server ~ ANY)* } chevron_left_server = { "<%" }
-chevron_right_server = { "%>" } // // NODES // node = _{ code | server |
-comment | node_element | text | other } comment = { comment_if | comment_normal
-} text = ${ (!(chevron_left_normal | comment_tag_start ) ~ ANY)+ } // NOTE:
-Should we be able to write < in text? ^^ node_element = { el_void | el_void_xml
-| el_process_instruct | javascript_text | style_text | el_raw_text | el_normal
-| el_dangling } // // COMMENTS // comment_normal = _{ comment_tag_start ~
+//! HTML Parser //! //! Fork from: //! https://github.com/mathiversen/html-
+parser/blob/v0.6.3/src/grammar/rules.pest item = _{ SOI ~ comment* ~ doctype? ~
+node* ~ EOI } // Other other = { !(comment | node_element | server | text) ~
+ANY } WHITESPACE = { " " | "\t" | NEWLINE } /// Code code = ${ "" ~ (!"" ~
+ANY)* ~ "
+" } /// DOCTYPE doctype = { chevron_left_bang ~ doctype_name ~ attr* ~
+chevron_right_normal } doctype_name = @{ ^"doctype" } /// SERVER CODE server =
+${ chevron_left_server ~ server_code ~ chevron_right_server } server_code = {
+(!chevron_right_server ~ ANY)* } chevron_left_server = { "<%" }
+chevron_right_server = { "%>" } /// NODES node = _{ code | server | comment |
+node_element | text | other } comment = { comment_if | comment_normal } text =
+${ (!(chevron_left_normal | comment_tag_start) ~ ANY)+ } // NOTE: Should we be
+able to write < in text? ^^ node_element = { el_void | el_void_xml |
+el_process_instruct | javascript_text | style_text | el_raw_text | el_normal |
+el_dangling } /// COMMENTS comment_normal = _{ comment_tag_start ~
 (!comment_tag_end ~ ANY)* ~ comment_tag_end } comment_tag_start = _
 { chevron_left_bang ~ "--" } comment_tag_end = _{ "--" ~ chevron_right_normal }
-// Compatability with old IE browsers... This is not necessary for newer
+/// Compatability with old IE browsers... This is not necessary for newer
 browsers comment_if = _{ comment_if_start ~ (!comment_if_end ~ ANY)* ~
 comment_if_end } comment_if_start = _{ comment_tag_start ~ "[" ~ ^"if" }
 comment_if_end = _{ chevron_left_bang ~ "[" ~ ^"endif" ~ "]" ~ comment_tag_end
-} // // ATTRIBUTES // attr = { attr_key ~ (equal ~ (attr_non_quoted |
-attr_quoted ))? } attr_quoted = { PUSH(quote) ~ attr_value ~ PUSH(quote) }
-attr_non_quoted = @{ !quote ~ (!(WHITESPACE | chevron_right) ~ ANY)* } attr_key
-= ${ !WHITESPACE ~ (":" | "@" | "#" | ".")? ~ ASCII_ALPHA ~ text_chars* }
-attr_value = ${ WHITESPACE* ~ (!PEEK ~ ANY)* ~ WHITESPACE* } // // ELEMENTS /
-/ el_name = @{ ASCII_ALPHA ~ text_chars* } // Void element aka self-closing
-element // Ex:
+} /// ATTRIBUTES attr = { attr_key ~ (equal ~ (attr_non_quoted | attr_quoted))?
+} attr_quoted = { PUSH(quote) ~ attr_value ~ end_attr_quoted } end_attr_quoted
+= { POP } attr_non_quoted = @{ !quote ~ (!(WHITESPACE | chevron_right) ~ ANY)*
+} attr_key = ${ !WHITESPACE ~ (":" | "@" | "#" | ".")? ~ ASCII_ALPHA ~
+text_chars* } attr_value = ${ WHITESPACE* ~ (!PEEK ~ ANY)* ~ WHITESPACE* } //
+/ ELEMENTS el_name = @{ ASCII_ALPHA ~ text_chars* } /// Void element aka self-
+closing element /// Ex:
 ===============================================================================
 el_void_name_html = @{ ^"area" | ^"base" | ^"br" | ^"col" | ^"command" |
 ^"embed" | ^"hr" | ^"img" | ^"input" | ^"keygen" | ^"link" | ^"meta" | ^"param"
 | ^"source" | ^"track" | ^"wbr" | ^"meta" } // NOTE: This should not have to be
 a rule, but people doesn't know what void elements are... el_void_name_svg = @
 { ^"path" | ^"polygon" | ^"rect" | ^"circle" } el_void_name = @
 { el_void_name_html | el_void_name_svg } el_void = _{ chevron_left_normal ~
 el_void_name ~ attr* ~ (chevron_right_normal | chevron_right_closed) }
 el_void_xml = _{ chevron_left_normal ~ el_name ~ attr* ~ chevron_right_closed }
-// Open elements are default element that can take children // and have both a
-start tag and an end tag // Ex:
+/// Open elements are default element that can take children /// and have both
+a start tag and an end tag /// Ex:
 el_normal = _{ el_normal_start ~ (!el_normal_end ~ node)* ~ el_normal_end }
 el_normal_start = _{ chevron_left_normal ~ PUSH(el_name) ~ attr* ~
-chevron_right_normal} el_normal_end = _{ chevron_left_closed ~ PUSH(el_name) ~
-chevron_right_normal} // Raw text elements are elements with text/script
-content that // might interfere with the normal html syntax el_raw_text_name =
+chevron_right_normal } el_normal_end = _{ chevron_left_closed ~ PUSH(el_name) ~
+chevron_right_normal } /// Raw text elements are elements with text/script
+content that /// might interfere with the normal html syntax el_raw_text_name =
 { ^"title" | ^"textarea" } el_raw_text_content = ${ (!el_raw_text_end ~ ANY)* }
 el_raw_text = _{ el_raw_text_start ~ el_raw_text_content ~ el_raw_text_end }
 el_raw_text_start = _{ chevron_left_normal ~ PUSH(el_raw_text_name) ~ attr* ~
-chevron_right_normal} el_raw_text_end = { chevron_left_closed ~ PUSH
-(el_raw_text_name) ~ chevron_right_normal} inline_javascript = ${
+chevron_right_normal } el_raw_text_end = { chevron_left_closed ~ PUSH
+(el_raw_text_name) ~ chevron_right_normal } inline_javascript = ${
 (!javascript_end ~ ANY)* } javascript_text = _{ javascript_start ~
 inline_javascript ~ javascript_end } el_javascript_name = @{ ^"script" }
 javascript_start = _{ chevron_left_normal ~ PUSH(el_javascript_name) ~ attr* ~
-chevron_right_normal} javascript_end = { chevron_left_closed ~ PUSH
-(el_javascript_name) ~ chevron_right_normal} inline_style = ${ (!style_end ~
+chevron_right_normal } javascript_end = { chevron_left_closed ~ PUSH
+(el_javascript_name) ~ chevron_right_normal } inline_style = ${ (!style_end ~
 ANY)* } el_style_name = @{ ^"style" } style_text = _{ style_start ~
 inline_style ~ style_end } style_start = _{ chevron_left_normal ~ PUSH
-(el_style_name) ~ attr* ~ chevron_right_normal} style_end =
-{ chevron_left_closed ~ PUSH(el_style_name) ~ chevron_right_normal} // XML
-processing instruction // Ex: <?xml version="1.0" ?> el_process_instruct =
-{ chevron_left_question ~ el_name? ~ attr* ~ chevron_right_question } // Catch
-dangling elements // Ex:
-el_dangling = { chevron_left_closed ~ el_name ~ chevron_right_normal} // /
-/ SYMBOLS / CHARACTERS // text_chars = _{'a'..'z' | 'A'..'Z' | "_" | "-" | ":
-" |'0'..'9'} chevron_left_normal = { "<"} chevron_left_closed = { "
+(el_style_name) ~ attr* ~ chevron_right_normal } style_end =
+{ chevron_left_closed ~ PUSH(el_style_name) ~ chevron_right_normal } /// XML
+processing instruction /// Ex: <?xml version="1.0" ?> el_process_instruct =
+{ chevron_left_question ~ el_name? ~ attr* ~ chevron_right_question } /// Catch
+dangling elements /// Ex:
+el_dangling = { chevron_left_closed ~ el_name ~ chevron_right_normal } //
+/ SYMBOLS / CHARACTERS text_chars = _{ 'a'..'z' | 'A'..'Z' | "_" | "-" | ":" |
+'0'..'9' } /// tag left chevron_left_normal = { "<" } chevron_left_closed = { "
  } chevron_left_bang = { "
- } chevron_left_question = { "<?" } chevron_right_normal = { ">" }
-chevron_right_closed = { "/>" } chevron_right_question = { "?>" } chevron_right
-= _{ chevron_right_normal | chevron_right_closed | chevron_right_question }
-equal = { "=" } quote_dubble = { "\"" } quote_single = { "'" } quote = _
-{ quote_dubble | quote_single }
+ } chevron_left_question = { "<?" } /// tag right chevron_right_normal = { ">"
+} chevron_right_closed = { "/>" } chevron_right_question = { "?>" }
+chevron_right = _{ chevron_right_normal | chevron_right_closed |
+chevron_right_question } /// other equal = @{ "=" } quote = @{ "\"" | "'" }
```

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/java.pest` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/java.pest`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-item = _{ SOI ~ line* ~ EOI } 
-line = _{ regexp | string | other }
-
-other = ${ !(string) ~ ANY }
-
-WHITESPACE = { " " | "\t" | NEWLINE }
+//! Java Parser
+item       = _{ SOI ~ line* ~ EOI }
+line       = _{ regexp | string | other }
+other      = ${ !(string) ~ ANY }
+WHITESPACE =  { " " | "\t" | NEWLINE }
 
+/// Comment
 line_comment  = _{ "//" ~ (!(NEWLINE) ~ ANY)* }
-block_comment = _{ "/*" ~ (!("*/") ~ ANY)* ~ "*/"}
+block_comment = _{ "/*" ~ (!("*/") ~ ANY)* ~ "*/" }
 COMMENT       = ${ line_comment | block_comment }
 
-string = ${ inner_string }
-inner_string = _{ 
-  ("\"\"\"" ~ (!("\"\"\"") ~ ANY)* ~ "\"\"\"") 
-  | ("\"" ~ (!(NEWLINE | "\"") ~ ANY)* ~ "\"") 
+/// String
+string       = ${ inner_string }
+inner_string = _{
+    ("\"\"\"" ~ (!("\"\"\"") ~ ANY)* ~ "\"\"\"")
+  | ("\"" ~ (!(NEWLINE | "\"") ~ ANY)* ~ "\"")
 }
 
+/// Regexp
 regexp = ${
-  ("Pattern." ~ (ASCII_ALPHA)+  ~ "(" ~ " "* ~ inner_string ~ (!")" ~ ANY)* ~ ")" )
+    ("Pattern." ~ (ASCII_ALPHA)+ ~ "(" ~ " "* ~ inner_string ~ (!")" ~ ANY)* ~ ")")
 }
```

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/javascript.pest` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/javascript.pest`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,49 @@
-item = _{ SOI ~ line* ~ EOI } 
-line = _{ expr | html }
-
-html = _{  html_node | html_void | text }
-expr = _{ pair | string | regexp | other }
-
-other = ${ !(string | open_html) ~ ANY }
-
-WHITESPACE = { " " | "\t" | NEWLINE }
+//! JavaScript Parser
+//!
+//! Support JavaScript and TypeScript.
+item       = _{ SOI ~ line* ~ EOI }
+line       = _{ expr | html }
+other      = ${ !(string | open_html) ~ ANY }
+WHITESPACE =  { " " | "\t" | NEWLINE }
 
+/// Comment
+COMMENT       = ${ line_comment | block_comment }
 line_comment  = _{ "//" ~ (!(NEWLINE) ~ ANY)* }
 block_comment = _{ "/*" ~ (!("*/") ~ ANY)* ~ "*/" }
-COMMENT       = ${ line_comment | block_comment }
 
+/// HTML tags
+html = _{ html_node | html_void | text }
+expr = _{ pair | string | regexp | other }
+
+/// other text
 text = ${ (!("<") ~ ANY)+ }
 
-html_void  = @{ "<" ~ (!("/>" | ">") ~ ANY)* ~ (">" | "/>") }
-html_node  = ${ open_html ~ (!(close_html) ~ (html_node | text))+  ~ close_html }
-inner_html = @{ (!(">") ~ ANY)* }
-open_html  = @{ "<" ~ PUSH(inner_html) ~ chevron_right }
-close_html = @{ "</" ~ PUSH(inner_html) ~ ">"}
+/// HTML void
+html_void = @{ "<" ~ (!("/>" | ">") ~ ANY)* ~ (">" | "/>") }
 
+/// HTML node
+html_node     = ${ open_html ~ (!(close_html) ~ (html_node | text))+ ~ close_html }
+inner_html    = @{ (!(">") ~ ANY)* }
+open_html     = @{ "<" ~ inner_html ~ chevron_right }
+close_html    = @{ "</" ~ inner_html ~ ">" }
 chevron_right = @{
-  ">"
+    ">"
   | "/>"
   | "?>"
 }
 
-string = ${ inner_string }
+/// String
+string       = ${ inner_string }
 inner_string = _{
-    ("'" ~ (!("'") ~ ANY)* ~ "'") 
-  | ("\"" ~ (!(NEWLINE | "\"") ~ ANY)* ~ "\"") 
-  | ("`" ~ (!("`") ~ ANY)* ~ "`"+) 
+    ("'" ~ (!("'") ~ ANY)* ~ "'")
+  | ("\"" ~ (!(NEWLINE | "\"") ~ ANY)* ~ "\"")
+  | ("`" ~ (!("`") ~ ANY)* ~ "`"+)
 }
-key = ${ inner_string ~ (" ")* ~ ":" ~ (" ")* }
-pair = _{ key ~ string }
+key          = ${ inner_string ~ (" ")* ~ ":" ~ (" ")* }
+pair         = _{ key ~ string }
 
+/// Regexp
 regexp = ${
-  ( "/" ~ (!(NEWLINE | "/") ~ ANY)* ~ "/" )
+    ("/" ~ (!(NEWLINE | "/") ~ ANY)* ~ "/")
   | ("RegExp" ~ "(" ~ " "* ~ inner_string ~ (!")" ~ ANY)* ~ ")")
 }
-
```

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/json.pest` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/json.pest`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,44 @@
-item = _{ SOI ~ line* ~ EOI } 
-line = _{ object | array | other }
+//! JSON Parser
+item       = _{ SOI ~ line* ~ EOI }
+line       = _{ object | array | other }
+other      = ${ !(pair) ~ ANY }
+WHITESPACE =  { " " | "\t" | NEWLINE }
+
+// Comment
+COMMENT      =  { line_comment | block_comment }
+line_comment = @{ "//" ~ (!(NEWLINE) ~ ANY)* }
 
-other = ${ !(pair) ~ ANY }
-
-WHITESPACE = { " " | "\t" | NEWLINE }
-
-line_comment  = @{ "//" ~ (!(NEWLINE) ~ ANY)* }
-block_comment = @{ "/*" ~ (!("*/") ~ ANY)* ~ "*/"}
-COMMENT       = { line_comment | block_comment }
+block_comment = @{ "/*" ~ (!("*/") ~ ANY)* ~ "*/" }
 
+/// Value
 value        = _{ string | number | object | array | bool | null }
 string       = @{ inner_string }
 inner_string = @{ "\"" ~ inner ~ "\"" }
 
+/// Number
 number = @{ "-"? ~ int ~ ("." ~ ASCII_DIGIT+ ~ exp? | exp)? }
 int    = @{ "0" | ASCII_NONZERO_DIGIT ~ ASCII_DIGIT* }
 exp    = @{ ("E" | "e") ~ ("+" | "-")? ~ ASCII_DIGIT+ }
 bool   = @{ "true" | "false" }
 null   = @{ "null" }
 
-object       = { open_object ~ pair ~ (comma ~ pair?)* ~ close_object | open_object ~ close_object }
+/// Object
+object       =  { open_object ~ pair ~ (comma ~ pair?)* ~ close_object | open_object ~ close_object }
 open_object  = @{ "{" }
 close_object = @{ "}" }
 
-array       = { open_array ~ value ~ (comma ~ value?)* ~ close_array | open_array ~ close_array }
+/// Array
+array       =  { open_array ~ value ~ (comma ~ value?)* ~ close_array | open_array ~ close_array }
 open_array  = @{ "[" }
 close_array = @{ "]" }
 
-comma = @{ "," }
-
-pair    = { key ~ value }
-key     = { inner_string ~ colon }
-colon   = @{ ":" }
+/// Pair
+pair  =  { key ~ value }
+key   =  { inner_string ~ colon }
+colon = @{ ":" }
 
+/// Misc
+comma   = @{ "," }
 inner   = @{ (!("\"" | "\\") ~ ANY)* ~ (escape ~ inner)? }
 escape  = @{ "\\" ~ ("\"" | "\\" | "/" | "b" | "f" | "n" | "r" | "t" | unicode) }
 unicode = @{ "u" ~ ASCII_HEX_DIGIT{4} }
```

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/jupyter.pest` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/jupyter.pest`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-// The Jupyter Notebook Format
-// https://nbformat.readthedocs.io/en/latest/
-item = _{ SOI ~ line* ~ EOI } 
-line = _{ object | array | other }
-
-other = _{ ANY }
-
+//! The Jupyter Notebook Format
+//! https://nbformat.readthedocs.io/en/latest/
+item       = _{ SOI ~ line* ~ EOI }
+line       = _{ object | array | other }
+other      = _{ ANY }
 WHITESPACE = _{ " " | "\t" | NEWLINE }
 
-
-value        = _{ quote ~ string ~ quote | number | object | array | bool | null }
-string       = { inner }
+/// value
+value  = _{ quote ~ string ~ quote | number | object | array | bool | null }
+string =  { inner }
 number = @{ "-"? ~ int ~ ("." ~ ASCII_DIGIT+ ~ exp? | exp)? }
 int    = @{ "0" | ASCII_NONZERO_DIGIT ~ ASCII_DIGIT* }
 exp    = @{ ("E" | "e") ~ ("+" | "-")? ~ ASCII_DIGIT+ }
-bool = { "true" | "false" }
-null = { "null" }
+bool   =  { "true" | "false" }
+null   =  { "null" }
 
-object = { open_object ~ pair ~ (comma ~ pair?)* ~ close_object | open_object ~ close_object }
-open_object = _{ "{" }
+/// Object
+object       =  { open_object ~ pair ~ (comma ~ pair?)* ~ close_object | open_object ~ close_object }
+open_object  = _{ "{" }
 close_object = _{ "}" }
 
-array = { open_array ~ value ~ (comma ~ value?)* ~ close_array | open_array ~ close_array }
-open_array = _{ "[" }
+/// Array
+array       =  { open_array ~ value ~ (comma ~ value?)* ~ close_array | open_array ~ close_array }
+open_array  = _{ "[" }
 close_array = _{ "]" }
 
-comma = _{ "," }
-
-pair    = _{ quote ~ key ~ quote ~ colon ~ value }
-key     = @{ string }
-quote   = _{ "\"" }
-colon   = _{ ":" }
+/// Pair
+pair  = _{ quote ~ key ~ quote ~ colon ~ value }
+key   = @{ string }
+quote = _{ "\"" }
+colon = _{ ":" }
 
+/// Misc
 inner   = _{ (!(quote | "\\") ~ ANY)* ~ (escape ~ inner)? }
 escape  = _{ "\\" ~ (quote | "\\" | "/" | "b" | "f" | "n" | "r" | "t" | unicode) }
-unicode = _{ "u" ~ ASCII_HEX_DIGIT{4} }
+unicode = _{ "u" ~ ASCII_HEX_DIGIT{4} }
+comma   = _{ "," }
```

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/kotlin.pest` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/kotlin.pest`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-item = _{ SOI ~ line* ~ EOI } 
-line = _{ regexp | string | other }
+//! Kotlin Parser
+item       = _{ SOI ~ line* ~ EOI }
+line       = _{ regexp | string | other }
+other      = ${ !(string) ~ ANY }
+WHITESPACE =  { " " | "\t" | NEWLINE }
 
-other = ${ !(string) ~ ANY }
-
-WHITESPACE = { " " | "\t" | NEWLINE }
-
-line_comment  = _{ "//" ~ (!(NEWLINE) ~ ANY)* }
-block_comment = _{ "/*" ~ (!("*/") ~ ANY)* ~ "*/"}
+/// Comment
 COMMENT       = ${ line_comment | block_comment }
+line_comment  = _{ "//" ~ (!(NEWLINE) ~ ANY)* }
+block_comment = _{ "/*" ~ (!("*/") ~ ANY)* ~ "*/" }
 
-string = ${ inner_string }
-inner_string = _{ 
-  ("\"\"\"" ~ (!("\"\"\"") ~ ANY)* ~ "\"\"\"") 
-  | ("\"" ~ (!(NEWLINE | "\"") ~ ANY)* ~ "\"") 
+/// String
+string       = ${ inner_string }
+inner_string = _{
+    ("\"\"\"" ~ (!("\"\"\"") ~ ANY)* ~ "\"\"\"")
+  | ("\"" ~ (!(NEWLINE | "\"") ~ ANY)* ~ "\"")
 }
 
+/// Regexp
 regexp = ${
-  ("Regex(" ~ " "* ~ inner_string ~ (!")" ~ ANY)* ~ ")")
+    ("Regex(" ~ " "* ~ inner_string ~ (!")" ~ ANY)* ~ ")")
   | (inner_string ~ ".toRegex()")
 }
```

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/markdown.pest` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/markdown.pest`

 * *Files 8% similar despite different names*

```diff
@@ -1,145 +1,126 @@
 //! Markdown grammar for supports CommonMark and GFM.
 item = _{ SOI ~ line* ~ EOI }
 line = _{ expr | newline }
-
-expr = _{ 
-  comment | html | meta_info | block | inline | td_tag
+expr = _{
+    comment
+  | html
+  | meta_info
+  | block
+  | inline
+  | td_tag
 }
 
 /// Matches a CJK character
-CJK = { 
-  HAN
-  | HANGUL 
-  | KATAKANA | HIRAGANA
+CJK = {
+    HAN
+  | HANGUL
+  | KATAKANA
+  | HIRAGANA
   | BOPOMOFO
 }
 
 /// Block elements, e.g.: paragraphs, lists, code blocks, etc.
-block = ${ 
-  meta_tags
+block = ${
+    meta_tags
   | hr
   | list
   | codeblock
   | block_item
-  | paragraph  
+  | paragraph
 }
+
 /// Inline elements, e.g.: links, images, bold, italic, code, etc.
-inline = ${ wikilinks | img | link | code | mark }
-paragraph = { (inline | text)+ }
-text   = @{ string ~ (newline ~ string)* } 
+inline    = ${ wikilinks | img | link | code | mark }
+paragraph =  { (inline | text)+ }
+text      = @{ string ~ (newline ~ string)* }
 
 /// Matches HTML tags (In some Markdown implementations, HTML tags are allowed)
-html = { tag_self | tag_start ~ ws* ~ inner_html* ~ ws* ~ tag_end }
+html       =  { tag_self | tag_start ~ ws* ~ inner_html* ~ ws* ~ tag_end }
 inner_html = _{ html | inner_text }
-inner_text = { (!("<" | ">") ~ ANY)+ } 
-tag_start = @{ "<" ~ ws* ~ (!("/" | ">") ~ ANY)* ~ ws* ~ ">" }
-tag_end = @{ "</" ~ ws* ~ (!">" ~ ANY)* ~ ws* ~ ">" }
-tag_self = @{ "<" ~ ws* ~ (!(">" | "/>") ~ ANY)* ~ ws* ~ "/>" }
-
-hr = @{ "--" ~ "-"+ }
-
+inner_text =  { (!("<" | ">") ~ ANY)+ }
+tag_start  = @{ "<" ~ ws* ~ (!("/" | ">") ~ ANY)* ~ ws* ~ ">" }
+tag_end    = @{ "</" ~ ws* ~ (!">" ~ ANY)* ~ ws* ~ ">" }
+tag_self   = @{ "<" ~ ws* ~ (!(">" | "/>") ~ ANY)* ~ ws* ~ "/>" }
+hr         = @{ "--" ~ "-"+ }
 identifier = @{ ("_" | "-" | "." | ASCII_ALPHANUMERIC) }
-
-newline = @{ "\n" | "\r\n" }
-space = @{ " " }
+newline    = @{ "\n" | "\r\n" }
+space      = @{ " " }
 blank_line = @{ space* ~ newline }
-ws = @{ space | newline }
+ws         = @{ space | newline }
 
 /// 4 spaces or a tab
-indent = @{ " "{4,} | "\t" }
-
+indent    = @{ " "{4, } | "\t" }
 codeblock = ${
-  PUSH("```") ~ codeblock_lang ~ codeblock_code ~ POP
+    PUSH("```") ~ codeblock_lang ~ codeblock_code ~ POP
   | indent_code+
 }
+
 /// Codeblock that used 4 spaces or a tab as indent
-indent_code = @{
-  indent ~ (!"\n" ~ ANY)* ~ newline
+indent_code    = @{
+    indent ~ (!"\n" ~ ANY)* ~ newline
 }
-codeblock_lang = { identifier* }
-codeblock_code = { (!(PEEK) ~ ANY)* }
+codeblock_lang =  { identifier* }
+codeblock_code =  { (!(PEEK) ~ ANY)* }
 
 /// Matches table cell
-td_tag = @{ space* ~ "|" ~ space* }
-
-block_prefix = @{
-   ("######" | "#####" | "####" | "###" | "##" | "#" | ">")
-}
-block_item = { (block_prefix ~ space* ~ (inline | string)+)  }
-
-list = { list_item ~ (list_item | list_paragraph)*  }
-list_item = ${ list_prefix ~ (inline | string)+ ~ newline+ }
-list_paragraph = { indent ~ (inline | string)* ~ newline+ }
-list_prefix = @{
-  /*
-    - Foo
-    * Foo
-    1. Foo
-    [ ] Foo
-    [x] Foo
-  */
-  (
-    space* ~ 
-    (
-      "*" 
-      | "-" 
-      | ASCII_DIGIT ~ "." 
-      | "[" ~ (" " | "x" | "X") ~ "]"
-    ) ~ " "*
-  )
+td_tag         = @{ space* ~ "|" ~ space* }
+block_prefix   = @{
+    ("######" | "#####" | "####" | "###" | "##" | "#" | ">")
+}
+block_item     =  { (block_prefix ~ space* ~ (inline | string)+) }
+list           =  { list_item ~ (list_item | list_paragraph)* }
+list_item      = ${ list_prefix ~ (inline | string)+ ~ newline+ }
+list_paragraph =  { indent ~ (inline | string)* ~ newline+ }
+list_prefix    = @{
+    (space* ~ ("*" | "-" | ASCII_DIGIT ~ "." | "[" ~ (" " | "x" | "X") ~ "]") ~ " "*)
 }
 
 /// Matches meta info for some special Markdown implementations, e.g.: YAML front matter
 /// For example:
 ///
 /// ------------------
 /// title: Hello World
 /// author: Jason Lee
 /// tags: Rust, JavaScript
 /// ------------------
 meta_info = ${ meta_wrap ~ newline ~ meta_pair* ~ meta_wrap ~ newline* }
-meta_wrap = @{ "-"{3,} }
+meta_wrap = @{ "-"{3, } }
 meta_pair = ${ meta_key ~ string ~ newline }
-meta_key = @{ (!(":" | newline) ~ identifier)* ~ ":" ~ " "* }
+meta_key  = @{ (!(":" | newline) ~ identifier)* ~ ":" ~ " "* }
 
 /// Ignore tags in Markdown, e.g.: "tags: 美国, 中国"
-meta_tags = @{ meta_key ~ meta_tags_val+ ~ meta_tags_item ~ newline }
-meta_tags_val = @{ meta_tags_item ~ meta_tags_divider }
-meta_tags_item = { (!(newline | ",")  ~ (CJK | " " | ASCII_ALPHANUMERIC))* }
-meta_tags_divider = { " "* ~ "," ~ " "* }
-
-image_prefix = @{ "!" }
-img = ${ image_prefix ~ link }
+meta_tags         = @{ meta_key ~ meta_tags_val+ ~ meta_tags_item ~ newline }
+meta_tags_val     = @{ meta_tags_item ~ meta_tags_divider }
+meta_tags_item    =  { (!(newline | ",") ~ (CJK | " " | ASCII_ALPHANUMERIC))* }
+meta_tags_divider =  { " "* ~ "," ~ " "* }
+image_prefix      = @{ "!" }
+img               = ${ image_prefix ~ link }
 
 /// Matches link, e.g.: `[Hello](/hello)` or `[Hello]`
-link = ${ link_string_wrap ~ href? }
-link_string_wrap = { open_bracket ~ (mark* ~ link_string ~ mark*) ~ close_bracket }
-link_string = @{ (!(close_bracket) ~ ANY)* }
-open_bracket = @{ "[" }
-close_bracket = @{ "]" }
-href = @{ paren }
-
-wikilinks = ${"[[" ~ (!("]]") ~ ANY)* ~ "]]" }
-
-mark = ${ code | PUSH(open_mark) ~ (mark | mark_string) ~ close_mark }
-open_mark = @{ "***" | "**" | "*" | "~~" | "\"" }
-close_mark = @{ POP }
-mark_string = { (!(PEEK | inline) ~ ANY)* }
-
-code = ${ PUSH(open_code) ~ inner_code ~ close_code }
-open_code = @{ "`" }
-close_code = @{ POP }
-inner_code = @{ (!(newline | PEEK) ~ ANY)*  }
-
-string = @{ (!(newline | inline) ~ ANY)+ }
+link             = ${ link_string_wrap ~ href? }
+link_string_wrap =  { open_bracket ~ (mark* ~ link_string ~ mark*) ~ close_bracket }
+link_string      = @{ (!(close_bracket) ~ ANY)* }
+open_bracket     = @{ "[" }
+close_bracket    = @{ "]" }
+href             = @{ paren }
+wikilinks        = ${ "[[" ~ (!("]]") ~ ANY)* ~ "]]" }
+mark             = ${ code | PUSH(open_mark) ~ (mark | mark_string) ~ close_mark }
+open_mark        = @{ "***" | "**" | "*" | "~~" | "\"" }
+close_mark       = @{ POP }
+mark_string      =  { (!(PEEK | inline) ~ ANY)* }
+code             = ${ PUSH(open_code) ~ inner_code ~ close_code }
+open_code        = @{ "`" }
+close_code       = @{ POP }
+inner_code       = @{ (!(newline | PEEK) ~ ANY)* }
+string           = @{ (!(newline | inline) ~ ANY)+ }
 
 /// HTML comment, e.g.: <!-- This is a comment -->
-comment = ${ open_comment ~ (!close_comment ~ ANY)* ~ close_comment }
-open_comment  = @{  "<!--" }
+comment       = ${ open_comment ~ (!close_comment ~ ANY)* ~ close_comment }
+open_comment  = @{ "<!--" }
 close_comment = @{ "-->" }
 
 /// Matches link href part, e.g.: `(hello (world))`
-paren = { open_paren ~ inner_paren ~ paren* ~ inner_paren* ~ close_paren | open_paren ~ close_paren }
+paren       = { open_paren ~ inner_paren ~ paren* ~ inner_paren* ~ close_paren | open_paren ~ close_paren }
 inner_paren = { (!(newline | open_paren | close_paren) ~ ANY)+ }
 open_paren  = { "(" }
 close_paren = { ")" }
```

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/objective_c.pest` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/objective_c.pest`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-item = _{ SOI ~ line* ~ EOI } 
-line = _{ ignore_string | string | other }
+//! Objective-C Parser
+item       = _{ SOI ~ line* ~ EOI }
+line       = _{ ignore_string | string | other }
+other      = ${ !(string) ~ ANY }
+WHITESPACE =  { " " | "\t" | NEWLINE }
 
-other = ${ !(string) ~ ANY }
-
-WHITESPACE = { " " | "\t" | NEWLINE }
-
-line_comment = _{ "//" ~ (!NEWLINE ~ ANY)* }
+/// Comment
 COMMENT      = ${ line_comment }
+line_comment = _{ "//" ~ (!NEWLINE ~ ANY)* }
 
+/// String
 string       = ${ inner_string }
 inner_string = _{
-  "@\"" ~ (!(NEWLINE | "\"") ~ ANY)* ~ "\""
+    "@\"" ~ (!(NEWLINE | "\"") ~ ANY)* ~ "\""
 }
 
-ignore_string = ${
-  ingore_methods ~ "(" ~ WHITE_SPACE* ~ inner_string
+/// String to ingore
+ignore_string    = ${
+    ingore_methods ~ "(" ~ WHITE_SPACE* ~ inner_string
   | ignore_arguments ~ WHITE_SPACE* ~ inner_string
 }
 ingore_methods   = _{ "NSRegularExpression" | "NSLocalizedString" | "Match" }
-ignore_arguments = _{ ("WithPattern" | "WithKey") ~ ":"  }
+ignore_arguments = _{ ("WithPattern" | "WithKey") ~ ":" }
```

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/php.pest` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/php.pest`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,30 @@
-item = _{ SOI ~ line* ~ EOI } 
-line = _{ php | other }
-
-other = ${ !(php) ~ ANY }
+//! PHP Parser
+item       = _{ SOI ~ line* ~ EOI }
+line       = _{ php | other }
+other      = ${ !(php) ~ ANY }
+WHITESPACE =  { " " | "\t" | NEWLINE }
+
+/// Comment
+COMMENT       = ${ line_comment | block_comment }
+line_comment  = _{ ("//" | "#") ~ (!(NEWLINE) ~ ANY)* }
+block_comment = _{ "/*" ~ (!("*/") ~ ANY)* ~ "*/" }
 
+/// PHP entry
 php       = _{ open_php ~ (!close_php ~ expr)* ~ close_php }
 open_php  = ${ "<?php" }
 close_php = ${ "?>" }
 
+/// Expressions
 expr = { regexp | string | other }
 
-WHITESPACE = { " " | "\t" | NEWLINE }
-
-line_comment  = _{ ("//" | "#") ~ (!(NEWLINE) ~ ANY)*  }
-block_comment = _{ "/*" ~ (!("*/") ~ ANY)* ~ "*/" }
-COMMENT = ${ line_comment | block_comment }
-
-string = ${ inner_string }
+/// String
+string       = ${ inner_string }
 inner_string = _{
-  ("\"\"\"" ~ (!("\"\"\"") ~ ANY)* ~ "\"\"\"") 
-  | ("\"" ~ (!("\"") ~ ANY)* ~ "\"") 
+    ("\"\"\"" ~ (!("\"\"\"") ~ ANY)* ~ "\"\"\"")
+  | ("\"" ~ (!("\"") ~ ANY)* ~ "\"")
 }
 
+/// Regexp
 regexp = ${
-  (("preg_match_all" | "preg_match") ~ "(" ~ " "* ~ inner_string ~ (!")" ~ ANY)* ~ ")")
-}
-
+    (("preg_match_all" | "preg_match") ~ "(" ~ " "* ~ inner_string ~ (!")" ~ ANY)* ~ ")")
+}
```

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/ruby.pest` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/csharp.pest`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-item = _{ SOI ~ line* ~ EOI } 
-line = _{ string | regexp | other }
-other = ${ !(string) ~ ANY }
+//! C# Parser
+item       = _{ SOI ~ line* ~ EOI }
+line       = _{ regexp | string | other }
+other      = ${ !(string) ~ ANY }
+WHITESPACE =  { " " | "\t" | NEWLINE }
 
-WHITESPACE = { " " | "\t" | NEWLINE }
+/// Comment
+line_comment  = _{ "//" ~ (!(NEWLINE) ~ ANY)* }
+block_comment = _{ "/*" ~ (!("*/") ~ ANY)* ~ "*/" }
+COMMENT       = ${ line_comment | block_comment }
 
-line_comment = _{ "#" ~ (!(NEWLINE) ~ ANY)* }
-block_comment = _{ "/*" ~ (!("*/") ~ ANY)* ~ "*/"}
-COMMENT = ${ line_comment | block_comment }
-
-string = ${ 
-  PUSH("'") ~ inner_string ~ POP |
-  PUSH("\"") ~ inner_string ~ POP 
+/// String
+string       = ${ inner_string }
+inner_string = _{
+    ("@\"" ~ (!("\"") ~ ANY)* ~ "\"")
+  | ("\"" ~ (!(NEWLINE | "\"") ~ ANY)* ~ "\"")
+  | ("$\"" ~ (!(NEWLINE | "\"") ~ ANY)* ~ "\"")
 }
-inner_string = { (!(NEWLINE | PEEK) ~ ANY)* }
 
-regexp = ${
-  PUSH("/") ~ (!(NEWLINE | "/") ~ ANY)* ~ POP
-  | ( "%r{" ~ (!(NEWLINE | "}") ~ ANY)* ~ "}" )
-  | ("Regexp.new(" ~ " "* ~ (!")" ~ ANY)* ~ ")")
-}
+/// Regex
+regexp = ${ "Regex(" ~ " "* ~ inner_string ~ (!")" ~ ANY)* ~ ")" }
```

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/scala.pest` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/rust.pest`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-item = _{ SOI ~ line* ~ EOI } 
-line = _{ regexp | string_literal | string | other }
-
-other = ${ !(string) ~ ANY }
-
-WHITESPACE = { " " | "\t" | NEWLINE }
-
-line_comment = _{ "//" ~ (!(NEWLINE) ~ ANY)* }
-block_comment = _{ "/*" ~ (!("*/") ~ ANY)* ~ "*/"}
-COMMENT = ${ line_comment | block_comment }
-
-string = ${ inner_string }
-inner_string = _{ 
-  ("\"\"\"" ~ (!("\"\"\"") ~ ANY)* ~ "\"\"\"") 
-  | ("\"" ~ (!(NEWLINE | "\"") ~ ANY)* ~ "\"") 
+//! Rust Parser
+item       = _{ SOI ~ line* ~ EOI }
+line       = _{ regexp | string | other }
+other      = ${ !(string) ~ ANY }
+WHITESPACE =  { " " | "\t" | NEWLINE }
+
+/// Comment
+COMMENT       =  { line_comment | block_comment }
+line_comment  = _{ "//" ~ ("!" | "/")* ~ (!(NEWLINE) ~ ANY)* }
+block_comment = _{ "/*" ~ (!("*/") ~ ANY)* ~ "*/" }
+
+/// String
+string       = ${
+    PUSH("\"") ~ inner_string ~ POP
+  | "r" ~ PUSH("#"*) ~ "\"" ~ inner_string ~ "\"" ~ POP
 }
+inner_string = @{ (!(PEEK) ~ ANY)* }
 
-string_literal = ${ "s" ~ inner_string }
-
+/// Regexp
 regexp = ${
-  ("Regex(" ~ " "* ~ inner_string ~ (!")" ~ ANY)* ~ ")" )
-  | (inner_string ~ ".r" )
-}
-
+    ("r\"" ~ (!(NEWLINE | "\"") ~ ANY)* ~ "\"")
+}
```

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/swift.pest` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/swift.pest`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-item = _{ SOI ~ line* ~ EOI } 
-line = _{ ignore_string | string | other }
+//! Swift Parser
+item       = _{ SOI ~ line* ~ EOI }
+line       = _{ ignore_string | string | other }
+other      = ${ !(string) ~ ANY }
+WHITESPACE =  { " " | "\t" | NEWLINE }
 
-other = ${ !(string) ~ ANY }
-
-WHITESPACE = { " " | "\t" | NEWLINE }
-
-line_comment  = _{ "//" ~ (!NEWLINE ~ ANY)* }
-block_comment = _{ "/*" ~ (!"*/" ~ ANY)* ~ "*/"}
+/// Comment
 COMMENT       = ${ line_comment | block_comment }
+line_comment  = _{ "//" ~ (!NEWLINE ~ ANY)* }
+block_comment = _{ "/*" ~ (!"*/" ~ ANY)* ~ "*/" }
 
+/// String
 string       = ${ inner_string }
-inner_string = _{ 
-  "\"\"\"" ~ (!("\"\"\"") ~ ANY)* ~ "\"\"\""
+inner_string = _{
+    "\"\"\"" ~ (!("\"\"\"") ~ ANY)* ~ "\"\"\""
   | "\"" ~ (!(NEWLINE | "\"") ~ ANY)* ~ "\""
 }
 
-BLANK = _{ NEWLINE | WHITE_SPACE }
-
-ingore_methods = _{ "NSRegularExpression" | "NSLocalizedString" | "Match" }
-ignore_arguments = _{ ("pattern" | "key") ~ ":"  }
-
-ignore_string = ${
-  ignore_arguments ~ BLANK* ~ inner_string
+/// Ingores
+ingore_methods   = _{ "NSRegularExpression" | "NSLocalizedString" | "Match" }
+ignore_arguments = _{ ("pattern" | "key") ~ ":" }
+ignore_string    = ${
+    ignore_arguments ~ BLANK* ~ inner_string
   | ingore_methods ~ "(" ~ BLANK* ~ inner_string
 }
+
+/// Misc
+BLANK = _{ NEWLINE | WHITE_SPACE }
```

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/grammar/yaml.pest` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/grammar/yaml.pest`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-item = _{ (pair | comment | newline | other)+ }
+//! YAML Parser
+item  = _{ (pair | comment | newline | other)+ }
+other = ${ !(pair) ~ ANY }
 
-indent = ${ (^" "+)? }
+/// Comment
+comment = ${ "#" ~ (!(NEWLINE) ~ ANY)* }
+indent  = ${ (^" "+)? }
 newline = ${ "\n" | "\r" }
 
-other = ${ !(pair) ~ ANY }
-
-string_key = _{ "\"" ~ key_str* ~ "\""  }
-simple_key = _{ key_str* }
-key_str = _{ !(newline | ":" | "\"" | "'") ~ ANY }
+/// Pair
+pair = _{ key_part ~ string }
+key  = ${ (string_key | simple_key) ~ (":" ~ " "?) }
 
+/// String
+string       = ${ string_value | simple_value }
+string_key   = _{ "\"" ~ key_str* ~ "\"" }
+simple_key   = _{ key_str* }
+key_str      = _{ !(newline | ":" | "\"" | "'") ~ ANY }
 simple_value = _{ value_str* }
 string_value = _{ ("\"" ~ (!(newline | "\"") ~ ANY)* ~ "\"") | ("'" ~ (!(newline | "'") ~ ANY)* ~ "'") }
-value_str = _{ !(newline | "\"" | "'") ~ ANY }
-key_part = _{ indent ~ key }
-
-comment = ${ "#" ~ (!(NEWLINE) ~ ANY)* }
-
-pair = _{ key_part ~ string }
-key = ${ (string_key | simple_key) ~ (":" ~ " "?) }
-string = ${ string_value | simple_value }
+value_str    = _{ !(newline | "\"" | "'") ~ ANY }
+key_part     = _{ indent ~ key }
```

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/asciidoc.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/asciidoc.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/c.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/c.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/code.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/code.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/conf.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/conf.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/csharp.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/csharp.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/css.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/css.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/dart.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/dart.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/elixir.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/elixir.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/gettext.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/gettext.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/go.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/go.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/html.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/html.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/java.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/java.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/javascript.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/javascript.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/json.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/json.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/jupyter.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/jupyter.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/kotlin.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/kotlin.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/latex.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/latex.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/markdown.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/markdown.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/mod.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/mod.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/objective_c.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/objective_c.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/php.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/php.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/python.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/python.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/ruby.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/ruby.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/rust.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/rust.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/scala.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/scala.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/sql.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/sql.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/strings.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/strings.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/swift.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/swift.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/types.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/types.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/xml.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/xml.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/code/yaml.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/code/yaml.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/config/mod.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/config/mod.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/config/severity.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/config/severity.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/config/spellcheck.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/config/spellcheck.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/config/toggle.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/config/toggle.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/diff.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/diff.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/format.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/format.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/ignorer.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/ignorer.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/lib.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 
 pub mod config;
 pub mod ignorer;
 
 pub use code::{format_for, get_file_extension, is_support_type, lint_for};
 pub use config::Config;
 pub use format::*;
-pub use result::{FormatResult, LineResult, LintResult};
+pub use result::{json, rdjson, FormatResult, LineResult, LintResult};
 pub use rule::{halfwidth, spellcheck};
 
 #[cfg(test)]
 mod tests {
     use super::*;
 
     #[test]
```

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/result.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/result/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+pub mod json;
+pub mod rdjson;
 use serde::{Deserialize, Serialize};
 use serde_repr::*;
 
 use crate::config::toggle;
 
 #[derive(Serialize_repr, Deserialize_repr, PartialEq, Eq, Debug, Clone, Copy)]
 #[repr(u8)]
```

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/rule/fullwidth.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/rule/fullwidth.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/rule/halfwidth.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/rule/halfwidth.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/rule/mod.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/rule/mod.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/rule/rule.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/rule/rule.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/rule/spellcheck.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/rule/spellcheck.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/rule/strategery.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/rule/strategery.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/rule/word.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/rule/word.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/serde_any/de.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/serde_any/de.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/src/serde_any/error.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/src/serde_any/error.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/tests/fixtures/jupyter.expected.json` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/tests/fixtures/jupyter.expected.json`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/tests/fixtures/jupyter.expected.txt` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/tests/fixtures/jupyter.expected.txt`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/tests/fixtures/jupyter.ipynb` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/tests/fixtures/jupyter.ipynb`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/tests/fixtures/jupyter.sm.ipynb` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/tests/fixtures/jupyter.sm.ipynb`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/local_dependencies/autocorrect/tests/format.rs` & `autocorrect_py-2.8.0/local_dependencies/autocorrect/tests/format.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/Cargo.toml` & `autocorrect_py-2.8.0/Cargo.toml`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 description = "A linter and formatter for help you improve copywriting, to correct spaces, words, punctuations between CJK (Chinese, Japanese, Korean)."
 edition = "2018"
 homepage = "https://github.com/huacnlee/autocorrect"
 license = "MIT"
 name = "autocorrect-py"
 readme = "README.md"
 repository = "https://github.com/huacnlee/autocorrect"
-version = "2.6.2"
+version = "2.8.0"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 crate-type = ["cdylib"]
 name = "autocorrect_py"
 
 [dependencies]
```

### Comparing `autocorrect_py-2.6.2/.gitignore` & `autocorrect_py-2.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/README.md` & `autocorrect_py-2.8.0/README.md`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/autocorrect_py.pyi` & `autocorrect_py-2.8.0/autocorrect_py.pyi`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/src/lib.rs` & `autocorrect_py-2.8.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/test_autocorrect_py.py` & `autocorrect_py-2.8.0/test_autocorrect_py.py`

 * *Files identical despite different names*

### Comparing `autocorrect_py-2.6.2/PKG-INFO` & `autocorrect_py-2.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autocorrect-py
-Version: 2.6.2
+Version: 2.8.0
 Summary: A linter and formatter for help you improve copywriting, to correct spaces, words, punctuations between CJK (Chinese, Japanese, Korean).
 Home-Page: https://github.com/huacnlee/autocorrect
 License: MIT
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/huacnlee/autocorrect
 
 # AutoCorrect for Python
```

