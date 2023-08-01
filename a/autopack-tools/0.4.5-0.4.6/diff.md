# Comparing `tmp/autopack_tools-0.4.5.tar.gz` & `tmp/autopack_tools-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopack_tools-0.4.5.tar", max compression
+gzip compressed data, was "autopack_tools-0.4.6.tar", max compression
```

## Comparing `autopack_tools-0.4.5.tar` & `autopack_tools-0.4.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1069 2023-06-25 23:21:07.938011 autopack_tools-0.4.5/LICENSE
--rw-r--r--   0        0        0     2050 2023-07-23 21:43:01.334058 autopack_tools-0.4.5/README.md
--rw-r--r--   0        0        0        6 2023-07-27 22:24:02.938972 autopack_tools-0.4.5/autopack/VERSION
--rw-r--r--   0        0        0       51 2023-07-27 22:24:02.910492 autopack_tools-0.4.5/autopack/__init__.py
--rw-r--r--   0        0        0      134 2023-07-27 22:24:02.910843 autopack_tools-0.4.5/autopack/__main__.py
--rw-r--r--   0        0        0     2824 2023-07-27 22:27:08.593199 autopack_tools-0.4.5/autopack/api.py
--rw-r--r--   0        0        0     1078 2023-07-29 02:31:38.503800 autopack_tools-0.4.5/autopack/cli.py
--rw-r--r--   0        0        0      317 2023-07-27 22:24:02.924415 autopack_tools-0.4.5/autopack/errors.py
--rw-r--r--   0        0        0        0 2023-07-27 22:24:02.929186 autopack_tools-0.4.5/autopack/filesystem_emulation/__init__.py
--rw-r--r--   0        0        0      950 2023-07-27 22:24:02.935685 autopack_tools-0.4.5/autopack/filesystem_emulation/file_manager.py
--rw-r--r--   0        0        0     3562 2023-07-27 22:24:02.927211 autopack_tools-0.4.5/autopack/filesystem_emulation/filesystem_file_manager.py
--rw-r--r--   0        0        0     2985 2023-07-27 22:24:02.928880 autopack_tools-0.4.5/autopack/filesystem_emulation/ram_file_manager.py
--rw-r--r--   0        0        0     4052 2023-07-27 22:24:02.934181 autopack_tools-0.4.5/autopack/filesystem_emulation/workspace_file_manager.py
--rw-r--r--   0        0        0     3199 2023-07-27 22:24:02.936287 autopack_tools-0.4.5/autopack/get_pack.py
--rw-r--r--   0        0        0     4063 2023-07-27 22:24:02.936559 autopack_tools-0.4.5/autopack/installation.py
--rw-r--r--   0        0        0      746 2023-07-27 22:24:02.936811 autopack_tools-0.4.5/autopack/langchain_wrapper.py
--rw-r--r--   0        0        0     5529 2023-07-27 22:24:02.937091 autopack_tools-0.4.5/autopack/pack.py
--rw-r--r--   0        0        0     3309 2023-07-27 22:26:44.374185 autopack_tools-0.4.5/autopack/pack_config.py
--rw-r--r--   0        0        0      502 2023-07-27 22:24:02.937629 autopack_tools-0.4.5/autopack/pack_response.py
--rw-r--r--   0        0        0     2217 2023-07-27 22:24:02.937878 autopack_tools-0.4.5/autopack/prompts.py
--rw-r--r--   0        0        0      394 2023-07-27 22:24:02.938125 autopack_tools-0.4.5/autopack/search.py
--rw-r--r--   0        0        0     4930 2023-07-27 22:24:02.938390 autopack_tools-0.4.5/autopack/selection.py
--rw-r--r--   0        0        0     8049 2023-07-28 20:01:33.520893 autopack_tools-0.4.5/autopack/utils.py
--rw-r--r--   0        0        0     1101 2023-07-29 04:38:49.091229 autopack_tools-0.4.5/pyproject.toml
--rw-r--r--   0        0        0     2940 1970-01-01 00:00:00.000000 autopack_tools-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-25 23:21:07.938011 autopack_tools-0.4.6/LICENSE
+-rw-r--r--   0        0        0     2050 2023-07-23 21:43:01.334058 autopack_tools-0.4.6/README.md
+-rw-r--r--   0        0        0        6 2023-07-27 22:24:02.938972 autopack_tools-0.4.6/autopack/VERSION
+-rw-r--r--   0        0        0       51 2023-07-27 22:24:02.910492 autopack_tools-0.4.6/autopack/__init__.py
+-rw-r--r--   0        0        0      134 2023-07-27 22:24:02.910843 autopack_tools-0.4.6/autopack/__main__.py
+-rw-r--r--   0        0        0     2824 2023-07-27 22:27:08.593199 autopack_tools-0.4.6/autopack/api.py
+-rw-r--r--   0        0        0     1078 2023-07-29 02:31:38.503800 autopack_tools-0.4.6/autopack/cli.py
+-rw-r--r--   0        0        0      317 2023-07-27 22:24:02.924415 autopack_tools-0.4.6/autopack/errors.py
+-rw-r--r--   0        0        0        0 2023-07-27 22:24:02.929186 autopack_tools-0.4.6/autopack/filesystem_emulation/__init__.py
+-rw-r--r--   0        0        0     1201 2023-08-01 19:38:25.248999 autopack_tools-0.4.6/autopack/filesystem_emulation/file_manager.py
+-rw-r--r--   0        0        0     5486 2023-08-01 19:41:06.050910 autopack_tools-0.4.6/autopack/filesystem_emulation/filesystem_file_manager.py
+-rw-r--r--   0        0        0     3274 2023-08-01 19:39:24.390453 autopack_tools-0.4.6/autopack/filesystem_emulation/ram_file_manager.py
+-rw-r--r--   0        0        0     6186 2023-08-01 19:42:21.775214 autopack_tools-0.4.6/autopack/filesystem_emulation/workspace_file_manager.py
+-rw-r--r--   0        0        0     3199 2023-07-27 22:24:02.936287 autopack_tools-0.4.6/autopack/get_pack.py
+-rw-r--r--   0        0        0     4063 2023-07-27 22:24:02.936559 autopack_tools-0.4.6/autopack/installation.py
+-rw-r--r--   0        0        0      746 2023-07-27 22:24:02.936811 autopack_tools-0.4.6/autopack/langchain_wrapper.py
+-rw-r--r--   0        0        0     5529 2023-07-27 22:24:02.937091 autopack_tools-0.4.6/autopack/pack.py
+-rw-r--r--   0        0        0     3309 2023-07-27 22:26:44.374185 autopack_tools-0.4.6/autopack/pack_config.py
+-rw-r--r--   0        0        0      502 2023-07-27 22:24:02.937629 autopack_tools-0.4.6/autopack/pack_response.py
+-rw-r--r--   0        0        0     2217 2023-07-27 22:24:02.937878 autopack_tools-0.4.6/autopack/prompts.py
+-rw-r--r--   0        0        0      394 2023-07-27 22:24:02.938125 autopack_tools-0.4.6/autopack/search.py
+-rw-r--r--   0        0        0     4930 2023-07-27 22:24:02.938390 autopack_tools-0.4.6/autopack/selection.py
+-rw-r--r--   0        0        0     8049 2023-07-28 20:01:33.520893 autopack_tools-0.4.6/autopack/utils.py
+-rw-r--r--   0        0        0     1101 2023-08-01 19:42:50.779857 autopack_tools-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0     2940 1970-01-01 00:00:00.000000 autopack_tools-0.4.6/PKG-INFO
```

### Comparing `autopack_tools-0.4.5/LICENSE` & `autopack_tools-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.5/README.md` & `autopack_tools-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.5/autopack/api.py` & `autopack_tools-0.4.6/autopack/api.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.5/autopack/cli.py` & `autopack_tools-0.4.6/autopack/cli.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.5/autopack/filesystem_emulation/file_manager.py` & `autopack_tools-0.4.6/autopack/filesystem_emulation/file_manager.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,21 +15,33 @@
         self.config = config or PackConfig.global_config()
 
     @abstractmethod
     def read_file(self, file_path: str) -> str:
         pass
 
     @abstractmethod
+    def aread_file(self, file_path: str) -> str:
+        pass
+
+    @abstractmethod
     def write_file(self, file_path: str, content: str) -> str:
         pass
 
     @abstractmethod
     async def awrite_file(self, file_path: str, content: str) -> str:
         pass
 
     @abstractmethod
     def delete_file(self, file_path: str) -> str:
         pass
 
     @abstractmethod
+    def adelete_file(self, file_path: str) -> str:
+        pass
+
+    @abstractmethod
     def list_files(self, dir_path: str) -> str:
         pass
+
+    @abstractmethod
+    def alist_files(self, dir_path: str) -> str:
+        pass
```

### Comparing `autopack_tools-0.4.5/autopack/filesystem_emulation/filesystem_file_manager.py` & `autopack_tools-0.4.6/autopack/filesystem_emulation/filesystem_file_manager.py`

 * *Files 27% similar despite different names*

```diff
@@ -27,14 +27,30 @@
         absolute_path = Path(file_path)
         if absolute_path.exists():
             with open(absolute_path, "r") as file:
                 return file.read()
         else:
             return "Error: File not found"
 
+    async def aread_file(self, file_path: str) -> str:
+        """Reads a file from the local file system asynchronously.
+
+        Args:
+            file_path (str): The absolute path to the file to be read.
+
+        Returns:
+            str: The content of the file. If the file does not exist, returns an error message.
+        """
+        absolute_path = Path(file_path)
+        if absolute_path.exists():
+            async with aiofiles.open(absolute_path, mode="r") as file:
+                return await file.read()
+        else:
+            return "Error: File not found"
+
     def write_file(self, file_path: str, content: str) -> str:
         """Writes to a file on the local file system.
 
         Args:
             file_path (str): The absolute path to the file to be written to.
             content (str): The content to be written to the file.
 
@@ -79,22 +95,54 @@
         absolute_path = Path(file_path)
         if absolute_path.exists():
             os.remove(absolute_path)
             return f"Successfully deleted file {file_path}."
         else:
             return f"Error: File not found '{file_path}'"
 
+    async def adelete_file(self, file_path: str) -> str:
+        """Deletes a file from the local file system asynchronously.
+
+        Args:
+            file_path (str): The absolute path to the file to be deleted.
+
+        Returns:
+            str: A success message indicating the file was deleted. If the file does not exist, returns an error message.
+        """
+        absolute_path = Path(file_path)
+        if absolute_path.exists():
+            os.remove(absolute_path)
+            return f"Successfully deleted file {file_path}."
+        else:
+            return f"Error: File not found '{file_path}'"
+
     def list_files(self, dir_path: str) -> str:
         """Lists all files in the specified directory on the local file system.
 
         Args:
             dir_path (str): The absolute path to the directory to list files from.
 
         Returns:
             str: A list of all files in the directory. If the directory does not exist, returns an error message.
         """
+        absolute_dir_path = Path(dir_path)
+        if absolute_dir_path.exists() and absolute_dir_path.is_dir():
+            files_in_dir = absolute_dir_path.glob("*")
+            return "\n".join(str(file) for file in files_in_dir if file not in self.IGNORE_FILES)
+        else:
+            return f"Error: No such directory {dir_path}."
+
+    async def alist_files(self, dir_path: str) -> str:
+        """Lists all files in the specified directory on the local file system asynchronously.
+
+        Args:
+            dir_path (str): The absolute path to the directory to list files from.
+
+        Returns:
+            str: A list of all files in the directory. If the directory does not exist, returns an error message.
+        """
         absolute_dir_path = Path(dir_path)
         if absolute_dir_path.exists() and absolute_dir_path.is_dir():
             files_in_dir = absolute_dir_path.glob("*")
             return "\n".join(str(file) for file in files_in_dir if file not in self.IGNORE_FILES)
         else:
             return f"Error: No such directory {dir_path}."
```

### Comparing `autopack_tools-0.4.5/autopack/filesystem_emulation/ram_file_manager.py` & `autopack_tools-0.4.6/autopack/filesystem_emulation/ram_file_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,17 @@
             str: The content of the file. If the file does not exist, returns an error message.
         """
         if file_path in self.files:
             return self.files[file_path]
         else:
             return "Error: File not found"
 
+    async def aread_file(self, file_path: str) -> str:
+        return self.read_file(file_path)
+
     def write_file(self, file_path: str, content: str) -> str:
         """Writes to a file in the virtual file system in RAM.
 
         Args:
             file_path (str): The path to the file to be written to.
             content (str): The content to be written to the file.
 
@@ -53,14 +56,17 @@
         """
         if file_path in self.files:
             del self.files[file_path]
             return f"Successfully deleted file {file_path}."
         else:
             return f"Error: File not found '{file_path}'"
 
+    async def adelete_file(self, file_path: str) -> str:
+        return self.delete_file(file_path)
+
     def list_files(self, dir_path: str) -> str:
         """Lists all files in the specified directory in the virtual file system in RAM.
 
         Args:
             dir_path (str): The path to the directory to list files from.
 
         Returns:
@@ -73,7 +79,10 @@
             for file_path in self.files.keys()
             if file_path.startswith(dir_path) and file_path not in self.IGNORE_FILES
         ]
         if files_in_dir:
             return "\n".join(files_in_dir)
         else:
             return f"Error: No such directory {dir_path}."
+
+    def alist_files(self, dir_path: str) -> str:
+        return self.list_files(dir_path)
```

### Comparing `autopack_tools-0.4.5/autopack/filesystem_emulation/workspace_file_manager.py` & `autopack_tools-0.4.6/autopack/filesystem_emulation/workspace_file_manager.py`

 * *Files 22% similar despite different names*

```diff
@@ -31,14 +31,30 @@
         absolute_path = self.workspace_dir / file_path
         if absolute_path.exists():
             with open(absolute_path, "r") as file:
                 return file.read()
         else:
             return "Error: File not found"
 
+    async def aread_file(self, file_path: str) -> str:
+        """Reads a file from the workspace directory on the local file system asynchronously.
+
+        Args:
+            file_path (str): The path to the file to be read, relative to the workspace directory.
+
+        Returns:
+            str: The content of the file. If the file does not exist, returns an error message.
+        """
+        absolute_path = self.workspace_dir / file_path
+        if absolute_path.exists():
+            async with aiofiles.open(absolute_path, mode="r") as file:
+                return await file.read()
+        else:
+            return "Error: File not found"
+
     def write_file(self, file_path: str, content: str) -> str:
         """Writes to a file in the workspace directory on the local file system.
 
         Args:
             file_path (str): The path to the file to be written to, relative to the workspace directory.
             content (str): The content to be written to the file.
 
@@ -83,22 +99,54 @@
         absolute_path = self.workspace_dir / file_path
         if absolute_path.exists():
             os.remove(absolute_path)
             return f"Successfully deleted file {file_path}."
         else:
             return f"Error: File not found '{file_path}'"
 
+    async def adelete_file(self, file_path: str) -> str:
+        """Deletes a file from the workspace directory on the local file system asynchronously.
+
+        Args:
+            file_path (str): The path to the file to be deleted, relative to the workspace directory.
+
+        Returns:
+            str: A success message indicating the file was deleted. If the file does not exist, returns an error message.
+        """
+        absolute_path = self.workspace_dir / file_path
+        if absolute_path.exists():
+            os.remove(absolute_path)
+            return f"Successfully deleted file {file_path}."
+        else:
+            return f"Error: File not found '{file_path}'"
+
     def list_files(self, dir_path: str) -> str:
         """Lists all files in the specified directory in the workspace directory on the local file system.
 
         Args:
             dir_path (str): The path to the directory to list files from, relative to the workspace directory.
 
         Returns:
             str: A list of all files in the directory. If the directory does not exist, returns an error message.
         """
+        absolute_dir_path = self.workspace_dir / dir_path
+        if absolute_dir_path.exists() and absolute_dir_path.is_dir():
+            files_in_dir = absolute_dir_path.glob("*")
+            return "\n".join(str(file) for file in files_in_dir if file not in self.IGNORE_FILES)
+        else:
+            return f"Error: No such directory {dir_path}."
+
+    async def alist_files(self, dir_path: str) -> str:
+        """Lists all files in the specified directory in the workspace directory on the local file system asynchronously.
+
+        Args:
+            dir_path (str): The path to the directory to list files from, relative to the workspace directory.
+
+        Returns:
+            str: A list of all files in the directory. If the directory does not exist, returns an error message.
+        """
         absolute_dir_path = self.workspace_dir / dir_path
         if absolute_dir_path.exists() and absolute_dir_path.is_dir():
             files_in_dir = absolute_dir_path.glob("*")
             return "\n".join(str(file) for file in files_in_dir if file not in self.IGNORE_FILES)
         else:
             return f"Error: No such directory {dir_path}."
```

### Comparing `autopack_tools-0.4.5/autopack/get_pack.py` & `autopack_tools-0.4.6/autopack/get_pack.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.5/autopack/installation.py` & `autopack_tools-0.4.6/autopack/installation.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.5/autopack/langchain_wrapper.py` & `autopack_tools-0.4.6/autopack/langchain_wrapper.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.5/autopack/pack.py` & `autopack_tools-0.4.6/autopack/pack.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.5/autopack/pack_config.py` & `autopack_tools-0.4.6/autopack/pack_config.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.5/autopack/prompts.py` & `autopack_tools-0.4.6/autopack/prompts.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.5/autopack/selection.py` & `autopack_tools-0.4.6/autopack/selection.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.5/autopack/utils.py` & `autopack_tools-0.4.6/autopack/utils.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.5/pyproject.toml` & `autopack_tools-0.4.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autopack-tools"
-version = "0.4.5"
+version = "0.4.6"
 repository = "https://github.com/AutoPackAI/autopack"
 homepage = "https://autopack.ai"
 description = "Package Manager for AI Agent tools"
 authors = ["Erik Peterson <e@eriklp.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "autopack" }]
```

### Comparing `autopack_tools-0.4.5/PKG-INFO` & `autopack_tools-0.4.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopack-tools
-Version: 0.4.5
+Version: 0.4.6
 Summary: Package Manager for AI Agent tools
 Home-page: https://autopack.ai
 License: MIT
 Author: Erik Peterson
 Author-email: e@eriklp.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

