# Comparing `tmp/ezkl-1.2.0-cp37-abi3-win_amd64.whl.zip` & `tmp/ezkl-1.7.17-cp37-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 9963371 bytes, number of entries: 6
--rw-r--r--  4.6 unx     5716 b- defN 23-Jul-12 17:50 ezkl-1.2.0.dist-info/METADATA
--rw-r--r--  4.6 unx       96 b- defN 23-Jul-12 17:50 ezkl-1.2.0.dist-info/WHEEL
--rw-r--r--  4.6 unx    11558 b- defN 23-Jul-12 17:50 ezkl-1.2.0.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx       99 b- defN 23-Jul-12 17:50 ezkl/__init__.py
--rwxr-xr-x  4.6 unx 28567040 b- defN 23-Jul-12 17:50 ezkl/ezkl.pyd
--rw-r--r--  4.6 unx      442 b- defN 23-Jul-12 17:50 ezkl-1.2.0.dist-info/RECORD
-6 files, 28584951 bytes uncompressed, 9962587 bytes compressed:  65.1%
+Zip file size: 10115962 bytes, number of entries: 6
+-rw-r--r--  4.6 unx     5930 b- defN 23-Aug-01 13:49 ezkl-1.7.17.dist-info/METADATA
+-rw-r--r--  4.6 unx       96 b- defN 23-Aug-01 13:49 ezkl-1.7.17.dist-info/WHEEL
+-rw-r--r--  4.6 unx    11558 b- defN 23-Aug-01 13:49 ezkl-1.7.17.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx       99 b- defN 23-Aug-01 13:49 ezkl/__init__.py
+-rwxr-xr-x  4.6 unx 29475328 b- defN 23-Aug-01 13:49 ezkl/ezkl.pyd
+-rw-r--r--  4.6 unx      446 b- defN 23-Aug-01 13:49 ezkl-1.7.17.dist-info/RECORD
+6 files, 29493457 bytes uncompressed, 10115170 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: ezkl-1.2.0.dist-info/METADATA
+Filename: ezkl-1.7.17.dist-info/METADATA
 Comment: 
 
-Filename: ezkl-1.2.0.dist-info/WHEEL
+Filename: ezkl-1.7.17.dist-info/WHEEL
 Comment: 
 
-Filename: ezkl-1.2.0.dist-info/license_files/LICENSE
+Filename: ezkl-1.7.17.dist-info/license_files/LICENSE
 Comment: 
 
 Filename: ezkl/__init__.py
 Comment: 
 
 Filename: ezkl/ezkl.pyd
 Comment: 
 
-Filename: ezkl-1.2.0.dist-info/RECORD
+Filename: ezkl-1.7.17.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ezkl-1.2.0.dist-info/METADATA` & `ezkl-1.7.17.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezkl
-Version: 1.2.0
+Version: 1.7.17
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
@@ -44,28 +44,31 @@
 
 
 ### resources 📖
 
 |  |  |
 | --- | --- |
 | [docs](https://docs.ezkl.xyz ) | the official ezkl docs page |
-| [colab notebook demo](https://colab.research.google.com/drive/1XuXNKqH7axOelZXyU3gpoTOCvFetIsKu?usp=sharing) | demo of ezkl python bindings on google's colab
 | `cargo doc --open` | compile and open the docs in your default browser locally |
+| [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/zkonduit/ezkl/blob/master/examples/notebooks/simple_demo.ipynb)| a simple demo of the python bindings in action on Colab |
+
+
+
 
 #### tutorials 
 
 You can find a range of python based tutorials in the `examples/notebooks` section. These all assume you have the `ezkl` python library installed. If you want the bleeding edge version of the library, you can install it from the `main` branch with:
 
 ```bash
 python -m venv .env
 source .env/bin/activate
 pip install -r requirements.txt
 maturin develop --release --features python-bindings
 # dependencies specific to tutorials
-pip install torch pandas numpy seaborn jupyter onnx kaggle py-solc-x web3 librosa
+pip install torch pandas numpy seaborn jupyter onnx kaggle py-solc-x web3 librosa tensorflow keras tf2onnx
 ```
 
 
 ----------------------
 
 ## Getting Started ⚙️
 
@@ -74,15 +77,16 @@
 https://user-images.githubusercontent.com/45801863/236771676-5bbbbfd1-ba6f-418a-902e-20738ce0e9f0.mp4
 
 
 ### building the project 🔨
 Note that the library requires a nightly version of the rust toolchain. You can change the default toolchain by running:
 
 ```bash
-rustup override set nightly
+# we set it to this version because of https://github.com/rust-lang/rust/issues/110829
+rustup override set nightly-2023-04-17
 ```
 
 After which you may build the library
 
 ```bash
 cargo build --release
 ```
```

## Comparing `ezkl-1.2.0.dist-info/license_files/LICENSE` & `ezkl-1.7.17.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

