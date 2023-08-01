# Comparing `tmp/shshsh-1.0.0.tar.gz` & `tmp/shshsh-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shshsh-1.0.0.tar", max compression
+gzip compressed data, was "shshsh-1.0.1.tar", max compression
```

## Comparing `shshsh-1.0.0.tar` & `shshsh-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1387 2023-07-30 08:02:23.520980 shshsh-1.0.0/README.md
--rw-r--r--   0        0        0      345 2023-07-30 08:09:30.351000 shshsh-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      162 2023-07-29 10:25:39.320698 shshsh-1.0.0/shshsh/__init__.py
--rw-r--r--   0        0        0      449 2023-07-29 15:04:40.678142 shshsh-1.0.0/shshsh/pipe.py
--rw-r--r--   0        0        0     2303 2023-07-30 07:16:32.510852 shshsh-1.0.0/shshsh/quick.py
--rw-r--r--   0        0        0    13265 2023-07-30 07:25:13.704210 shshsh-1.0.0/shshsh/shell.py
--rw-r--r--   0        0        0     5631 2023-07-30 07:23:09.174204 shshsh-1.0.0/shshsh/streamer.py
--rw-r--r--   0        0        0      411 2023-07-29 10:26:49.430701 shshsh-1.0.0/shshsh/utils.py
--rw-r--r--   0        0        0     1795 1970-01-01 00:00:00.000000 shshsh-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1657 2023-08-01 18:09:47.654031 shshsh-1.0.1/README.md
+-rw-r--r--   0        0        0      345 2023-08-01 18:05:36.107353 shshsh-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      176 2023-08-01 18:14:56.490713 shshsh-1.0.1/shshsh/__init__.py
+-rw-r--r--   0        0        0       52 2023-08-01 19:00:12.394172 shshsh-1.0.1/shshsh/global_vars.py
+-rw-r--r--   0        0        0      449 2023-07-29 15:04:40.678142 shshsh-1.0.1/shshsh/pipe.py
+-rw-r--r--   0        0        0     2656 2023-08-01 19:05:37.427520 shshsh-1.0.1/shshsh/quick.py
+-rw-r--r--   0        0        0    14782 2023-08-01 19:26:56.044246 shshsh-1.0.1/shshsh/shell.py
+-rw-r--r--   0        0        0     5748 2023-08-01 19:06:50.924190 shshsh-1.0.1/shshsh/streamer.py
+-rw-r--r--   0        0        0      934 2023-08-01 19:23:06.874235 shshsh-1.0.1/shshsh/utils.py
+-rw-r--r--   0        0        0     2115 1970-01-01 00:00:00.000000 shshsh-1.0.1/PKG-INFO
```

### Comparing `shshsh-1.0.0/README.md` & `shshsh-1.0.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,59 @@
 # shshsh 🐍❤️🐚
+[![PyPI](https://img.shields.io/badge/python-3.9%7C3.10%7C3.11-blue.svg)](https://pypi.org/project/shshsh/)
+
 Shshsh is a bridge connects python and shell.
 - A simple way to write shell in python.
 - Flexable.
 - Support directly chain a python function in pipe.
 
 ## Installation
 To install shshsh with pip, run: `pip install shshsh`
 
 To install shshsh with conda, run: `conda install shshsh -c conda-forge`
 
 To install shshsh from source, clone the repository and run: `pip install poetry;poetry install`
 
+⚠️ **If you are using python3.8**: Be very careful with python function Pipe, there are known bugs!
+
 ## Basic Usage
-You can use `I >> "[command]"` or `Sh("[command]")`in any Python object.
+You can use `I >> "[command]"` or `Sh("[command]")`in any Python project.
 
-Here's an example of get all file which name contains "test":
+Here's an example of getting all file which name contains "test":
 ```python
 from shshsh import I
 
 for filename in I >> "ls" | "grep test":
     print(filename)
 
 ```
 Also, you can safely pass parameter without command injection, shshsh will help you escape all bash control character:
 ```python
 from shshsh import I
 from sys import stdout
 
-(I >> "echo #{}") % "dangerous; cat /etc/passwd" | stdout
+res = (I >> "echo #{}") % "dangerous; cat /etc/passwd" | stdout
+res.wait()
 # dangerous; cat /etc/passwd
 
 ```
 Python function or iterable can be part of chain, you no longer have to search Google (or chatgpt) repeatedly to write sed or awk😇:
 ```python
 from shshsh import I
 from sys import stdout
 
 # as map function
 def add_suffix(line: str) -> str:
     return line + ".py"
 
-I >> "ls -alh" | add_suffix | "grep test" | stdout
+res = I >> "ls -alh" | add_suffix | "grep test" | stdout
+res.wait()
 
 # as data source
 def data_source():
     for i in range(10):
         yield f"test{i}"
 
-I >> data_source() | "grep test1" | stdout
+res = I >> data_source() | "grep test1" | stdout
+res.wait()
 
 ```
```

### Comparing `shshsh-1.0.0/shshsh/quick.py` & `shshsh-1.0.1/shshsh/quick.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Optional, List, IO, Union, overload, Iterable, Generator, Any
 import io
 import subprocess
+from . import global_vars
 from .pipe import Pipe
 from .streamer import P
 from .shell import Sh
 
 
 class _I:
     def __init__(
@@ -27,29 +28,43 @@
     def __rshift__(self, other: Pipe) -> "_I":
         ...
 
     @overload
     def __rshift__(self, other: IO[bytes]) -> "_I":
         ...
 
+    @overload
+    def __rshift__(self, other: Generator[str, Any, None]) -> "P":
+        ...
+
+    @overload
+    def __rshift__(self, other: Generator[bytes, Any, None]) -> "P":
+        ...
+
     def __rshift__(
         self,
         other: Union[
             str,
             int,
             Pipe,
             IO[bytes],
             Iterable[str],
             Iterable[bytes],
             Generator[str, Any, None],
             Generator[bytes, Any, None],
         ],
     ):
         if isinstance(other, str):
-            return Sh(other, pass_fds=self.with_fds or (), stdin=self.with_stdin)
+            return Sh(
+                other,
+                pass_fds=self.with_fds or (),
+                stdin=self.with_stdin,
+                cwd=global_vars.CWD,
+                env=global_vars.ENV,
+            )
         elif isinstance(other, int):
             if self.with_fds:
                 return _I(with_stdin=other, with_fds=[*self.with_fds, other])
             else:
                 return _I(with_stdin=other)
         elif isinstance(other, io.IOBase):
             if self.with_fds:
```

### Comparing `shshsh-1.0.0/shshsh/shell.py` & `shshsh-1.0.1/shshsh/shell.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import shlex
 from threading import Thread
 from .streamer import str_streamer, bytes_streamer, P
 import io
 import sys
 import copy
 import re
+from . import global_vars
 from typing import (
     IO,
     Iterable,
     List,
     Generator,
     overload,
     Type,
@@ -33,14 +34,15 @@
 
     def __str__(self) -> str:
         return f"Symbol[{self._name}]"
 
 
 stdout = sys.stdout
 stderr = sys.stderr
+keep = subprocess.PIPE
 fork_stream = Symbol("fork_stream")
 
 _STD = Optional[Union[IO[bytes], int]]
 
 
 class Sh:
     @staticmethod
@@ -150,22 +152,26 @@
                 param_complete = False
         return param_complete, cmd_list
 
     def __init__(
         self,
         cmd: str,
         arg_placeholder: str = "#{*}",
-        stdin: _STD = None,
-        stdout: _STD = subprocess.PIPE,
-        stderr: _STD = subprocess.PIPE,
+        stdin: Union[_STD, TextIO] = None,
+        stdout: Union[_STD, TextIO] = subprocess.PIPE,
+        stderr: Union[_STD, TextIO] = stderr,
         pass_fds: Collection[int] = (),
         callback: Optional[Callable[..., Any]] = None,
+        env: Optional[Dict[str, str]] = None,
+        cwd: Optional[str] = None,
         *args: Any,
         **kwargs: Any,
     ) -> None:
+        self._env = copy.copy(env) or global_vars.ENV
+        self._cwd = cwd or global_vars.CWD
         self._proc = None
         self._stdin = stdin
         self._stdout = stdout
         self._stderr = stderr
         self.pass_fds = pass_fds
         assert self._if_placeholder_valid(
             arg_placeholder
@@ -182,40 +188,58 @@
         )
 
     def set_stdin(self, stdin: Union[int, IO[bytes]]):
         assert not self._proc, "is running, cannot set stdin"
         self._stdin = stdin
 
     @property
+    def stdout_readable(self):
+        assert self._proc, "process not start yet"
+        return bool(self._proc.stdout)
+
+    @property
+    def stderr_readable(self):
+        assert self._proc, "process not start yet"
+        return bool(self._proc.stderr)
+
+    @property
     def stdout(self):
         if self._proc is None:
+            self._stdout = subprocess.PIPE
             self.run()
         assert self._proc
-        assert self._proc.stdout
+        assert (
+            self._proc.stdout
+        ), f"cannot get stdout, current stdout is redirect to {self._stdout}"
         return self._proc.stdout
 
     @property
     def stderr(self):
         if self._proc is None:
+            self._stderr = subprocess.PIPE
             self.run()
         assert self._proc
-        assert self._proc.stderr
+        assert (
+            self._proc.stderr
+        ), f"cannot get stderr, current stderr is redirect to {self._stderr}"
         return self._proc.stderr
 
     def run(self):
         assert (
             not self._proc
         ), f"cannot run twice, command {self.cmd} already run, place create a new Sh"
         if self.param_complete:
             self._proc = subprocess.Popen(
                 self.cmd,
                 stdin=self._stdin,
                 stderr=self._stderr,
-                stdout=self._stdout,
+                stdout=self._stdout,  # type: ignore
                 pass_fds=self.pass_fds,
+                cwd=self._cwd,
+                env=self._env,
             )
 
             # wait done and call callback
             def wait_done():
                 assert self._proc
                 self._proc.wait()
                 assert self.callback
@@ -302,46 +326,50 @@
             str,
             P,
             Callable[[Union[str, bytes]], Union[str, bytes]],
             Iterable[Union[str, bytes]],
         ],
     ) -> Union["Sh", P]:
         if isinstance(other, io.IOBase):
+            self._stdout = other
             if not self._proc:
                 self.run()
-            while True:
-                chunk = self.stdout.read(1024)
-                other.buffer.write(chunk)  # type: ignore
-                if len(chunk) < 1024:
-                    break
-            other.flush()
             return self
         elif isinstance(other, Sh):
             assert other._proc is None, f"cannot pipe after cmd run.({other.cmd})"
             if not self._proc:
                 self.run()
             assert self._proc
+            self._stdout = subprocess.PIPE
             other._stdin = self._proc.stdout
             return other
         elif isinstance(other, P):
+            self._stdout = subprocess.PIPE
             other.set_source(self.stdout)
             return other
         elif isinstance(other, str):
             if not other:
                 return self
             if not self._proc:
+                self._stdout = subprocess.PIPE
                 self.run()
             assert self._proc
             assert self._proc.stdout
-            new_sh = Sh(other, stdin=self.stdout)
+            new_sh = Sh(
+                other, stdin=self.stdout, cwd=global_vars.CWD, env=global_vars.ENV
+            )
             return new_sh
         elif isinstance(other, Callable) or isinstance(other, Iterable):  # type: ignore
             p = P(other)
-            self.run()
-            assert self.stdout
+            if not self._proc:
+                self._stdout = subprocess.PIPE
+                self.run()
+            assert (
+                self.stdout
+            ), f"cannot get stdout and put to {other}, process already running and its stdout is not pipe, is {self._stdout}"
             p.set_source(self.stdout)
             return p
         else:
             raise ValueError(f"chain opt not support {other}")
 
     @overload
     def iter(
@@ -379,42 +407,53 @@
     def __iter__(self) -> Generator[str, Any, None]:
         return self.iter()  # type: ignore
 
     def __and__(self, other: Union["Sh", str]) -> "Sh":
         if self._proc is None:
             self.run()
         self.wait()
-        code = self.code
-        if code == 0:
+        if self.code == 0:
             if isinstance(other, str):
                 if not other:
                     return self
-                res = Sh(other)
-                res.run()
-                return res
+                return Sh(
+                    other,
+                    cwd=global_vars.CWD,
+                    env=global_vars.ENV,
+                )
             elif isinstance(other, Sh):  # type: ignore
-                other.run()
                 return other
         return self
 
-    def __floordiv__(self, other: Union["Sh", str]) -> "Sh":
+    def __gt__(self, other: Union[_STD, TextIO]) -> "Sh":
+        assert not self._proc, "cannot set stdout after run"
+        self._stdout = other
+        return self
+
+    def __ge__(self, other: Union[_STD, TextIO]) -> "Sh":
+        assert not self._proc, "cannot set stdout after run"
+        self._stderr = other
+        return self
+
+    def or_(self, other: Union["Sh", str]) -> "Sh":
         if self._proc is None:
             self.run()
         self.wait()
         code = self.code
         if code != 0:
             if isinstance(other, str):
                 if not other:
                     return self
-                res = Sh(other)
+                res = Sh(
+                    other,
+                    cwd=global_vars.CWD,
+                    env=global_vars.ENV,
+                )
                 res.run()
                 return res
             elif isinstance(other, Sh):  # type: ignore
                 other.run()
                 return other
         return self
 
     def and_(self, other: Union["Sh", str]) -> "Sh":
         return self & other
-
-    def or_(self, other: Union["Sh", str]) -> "Sh":
-        return self // other
```

### Comparing `shshsh-1.0.0/shshsh/streamer.py` & `shshsh-1.0.1/shshsh/streamer.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     Union,
     TypeVar,
     List,
     Optional,
     TYPE_CHECKING,
     overload,
 )
+from . import global_vars
 import io
 import os
 import copy
 from threading import Thread
 import inspect
 
 if TYPE_CHECKING:
@@ -24,15 +25,15 @@
     chunk_data = b""
     while True:
         chunk_data += stream.read(chunk_size)
         chunks = chunk_data.split(sep)
         for chunk in chunks[:-1]:
             yield chunk
         chunk_data = chunks[-1]
-        if len(chunk_data) < chunk_size:
+        if not chunk_data:
             return
 
 
 def str_streamer(stream: IO[bytes], sep: str = "\n", chunk_size: int = 1024):
     for chunk in bytes_streamer(stream, sep=sep.encode("utf8"), chunk_size=chunk_size):
         yield chunk.decode("utf8")
 
@@ -155,21 +156,26 @@
         from .shell import Sh
 
         if not self.t:
             self.run()
         assert self.t
 
         if isinstance(other, str):
-            return Sh(other, stdin=self.out_fd)
+            return Sh(
+                other,
+                stdin=self.out_fd,
+                cwd=global_vars.CWD,
+                env=global_vars.ENV,
+            )
         if isinstance(other, io.IOBase):
             stdout = os.fdopen(self.out_fd, "rb")
             while True:
-                chunk = stdout.read(self._chunk_size)
+                chunk = stdout.readline(self._chunk_size)
                 other.buffer.write(chunk)  # type: ignore
-                if len(chunk) < self._chunk_size:
+                if not chunk:
                     break
             other.flush()
             stdout.close()
         elif isinstance(other, Sh):  # type: ignore
             other = copy.copy(other)
             other.set_stdin(self.out_fd)
             return other
```

### Comparing `shshsh-1.0.0/PKG-INFO` & `shshsh-1.0.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,66 +1,74 @@
 Metadata-Version: 2.1
 Name: shshsh
-Version: 1.0.0
+Version: 1.0.1
 Summary: bridge of python and shell
 Author: zqqqqz2000
 Author-email: zqqqqz2000@sina.cn
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # shshsh 🐍❤️🐚
+[![PyPI](https://img.shields.io/badge/python-3.9%7C3.10%7C3.11-blue.svg)](https://pypi.org/project/shshsh/)
+
 Shshsh is a bridge connects python and shell.
 - A simple way to write shell in python.
 - Flexable.
 - Support directly chain a python function in pipe.
 
 ## Installation
 To install shshsh with pip, run: `pip install shshsh`
 
 To install shshsh with conda, run: `conda install shshsh -c conda-forge`
 
 To install shshsh from source, clone the repository and run: `pip install poetry;poetry install`
 
+⚠️ **If you are using python3.8**: Be very careful with python function Pipe, there are known bugs!
+
 ## Basic Usage
-You can use `I >> "[command]"` or `Sh("[command]")`in any Python object.
+You can use `I >> "[command]"` or `Sh("[command]")`in any Python project.
 
-Here's an example of get all file which name contains "test":
+Here's an example of getting all file which name contains "test":
 ```python
 from shshsh import I
 
 for filename in I >> "ls" | "grep test":
     print(filename)
 
 ```
 Also, you can safely pass parameter without command injection, shshsh will help you escape all bash control character:
 ```python
 from shshsh import I
 from sys import stdout
 
-(I >> "echo #{}") % "dangerous; cat /etc/passwd" | stdout
+res = (I >> "echo #{}") % "dangerous; cat /etc/passwd" | stdout
+res.wait()
 # dangerous; cat /etc/passwd
 
 ```
 Python function or iterable can be part of chain, you no longer have to search Google (or chatgpt) repeatedly to write sed or awk😇:
 ```python
 from shshsh import I
 from sys import stdout
 
 # as map function
 def add_suffix(line: str) -> str:
     return line + ".py"
 
-I >> "ls -alh" | add_suffix | "grep test" | stdout
+res = I >> "ls -alh" | add_suffix | "grep test" | stdout
+res.wait()
 
 # as data source
 def data_source():
     for i in range(10):
         yield f"test{i}"
 
-I >> data_source() | "grep test1" | stdout
+res = I >> data_source() | "grep test1" | stdout
+res.wait()
 
 ```
```

