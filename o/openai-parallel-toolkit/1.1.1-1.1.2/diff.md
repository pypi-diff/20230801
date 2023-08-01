# Comparing `tmp/openai_parallel_toolkit-1.1.1-py3-none-any.whl.zip` & `tmp/openai_parallel_toolkit-1.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 12918 bytes, number of entries: 15
+Zip file size: 12933 bytes, number of entries: 15
 -rw-r--r--  2.0 unx       77 b- defN 23-Jul-28 11:58 openai_parallel_toolkit/__init__.py
 -rw-r--r--  2.0 unx     3100 b- defN 23-Jul-31 02:05 openai_parallel_toolkit/main.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Aug-01 07:30 openai_parallel_toolkit/api/__init__.py
 -rw-r--r--  2.0 unx     3809 b- defN 23-Jul-29 05:11 openai_parallel_toolkit/api/keys.py
 -rw-r--r--  2.0 unx     1348 b- defN 23-Jul-27 06:52 openai_parallel_toolkit/api/model.py
--rw-r--r--  2.0 unx     4504 b- defN 23-Jul-29 02:34 openai_parallel_toolkit/api/request.py
+-rw-r--r--  2.0 unx     4522 b- defN 23-Aug-01 07:44 openai_parallel_toolkit/api/request.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Aug-01 07:33 openai_parallel_toolkit/utils/__init__.py
 -rw-r--r--  2.0 unx     1488 b- defN 23-Jul-28 13:01 openai_parallel_toolkit/utils/logger.py
 -rw-r--r--  2.0 unx      424 b- defN 23-Jul-28 13:01 openai_parallel_toolkit/utils/process_bar.py
--rw-r--r--  2.0 unx     3036 b- defN 23-Aug-01 07:32 openai_parallel_toolkit/utils/reader.py
--rw-r--r--  2.0 unx     1063 b- defN 23-Aug-01 07:33 openai_parallel_toolkit-1.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     8218 b- defN 23-Aug-01 07:33 openai_parallel_toolkit-1.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-01 07:33 openai_parallel_toolkit-1.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       24 b- defN 23-Aug-01 07:33 openai_parallel_toolkit-1.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1404 b- defN 23-Aug-01 07:33 openai_parallel_toolkit-1.1.1.dist-info/RECORD
-15 files, 28587 bytes uncompressed, 10524 bytes compressed:  63.2%
+-rw-r--r--  2.0 unx     3108 b- defN 23-Aug-01 07:44 openai_parallel_toolkit/utils/reader.py
+-rw-r--r--  2.0 unx     1063 b- defN 23-Aug-01 07:45 openai_parallel_toolkit-1.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8218 b- defN 23-Aug-01 07:45 openai_parallel_toolkit-1.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-01 07:45 openai_parallel_toolkit-1.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       24 b- defN 23-Aug-01 07:45 openai_parallel_toolkit-1.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1404 b- defN 23-Aug-01 07:45 openai_parallel_toolkit-1.1.2.dist-info/RECORD
+15 files, 28677 bytes uncompressed, 10539 bytes compressed:  63.2%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: openai_parallel_toolkit/utils/process_bar.py
 Comment: 
 
 Filename: openai_parallel_toolkit/utils/reader.py
 Comment: 
 
-Filename: openai_parallel_toolkit-1.1.1.dist-info/LICENSE
+Filename: openai_parallel_toolkit-1.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: openai_parallel_toolkit-1.1.1.dist-info/METADATA
+Filename: openai_parallel_toolkit-1.1.2.dist-info/METADATA
 Comment: 
 
-Filename: openai_parallel_toolkit-1.1.1.dist-info/WHEEL
+Filename: openai_parallel_toolkit-1.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: openai_parallel_toolkit-1.1.1.dist-info/top_level.txt
+Filename: openai_parallel_toolkit-1.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: openai_parallel_toolkit-1.1.1.dist-info/RECORD
+Filename: openai_parallel_toolkit-1.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## openai_parallel_toolkit/api/request.py

```diff
@@ -68,15 +68,15 @@
                                  process_bar: ProgressBar, lock: Lock, max_retries: int, output_path: str = None):
     key, prompt = item
     result = request_openai_api(openai_model=openai_model, prompt=prompt, key_manager=key_manager,
                                 max_retries=max_retries)
 
     if output_path:
         with lock:
-            with open(output_path, 'a') as file:
+            with open(output_path, 'a', encoding='utf-8') as file:
                 file.write(json.dumps({key: result}, ensure_ascii=False) + '\n')
                 file.flush()
     process_bar.update()
     return result
 
 
 def parallel_request_openai(data: Dict[int, Prompt], openai_model: OpenAIModel,
```

## openai_parallel_toolkit/utils/reader.py

```diff
@@ -13,29 +13,29 @@
         if "api_base" in config:
             api_base = config['api_base']
     return api_keys, api_base
 
 
 def read_jsonl_to_dict(jsonl_file: str) -> Dict[int, Prompt]:
     new_dict = {}
-    with open(jsonl_file, 'r') as f:
+    with open(jsonl_file, 'r', encoding='utf-8') as f:
         for line in f:
             obj = json.loads(line)
             index = obj['index']
             new_dict[index] = Prompt(instruction=obj['instruction'], input=obj['input'])
     return new_dict
 
 
 def filter(data: dict, path) -> dict:
     data_copy = data.copy()
 
     if not os.path.exists(path):
         return data_copy
 
-    with open(path, 'r') as f:
+    with open(path, 'r', encoding='utf-8') as f:
         for line in f:
             item = json.loads(line)
             key = list(item.keys())[0]
             if key in data_copy:
                 del data_copy[key]
 
     return data_copy
@@ -46,27 +46,27 @@
 
     with open(path, 'r') as f:
         for line in f:
             item = json.loads(line)
             data.append((int(list(item.keys())[0]), list(item.values())[0]))
     data.sort(key=lambda x: x[0])
 
-    with open(path, 'w') as f:
+    with open(path, 'w', encoding='utf-8') as f:
         for key, value in data:
             json.dump({key: value}, f, ensure_ascii=False)
             f.write('\n')
 
 
 def remove_nulls_from_jsonl(file_path):
     if not os.path.exists(file_path):
         return
     non_null_data = []
 
     # Read non-null data into a list.
-    with open(file_path, 'r') as f:
+    with open(file_path, 'r', encoding='utf-8') as f:
         for line in f:
             data = json.loads(line)
             if any(value is None for value in data.values()):
                 continue
             non_null_data.append(data)
 
     # Write the non-null data back to the file.
```

## Comparing `openai_parallel_toolkit-1.1.1.dist-info/LICENSE` & `openai_parallel_toolkit-1.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `openai_parallel_toolkit-1.1.1.dist-info/METADATA` & `openai_parallel_toolkit-1.1.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-parallel-toolkit
-Version: 1.1.1
+Version: 1.1.2
 Summary: OpenAI-Parallel-Toolkit is a Python library for handling multiple OpenAI API keys and parallel tasks. It provides API key rotation, multithreading for faster task execution, and utility functions to boost your OpenAI integration. Ideal for efficient large-scale OpenAI usage.
 Home-page: https://github.com/CZT0/OpenAI-Parallel-Toolkit
 Author: Jellow
 Author-email: dvdx@foxmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

## Comparing `openai_parallel_toolkit-1.1.1.dist-info/RECORD` & `openai_parallel_toolkit-1.1.2.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 openai_parallel_toolkit/__init__.py,sha256=ZZxiwZF7ASUBX-pVvy-lD2UMguKiuTxJpKlesjkiXYs,77
 openai_parallel_toolkit/main.py,sha256=tulufpdSmKdkMSw-N-RS_aYg9Dt7jxF0ZvsqPXOc1Kc,3100
 openai_parallel_toolkit/api/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 openai_parallel_toolkit/api/keys.py,sha256=7KNffVMz5g3-D2JSYSiiAiIw2iKxEq5hsY1P-7Q7hNc,3809
 openai_parallel_toolkit/api/model.py,sha256=54LMbmK096CFI3ZvY7lreQVSqp5SZndY7THkeinSFaU,1348
-openai_parallel_toolkit/api/request.py,sha256=laVtfdmxPgPQM1XL5S2XC2k9XYoWiit2pzfjw6Lt2yQ,4504
+openai_parallel_toolkit/api/request.py,sha256=eFK5N6noxCNfQn3w34Q1mkf5spzUZUiDaYqWSf5a24I,4522
 openai_parallel_toolkit/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 openai_parallel_toolkit/utils/logger.py,sha256=fjjSDWHa2P3wqcI2EilAEi8H8GtcVzY2sn29kkvXKdk,1488
 openai_parallel_toolkit/utils/process_bar.py,sha256=CAlHeTneAEPiDxo3eEVjI4a9XburGTZZ5tywd2D9mdI,424
-openai_parallel_toolkit/utils/reader.py,sha256=e8lFvhgHf6_z9Fvf7d67mE98dKwuOPdMSZfAo80DcGA,3036
-openai_parallel_toolkit-1.1.1.dist-info/LICENSE,sha256=GcBhJWMnrpUPC70Dvfs6cFG8fLIitA0WwucEgQjGWcw,1063
-openai_parallel_toolkit-1.1.1.dist-info/METADATA,sha256=dWzucdFjaJBUdvHAMcQNaTXM3LlOPKCJTw85WOB54eY,8218
-openai_parallel_toolkit-1.1.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-openai_parallel_toolkit-1.1.1.dist-info/top_level.txt,sha256=EaHQWFuNRtse4G2kzDTEMstiiaGFy0zIAHBJ0Mm9a_E,24
-openai_parallel_toolkit-1.1.1.dist-info/RECORD,,
+openai_parallel_toolkit/utils/reader.py,sha256=KeVKuqvX_fiapxjoQaHgw6LhZDJZQSSjLmCmhbSFtr4,3108
+openai_parallel_toolkit-1.1.2.dist-info/LICENSE,sha256=GcBhJWMnrpUPC70Dvfs6cFG8fLIitA0WwucEgQjGWcw,1063
+openai_parallel_toolkit-1.1.2.dist-info/METADATA,sha256=jprL8c_vjniGbYwAdtXT5woOui1fcbWMgGZxtnCSHGY,8218
+openai_parallel_toolkit-1.1.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+openai_parallel_toolkit-1.1.2.dist-info/top_level.txt,sha256=EaHQWFuNRtse4G2kzDTEMstiiaGFy0zIAHBJ0Mm9a_E,24
+openai_parallel_toolkit-1.1.2.dist-info/RECORD,,
```

