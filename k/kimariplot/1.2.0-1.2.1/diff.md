# Comparing `tmp/kimariplot-1.2.0.tar.gz` & `tmp/kimariplot-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kimariplot-1.2.0.tar", last modified: Tue Aug  1 09:44:21 2023, max compression
+gzip compressed data, was "kimariplot-1.2.1.tar", last modified: Tue Aug  1 10:06:16 2023, max compression
```

## Comparing `kimariplot-1.2.0.tar` & `kimariplot-1.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 09:44:21.347551 kimariplot-1.2.0/
--rw-rw-rw-   0        0        0     1086 2023-07-30 18:07:15.000000 kimariplot-1.2.0/LICENSE
--rw-rw-rw-   0        0        0     4398 2023-08-01 09:44:21.346547 kimariplot-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3953 2023-08-01 09:43:44.000000 kimariplot-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 09:44:21.334551 kimariplot-1.2.0/kimariplot/
--rw-rw-rw-   0        0        0        0 2023-08-01 04:25:08.000000 kimariplot-1.2.0/kimariplot/__init__.py
--rw-rw-rw-   0        0        0     7432 2023-08-01 09:01:20.000000 kimariplot-1.2.0/kimariplot/plotter.py
-drwxrwxrwx   0        0        0        0 2023-08-01 09:44:21.344554 kimariplot-1.2.0/kimariplot.egg-info/
--rw-rw-rw-   0        0        0     4398 2023-08-01 09:44:21.000000 kimariplot-1.2.0/kimariplot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-08-01 09:44:21.000000 kimariplot-1.2.0/kimariplot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 09:44:21.000000 kimariplot-1.2.0/kimariplot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-08-01 09:44:21.000000 kimariplot-1.2.0/kimariplot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       11 2023-08-01 09:44:21.000000 kimariplot-1.2.0/kimariplot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 09:44:21.347551 kimariplot-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      804 2023-08-01 08:57:32.000000 kimariplot-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 10:06:16.095988 kimariplot-1.2.1/
+-rw-rw-rw-   0        0        0     1086 2023-07-30 18:07:15.000000 kimariplot-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0     4398 2023-08-01 10:06:16.095023 kimariplot-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3953 2023-08-01 09:43:44.000000 kimariplot-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 10:06:16.085986 kimariplot-1.2.1/kimariplot/
+-rw-rw-rw-   0        0        0        0 2023-08-01 04:25:08.000000 kimariplot-1.2.1/kimariplot/__init__.py
+-rw-rw-rw-   0        0        0     7416 2023-08-01 10:05:49.000000 kimariplot-1.2.1/kimariplot/plotter.py
+drwxrwxrwx   0        0        0        0 2023-08-01 10:06:16.093986 kimariplot-1.2.1/kimariplot.egg-info/
+-rw-rw-rw-   0        0        0     4398 2023-08-01 10:06:15.000000 kimariplot-1.2.1/kimariplot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-08-01 10:06:16.000000 kimariplot-1.2.1/kimariplot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 10:06:15.000000 kimariplot-1.2.1/kimariplot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-08-01 10:06:15.000000 kimariplot-1.2.1/kimariplot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       11 2023-08-01 10:06:15.000000 kimariplot-1.2.1/kimariplot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 10:06:16.095988 kimariplot-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      804 2023-08-01 10:05:49.000000 kimariplot-1.2.1/setup.py
```

### Comparing `kimariplot-1.2.0/LICENSE` & `kimariplot-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kimariplot-1.2.0/PKG-INFO` & `kimariplot-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kimariplot
-Version: 1.2.0
+Version: 1.2.1
 Summary: A tool for generating Kimari-plots.
 Home-page: https://github.com/kimariyb/kimariPlot
 Author: Kimariyb
 Author-email: kimariyb@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kimariplot-1.2.0/README.md` & `kimariplot-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `kimariplot-1.2.0/kimariplot/plotter.py` & `kimariplot-1.2.1/kimariplot/plotter.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,15 +170,15 @@
     save_name = "figure." + output_type
     # 保存
     fig.savefig(save_name, dpi=dpi, bbox_inches='tight')
 
 
 def main():
     # 版本参数
-    version = '1.2.0'
+    version = '1.2.1'
     # 创建 ArgumentParser 对象
     parser = argparse.ArgumentParser(description='Generate a energy profile using kimariplot', add_help=False)
     # 添加 -h 参数
     parser.add_argument('--help', '-h', action='help', help='Show this help message and exit')
     # 添加输入文件参数
     parser.add_argument('input_file', type=str, help='Please input a Toml file')
     # 添加输出文件格式参数
@@ -187,15 +187,15 @@
     # 添加输出文件 dpi 参数
     parser.add_argument('--dpi', '-d', dest='dpi', type=int, help='The dpi of the output graph', default=500)
     # 添加全局字体参数
     parser.add_argument('--font', '-f', dest='font', type=str, help='The font family of the graph', default='Arial')
     # 添加图像大小参数
     parser.add_argument('--size', '-s', dest='size', type=str, help='The size of the graph', default='10,7.5')
     # 添加查询版本参数
-    parser.add_argument('--version', '-v', dest='version', action='version', version=f'kimariplot version {version}')
+    parser.add_argument('--version', '-v', action='version', version=f'kimariplot version {version}')
     # 解析命令行参数
     args = parser.parse_args()
     # 如果用户输入了 -v 参数，输出版本信息并退出
     if args.version:
         print(f'kimariplot version {version}')
         exit()
     # 得到 Toml 文件中的数据列表
```

### Comparing `kimariplot-1.2.0/kimariplot.egg-info/PKG-INFO` & `kimariplot-1.2.1/kimariplot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kimariplot
-Version: 1.2.0
+Version: 1.2.1
 Summary: A tool for generating Kimari-plots.
 Home-page: https://github.com/kimariyb/kimariPlot
 Author: Kimariyb
 Author-email: kimariyb@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kimariplot-1.2.0/setup.py` & `kimariplot-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="kimariplot",
-    version="1.2.0",
+    version="1.2.1",
     author="Kimariyb",
     author_email="kimariyb@163.com",
     description="A tool for generating Kimari-plots.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kimariyb/kimariPlot",
     packages=setuptools.find_packages(),
```

