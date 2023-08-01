# Comparing `tmp/pydatawork-0.17.5.9.tar.gz` & `tmp/pydatawork-0.17.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydatawork-0.17.5.9.tar", last modified: Sat Jul 29 16:12:22 2023, max compression
+gzip compressed data, was "dist/pydatawork-0.17.6.0.tar", last modified: Tue Aug  1 20:13:25 2023, max compression
```

## Comparing `pydatawork-0.17.5.9.tar` & `pydatawork-0.17.6.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-29 16:12:22.000000 pydatawork-0.17.5.9/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    22368 2023-07-29 16:12:22.000000 pydatawork-0.17.5.9/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    17049 2023-07-29 16:11:28.000000 pydatawork-0.17.5.9/README.md
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-29 16:12:22.000000 pydatawork-0.17.5.9/pydatawork.egg-info/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    22368 2023-07-29 16:12:22.000000 pydatawork-0.17.5.9/pydatawork.egg-info/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-07-29 16:12:22.000000 pydatawork-0.17.5.9/pydatawork.egg-info/SOURCES.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-07-29 16:12:22.000000 pydatawork-0.17.5.9/pydatawork.egg-info/dependency_links.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-07-29 16:12:22.000000 pydatawork-0.17.5.9/pydatawork.egg-info/top_level.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    53428 2023-07-24 01:35:40.000000 pydatawork-0.17.5.9/pydatawork.py
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-07-29 16:12:22.000000 pydatawork-0.17.5.9/setup.cfg
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      796 2023-07-29 16:12:04.000000 pydatawork-0.17.5.9/setup.py
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-08-01 20:13:25.000000 pydatawork-0.17.6.0/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    23103 2023-08-01 20:13:25.000000 pydatawork-0.17.6.0/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    17648 2023-08-01 20:11:33.000000 pydatawork-0.17.6.0/README.md
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-08-01 20:13:25.000000 pydatawork-0.17.6.0/pydatawork.egg-info/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    23103 2023-08-01 20:13:25.000000 pydatawork-0.17.6.0/pydatawork.egg-info/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-08-01 20:13:25.000000 pydatawork-0.17.6.0/pydatawork.egg-info/SOURCES.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-08-01 20:13:25.000000 pydatawork-0.17.6.0/pydatawork.egg-info/dependency_links.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-08-01 20:13:25.000000 pydatawork-0.17.6.0/pydatawork.egg-info/top_level.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    55728 2023-08-01 20:11:16.000000 pydatawork-0.17.6.0/pydatawork.py
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-08-01 20:13:25.000000 pydatawork-0.17.6.0/setup.cfg
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      796 2023-08-01 20:01:49.000000 pydatawork-0.17.6.0/setup.py
```

### Comparing `pydatawork-0.17.5.9/PKG-INFO` & `pydatawork-0.17.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.17.5.9
+Version: 0.17.6.0
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         pydatawork功能建议收集表：
@@ -357,14 +357,31 @@
             """
         ```
         
         
         
         # Data Processing
         
+        ## md_neatreader_note_timestamps() neatreader导出的md笔记整理：将每条笔记的时间戳放到内容之前 （v 0.17.6.0） 
+        
+        ###### Wed Aug 2 03:59:07 CST 2023
+        
+        ```python
+        def md_neatreader_note_timestamps(raw_path):
+            """
+            功能：针对neatreader导出的md笔记，将每条笔记的时间戳放到内容之前。
+        
+            参数：
+        
+            raw_path：文件路径。可以是存放md的文件夹路径，也可以是单个md文件路径。如果输入文件夹路径，将会处理文件夹中全部md文档（不遍历子文件夹）。建议使用单个文件路径。
+            """
+        ```
+        
+        
+        
         ## obsidian_bookmarks_merge_and_deduplicate() obsidian中surfing插件产生的书签整理：先合并，再去重 （v 0.1.31）
         
         ###### Mon Jun 26 22:50:45 CST 2023
         
         ```python
         def obsidian_bookmarks_merge_and_deduplicate(original_bookmarks_path,result_path):
             """
```

### Comparing `pydatawork-0.17.5.9/README.md` & `pydatawork-0.17.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -349,14 +349,31 @@
     """
 ```
 
 
 
 # Data Processing
 
+## md_neatreader_note_timestamps() neatreader导出的md笔记整理：将每条笔记的时间戳放到内容之前 （v 0.17.6.0） 
+
+###### Wed Aug 2 03:59:07 CST 2023
+
+```python
+def md_neatreader_note_timestamps(raw_path):
+    """
+    功能：针对neatreader导出的md笔记，将每条笔记的时间戳放到内容之前。
+
+    参数：
+
+    raw_path：文件路径。可以是存放md的文件夹路径，也可以是单个md文件路径。如果输入文件夹路径，将会处理文件夹中全部md文档（不遍历子文件夹）。建议使用单个文件路径。
+    """
+```
+
+
+
 ## obsidian_bookmarks_merge_and_deduplicate() obsidian中surfing插件产生的书签整理：先合并，再去重 （v 0.1.31）
 
 ###### Mon Jun 26 22:50:45 CST 2023
 
 ```python
 def obsidian_bookmarks_merge_and_deduplicate(original_bookmarks_path,result_path):
     """
```

### Comparing `pydatawork-0.17.5.9/pydatawork.egg-info/PKG-INFO` & `pydatawork-0.17.6.0/pydatawork.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.17.5.9
+Version: 0.17.6.0
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         pydatawork功能建议收集表：
@@ -357,14 +357,31 @@
             """
         ```
         
         
         
         # Data Processing
         
+        ## md_neatreader_note_timestamps() neatreader导出的md笔记整理：将每条笔记的时间戳放到内容之前 （v 0.17.6.0） 
+        
+        ###### Wed Aug 2 03:59:07 CST 2023
+        
+        ```python
+        def md_neatreader_note_timestamps(raw_path):
+            """
+            功能：针对neatreader导出的md笔记，将每条笔记的时间戳放到内容之前。
+        
+            参数：
+        
+            raw_path：文件路径。可以是存放md的文件夹路径，也可以是单个md文件路径。如果输入文件夹路径，将会处理文件夹中全部md文档（不遍历子文件夹）。建议使用单个文件路径。
+            """
+        ```
+        
+        
+        
         ## obsidian_bookmarks_merge_and_deduplicate() obsidian中surfing插件产生的书签整理：先合并，再去重 （v 0.1.31）
         
         ###### Mon Jun 26 22:50:45 CST 2023
         
         ```python
         def obsidian_bookmarks_merge_and_deduplicate(original_bookmarks_path,result_path):
             """
```

### Comparing `pydatawork-0.17.5.9/pydatawork.py` & `pydatawork-0.17.6.0/pydatawork.py`

 * *Files 4% similar despite different names*

```diff
@@ -802,14 +802,76 @@
 
 
 
 
 # Data Processing
 
 
+def md_neatreader_note_timestamps(raw_path):
+    """
+    功能：针对neatreader导出的md笔记，将每条笔记的时间戳放到内容之前。
+
+    参数：
+
+    raw_path：文件路径。可以是存放md的文件夹路径，也可以是单个md文件路径。如果输入文件夹路径，将会处理文件夹中全部md文档（不遍历子文件夹）。建议使用单个文件路径。
+    """
+
+    def swap_timestamps(md_text):
+        lines = md_text.split('\n')
+        timestamps = []
+        for i in range(1, len(lines)):
+            if re.match(r'\d{4}-\d{2}-\d{2} \d{2}:\d{2}:\d{2}', lines[i]):
+                timestamps.append((lines[i], lines[i-1]))
+        for timestamp, line_before in timestamps:
+            md_text = md_text.replace(line_before + '\n' + timestamp, timestamp + '\n' + line_before + '\n')
+        md_text = re.sub(r'\n{2,}', '\n\n', md_text)  # 保留一个空行。将连续出现两个或更多个换行符的情况替换为一个空行，即保留一个空行。
+        return md_text
+
+    # 文件，单个处理
+    def modify_by_md(file_path):
+        # 读取md文档内容
+        with open(file_path, 'r') as file:
+            md_text = file.read()
+
+        # 调换时间戳与前一行的位置
+        new_md_text = swap_timestamps(md_text)
+
+        # 将修改后的内容写回md文档
+        with open(file_path, 'w') as file:
+            file.write(new_md_text)
+
+    # 文件夹，遍历处理
+    def modify_by_dir(path):
+        # 获取md文件列表
+        md_files = [f for f in os.listdir(path) if f.endswith('.md')]
+
+        for md_file in md_files:
+            file_path = os.path.join(path, md_file)
+            modify_by_md(file_path)
+
+    # 判断路径是文件路径还是文件夹路径，根据路径性质选择处理方式
+    def check_path_type(raw_path):
+        if os.path.isfile(raw_path):
+            print(f"{raw_path} 是一个文件路径。")
+            modify_by_md(raw_path)
+        elif os.path.isdir(raw_path):
+            print(f"{raw_path} 是一个文件夹路径。")
+            modify_by_dir(raw_path)
+        else:
+            print(f"{raw_path} 不是有效的路径。")
+
+    # 指定md文档所在的路径
+    raw_path = raw_path
+    check_path_type(raw_path)
+
+    print("处理完毕")
+
+
+
+
 def obsidian_move_md_or_canvas_linked_images(images_path,folder_path,target_folder):
     """
     功能：指定相关路径，提取obsidian中.md文档、.canvas文档中链接的图片，实现附件管理、库空间管理、笔记归档。
 
     参数：
 
     images_path：图片附件所在的文件夹。通常是笔记库的附件文件夹。
```

### Comparing `pydatawork-0.17.5.9/setup.py` & `pydatawork-0.17.6.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pydatawork',
-    version='0.17.5.9',
+    version='0.17.6.0',
     py_modules=['pydatawork'],
     author='jk.zhou',
     author_email='zhouqiling.bjfu@foxmail.com',
     description="jk.zhou's datawork",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
```

