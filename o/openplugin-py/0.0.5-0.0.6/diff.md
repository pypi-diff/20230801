# Comparing `tmp/openplugin-py-0.0.5.tar.gz` & `tmp/openplugin-py-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openplugin-py-0.0.5.tar", last modified: Tue Jul 25 03:37:58 2023, max compression
+gzip compressed data, was "openplugin-py-0.0.6.tar", last modified: Tue Aug  1 03:23:49 2023, max compression
```

## Comparing `openplugin-py-0.0.5.tar` & `openplugin-py-0.0.6.tar`

### file list

```diff
@@ -1,42 +1,45 @@
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-25 03:37:58.595705 openplugin-py-0.0.5/
--rw-r--r--   0 4paradigm   (501) staff       (20)    11357 2023-06-28 13:02:04.000000 openplugin-py-0.0.5/LICENSE
--rw-r--r--   0 4paradigm   (501) staff       (20)     4113 2023-07-25 03:37:58.595571 openplugin-py-0.0.5/PKG-INFO
--rw-r--r--   0 4paradigm   (501) staff       (20)     3032 2023-07-25 03:33:26.000000 openplugin-py-0.0.5/README.md
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-25 03:37:58.589037 openplugin-py-0.0.5/openplugin/
--rw-r--r--   0 4paradigm   (501) staff       (20)     1114 2023-07-12 05:10:25.000000 openplugin-py-0.0.5/openplugin/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-25 03:37:58.589534 openplugin-py-0.0.5/openplugin/cli/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-06-26 08:37:33.000000 openplugin-py-0.0.5/openplugin/cli/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3080 2023-07-02 15:52:03.000000 openplugin-py-0.0.5/openplugin/cli/cli.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-25 03:37:58.590299 openplugin-py-0.0.5/openplugin/install/
--rw-r--r--   0 4paradigm   (501) staff       (20)     2855 2023-07-25 02:58:36.000000 openplugin-py-0.0.5/openplugin/install/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1528 2023-07-12 02:25:06.000000 openplugin-py-0.0.5/openplugin/install/local_install.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1799 2023-07-25 03:23:23.000000 openplugin-py-0.0.5/openplugin/install/zip_install.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-25 03:37:58.591118 openplugin-py-0.0.5/openplugin/plugin/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-07-12 02:12:45.000000 openplugin-py-0.0.5/openplugin/plugin/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      928 2023-07-12 02:20:17.000000 openplugin-py-0.0.5/openplugin/plugin/base_plugin.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2194 2023-07-12 02:25:08.000000 openplugin-py-0.0.5/openplugin/plugin/webapp_plugin.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-25 03:37:58.591611 openplugin-py-0.0.5/openplugin/run/
--rw-r--r--   0 4paradigm   (501) staff       (20)     1259 2023-07-12 02:25:06.000000 openplugin-py-0.0.5/openplugin/run/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1014 2023-07-12 02:25:06.000000 openplugin-py-0.0.5/openplugin/run/local_run.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-25 03:37:58.592925 openplugin-py-0.0.5/openplugin/template/
--rw-r--r--   0 4paradigm   (501) staff       (20)      876 2023-07-02 15:52:03.000000 openplugin-py-0.0.5/openplugin/template/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1192 2023-07-02 15:52:03.000000 openplugin-py-0.0.5/openplugin/template/base_template.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      901 2023-07-02 15:52:03.000000 openplugin-py-0.0.5/openplugin/template/json_template.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      901 2023-07-02 15:52:03.000000 openplugin-py-0.0.5/openplugin/template/utils.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      902 2023-07-02 15:52:03.000000 openplugin-py-0.0.5/openplugin/template/yaml_template.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-25 03:37:58.594495 openplugin-py-0.0.5/openplugin/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-06-26 08:58:04.000000 openplugin-py-0.0.5/openplugin/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    17531 2023-06-30 09:22:51.000000 openplugin-py-0.0.5/openplugin/utils/app_util.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      915 2023-06-30 09:22:51.000000 openplugin-py-0.0.5/openplugin/utils/errors.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1022 2023-07-25 03:26:46.000000 openplugin-py-0.0.5/openplugin/utils/local_plugin_utils.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1798 2023-07-12 02:25:06.000000 openplugin-py-0.0.5/openplugin/utils/network_utils.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2321 2023-07-12 02:25:06.000000 openplugin-py-0.0.5/openplugin/utils/util.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-25 03:37:58.595393 openplugin-py-0.0.5/openplugin_py.egg-info/
--rw-r--r--   0 4paradigm   (501) staff       (20)     4113 2023-07-25 03:37:58.000000 openplugin-py-0.0.5/openplugin_py.egg-info/PKG-INFO
--rw-r--r--   0 4paradigm   (501) staff       (20)      931 2023-07-25 03:37:58.000000 openplugin-py-0.0.5/openplugin_py.egg-info/SOURCES.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)        1 2023-07-25 03:37:58.000000 openplugin-py-0.0.5/openplugin_py.egg-info/dependency_links.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       46 2023-07-25 03:37:58.000000 openplugin-py-0.0.5/openplugin_py.egg-info/entry_points.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)      167 2023-07-25 03:37:58.000000 openplugin-py-0.0.5/openplugin_py.egg-info/requires.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       11 2023-07-25 03:37:58.000000 openplugin-py-0.0.5/openplugin_py.egg-info/top_level.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       38 2023-07-25 03:37:58.595754 openplugin-py-0.0.5/setup.cfg
--rw-r--r--   0 4paradigm   (501) staff       (20)     2869 2023-06-30 09:40:35.000000 openplugin-py-0.0.5/setup.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-01 03:23:49.951027 openplugin-py-0.0.6/
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11357 2023-06-28 13:02:04.000000 openplugin-py-0.0.6/LICENSE
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4111 2023-08-01 03:23:49.950885 openplugin-py-0.0.6/PKG-INFO
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3030 2023-08-01 03:16:06.000000 openplugin-py-0.0.6/README.md
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-01 03:23:49.943615 openplugin-py-0.0.6/openplugin/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1114 2023-07-25 03:39:59.000000 openplugin-py-0.0.6/openplugin/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-01 03:23:49.944061 openplugin-py-0.0.6/openplugin/cli/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-06-26 08:37:33.000000 openplugin-py-0.0.6/openplugin/cli/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3103 2023-08-01 03:02:16.000000 openplugin-py-0.0.6/openplugin/cli/cli.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-01 03:23:49.945520 openplugin-py-0.0.6/openplugin/install/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1381 2023-08-01 03:20:13.000000 openplugin-py-0.0.6/openplugin/install/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1037 2023-08-01 03:20:15.000000 openplugin-py-0.0.6/openplugin/install/list_plugins.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1674 2023-08-01 03:20:15.000000 openplugin-py-0.0.6/openplugin/install/local_install.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1801 2023-08-01 03:20:15.000000 openplugin-py-0.0.6/openplugin/install/remote_install.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1244 2023-08-01 03:20:15.000000 openplugin-py-0.0.6/openplugin/install/uninstall.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1901 2023-08-01 03:20:15.000000 openplugin-py-0.0.6/openplugin/install/zip_install.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-01 03:23:49.946238 openplugin-py-0.0.6/openplugin/plugin/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-07-12 02:12:45.000000 openplugin-py-0.0.6/openplugin/plugin/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      928 2023-07-12 02:20:17.000000 openplugin-py-0.0.6/openplugin/plugin/base_plugin.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2194 2023-08-01 03:20:15.000000 openplugin-py-0.0.6/openplugin/plugin/webapp_plugin.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-01 03:23:49.946908 openplugin-py-0.0.6/openplugin/run/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1259 2023-07-12 02:25:06.000000 openplugin-py-0.0.6/openplugin/run/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1014 2023-07-12 02:25:06.000000 openplugin-py-0.0.6/openplugin/run/local_run.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-01 03:23:49.948455 openplugin-py-0.0.6/openplugin/template/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      876 2023-07-02 15:52:03.000000 openplugin-py-0.0.6/openplugin/template/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1192 2023-07-02 15:52:03.000000 openplugin-py-0.0.6/openplugin/template/base_template.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      901 2023-07-02 15:52:03.000000 openplugin-py-0.0.6/openplugin/template/json_template.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      901 2023-07-02 15:52:03.000000 openplugin-py-0.0.6/openplugin/template/utils.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      902 2023-07-02 15:52:03.000000 openplugin-py-0.0.6/openplugin/template/yaml_template.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-01 03:23:49.949900 openplugin-py-0.0.6/openplugin/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-06-26 08:58:04.000000 openplugin-py-0.0.6/openplugin/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    17531 2023-06-30 09:22:51.000000 openplugin-py-0.0.6/openplugin/utils/app_util.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      915 2023-06-30 09:22:51.000000 openplugin-py-0.0.6/openplugin/utils/errors.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1025 2023-08-01 03:20:13.000000 openplugin-py-0.0.6/openplugin/utils/local_plugin_utils.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1798 2023-07-12 02:25:06.000000 openplugin-py-0.0.6/openplugin/utils/network_utils.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2671 2023-08-01 03:20:13.000000 openplugin-py-0.0.6/openplugin/utils/util.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-08-01 03:23:49.950702 openplugin-py-0.0.6/openplugin_py.egg-info/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4111 2023-08-01 03:23:49.000000 openplugin-py-0.0.6/openplugin_py.egg-info/PKG-INFO
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1035 2023-08-01 03:23:49.000000 openplugin-py-0.0.6/openplugin_py.egg-info/SOURCES.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)        1 2023-08-01 03:23:49.000000 openplugin-py-0.0.6/openplugin_py.egg-info/dependency_links.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       46 2023-08-01 03:23:49.000000 openplugin-py-0.0.6/openplugin_py.egg-info/entry_points.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)      167 2023-08-01 03:23:49.000000 openplugin-py-0.0.6/openplugin_py.egg-info/requires.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       11 2023-08-01 03:23:49.000000 openplugin-py-0.0.6/openplugin_py.egg-info/top_level.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       38 2023-08-01 03:23:49.951073 openplugin-py-0.0.6/setup.cfg
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2869 2023-06-30 09:40:35.000000 openplugin-py-0.0.6/setup.py
```

### Comparing `openplugin-py-0.0.5/LICENSE` & `openplugin-py-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.5/PKG-INFO` & `openplugin-py-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openplugin-py
-Version: 0.0.5
+Version: 0.0.6
 Summary: Toolkit and Collection for Plugins of Large Language Models
 Home-page: https://github.com/OpenRL-Lab/openplugin
 Author: openrl contributors
 Author-email: huangsy1314@163.com
 Project-URL: Code, https://github.com/OpenRL-Lab/openplugin
 Project-URL: Documentation, https://openplugin.readthedocs.io/
 Keywords: LLM plugin toolkit
@@ -45,27 +45,27 @@
 
 We provide plugins in [Plugin Store](https://openrl.net/plugin-store/). Users can download these plugins and use them with `op`.
 
 ## Usage
 
 - Check OpenPlugin's version with: `op --version`
 - Check system information: `op --system_info`
-- Install a plugin: `op install <plugin_name>`. You can also install local plugins with `op install ./`.
+- Install a plugin: `op install <plugin_name>`. You can also install local plugins with `op install .`.
   - You can also install a plugin from a zip file: `op install <zip_file_path>`.
 - Uninstall a plugin: `op uninstall <plugin_name>`
 - Start a plugin: `op run <plugin_name>`. You can use `-p` to specify the port of the plugin. By default, the port is 5003.  You can also run a local plugin with `op run ./`.
 - List installed plugins: `op list`
 - Reinstall plugin: `op reinstall <plugin_name>`
 
 ## An example for using QRcode_plugin
 
 - Install QRcode_plugin: `op install QRcode_plugin`
 - Or You can install QRcode_plugin from local:
   - Go to the directory of QRcode_plugin: `cd plugins/QRcode_plugin`
-  - Install QRcode_plugin: `op install ./`
+  - Install QRcode_plugin: `op install .`
 - Or you can install QRcode_plugin from a zip file: `op install QRcode_plugin.zip`
 - Start QRcode_plugin: `op run QRcode_plugin -p server_port`
 - Or you can start QRcode_plugin from local:
   - Go to the directory of QRcode_plugin: `cd plugins/QRcode_plugin`
   - Start QRcode_plugin: `op run ./ -p server_port`
 - Then you can get the `ai-plugin.json` file via visiting `http://<server_ip>:server_port/ai-plugin.json`
 - You can get the `openaip.yaml` file via visiting `http://<server_ip>:server_port/openaip.yaml`
```

### Comparing `openplugin-py-0.0.5/README.md` & `openplugin-py-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,27 +19,27 @@
 
 We provide plugins in [Plugin Store](https://openrl.net/plugin-store/). Users can download these plugins and use them with `op`.
 
 ## Usage
 
 - Check OpenPlugin's version with: `op --version`
 - Check system information: `op --system_info`
-- Install a plugin: `op install <plugin_name>`. You can also install local plugins with `op install ./`.
+- Install a plugin: `op install <plugin_name>`. You can also install local plugins with `op install .`.
   - You can also install a plugin from a zip file: `op install <zip_file_path>`.
 - Uninstall a plugin: `op uninstall <plugin_name>`
 - Start a plugin: `op run <plugin_name>`. You can use `-p` to specify the port of the plugin. By default, the port is 5003.  You can also run a local plugin with `op run ./`.
 - List installed plugins: `op list`
 - Reinstall plugin: `op reinstall <plugin_name>`
 
 ## An example for using QRcode_plugin
 
 - Install QRcode_plugin: `op install QRcode_plugin`
 - Or You can install QRcode_plugin from local:
   - Go to the directory of QRcode_plugin: `cd plugins/QRcode_plugin`
-  - Install QRcode_plugin: `op install ./`
+  - Install QRcode_plugin: `op install .`
 - Or you can install QRcode_plugin from a zip file: `op install QRcode_plugin.zip`
 - Start QRcode_plugin: `op run QRcode_plugin -p server_port`
 - Or you can start QRcode_plugin from local:
   - Go to the directory of QRcode_plugin: `cd plugins/QRcode_plugin`
   - Start QRcode_plugin: `op run ./ -p server_port`
 - Then you can get the `ai-plugin.json` file via visiting `http://<server_ip>:server_port/ai-plugin.json`
 - You can get the `openaip.yaml` file via visiting `http://<server_ip>:server_port/openaip.yaml`
```

### Comparing `openplugin-py-0.0.5/openplugin/__init__.py` & `openplugin-py-0.0.6/openplugin/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 
 
 __TITLE__ = "openplugin"
-__VERSION__ = "v0.0.5"
+__VERSION__ = "v0.0.6"
 __DESCRIPTION__ = "Toolkit and Collection for Plugins of Large Language Models"
 __AUTHOR__ = "OpenRL Contributors"
 __EMAIL__ = "huangshiyu@4paradigm.com"
 __version__ = __VERSION__
 
 import platform
```

### Comparing `openplugin-py-0.0.5/openplugin/cli/__init__.py` & `openplugin-py-0.0.6/openplugin/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.5/openplugin/cli/cli.py` & `openplugin-py-0.0.6/openplugin/cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,30 +90,30 @@
 
     install_plugin(plugin_name)
 
 
 @cli.command()
 @click.argument("plugin_name")
 def uninstall(plugin_name):
-    from openplugin.install import uninstall_plugin
+    from openplugin.install.uninstall import uninstall_plugin
 
     uninstall_plugin(plugin_name)
 
 
 @cli.command()
 @click.argument("plugin_name")
 def reinstall(plugin_name):
     from openplugin.install import reinstall_plugin
 
     reinstall_plugin(plugin_name)
 
 
 @cli.command()
 def list():
-    from openplugin.install import list_plugins
+    from openplugin.install.list_plugins import list_plugins
 
     list_plugins()
 
 
 @cli.command()
 @click.argument("plugin_name")
 @click.option(
```

### Comparing `openplugin-py-0.0.5/openplugin/install/local_install.py` & `openplugin-py-0.0.6/openplugin/install/local_install.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,23 +12,25 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 
-import json
 import os
 import shutil
 import tempfile
 import zipfile
-from pathlib import Path
 
 from openplugin.utils.local_plugin_utils import check_local_plugin
-from openplugin.utils.util import get_plugin_directory, make_zip_file
+from openplugin.utils.util import (
+    get_plugin_directory,
+    get_plugin_version,
+    make_zip_file,
+)
 
 
 def install_local_plugin() -> bool:
     plugin_name = check_local_plugin()
     print("Installing plugin: {}...".format(plugin_name))
 
     tempdir = tempfile.mkdtemp()
@@ -39,8 +41,10 @@
     z = zipfile.ZipFile(filepath)
     plugin_directory = get_plugin_directory()
     if not plugin_directory.exists():
         plugin_directory.mkdir(parents=True)
     print("Extracting plugin to {}".format(plugin_directory / plugin_name))
     z.extractall(os.path.join(get_plugin_directory(), plugin_name))
     shutil.rmtree(tempdir, ignore_errors=True)
+    plugin_version = get_plugin_version(plugin_directory / plugin_name)
+    print("Installed plugin: {}:{}!".format(plugin_name, plugin_version))
     return True
```

### Comparing `openplugin-py-0.0.5/openplugin/install/zip_install.py` & `openplugin-py-0.0.6/openplugin/install/zip_install.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,49 +11,47 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
-import os.path
+
 import shutil
 import tempfile
 import zipfile
-
 from pathlib import Path
 
 from openplugin.utils.local_plugin_utils import check_local_plugin
-
 from openplugin.utils.util import (
-    get_plugin_list,
     get_plugin_directory,
-
+    get_plugin_list,
+    get_plugin_version,
 )
 
+
 def install_zip_plugin(plugin_zip_file_path: str) -> bool:
     assert plugin_zip_file_path.endswith(".zip")
 
     tempdir = tempfile.mkdtemp()
     z = zipfile.ZipFile(plugin_zip_file_path)
     z.extractall(tempdir)
 
-
     plugin_name = check_local_plugin(Path(tempdir).iterdir().__next__())
     shutil.rmtree(tempdir, ignore_errors=True)
     plugin_list = get_plugin_list()
     if plugin_name in plugin_list:
         print("Plugin {} already installed!".format(plugin_name))
         return True
 
     try:
         plugin_directory = get_plugin_directory()
         if not plugin_directory.exists():
             plugin_directory.mkdir(parents=True)
         print("Extracting plugin to {}".format(plugin_directory / plugin_name))
         z.extractall(get_plugin_directory())
+        plugin_version = get_plugin_version(plugin_directory / plugin_name)
     except:
         raise ValueError("Install {} failed".format(plugin_name))
 
-
-    print("Installed plugin: {}!".format(plugin_name))
-    return True
+    print("Installed plugin: {}:{}!".format(plugin_name, plugin_version))
+    return True
```

### Comparing `openplugin-py-0.0.5/openplugin/plugin/__init__.py` & `openplugin-py-0.0.6/openplugin/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.5/openplugin/plugin/base_plugin.py` & `openplugin-py-0.0.6/openplugin/plugin/base_plugin.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.5/openplugin/plugin/webapp_plugin.py` & `openplugin-py-0.0.6/openplugin/plugin/webapp_plugin.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.5/openplugin/run/__init__.py` & `openplugin-py-0.0.6/openplugin/run/__init__.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.5/openplugin/run/local_run.py` & `openplugin-py-0.0.6/openplugin/run/local_run.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.5/openplugin/template/__init__.py` & `openplugin-py-0.0.6/openplugin/template/__init__.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.5/openplugin/template/base_template.py` & `openplugin-py-0.0.6/openplugin/template/base_template.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.5/openplugin/template/json_template.py` & `openplugin-py-0.0.6/openplugin/template/json_template.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.5/openplugin/template/utils.py` & `openplugin-py-0.0.6/openplugin/template/utils.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.5/openplugin/template/yaml_template.py` & `openplugin-py-0.0.6/openplugin/template/yaml_template.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.5/openplugin/utils/__init__.py` & `openplugin-py-0.0.6/openplugin/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.5/openplugin/utils/app_util.py` & `openplugin-py-0.0.6/openplugin/utils/app_util.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.5/openplugin/utils/errors.py` & `openplugin-py-0.0.6/openplugin/utils/errors.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.5/openplugin/utils/local_plugin_utils.py` & `openplugin-py-0.0.6/openplugin/utils/local_plugin_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # limitations under the License.
 
 """"""
 import json
 from pathlib import Path
 
 
-def check_local_plugin(plugin_path:str = "./") -> str:
-    info_file = Path(plugin_path)/"info.json"
+def check_local_plugin(plugin_path: str = "./") -> str:
+    info_file = Path(plugin_path) / "info.json"
 
     assert info_file.exists(), "info.json not found"
     info_dict = json.load(open(info_file, "r"))
     assert "plugin_name" in info_dict, "plugin_name not found in info.json"
     plugin_name = info_dict["plugin_name"]
     return plugin_name
```

### Comparing `openplugin-py-0.0.5/openplugin/utils/network_utils.py` & `openplugin-py-0.0.6/openplugin/utils/network_utils.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.5/openplugin/utils/util.py` & `openplugin-py-0.0.6/openplugin/utils/util.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,20 +11,21 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
+import json
 import os
 import platform
 import re
 import shutil
 from pathlib import Path
-from typing import Dict
+from typing import Dict, Union
 
 import numpy as np
 
 import openplugin
 
 REMOTE_URL = "https://openrl.net/plugin-store/download"
 
@@ -43,14 +44,25 @@
     if plugin_directory.is_dir():
         for plugin in plugin_directory.iterdir():
             if plugin.is_dir():
                 plugin_list.append(plugin.name)
     return plugin_list
 
 
+def get_plugin_version(plugin_path: Union[Path, str]) -> str:
+    if isinstance(plugin_path, str):
+        plugin_path = Path(plugin_path)
+    info_file = plugin_path / "info.json"
+    assert info_file.exists(), "Plugin info file not found!"
+
+    with open(info_file) as f:
+        info = json.load(f)
+    return info["version"]
+
+
 def make_zip_file(dir_to_put_file_in, plugin_directory, plugin_name):
     # create a zip file
     zip_file_name = plugin_name
     zip_file_parent = Path(plugin_directory).parent
     zip_file_path = os.path.join(dir_to_put_file_in, zip_file_name)
     shutil.make_archive(zip_file_path, "zip", zip_file_parent, plugin_directory)
     return os.path.join(dir_to_put_file_in, zip_file_name + ".zip")
```

### Comparing `openplugin-py-0.0.5/openplugin_py.egg-info/PKG-INFO` & `openplugin-py-0.0.6/openplugin_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openplugin-py
-Version: 0.0.5
+Version: 0.0.6
 Summary: Toolkit and Collection for Plugins of Large Language Models
 Home-page: https://github.com/OpenRL-Lab/openplugin
 Author: openrl contributors
 Author-email: huangsy1314@163.com
 Project-URL: Code, https://github.com/OpenRL-Lab/openplugin
 Project-URL: Documentation, https://openplugin.readthedocs.io/
 Keywords: LLM plugin toolkit
@@ -45,27 +45,27 @@
 
 We provide plugins in [Plugin Store](https://openrl.net/plugin-store/). Users can download these plugins and use them with `op`.
 
 ## Usage
 
 - Check OpenPlugin's version with: `op --version`
 - Check system information: `op --system_info`
-- Install a plugin: `op install <plugin_name>`. You can also install local plugins with `op install ./`.
+- Install a plugin: `op install <plugin_name>`. You can also install local plugins with `op install .`.
   - You can also install a plugin from a zip file: `op install <zip_file_path>`.
 - Uninstall a plugin: `op uninstall <plugin_name>`
 - Start a plugin: `op run <plugin_name>`. You can use `-p` to specify the port of the plugin. By default, the port is 5003.  You can also run a local plugin with `op run ./`.
 - List installed plugins: `op list`
 - Reinstall plugin: `op reinstall <plugin_name>`
 
 ## An example for using QRcode_plugin
 
 - Install QRcode_plugin: `op install QRcode_plugin`
 - Or You can install QRcode_plugin from local:
   - Go to the directory of QRcode_plugin: `cd plugins/QRcode_plugin`
-  - Install QRcode_plugin: `op install ./`
+  - Install QRcode_plugin: `op install .`
 - Or you can install QRcode_plugin from a zip file: `op install QRcode_plugin.zip`
 - Start QRcode_plugin: `op run QRcode_plugin -p server_port`
 - Or you can start QRcode_plugin from local:
   - Go to the directory of QRcode_plugin: `cd plugins/QRcode_plugin`
   - Start QRcode_plugin: `op run ./ -p server_port`
 - Then you can get the `ai-plugin.json` file via visiting `http://<server_ip>:server_port/ai-plugin.json`
 - You can get the `openaip.yaml` file via visiting `http://<server_ip>:server_port/openaip.yaml`
```

### Comparing `openplugin-py-0.0.5/openplugin_py.egg-info/SOURCES.txt` & `openplugin-py-0.0.6/openplugin_py.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 LICENSE
 README.md
 setup.py
 openplugin/__init__.py
 openplugin/cli/__init__.py
 openplugin/cli/cli.py
 openplugin/install/__init__.py
+openplugin/install/list_plugins.py
 openplugin/install/local_install.py
+openplugin/install/remote_install.py
+openplugin/install/uninstall.py
 openplugin/install/zip_install.py
 openplugin/plugin/__init__.py
 openplugin/plugin/base_plugin.py
 openplugin/plugin/webapp_plugin.py
 openplugin/run/__init__.py
 openplugin/run/local_run.py
 openplugin/template/__init__.py
```

### Comparing `openplugin-py-0.0.5/setup.py` & `openplugin-py-0.0.6/setup.py`

 * *Files identical despite different names*

