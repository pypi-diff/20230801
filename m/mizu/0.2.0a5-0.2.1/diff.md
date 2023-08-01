# Comparing `tmp/mizu-0.2.0a5.tar.gz` & `tmp/mizu-0.2.1.tar.gz`

## Comparing `mizu-0.2.0a5.tar` & `mizu-0.2.1.tar`

### file list

```diff
@@ -1,26 +1,29 @@
--rw-r--r--   0        0        0      345 1970-01-01 00:00:00.000000 mizu-0.2.0a5/Cargo.toml
--rw-r--r--   0     1001      123     1698 2022-12-19 08:34:24.000000 mizu-0.2.0a5/.github/workflows/CI.yml
--rw-r--r--   0     1001      123     1094 2022-12-19 08:34:24.000000 mizu-0.2.0a5/.github/workflows/docs.yml
--rw-r--r--   0     1001      123     1387 2022-12-19 08:34:24.000000 mizu-0.2.0a5/.github/workflows/python-app.yml
--rw-r--r--   0     1001      123      685 2022-12-19 08:34:24.000000 mizu-0.2.0a5/.gitignore
--rw-r--r--   0     1001      123     1065 2022-12-19 08:34:24.000000 mizu-0.2.0a5/LICENSE
--rw-r--r--   0     1001      123      965 2022-12-19 08:34:24.000000 mizu-0.2.0a5/README.md
--rw-r--r--   0     1001      123      638 2022-12-19 08:34:24.000000 mizu-0.2.0a5/docs/Makefile
--rw-r--r--   0     1001      123      804 2022-12-19 08:34:24.000000 mizu-0.2.0a5/docs/make.bat
--rw-r--r--   0     1001      123       12 2022-12-19 08:34:24.000000 mizu-0.2.0a5/docs/requirements.txt
--rw-r--r--   0     1001      123     1016 2022-12-19 08:34:24.000000 mizu-0.2.0a5/docs/source/conf.py
--rw-r--r--   0     1001      123      447 2022-12-19 08:34:24.000000 mizu-0.2.0a5/docs/source/index.rst
--rw-r--r--   0     1001      123      157 2022-12-19 08:34:24.000000 mizu-0.2.0a5/docs/source/mizu.rst
--rw-r--r--   0     1001      123       49 2022-12-19 08:34:24.000000 mizu-0.2.0a5/docs/source/modules.rst
--rw-r--r--   0     1001      123      491 2022-12-19 08:34:24.000000 mizu-0.2.0a5/mizu/__init__.py
--rw-r--r--   0     1001      123      263 2022-12-19 08:34:24.000000 mizu-0.2.0a5/mizu/mizu.pyi
--rw-r--r--   0     1001      123     1340 2022-12-19 08:34:24.000000 mizu-0.2.0a5/mizu/options.py
--rw-r--r--   0     1001      123      429 2022-12-19 08:34:24.000000 mizu-0.2.0a5/pyproject.toml
--rwxr-xr-x   0     1001      123      767 2022-12-19 08:35:02.000000 mizu-0.2.0a5/run-maturin-action.sh
--rw-r--r--   0     1001      123      415 2022-12-19 08:34:24.000000 mizu-0.2.0a5/src/asyncio.rs
--rw-r--r--   0     1001      123     2639 2022-12-19 08:34:24.000000 mizu-0.2.0a5/src/core.rs
--rw-r--r--   0     1001      123      174 2022-12-19 08:34:24.000000 mizu-0.2.0a5/src/lib.rs
--rw-r--r--   0     1001      123      206 2022-12-19 08:34:24.000000 mizu-0.2.0a5/tests/test_async.py
--rw-r--r--   0     1001      123      120 2022-12-19 08:34:24.000000 mizu-0.2.0a5/tests/test_md.py
--rw-r--r--   0     1001      123     8742 2022-12-19 08:34:24.000000 mizu-0.2.0a5/Cargo.lock
--rw-r--r--   0        0        0     1457 1970-01-01 00:00:00.000000 mizu-0.2.0a5/PKG-INFO
+-rw-r--r--   0        0        0      338 1970-01-01 00:00:00.000000 mizu-0.2.1/Cargo.toml
+-rw-r--r--   0     1001      123     1158 2023-08-01 05:29:30.000000 mizu-0.2.1/.devcontainer/devcontainer.json
+-rw-r--r--   0     1001      123     1698 2023-08-01 05:29:30.000000 mizu-0.2.1/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123     1094 2023-08-01 05:29:30.000000 mizu-0.2.1/.github/workflows/docs.yml
+-rw-r--r--   0     1001      123     1387 2023-08-01 05:29:30.000000 mizu-0.2.1/.github/workflows/python-app.yml
+-rw-r--r--   0     1001      123      693 2023-08-01 05:29:30.000000 mizu-0.2.1/.gitignore
+-rw-r--r--   0     1001      123      771 2023-08-01 05:29:30.000000 mizu-0.2.1/Dockerfile
+-rw-r--r--   0     1001      123     1065 2023-08-01 05:29:30.000000 mizu-0.2.1/LICENSE
+-rw-r--r--   0     1001      123      917 2023-08-01 05:29:30.000000 mizu-0.2.1/README.md
+-rw-r--r--   0     1001      123      367 2023-08-01 05:29:30.000000 mizu-0.2.1/docs/build.py
+-rw-r--r--   0     1001      123      291 2023-08-01 05:29:30.000000 mizu-0.2.1/docs/index.html
+-rw-r--r--   0     1001      123     1407 2023-08-01 05:29:30.000000 mizu-0.2.1/docs/main.md
+-rw-r--r--   0     1001      123      291 2023-08-01 05:29:30.000000 mizu-0.2.1/docs/main.tpl
+-rw-r--r--   0     1001      123       12 2023-08-01 05:29:30.000000 mizu-0.2.1/docs/requirements.txt
+-rw-r--r--   0     1001      123     1016 2023-08-01 05:29:30.000000 mizu-0.2.1/docs/source/conf.py
+-rw-r--r--   0     1001      123      157 2023-08-01 05:29:30.000000 mizu-0.2.1/docs/source/mizu.rst
+-rw-r--r--   0     1001      123      175 2023-08-01 05:29:30.000000 mizu-0.2.1/mizu/__init__.py
+-rw-r--r--   0     1001      123      371 2023-08-01 05:29:30.000000 mizu-0.2.1/mizu/mizu.pyi
+-rw-r--r--   0     1001      123     1340 2023-08-01 05:29:30.000000 mizu-0.2.1/mizu/options.py
+-rw-r--r--   0     1001      123      948 2023-08-01 05:29:30.000000 mizu-0.2.1/mizu/parse.py
+-rw-r--r--   0     1001      123      429 2023-08-01 05:29:30.000000 mizu-0.2.1/pyproject.toml
+-rw-r--r--   0     1001      123      107 2023-08-01 05:29:30.000000 mizu-0.2.1/renovate.json
+-rw-r--r--   0     1001      123      415 2023-08-01 05:29:30.000000 mizu-0.2.1/src/asyncio.rs
+-rw-r--r--   0     1001      123     2833 2023-08-01 05:29:30.000000 mizu-0.2.1/src/core.rs
+-rw-r--r--   0     1001      123      174 2023-08-01 05:29:30.000000 mizu-0.2.1/src/lib.rs
+-rw-r--r--   0     1001      123      205 2023-08-01 05:29:30.000000 mizu-0.2.1/tests/test_async.py
+-rw-r--r--   0     1001      123      120 2023-08-01 05:29:30.000000 mizu-0.2.1/tests/test_md.py
+-rw-r--r--   0        0        0     8745 2023-08-01 05:30:30.000000 mizu-0.2.1/Cargo.lock
+-rw-r--r--   0        0        0     1407 1970-01-01 00:00:00.000000 mizu-0.2.1/PKG-INFO
```

### Comparing `mizu-0.2.0a5/.github/workflows/CI.yml` & `mizu-0.2.1/.github/workflows/CI.yml`

 * *Files 2% similar despite different names*

```diff
@@ -16,54 +16,54 @@
     - uses: actions/checkout@v3
     - uses: messense/maturin-action@v1
       with:
         manylinux: auto
         command: build
         args: --release --sdist -o dist --find-interpreter
     - name: Upload wheels
-      uses: actions/upload-artifact@v2
+      uses: actions/upload-artifact@v3
       with:
         name: wheels
         path: dist
 
   windows:
     runs-on: windows-latest
     steps:
     - uses: actions/checkout@v3
     - uses: messense/maturin-action@v1
       with:
         command: build
         args: --release -o dist --find-interpreter
     - name: Upload wheels
-      uses: actions/upload-artifact@v2
+      uses: actions/upload-artifact@v3
       with:
         name: wheels
         path: dist
 
   macos:
     runs-on: macos-latest
     steps:
     - uses: actions/checkout@v3
     - uses: messense/maturin-action@v1
       with:
         command: build
         args: --release -o dist --universal2 --find-interpreter
     - name: Upload wheels
-      uses: actions/upload-artifact@v2
+      uses: actions/upload-artifact@v3
       with:
         name: wheels
         path: dist
 
   release:
     name: Release
     runs-on: ubuntu-latest
     if: "startsWith(github.ref, 'refs/tags/')"
     needs: [ macos, windows, linux ]
     steps:
-      - uses: actions/download-artifact@v2
+      - uses: actions/download-artifact@v3
         with:
           name: wheels
       - name: Publish to PyPI
         uses: messense/maturin-action@v1
         env:
           MATURIN_PYPI_TOKEN: ${{ secrets.PYPI_API_TOKEN }}
         with:
```

### Comparing `mizu-0.2.0a5/.github/workflows/docs.yml` & `mizu-0.2.1/.github/workflows/docs.yml`

 * *Files 5% similar despite different names*

```diff
@@ -23,19 +23,19 @@
           pip install maturin
           maturin develop
           pip install -r docs/requirements.txt
       - name: Build document
         run: |
           source venv/bin/activate
           cd docs
-          make html
+          python3 -OO build.py
       - name: Upload artifact
-        uses: actions/upload-pages-artifact@v1
+        uses: actions/upload-pages-artifact@v2
         with:
-          path: ./docs/build/html
+          path: ./docs
   deploy:
     environment:
       name: github-pages
       url: ${{ steps.deployment.outputs.page_url }}
     permissions:
       pages: write
       id-token: write
```

### Comparing `mizu-0.2.0a5/.github/workflows/python-app.yml` & `mizu-0.2.1/.github/workflows/python-app.yml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
   build:
 
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python 3.10
-      uses: actions/setup-python@v3
+      uses: actions/setup-python@v4
       with:
         python-version: "3.10"
     - uses: actions/cache@v3
       with:
         path: |
           ~/.cargo/bin/
           ~/.cargo/registry/index/
```

### Comparing `mizu-0.2.0a5/.gitignore` & `mizu-0.2.1/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 /target
+Cargo.lock
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 .pytest_cache/
 *.py[cod]
 
 # C extensions
@@ -55,18 +56,18 @@
 
 # Django stuff:
 *.log
 *.pot
 
 .DS_Store
 
-# Sphinx documentation
-docs/_build/
+# Documentation
+docs/index.html
 
 # PyCharm
 .idea/
 
 # VSCode
 .vscode/
 
 # Pyenv
-.python-version
+.python-version
```

### Comparing `mizu-0.2.0a5/LICENSE` & `mizu-0.2.1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 tuna2134
+Copyright (c) 2023 tuna2134
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mizu-0.2.0a5/README.md` & `mizu-0.2.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # mizu 💧
 
-**Warning:** This library is now developing. Please use stable version.
-
 [![Version](https://img.shields.io/pypi/v/mizu)](https://pypi.org/project/mizu/)
 [![Downloads](https://pepy.tech/badge/mizu)](https://pepy.tech/project/mizu)
 [![Downloads](https://pepy.tech/badge/mizu/month)](https://pepy.tech/project/mizu)
 [![Downloads](https://pepy.tech/badge/mizu/week)](https://pepy.tech/project/mizu)
 
 [Documentation](https://tuna2134.github.io/mizu)
 
@@ -23,15 +21,16 @@
 pip install "mizu @ git+https://github.com/tuna2134/mizu"
 ```
 
 ## Performance
 
 These performance test codes are in tests.
 
-`26ms`
+- 3.10: `26ms`
+- 3.11: `0.32ms`
 
 ## Example
 
 Basic:
 
 ```py
 from mizu import Mizu
```

### Comparing `mizu-0.2.0a5/docs/source/conf.py` & `mizu-0.2.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mizu-0.2.0a5/mizu/options.py` & `mizu-0.2.1/mizu/options.py`

 * *Files identical despite different names*

### Comparing `mizu-0.2.0a5/src/core.rs` & `mizu-0.2.1/src/core.rs`

 * *Files 5% similar despite different names*

```diff
@@ -13,47 +13,54 @@
     options: Options,
     loop_: Option<PyObject>,
 }
 
 #[pymethods]
 impl Mizu {
     #[new]
-    #[args(options = "Options::empty()")]
+    #[pyo3(signature = (options = Options::empty()))]
     pub fn new(
         #[pyo3(from_py_with = "get_options")] options: Options,
-        loop_: Option<PyObject>,
     ) -> Self {
         Mizu {
-            options: options,
-            loop_: loop_,
+            options,
+            loop_: None,
         }
     }
 
+    fn set_loop(&mut self, loop_: PyObject) -> PyResult<()> {
+        self.loop_ = Some(loop_);
+        Ok(())
+    }
+
     /// Parse markdown text to html.
     ///
     /// Args:
     ///     text (str): Markdown text.
-    #[args(text)]
-    #[pyo3(text_signature = "(text, /)")]
+    #[pyo3(text_signature = "(text, /)", signature = (text))]
     fn parse(&self, text: &str) -> PyResult<String> {
         let parser: Parser = Parser::new_ext(text, self.options);
 
         let mut output: String = String::new();
         html::push_html(&mut output, parser);
         Ok(output)
     }
 
+    /// Parse markdown text to html (async version)
+    /// 
+    /// Args:
+    ///     text (str): Markdown text
     fn aioparse(&self, py: Python, text: String) -> PyResult<PyObject> {
         if self.loop_.is_none() {
             return Err(pyo3::exceptions::PyValueError::new_err(
                 "Event loop is not set",
             ));
         }
         let future = create_future(py, self.loop_.clone().unwrap())?;
-        let options = self.options.clone();
+        let options = self.options;
         let fut_clone = future.clone_ref(py);
         let loop_ = self.loop_.clone().unwrap();
         std::thread::spawn(move || {
             Python::with_gil(|py| {
                 let parser: Parser = Parser::new_ext(text.as_str(), options);
                 let mut output: String = String::new();
                 html::push_html(&mut output, parser);
```

### Comparing `mizu-0.2.0a5/Cargo.lock` & `mizu-0.2.1/Cargo.lock`

 * *Files 11% similar despite different names*

```diff
@@ -27,296 +27,296 @@
 checksum = "14dbbfd5c71d70241ecf9e6f13737f7b5ce823821063188d7e46c41d371eebd5"
 dependencies = [
  "unicode-width",
 ]
 
 [[package]]
 name = "indoc"
-version = "1.0.7"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "adab1eaa3408fb7f0c777a73e7465fd5656136fc93b670eb6df3c88c2c1344e3"
+checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "libc"
-version = "0.2.135"
+version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "68783febc7782c6c5cb401fbda4de5a9898be1762314da0bb2c10ced61f18b0c"
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
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
 [[package]]
 name = "memoffset"
-version = "0.6.5"
+version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5aa361d4faea93603064a027415f07bd8e1d5c88c9fbf68bf56a285428fd79ce"
+checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "mizu"
-version = "0.2.0-alpha5"
+version = "0.2.1"
 dependencies = [
  "pulldown-cmark",
  "pyo3",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.15.0"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e82dad04139b71a90c080c8463fe0dc7902db5192d939bd0950f074d014339e1"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.4"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4dc9e0dc2adc1c69d09143aff38d3d30c5c3f0df0dad82e6d25547af174ebec0"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys",
+ "windows-targets",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.47"
+version = "1.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ea3d908b0e36316caf9e9e2c4625cdde190a7e6f440d794667ed17a1855e725"
+checksum = "18fb31db3f9bddb2ea821cde30a9f70117e3f119938b5ee630b7403aa6e2ead9"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pulldown-cmark"
-version = "0.9.2"
+version = "0.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2d9cc634bc78768157b5cbfe988ffcd1dcba95cd2b2f03a88316c08c6d00ed63"
+checksum = "77a1a2f1f0a7ecff9c31abbe177637be0e97a0aef46cf8738ece09327985d998"
 dependencies = [
  "bitflags",
  "getopts",
  "memchr",
  "unicase",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.17.2"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "201b6887e5576bf2f945fe65172c1fcbf3fcf285b23e4d71eb171d9736e38d32"
+checksum = "ffb88ae05f306b4bfcde40ac4a51dc0b05936a9207a4b75b798c7729c4258a59"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.17.2"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf0708c9ed01692635cbf056e286008e5a2927ab1a5e48cdd3aeb1ba5a6fef47"
+checksum = "554db24f0b3c180a9c0b1268f91287ab3f17c162e15b54caaae5a6b3773396b0"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.17.2"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "90352dea4f486932b72ddf776264d293f85b79a1d214de1d023927b41461132d"
+checksum = "922ede8759e8600ad4da3195ae41259654b9c55da4f7eec84a0ccc7d067a70a4"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.17.2"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7eb24b804a2d9e88bfcc480a5a6dd76f006c1e3edaf064e8250423336e2cd79d"
+checksum = "8a5caec6a1dd355964a841fcbeeb1b89fe4146c87295573f94228911af3cc5a2"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.17.2"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f22bb49f6a7348c253d7ac67a6875f2dc65f36c2ae64a82c381d528972bea6d6"
+checksum = "e0b78ccbb160db1556cdb6fd96c50334c5d4ec44dc5e0a968d0a1208fa0efa8b"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.21"
+version = "1.0.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bbe448f377a7d6961e30f5955f9b8d106c3f5e449d493ee1b125c1d43c2b5179"
+checksum = "50f3b39ccfb720540debaa0164757101c08ecb8d326b15358ce76a62c7e85965"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.16"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
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
-version = "1.0.102"
+version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fcd952facd492f9be3ef0d0b7032a6e442ee9b361d4acc2b1d0c4aaa5f613a1"
+checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.4"
+version = "0.12.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c02424087780c9b71cc96799eaeddff35af2bc513278cda5c99fc1f5d026d3c1"
+checksum = "9d0e916b1148c8e263850e1ebcbd046f333e0683c724876bb0da63ea4373dc8a"
 
 [[package]]
 name = "unicase"
 version = "2.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "50f37be617794602aabbeee0be4f259dc1778fabe05e2d67ee8f79326d5cb4f6"
 dependencies = [
  "version_check",
 ]
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.5"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ceab39d59e4c9499d4e5a8ee0e2735b891bb7308ac83dfb4e80cad195c9f6f3"
+checksum = "301abaae475aa91687eb82514b328ab47a211a533026cb25fc3e519b86adfc3c"
 
 [[package]]
 name = "unicode-width"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c0edd1e5b14653f783770bce4a4dabb4a5108a5370a5f5d8cfe8710c361f6c8b"
 
 [[package]]
 name = "unindent"
-version = "0.1.10"
+version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "58ee9362deb4a96cef4d437d1ad49cffc9b9e92d202b6995674e928ce684f112"
+checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
-name = "windows-sys"
-version = "0.42.0"
+name = "windows-targets"
+version = "0.48.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
+checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "41d2aa71f6f0cbe00ae5167d90ef3cfe66527d6f613ca78ac8024c3ccab9a19e"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd0f252f5a35cac83d6311b2e795981f5ee6e67eb1f9a7f64eb4500fbc4dcdb4"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fbeae19f6716841636c28d695375df17562ca208b2b7d0dc47635a50ae6c5de7"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84c12f65daa39dd2babe6e442988fc329d6243fdce47d7d2d155b8d874862246"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf7b1b21b5362cbc318f686150e5bcea75ecedc74dd157d874d754a2ca44b0ed"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09d525d2ba30eeb3297665bd434a54297e4170c7f1a44cad4ef58095b4cd2028"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f40009d85759725a34da6d89a94e63d7bdc50a862acf0dbc7c8e488f1edcb6f5"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
```

### Comparing `mizu-0.2.0a5/PKG-INFO` & `mizu-0.2.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: mizu
-Version: 0.2.0a5
+Version: 0.2.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Markdown library
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Source Code, https://github.com/tuna2134/mizu
 Project-URL: Documentation, https://tuna2134.github.io/mizu
+Project-URL: Source Code, https://github.com/tuna2134/mizu
 
 # mizu 💧
 
-**Warning:** This library is now developing. Please use stable version.
-
 [![Version](https://img.shields.io/pypi/v/mizu)](https://pypi.org/project/mizu/)
 [![Downloads](https://pepy.tech/badge/mizu)](https://pepy.tech/project/mizu)
 [![Downloads](https://pepy.tech/badge/mizu/month)](https://pepy.tech/project/mizu)
 [![Downloads](https://pepy.tech/badge/mizu/week)](https://pepy.tech/project/mizu)
 
 [Documentation](https://tuna2134.github.io/mizu)
 
@@ -36,15 +34,16 @@
 pip install "mizu @ git+https://github.com/tuna2134/mizu"
 ```
 
 ## Performance
 
 These performance test codes are in tests.
 
-`26ms`
+- 3.10: `26ms`
+- 3.11: `0.32ms`
 
 ## Example
 
 Basic:
 
 ```py
 from mizu import Mizu
```

