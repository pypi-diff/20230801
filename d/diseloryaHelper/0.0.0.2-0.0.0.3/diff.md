# Comparing `tmp/diseloryahelper-0.0.0.2.tar.gz` & `tmp/diseloryahelper-0.0.0.3.tar.gz`

## Comparing `diseloryahelper-0.0.0.2.tar` & `diseloryahelper-0.0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rwxr-xr-x   0        0        0      379 2020-02-02 00:00:00.000000 diseloryahelper-0.0.0.2/GetRequires.bat
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 diseloryahelper-0.0.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 diseloryahelper-0.0.0.2/src/diseloryaHelper/__init__.py
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 diseloryahelper-0.0.0.2/src/diseloryaHelper/chineseLanguageHelper.py
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 diseloryahelper-0.0.0.2/src/diseloryaHelper/ocrHelper.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 diseloryahelper-0.0.0.2/src/diseloryaHelper/pathHelper.py
--rw-r--r--   0        0        0    10594 2020-02-02 00:00:00.000000 diseloryahelper-0.0.0.2/src/diseloryaHelper/pdfHelper.py
--rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 diseloryahelper-0.0.0.2/src/diseloryaHelper/stringHelper.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 diseloryahelper-0.0.0.2/src/diseloryaHelper/terminalHelper.py
--rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 diseloryahelper-0.0.0.2/.gitignore
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 diseloryahelper-0.0.0.2/LICENSE
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 diseloryahelper-0.0.0.2/README.md
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 diseloryahelper-0.0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 diseloryahelper-0.0.0.2/PKG-INFO
+-rwxr-xr-x   0        0        0      379 2020-02-02 00:00:00.000000 diseloryahelper-0.0.0.3/GetRequires.bat
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 diseloryahelper-0.0.0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 diseloryahelper-0.0.0.3/src/diseloryaHelper/__init__.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 diseloryahelper-0.0.0.3/src/diseloryaHelper/chineseLanguageHelper.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 diseloryahelper-0.0.0.3/src/diseloryaHelper/ocrHelper.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 diseloryahelper-0.0.0.3/src/diseloryaHelper/pathHelper.py
+-rw-r--r--   0        0        0    10617 2020-02-02 00:00:00.000000 diseloryahelper-0.0.0.3/src/diseloryaHelper/pdfHelper.py
+-rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 diseloryahelper-0.0.0.3/src/diseloryaHelper/stringHelper.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 diseloryahelper-0.0.0.3/src/diseloryaHelper/terminalHelper.py
+-rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 diseloryahelper-0.0.0.3/.gitignore
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 diseloryahelper-0.0.0.3/LICENSE
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 diseloryahelper-0.0.0.3/README.md
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 diseloryahelper-0.0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 diseloryahelper-0.0.0.3/PKG-INFO
```

### Comparing `diseloryahelper-0.0.0.2/.github/workflows/python-publish.yml` & `diseloryahelper-0.0.0.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `diseloryahelper-0.0.0.2/src/diseloryaHelper/chineseLanguageHelper.py` & `diseloryahelper-0.0.0.3/src/diseloryaHelper/chineseLanguageHelper.py`

 * *Files identical despite different names*

### Comparing `diseloryahelper-0.0.0.2/src/diseloryaHelper/ocrHelper.py` & `diseloryahelper-0.0.0.3/src/diseloryaHelper/ocrHelper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from PIL import Image
 import cv2
 import numpy
 import pytesseract
-import chineseLanguageHelper as ch
-import pathHelper as ph
-import terminalHelper as th
-import stringHelper as sh
+from . import chineseLanguageHelper as ch
+from . import pathHelper as ph
+from . import terminalHelper as th
+from . import stringHelper as sh
 
 def get_text_from_image_with_save(image_data: bytes, save_path_name: str):
     # 图片输出为文件
     with open(save_path_name, 'wb') as image_file:
         image_file.write(image_data)
 
     # 将 JPG 格式图片转换为 PIL 格式图片，Tesseract 只支持 PIL（Python Imaging Library）的Image对象 或 OpenCV
```

### Comparing `diseloryahelper-0.0.0.2/src/diseloryaHelper/pathHelper.py` & `diseloryahelper-0.0.0.3/src/diseloryaHelper/pathHelper.py`

 * *Files identical despite different names*

### Comparing `diseloryahelper-0.0.0.2/src/diseloryaHelper/pdfHelper.py` & `diseloryahelper-0.0.0.3/src/diseloryaHelper/pdfHelper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import PyPDF2
 import re
 import pangu
-import stringHelper as sh
-import pdfHelper as ph
-import chineseLanguageHelper as ch
+from . import stringHelper as sh
+from . import chineseLanguageHelper as ch
+from . import ocrHelper as ocr
 
 
 def get_pdf_save_picture_path(pdf_file_name: str, page_num: int, image_count: int, output_path: str = '', picture_extname: str = 'jpg', folder_suffix: str = '.images'):
     # 图片保存在子文件夹中
     images_folder = os.path.join(output_path, pdf_file_name + folder_suffix)
     if not os.path.isdir(images_folder):
         os.makedirs(images_folder)
@@ -147,15 +147,15 @@
         extracted_text += page.extract_text().strip() + '\n'
         images_texts = []
 
         if including_picture:
             image_count = 0
             for image in page.images:
                 image_count += 1
-                text = ph.get_text_from_image_with_save(image.data, get_pdf_save_picture_path(filename_prefix, page_count, image_count, output_path))
+                text = ocr.get_text_from_image_with_save(image.data, get_pdf_save_picture_path(filename_prefix, page_count, image_count, output_path))
                 images_texts.append(text)
                 # print(f'Image-P{page_count}-{image_count}：\n{text}')
                 extracted_text += text
 
         images_text_of_each_pages.append(images_texts)
     
     count = len(extracted_text.strip())
```

### Comparing `diseloryahelper-0.0.0.2/src/diseloryaHelper/stringHelper.py` & `diseloryahelper-0.0.0.3/src/diseloryaHelper/stringHelper.py`

 * *Files identical despite different names*

### Comparing `diseloryahelper-0.0.0.2/.gitignore` & `diseloryahelper-0.0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `diseloryahelper-0.0.0.2/LICENSE` & `diseloryahelper-0.0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `diseloryahelper-0.0.0.2/pyproject.toml` & `diseloryahelper-0.0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "diseloryaHelper"
-version = "0.0.0.2"
+version = "0.0.0.3"
 description = "Lc's python helper."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 authors = [
   {name = "Diselorya"},
 ]
```

### Comparing `diseloryahelper-0.0.0.2/PKG-INFO` & `diseloryahelper-0.0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diseloryaHelper
-Version: 0.0.0.2
+Version: 0.0.0.3
 Summary: Lc's python helper.
 Project-URL: Homepage, https://github.com/Diselorya/LCsPythonHelper/
 Author: Diselorya
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

