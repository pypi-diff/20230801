# Comparing `tmp/delta-sharing-0.7.3.tar.gz` & `tmp/delta-sharing-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delta-sharing-0.7.3.tar", last modified: Wed Jul 26 20:39:36 2023, max compression
+gzip compressed data, was "delta-sharing-0.7.4.tar", last modified: Tue Aug  1 21:25:31 2023, max compression
```

## Comparing `delta-sharing-0.7.3.tar` & `delta-sharing-0.7.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 lin.zhou   (502) staff       (20)        0 2023-07-26 20:39:36.996597 delta-sharing-0.7.3/
--rw-r--r--   0 lin.zhou   (502) staff       (20)      534 2023-07-21 00:01:06.000000 delta-sharing-0.7.3/NOTICE.txt
--rw-r--r--   0 lin.zhou   (502) staff       (20)     2282 2023-07-26 20:39:36.996380 delta-sharing-0.7.3/PKG-INFO
--rw-r--r--   0 lin.zhou   (502) staff       (20)     1201 2023-07-10 07:05:33.000000 delta-sharing-0.7.3/README.md
-drwxr-xr-x   0 lin.zhou   (502) staff       (20)        0 2023-07-26 20:39:36.994321 delta-sharing-0.7.3/delta_sharing/
--rw-r--r--   0 lin.zhou   (502) staff       (20)     1274 2023-07-21 00:01:06.000000 delta-sharing-0.7.3/delta_sharing/__init__.py
--rw-r--r--   0 lin.zhou   (502) staff       (20)      855 2023-07-10 07:05:33.000000 delta-sharing-0.7.3/delta_sharing/_yarl_patch.py
--rw-r--r--   0 lin.zhou   (502) staff       (20)     5066 2023-07-10 07:05:33.000000 delta-sharing-0.7.3/delta_sharing/converter.py
--rw-r--r--   0 lin.zhou   (502) staff       (20)    12923 2023-07-21 00:01:06.000000 delta-sharing-0.7.3/delta_sharing/delta_sharing.py
--rw-r--r--   0 lin.zhou   (502) staff       (20)    10304 2023-07-21 00:01:06.000000 delta-sharing-0.7.3/delta_sharing/protocol.py
--rw-r--r--   0 lin.zhou   (502) staff       (20)     7912 2023-07-21 00:01:06.000000 delta-sharing-0.7.3/delta_sharing/reader.py
--rw-r--r--   0 lin.zhou   (502) staff       (20)    16644 2023-07-21 00:01:06.000000 delta-sharing-0.7.3/delta_sharing/rest_client.py
--rw-r--r--   0 lin.zhou   (502) staff       (20)      626 2023-07-26 20:38:43.000000 delta-sharing-0.7.3/delta_sharing/version.py
-drwxr-xr-x   0 lin.zhou   (502) staff       (20)        0 2023-07-26 20:39:36.995846 delta-sharing-0.7.3/delta_sharing.egg-info/
--rw-r--r--   0 lin.zhou   (502) staff       (20)     2282 2023-07-26 20:39:36.000000 delta-sharing-0.7.3/delta_sharing.egg-info/PKG-INFO
--rw-r--r--   0 lin.zhou   (502) staff       (20)      430 2023-07-26 20:39:36.000000 delta-sharing-0.7.3/delta_sharing.egg-info/SOURCES.txt
--rw-r--r--   0 lin.zhou   (502) staff       (20)        1 2023-07-26 20:39:36.000000 delta-sharing-0.7.3/delta_sharing.egg-info/dependency_links.txt
--rw-r--r--   0 lin.zhou   (502) staff       (20)      167 2023-07-26 20:39:36.000000 delta-sharing-0.7.3/delta_sharing.egg-info/requires.txt
--rw-r--r--   0 lin.zhou   (502) staff       (20)       14 2023-07-26 20:39:36.000000 delta-sharing-0.7.3/delta_sharing.egg-info/top_level.txt
--rw-r--r--   0 lin.zhou   (502) staff       (20)       38 2023-07-26 20:39:36.996649 delta-sharing-0.7.3/setup.cfg
--rw-r--r--   0 lin.zhou   (502) staff       (20)     2600 2023-07-10 07:05:33.000000 delta-sharing-0.7.3/setup.py
+drwxr-xr-x   0 lin.zhou   (502) staff       (20)        0 2023-08-01 21:25:31.767851 delta-sharing-0.7.4/
+-rw-r--r--   0 lin.zhou   (502) staff       (20)      534 2023-07-21 00:01:06.000000 delta-sharing-0.7.4/NOTICE.txt
+-rw-r--r--   0 lin.zhou   (502) staff       (20)     2282 2023-08-01 21:25:31.767668 delta-sharing-0.7.4/PKG-INFO
+-rw-r--r--   0 lin.zhou   (502) staff       (20)     1201 2023-07-10 07:05:33.000000 delta-sharing-0.7.4/README.md
+drwxr-xr-x   0 lin.zhou   (502) staff       (20)        0 2023-08-01 21:25:31.765659 delta-sharing-0.7.4/delta_sharing/
+-rw-r--r--   0 lin.zhou   (502) staff       (20)     1274 2023-07-21 00:01:06.000000 delta-sharing-0.7.4/delta_sharing/__init__.py
+-rw-r--r--   0 lin.zhou   (502) staff       (20)      855 2023-07-10 07:05:33.000000 delta-sharing-0.7.4/delta_sharing/_yarl_patch.py
+-rw-r--r--   0 lin.zhou   (502) staff       (20)     5066 2023-07-10 07:05:33.000000 delta-sharing-0.7.4/delta_sharing/converter.py
+-rw-r--r--   0 lin.zhou   (502) staff       (20)    12923 2023-07-21 00:01:06.000000 delta-sharing-0.7.4/delta_sharing/delta_sharing.py
+-rw-r--r--   0 lin.zhou   (502) staff       (20)    10304 2023-07-21 00:01:06.000000 delta-sharing-0.7.4/delta_sharing/protocol.py
+-rw-r--r--   0 lin.zhou   (502) staff       (20)     7920 2023-08-01 18:49:29.000000 delta-sharing-0.7.4/delta_sharing/reader.py
+-rw-r--r--   0 lin.zhou   (502) staff       (20)    16644 2023-07-21 00:01:06.000000 delta-sharing-0.7.4/delta_sharing/rest_client.py
+-rw-r--r--   0 lin.zhou   (502) staff       (20)      626 2023-08-01 21:24:15.000000 delta-sharing-0.7.4/delta_sharing/version.py
+drwxr-xr-x   0 lin.zhou   (502) staff       (20)        0 2023-08-01 21:25:31.767240 delta-sharing-0.7.4/delta_sharing.egg-info/
+-rw-r--r--   0 lin.zhou   (502) staff       (20)     2282 2023-08-01 21:25:31.000000 delta-sharing-0.7.4/delta_sharing.egg-info/PKG-INFO
+-rw-r--r--   0 lin.zhou   (502) staff       (20)      430 2023-08-01 21:25:31.000000 delta-sharing-0.7.4/delta_sharing.egg-info/SOURCES.txt
+-rw-r--r--   0 lin.zhou   (502) staff       (20)        1 2023-08-01 21:25:31.000000 delta-sharing-0.7.4/delta_sharing.egg-info/dependency_links.txt
+-rw-r--r--   0 lin.zhou   (502) staff       (20)      167 2023-08-01 21:25:31.000000 delta-sharing-0.7.4/delta_sharing.egg-info/requires.txt
+-rw-r--r--   0 lin.zhou   (502) staff       (20)       14 2023-08-01 21:25:31.000000 delta-sharing-0.7.4/delta_sharing.egg-info/top_level.txt
+-rw-r--r--   0 lin.zhou   (502) staff       (20)       38 2023-08-01 21:25:31.767900 delta-sharing-0.7.4/setup.cfg
+-rw-r--r--   0 lin.zhou   (502) staff       (20)     2600 2023-07-10 07:05:33.000000 delta-sharing-0.7.4/setup.py
```

### Comparing `delta-sharing-0.7.3/NOTICE.txt` & `delta-sharing-0.7.4/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `delta-sharing-0.7.3/PKG-INFO` & `delta-sharing-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delta-sharing
-Version: 0.7.3
+Version: 0.7.4
 Summary: Python Connector for Delta Sharing
 Home-page: https://github.com/delta-io/delta-sharing/
 Author: The Delta Lake Project Authors
 Author-email: delta-users@googlegroups.com
 License: Apache-2.0
 Project-URL: Source, https://github.com/delta-io/delta-sharing
 Project-URL: Documentation, https://github.com/delta-io/delta-sharing
```

### Comparing `delta-sharing-0.7.3/README.md` & `delta-sharing-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `delta-sharing-0.7.3/delta_sharing/__init__.py` & `delta-sharing-0.7.4/delta_sharing/__init__.py`

 * *Files identical despite different names*

### Comparing `delta-sharing-0.7.3/delta_sharing/_yarl_patch.py` & `delta-sharing-0.7.4/delta_sharing/_yarl_patch.py`

 * *Files identical despite different names*

### Comparing `delta-sharing-0.7.3/delta_sharing/converter.py` & `delta-sharing-0.7.4/delta_sharing/converter.py`

 * *Files identical despite different names*

### Comparing `delta-sharing-0.7.3/delta_sharing/delta_sharing.py` & `delta-sharing-0.7.4/delta_sharing/delta_sharing.py`

 * *Files identical despite different names*

### Comparing `delta-sharing-0.7.3/delta_sharing/protocol.py` & `delta-sharing-0.7.4/delta_sharing/protocol.py`

 * *Files identical despite different names*

### Comparing `delta-sharing-0.7.3/delta_sharing/reader.py` & `delta-sharing-0.7.4/delta_sharing/reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,15 +179,15 @@
                     else:
                         raise ValueError("Cannot partition on binary or complex columns")
                 else:
                     pdf[col] = None
 
         if for_cdf:
             # Add the change type col name to non cdc actions.
-            if type(action) != AddCdcFile:
+            if not isinstance(action, AddCdcFile):
                 pdf[DeltaSharingReader._change_type_col_name()] = action.get_change_type_col_value()
 
             # If available, add timestamp and version columns from the action.
             # All rows of the dataframe will get the same value.
             if action.version is not None:
                 assert DeltaSharingReader._commit_version_col_name() not in pdf.columns
                 pdf[DeltaSharingReader._commit_version_col_name()] = action.version
```

### Comparing `delta-sharing-0.7.3/delta_sharing/rest_client.py` & `delta-sharing-0.7.4/delta_sharing/rest_client.py`

 * *Files identical despite different names*

### Comparing `delta-sharing-0.7.3/delta_sharing/version.py` & `delta-sharing-0.7.4/delta_sharing/version.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = "0.7.3"
+__version__ = "0.7.4"
```

### Comparing `delta-sharing-0.7.3/delta_sharing.egg-info/PKG-INFO` & `delta-sharing-0.7.4/delta_sharing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delta-sharing
-Version: 0.7.3
+Version: 0.7.4
 Summary: Python Connector for Delta Sharing
 Home-page: https://github.com/delta-io/delta-sharing/
 Author: The Delta Lake Project Authors
 Author-email: delta-users@googlegroups.com
 License: Apache-2.0
 Project-URL: Source, https://github.com/delta-io/delta-sharing
 Project-URL: Documentation, https://github.com/delta-io/delta-sharing
```

### Comparing `delta-sharing-0.7.3/setup.py` & `delta-sharing-0.7.4/setup.py`

 * *Files identical despite different names*

