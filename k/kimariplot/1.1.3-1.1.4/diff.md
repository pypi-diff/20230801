# Comparing `tmp/kimariplot-1.1.3.tar.gz` & `tmp/kimariplot-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kimariplot-1.1.3.tar", last modified: Tue Aug  1 08:26:55 2023, max compression
+gzip compressed data, was "kimariplot-1.1.4.tar", last modified: Tue Aug  1 08:49:27 2023, max compression
```

## Comparing `kimariplot-1.1.3.tar` & `kimariplot-1.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 08:26:55.420193 kimariplot-1.1.3/
--rw-rw-rw-   0        0        0     1086 2023-07-30 18:07:15.000000 kimariplot-1.1.3/LICENSE
--rw-rw-rw-   0        0        0     3065 2023-08-01 08:26:55.419192 kimariplot-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2620 2023-08-01 08:14:46.000000 kimariplot-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 08:26:55.408195 kimariplot-1.1.3/kimariplot/
--rw-rw-rw-   0        0        0        0 2023-08-01 04:25:08.000000 kimariplot-1.1.3/kimariplot/__init__.py
--rw-rw-rw-   0        0        0     5682 2023-08-01 08:22:58.000000 kimariplot-1.1.3/kimariplot/poltter.py
-drwxrwxrwx   0        0        0        0 2023-08-01 08:26:55.417192 kimariplot-1.1.3/kimariplot.egg-info/
--rw-rw-rw-   0        0        0     3065 2023-08-01 08:26:55.000000 kimariplot-1.1.3/kimariplot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-08-01 08:26:55.000000 kimariplot-1.1.3/kimariplot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 08:26:55.000000 kimariplot-1.1.3/kimariplot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-08-01 08:26:55.000000 kimariplot-1.1.3/kimariplot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       11 2023-08-01 08:26:55.000000 kimariplot-1.1.3/kimariplot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 08:26:55.420193 kimariplot-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0      796 2023-08-01 08:26:52.000000 kimariplot-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:49:27.836411 kimariplot-1.1.4/
+-rw-rw-rw-   0        0        0     1086 2023-07-30 18:07:15.000000 kimariplot-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0     3065 2023-08-01 08:49:27.835410 kimariplot-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2620 2023-08-01 08:14:46.000000 kimariplot-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 08:49:27.823412 kimariplot-1.1.4/kimariplot/
+-rw-rw-rw-   0        0        0        0 2023-08-01 04:25:08.000000 kimariplot-1.1.4/kimariplot/__init__.py
+-rw-rw-rw-   0        0        0     7083 2023-08-01 08:49:15.000000 kimariplot-1.1.4/kimariplot/plotter.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:49:27.833410 kimariplot-1.1.4/kimariplot.egg-info/
+-rw-rw-rw-   0        0        0     3065 2023-08-01 08:49:27.000000 kimariplot-1.1.4/kimariplot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-08-01 08:49:27.000000 kimariplot-1.1.4/kimariplot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 08:49:27.000000 kimariplot-1.1.4/kimariplot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-08-01 08:49:27.000000 kimariplot-1.1.4/kimariplot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       11 2023-08-01 08:49:27.000000 kimariplot-1.1.4/kimariplot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 08:49:27.836411 kimariplot-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      804 2023-08-01 08:49:15.000000 kimariplot-1.1.4/setup.py
```

### Comparing `kimariplot-1.1.3/LICENSE` & `kimariplot-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kimariplot-1.1.3/PKG-INFO` & `kimariplot-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kimariplot
-Version: 1.1.3
+Version: 1.1.4
 Summary: A tool for generating Kimari-plots.
 Home-page: https://github.com/kimariyb/kimariPlot
 Author: Kimariyb
 Author-email: kimariyb@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kimariplot-1.1.3/README.md` & `kimariplot-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `kimariplot-1.1.3/kimariplot/poltter.py` & `kimariplot-1.1.4/kimariplot/plotter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import argparse
+
 import matplotlib.pyplot as plt
 import toml
 
 
 def parse(file_path: str):
     """
     读取 toml 文件，并返回一个 PlotData 对象列表
@@ -164,7 +166,33 @@
 
     # 显示图形
     fig.show()
     # 保存路径为当前文件夹下的 figure 文件
     save_name = "figure." + output_type
     # 保存
     fig.savefig(save_name, dpi=dpi, bbox_inches='tight')
+
+
+def main():
+    # 创建 ArgumentParser 对象
+    parser = argparse.ArgumentParser(description='Generate a energy profile using kimariplot', add_help=False)
+    # 添加 -h 参数
+    parser.add_argument('--help', '-h', action='help', help='Show this help message and exit')
+    # 添加输入文件参数
+    parser.add_argument('input_file', type=str, help='Please input a Toml file')
+    # 添加输出文件格式参数
+    parser.add_argument('--output_type', '-o', dest='output', type=str, help='The output type of the graph',
+                        default='png')
+    # 添加输出文件 dpi 参数
+    parser.add_argument('--dpi', '-d', dest='dpi', type=int, help='The dpi of the output graph', default=500)
+    # 添加全局字体参数
+    parser.add_argument('--font', '-f', dest='font', type=str, help='The font family of the graph', default='Arial')
+    # 添加图像大小参数
+    parser.add_argument('--size', '-s', dest='size', type=str, help='The size of the graph', default='10,7.5')
+    # 解析命令行参数
+    args = parser.parse_args()
+    # 得到 Toml 文件中的数据列表
+    plot_data_list = parse(args.input_file)
+    # 将 size 参数转换为元组类型
+    size = tuple(map(float, args.size.split(',')))
+    # 绘制所有路径
+    plot_all_line_paths(plot_data_list, args.dpi, size, args.font, args.output)
```

### Comparing `kimariplot-1.1.3/kimariplot.egg-info/PKG-INFO` & `kimariplot-1.1.4/kimariplot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kimariplot
-Version: 1.1.3
+Version: 1.1.4
 Summary: A tool for generating Kimari-plots.
 Home-page: https://github.com/kimariyb/kimariPlot
 Author: Kimariyb
 Author-email: kimariyb@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kimariplot-1.1.3/setup.py` & `kimariplot-1.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="kimariplot",
-    version="1.1.3",
+    version="1.1.4",
     author="Kimariyb",
     author_email="kimariyb@163.com",
     description="A tool for generating Kimari-plots.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kimariyb/kimariPlot",
     packages=setuptools.find_packages(),
     entry_points={
         'console_scripts': [
-            'kimariplot=kimariPlot:main',
+            'kimariplot=kimariplot.plotter:main',
         ],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

