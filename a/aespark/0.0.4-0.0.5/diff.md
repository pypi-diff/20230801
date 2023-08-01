# Comparing `tmp/aespark-0.0.4.tar.gz` & `tmp/aespark-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aespark-0.0.4.tar", last modified: Mon Jul 31 14:42:48 2023, max compression
+gzip compressed data, was "aespark-0.0.5.tar", last modified: Tue Aug  1 05:58:08 2023, max compression
```

## Comparing `aespark-0.0.4.tar` & `aespark-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 14:42:48.853349 aespark-0.0.4/
--rw-rw-rw-   0        0        0       89 2023-07-31 13:45:05.000000 aespark-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      731 2023-07-31 14:42:48.853349 aespark-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0        4 2023-07-31 13:30:16.000000 aespark-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 14:42:48.743981 aespark-0.0.4/aespark/
--rw-rw-rw-   0        0        0    16798 2023-07-31 14:41:52.000000 aespark-0.0.4/aespark/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 14:42:48.853349 aespark-0.0.4/aespark/static/
--rw-rw-rw-   0        0        0 70035392 2023-07-31 09:33:52.000000 aespark-0.0.4/aespark/static/ip.txt
--rw-rw-rw-   0        0        0    16706 2023-07-31 09:33:52.000000 aespark-0.0.4/aespark/static/材料模板.docx
-drwxrwxrwx   0        0        0        0 2023-07-31 14:42:48.759606 aespark-0.0.4/aespark.egg-info/
--rw-rw-rw-   0        0        0      731 2023-07-31 14:42:48.000000 aespark-0.0.4/aespark.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-07-31 14:42:48.000000 aespark-0.0.4/aespark.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 14:42:48.000000 aespark-0.0.4/aespark.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-31 14:42:48.000000 aespark-0.0.4/aespark.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       61 2023-07-31 14:42:48.000000 aespark-0.0.4/aespark.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-31 14:42:48.000000 aespark-0.0.4/aespark.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       63 2023-07-31 13:18:18.000000 aespark-0.0.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 14:42:48.853349 aespark-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1554 2023-07-31 14:42:23.000000 aespark-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 05:58:08.770706 aespark-0.0.5/
+-rw-rw-rw-   0        0        0       89 2023-07-31 13:45:05.000000 aespark-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      731 2023-08-01 05:58:08.770706 aespark-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0        4 2023-07-31 13:30:16.000000 aespark-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 05:58:08.660963 aespark-0.0.5/aespark/
+-rw-rw-rw-   0        0        0    16810 2023-08-01 04:55:26.000000 aespark-0.0.5/aespark/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 05:58:08.770706 aespark-0.0.5/aespark/static/
+-rw-rw-rw-   0        0        0 70035392 2023-07-31 09:33:52.000000 aespark-0.0.5/aespark/static/ip.txt
+-rw-rw-rw-   0        0        0    16706 2023-07-31 09:33:52.000000 aespark-0.0.5/aespark/static/材料模板.docx
+drwxrwxrwx   0        0        0        0 2023-08-01 05:58:08.660963 aespark-0.0.5/aespark.egg-info/
+-rw-rw-rw-   0        0        0      731 2023-08-01 05:58:08.000000 aespark-0.0.5/aespark.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-08-01 05:58:08.000000 aespark-0.0.5/aespark.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 05:58:08.000000 aespark-0.0.5/aespark.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-01 05:58:08.000000 aespark-0.0.5/aespark.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       61 2023-08-01 05:58:08.000000 aespark-0.0.5/aespark.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-01 05:58:08.000000 aespark-0.0.5/aespark.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       63 2023-07-31 13:18:18.000000 aespark-0.0.5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 05:58:08.770706 aespark-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1554 2023-08-01 04:55:45.000000 aespark-0.0.5/setup.py
```

### Comparing `aespark-0.0.4/PKG-INFO` & `aespark-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aespark
-Version: 0.0.4
+Version: 0.0.5
 Summary: Generate a QR code that can adapt to the cylinder
 Home-page: https://pypi.org/project/aespark/
 Author: wtianxin
 Author-email: 1007582510@qq.com
 License: MIT
 Keywords: aespark
 Classifier: Natural Language :: Chinese (Simplified)
```

### Comparing `aespark-0.0.4/aespark/__init__.py` & `aespark-0.0.5/aespark/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,29 +153,29 @@
 
 
 def oneSheetDataMerging(url: str, limit: int = 42000000, link: bool = False, lex: str = '*'):
     '''
     功能简介：
         合并单个sheet的文件
     参数解释：
-        url     目标文件夹路径(文件夹中只能有.xls或.xlsx格式的文件)；
+        url     目标文件夹路径(文件夹中只能有.csv.xls或.xlsx格式的文件)；
         limit   输出表容量（多少条数据存一张表；默认80万行）
         link    是否需要添加数据来源，默认不添加
         lex     需要合并的文件后缀，默认为所有；
     '''
     files = pd.DataFrame(columns=['文件名称', '文件路径'])
     geshi = pd.DataFrame(columns=['总文件名', '表格式', '文件数量'])
 
     for i in Path(url).rglob(f'*.{lex}'):
         files.loc[len(files)] = [Path(i).stem, i]
 
     for i in tqdm(files.index, desc='数据提取'):
 
         if lex == '*':
-            filelex = files['文件路径'][i]
+            filelex = str(files['文件路径'][i])
             iii = filelex[filelex.rindex('.'):]
             if 'xls' in iii or 'xlsx' in iii:
                 df = pd.read_excel(files['文件路径'][i], dtype='str')
             elif 'csv' in iii:
                 df = pd.read_csv(files['文件路径'][i],
                                  dtype='str', encoding='gb18030')
         elif lex in ['xls', 'xlsx']:
@@ -200,15 +200,15 @@
 
     geshi['总文件名'] = geshi['总文件名'].str.replace(
         '[^\u4e00-\u9fa5]', '', regex=True)
 
     for i in tqdm(geshi.index, desc='数据产出'):
 
         if geshi['总文件名'][i] != '':
-            file_name = pd.DataFrame(list(jieba.cut(geshi['表格式'][0])))
+            file_name = pd.DataFrame(list(jieba.cut(geshi['总文件名'][i])))
             file_name = pd.DataFrame(file_name.groupby(
                 0).size().sort_values(ascending=False))
             file_name = ''.join(
                 file_name[file_name[0] == file_name.iloc[0].values[0]].index.to_list())
         else:
             file_name = '未知'
```

### Comparing `aespark-0.0.4/aespark/static/ip.txt` & `aespark-0.0.5/aespark/static/ip.txt`

 * *Files identical despite different names*

### Comparing `aespark-0.0.4/aespark/static/材料模板.docx` & `aespark-0.0.5/aespark/static/材料模板.docx`

 * *Files identical despite different names*

### Comparing `aespark-0.0.4/aespark.egg-info/PKG-INFO` & `aespark-0.0.5/aespark.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aespark
-Version: 0.0.4
+Version: 0.0.5
 Summary: Generate a QR code that can adapt to the cylinder
 Home-page: https://pypi.org/project/aespark/
 Author: wtianxin
 Author-email: 1007582510@qq.com
 License: MIT
 Keywords: aespark
 Classifier: Natural Language :: Chinese (Simplified)
```

### Comparing `aespark-0.0.4/setup.py` & `aespark-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-setuptools.setup(name='aespark', version='0.0.4',
+setuptools.setup(name='aespark', version='0.0.5',
                  description='Generate a QR code that can adapt to the cylinder',
                  long_description=open(
                      'README.md', 'r', encoding='utf-8').read(),
                  author='wtianxin',
                  author_email='1007582510@qq.com',
                  url='https://pypi.org/project/aespark/',
                  license='MIT',  # 与之前你选用的许可证类型有关系
```

