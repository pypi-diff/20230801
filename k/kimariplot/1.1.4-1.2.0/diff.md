# Comparing `tmp/kimariplot-1.1.4.tar.gz` & `tmp/kimariplot-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kimariplot-1.1.4.tar", last modified: Tue Aug  1 08:49:27 2023, max compression
+gzip compressed data, was "kimariplot-1.2.0.tar", last modified: Tue Aug  1 09:44:21 2023, max compression
```

## Comparing `kimariplot-1.1.4.tar` & `kimariplot-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 08:49:27.836411 kimariplot-1.1.4/
--rw-rw-rw-   0        0        0     1086 2023-07-30 18:07:15.000000 kimariplot-1.1.4/LICENSE
--rw-rw-rw-   0        0        0     3065 2023-08-01 08:49:27.835410 kimariplot-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2620 2023-08-01 08:14:46.000000 kimariplot-1.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 08:49:27.823412 kimariplot-1.1.4/kimariplot/
--rw-rw-rw-   0        0        0        0 2023-08-01 04:25:08.000000 kimariplot-1.1.4/kimariplot/__init__.py
--rw-rw-rw-   0        0        0     7083 2023-08-01 08:49:15.000000 kimariplot-1.1.4/kimariplot/plotter.py
-drwxrwxrwx   0        0        0        0 2023-08-01 08:49:27.833410 kimariplot-1.1.4/kimariplot.egg-info/
--rw-rw-rw-   0        0        0     3065 2023-08-01 08:49:27.000000 kimariplot-1.1.4/kimariplot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-08-01 08:49:27.000000 kimariplot-1.1.4/kimariplot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 08:49:27.000000 kimariplot-1.1.4/kimariplot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-08-01 08:49:27.000000 kimariplot-1.1.4/kimariplot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       11 2023-08-01 08:49:27.000000 kimariplot-1.1.4/kimariplot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 08:49:27.836411 kimariplot-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0      804 2023-08-01 08:49:15.000000 kimariplot-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 09:44:21.347551 kimariplot-1.2.0/
+-rw-rw-rw-   0        0        0     1086 2023-07-30 18:07:15.000000 kimariplot-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     4398 2023-08-01 09:44:21.346547 kimariplot-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3953 2023-08-01 09:43:44.000000 kimariplot-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 09:44:21.334551 kimariplot-1.2.0/kimariplot/
+-rw-rw-rw-   0        0        0        0 2023-08-01 04:25:08.000000 kimariplot-1.2.0/kimariplot/__init__.py
+-rw-rw-rw-   0        0        0     7432 2023-08-01 09:01:20.000000 kimariplot-1.2.0/kimariplot/plotter.py
+drwxrwxrwx   0        0        0        0 2023-08-01 09:44:21.344554 kimariplot-1.2.0/kimariplot.egg-info/
+-rw-rw-rw-   0        0        0     4398 2023-08-01 09:44:21.000000 kimariplot-1.2.0/kimariplot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-08-01 09:44:21.000000 kimariplot-1.2.0/kimariplot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 09:44:21.000000 kimariplot-1.2.0/kimariplot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-08-01 09:44:21.000000 kimariplot-1.2.0/kimariplot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       11 2023-08-01 09:44:21.000000 kimariplot-1.2.0/kimariplot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 09:44:21.347551 kimariplot-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      804 2023-08-01 08:57:32.000000 kimariplot-1.2.0/setup.py
```

### Comparing `kimariplot-1.1.4/LICENSE` & `kimariplot-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kimariplot-1.1.4/PKG-INFO` & `kimariplot-1.2.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: kimariplot
-Version: 1.1.4
-Summary: A tool for generating Kimari-plots.
-Home-page: https://github.com/kimariyb/kimariPlot
-Author: Kimariyb
-Author-email: kimariyb@163.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <h1 align="center">
     <img src="figure/logo.png" width="200">
 </h1><br>
 
 KimariPlot 是一个开源的 Python 绘图脚本，用来绘制科研中的 Free Energy Profile。KimariPlot 使用简单，可以直接从命令行读取 Toml 文件绘制 Free Energy Profile，可以不需要用鼠标一直拖来拖去，是懒人绘制 Free Energy Profile 的极佳选择。
 
 ## 安装
@@ -30,21 +16,55 @@
 
 ```shell
 pip install matplotlib, toml
 ```
 
 ## 使用
 
-安装完 KimariPlot 之后，可以直接通过如下命令在命令行中运行。
+安装完 KimariPlot 之后，可以直接通过如下命令在命令行中运行。接着就会在当前目录下生成 figure.png 图像文件。`profile.toml` 是一个 toml 文件，用来记录颜色、曲线格式以及绘制所需要的数据。
 
 ```shell
 kimariplot profile.toml
 ```
 
-其中，`profile.toml` 是一个记录了颜色、曲线格式以及绘制所需要的数据的 Toml 文件。以下是 `kimariplot/example/profile1.toml` 和 `kimariplot/example/profile2.toml` 的内容，以及生成的 Free Energy Profile 图像。
+简要介绍一下 toml 文件所需要配置的内容。`n` 为从 1 开始的整数。`color` 为折线颜色，`style` 为折线的格式，可以为 `-` 或 `--`。`data` 为数据的列表，里面可以包括很多个 3 字符串元素的列表。第一个字符串表示名字；第二个字符串表示反应的进度，一般从 1 开始；第三个字符串表示反应的 Free Energy 能垒，一般都用 kcal/mol 表示。
+
+```toml
+[path.n]
+color = "black"
+style = "-"
+data = [
+    ["Name", "1", "0.0"],
+    ["", "", ""],
+]
+```
+
+使用 KimariPlot 命令时可以更改绘图的参数，KimariPlot 支持的参数如下所示。
+
+```shell
+usage: kimariplot [--help] [--output_type OUTPUT] [--dpi DPI] [--font FONT] [--size SIZE] [--version] input_file
+
+Generate a energy profile using kimariplot
+
+positional arguments:
+  input_file            Please input a Toml file
+
+options:
+  --help, -h            Show this help message and exit
+  --output_type OUTPUT, -o OUTPUT
+                        The output type of the graph
+  --dpi DPI, -d DPI     The dpi of the output graph
+  --font FONT, -f FONT  The font family of the graph
+  --size SIZE, -s SIZE  The size of the graph
+  --version, -v         show program's version number and exit
+```
+
+## 绘制效果
+
+本例在 `kimariplot` 的 `examples/profile1.toml` 中
 
 ```toml
 [path.1]
 color = "black"
 style = "-"
 data = [
     ["7", "1", "-0.7"],
@@ -65,14 +85,16 @@
     ["TS4", "4", "23.8"],
     ["10", "6", "-10.0"]
 ]
 ```
 
 <img src="figure/1.png">
 
+本例在 `kimariplot` 的 `examples/profile2.toml` 中
+
 ```toml
 [path.1]
 color = "black"
 style = "-"
 data = [
     ["R", "1", "0.0"],
     ["", "2", "-2.9"],
@@ -126,8 +148,8 @@
 - **SciPy**
 - **Toml**
 
 还要感谢所有为 KimariPlot 做出贡献的开发者 Kimariyb 和用户。
 
 ## 许可证
 
-KimariPlot 基于 **MIT** 许可证开源。这意味着您可以自由地使用、修改和分发代码。有关更多信息，请参见 LICENSE 文件。
+KimariPlot 基于 **MIT** 许可证开源。这意味着您可以自由地使用、修改和分发代码。有关更多信息，请参见 LICENSE 文件。
```

### Comparing `kimariplot-1.1.4/kimariplot/plotter.py` & `kimariplot-1.2.0/kimariplot/plotter.py`

 * *Files 3% similar despite different names*

```diff
@@ -169,14 +169,16 @@
     # 保存路径为当前文件夹下的 figure 文件
     save_name = "figure." + output_type
     # 保存
     fig.savefig(save_name, dpi=dpi, bbox_inches='tight')
 
 
 def main():
+    # 版本参数
+    version = '1.2.0'
     # 创建 ArgumentParser 对象
     parser = argparse.ArgumentParser(description='Generate a energy profile using kimariplot', add_help=False)
     # 添加 -h 参数
     parser.add_argument('--help', '-h', action='help', help='Show this help message and exit')
     # 添加输入文件参数
     parser.add_argument('input_file', type=str, help='Please input a Toml file')
     # 添加输出文件格式参数
@@ -184,15 +186,21 @@
                         default='png')
     # 添加输出文件 dpi 参数
     parser.add_argument('--dpi', '-d', dest='dpi', type=int, help='The dpi of the output graph', default=500)
     # 添加全局字体参数
     parser.add_argument('--font', '-f', dest='font', type=str, help='The font family of the graph', default='Arial')
     # 添加图像大小参数
     parser.add_argument('--size', '-s', dest='size', type=str, help='The size of the graph', default='10,7.5')
+    # 添加查询版本参数
+    parser.add_argument('--version', '-v', dest='version', action='version', version=f'kimariplot version {version}')
     # 解析命令行参数
     args = parser.parse_args()
+    # 如果用户输入了 -v 参数，输出版本信息并退出
+    if args.version:
+        print(f'kimariplot version {version}')
+        exit()
     # 得到 Toml 文件中的数据列表
     plot_data_list = parse(args.input_file)
     # 将 size 参数转换为元组类型
     size = tuple(map(float, args.size.split(',')))
     # 绘制所有路径
     plot_all_line_paths(plot_data_list, args.dpi, size, args.font, args.output)
```

### Comparing `kimariplot-1.1.4/setup.py` & `kimariplot-1.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="kimariplot",
-    version="1.1.4",
+    version="1.2.0",
     author="Kimariyb",
     author_email="kimariyb@163.com",
     description="A tool for generating Kimari-plots.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kimariyb/kimariPlot",
     packages=setuptools.find_packages(),
```

