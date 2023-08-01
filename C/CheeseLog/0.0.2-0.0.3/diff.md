# Comparing `tmp/CheeseLog-0.0.2.tar.gz` & `tmp/CheeseLog-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CheeseLog-0.0.2.tar", last modified: Thu Jul 27 15:16:30 2023, max compression
+gzip compressed data, was "CheeseLog-0.0.3.tar", last modified: Tue Aug  1 07:20:28 2023, max compression
```

## Comparing `CheeseLog-0.0.2.tar` & `CheeseLog-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-07-27 15:16:30.767676 CheeseLog-0.0.2/
-drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-07-27 15:16:30.766614 CheeseLog-0.0.2/CheeseLog/
--rw-r--r--   0 cheese     (501) staff       (20)     6173 2023-07-27 15:06:08.000000 CheeseLog-0.0.2/CheeseLog/__init__.py
-drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-07-27 15:16:30.767347 CheeseLog-0.0.2/CheeseLog.egg-info/
--rw-r--r--   0 cheese     (501) staff       (20)     3452 2023-07-27 15:16:30.000000 CheeseLog-0.0.2/CheeseLog.egg-info/PKG-INFO
--rw-r--r--   0 cheese     (501) staff       (20)      212 2023-07-27 15:16:30.000000 CheeseLog-0.0.2/CheeseLog.egg-info/SOURCES.txt
--rw-r--r--   0 cheese     (501) staff       (20)        1 2023-07-27 15:16:30.000000 CheeseLog-0.0.2/CheeseLog.egg-info/dependency_links.txt
--rw-r--r--   0 cheese     (501) staff       (20)       11 2023-07-27 15:16:30.000000 CheeseLog-0.0.2/CheeseLog.egg-info/requires.txt
--rw-r--r--   0 cheese     (501) staff       (20)       10 2023-07-27 15:16:30.000000 CheeseLog-0.0.2/CheeseLog.egg-info/top_level.txt
--rw-r--r--   0 cheese     (501) staff       (20)     1070 2023-07-26 07:27:31.000000 CheeseLog-0.0.2/LICENSE
--rw-r--r--   0 cheese     (501) staff       (20)     3452 2023-07-27 15:16:30.767550 CheeseLog-0.0.2/PKG-INFO
--rw-r--r--   0 cheese     (501) staff       (20)     2947 2023-07-26 09:44:29.000000 CheeseLog-0.0.2/README.md
--rw-r--r--   0 cheese     (501) staff       (20)       38 2023-07-27 15:16:30.767753 CheeseLog-0.0.2/setup.cfg
--rw-r--r--   0 cheese     (501) staff       (20)      829 2023-07-27 15:16:22.000000 CheeseLog-0.0.2/setup.py
+drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-08-01 07:20:28.143888 CheeseLog-0.0.3/
+drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-08-01 07:20:28.142709 CheeseLog-0.0.3/CheeseLog/
+-rw-r--r--   0 cheese     (501) staff       (20)     4922 2023-07-31 15:40:57.000000 CheeseLog-0.0.3/CheeseLog/__init__.py
+drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-08-01 07:20:28.143399 CheeseLog-0.0.3/CheeseLog.egg-info/
+-rw-r--r--   0 cheese     (501) staff       (20)     3452 2023-08-01 07:20:28.000000 CheeseLog-0.0.3/CheeseLog.egg-info/PKG-INFO
+-rw-r--r--   0 cheese     (501) staff       (20)      212 2023-08-01 07:20:28.000000 CheeseLog-0.0.3/CheeseLog.egg-info/SOURCES.txt
+-rw-r--r--   0 cheese     (501) staff       (20)        1 2023-08-01 07:20:28.000000 CheeseLog-0.0.3/CheeseLog.egg-info/dependency_links.txt
+-rw-r--r--   0 cheese     (501) staff       (20)       11 2023-08-01 07:20:28.000000 CheeseLog-0.0.3/CheeseLog.egg-info/requires.txt
+-rw-r--r--   0 cheese     (501) staff       (20)       10 2023-08-01 07:20:28.000000 CheeseLog-0.0.3/CheeseLog.egg-info/top_level.txt
+-rw-r--r--   0 cheese     (501) staff       (20)     1070 2023-07-26 07:27:31.000000 CheeseLog-0.0.3/LICENSE
+-rw-r--r--   0 cheese     (501) staff       (20)     3452 2023-08-01 07:20:28.143675 CheeseLog-0.0.3/PKG-INFO
+-rw-r--r--   0 cheese     (501) staff       (20)     2947 2023-07-26 09:44:29.000000 CheeseLog-0.0.3/README.md
+-rw-r--r--   0 cheese     (501) staff       (20)       38 2023-08-01 07:20:28.143939 CheeseLog-0.0.3/setup.cfg
+-rw-r--r--   0 cheese     (501) staff       (20)      829 2023-08-01 07:20:01.000000 CheeseLog-0.0.3/setup.py
```

### Comparing `CheeseLog-0.0.2/CheeseLog/__init__.py` & `CheeseLog-0.0.3/CheeseLog/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,84 +1,69 @@
-import os, sys, threading, queue, datetime, re
-from typing import Optional
+import os, sys, threading, queue, datetime
+from typing import Optional, Set
 
-sys.path.append(os.path.dirname(os.path.dirname(os.path.realpath(__file__))))
+sys.path.append(os.path.dirname(os.path.realpath(__file__)))
 
 from CheeseType import NonNegativeInt
 
 class Level:
-    def __init__(self, weight: NonNegativeInt, color: Optional[str] = None, messageTemplate: Optional[str] = None, timerTemplate: Optional[str] = None):
+    def __init__(self, weight: NonNegativeInt, color: Optional[str] = None, messageTemplate: Optional[str] = None):
         '''
-        ## Args
+        ### Args
 
         - weight：权重。小于日志过滤权重的消息会被忽略。
 
         - color：控制台打印的等级标签样式。
 
         - messageTemplate：消息格式，默认为`logger.messageTemplate`。
-
-        - timerTemplate：日期格式，默认为`logger.timerTemplate`。
         '''
 
         self.weight: NonNegativeInt = weight
         self.color: Optional[str] = color
         self.messageTemplate: Optional[str] = messageTemplate
-        self.timerTemplate: Optional[str] = timerTemplate
 
 class Logger(threading.Thread):
     def __init__(self):
         self.filePath: Optional[str] = None
-        self.messageTemplate: str = '(%level) %timer > %content'
-        self.timerTemplate: str = '%Y-%m-%d %H:%M:%S.%f'
-        self.filter: NonNegativeInt | set[str] = {}
+        self.messageTemplate: str = '(%level) %Y-%m-%d %H:%M:%S.%f > %content'
+        self.filter: NonNegativeInt | Set[str] = set()
         self.levels: dict[str, Level] = {
-            'DEBUG': Level(10, '34', None, None),
-            'INFO': Level(20, '32', None, None),
-            'STARTING': Level(20, '32', None, None),
-            'ENDING': Level(20, '34', None, None),
-            'HTTP': Level(20, None, None, None),
-            'WEBSOCKET': Level(20, None, None, None),
-            'WARNING': Level(30, '33', None, None),
-            'DANGER': Level(40, '31', None, None),
-            'ERROR': Level(50, '35', None, None)
+            'DEBUG': Level(10, '34', None),
+            'INFO': Level(20, '32', None),
+            'STARTING': Level(20, '32', None),
+            'ENDING': Level(20, '34', None),
+            'HTTP': Level(20, None, None),
+            'WEBSOCKET': Level(20, None, None),
+            'WARNING': Level(30, '33', None),
+            'DANGER': Level(40, '31', None),
+            'ERROR': Level(50, '35', None)
         }
         self.colorful: bool = True
         self._queue: queue.Queue = queue.Queue()
         self._flag: bool = False
 
         super().__init__(daemon = True)
 
     def run(self):
         self._flag = True
         while self._flag or not self._queue.empty():
             level, now, message = self._queue.get()
-
-            message = (logger.levels[level].messageTemplate or logger.messageTemplate).replace('%level', level).replace('%timer', now.strftime(logger.levels[level].timerTemplate or logger.timerTemplate)).replace('%content', message).replace('\n', '\n    ') + '\n'
+            message = now.strftime((self.levels[level].messageTemplate or self.messageTemplate).replace('%level', level).replace('%content', message).replace('\n', '\n    ')) + '\n'
             if self.filePath is not None:
                 os.makedirs(os.path.dirname(self.filePath), exist_ok = True)
                 with open(self.filePath, 'a', encoding = 'utf-8') as f:
                     f.write(message)
-            else:
-                self._flag = False
 
     def stop(self):
         self._flag = False
         self.join()
 
 logger = Logger()
 
-def default(level: str, message: str, colorfulMessage: Optional[str] = None, logger: Optional[Logger] = None):
-    '''
-    ## Args
-
-    - colorfulMessage: 不满足于自动的色彩填充，可以选择自定义的控制台内容。它仅会改变消息内容，对消息等级以及时间的样式不会有影响。
-
-    - logger: 应该不会用到...指定其他的日志实例输出消息。
-    '''
-
+def default(level: str, message: str, colorfulMessage: Optional[str] = None, logger: Optional[Logger] = logger):
     ''' Validate '''
     if level not in logger.levels:
         raise KeyError('no level with this key')
 
     ''' Filter '''
     if isinstance(logger.filter, set):
         for _level in logger.filter:
@@ -86,22 +71,20 @@
                 return
     elif logger.levels[level].weight <= NonNegativeInt(logger.filter):
         return
 
     ''' Terminal '''
     now = datetime.datetime.now()
     message = f'{message}'
-    if logger.colorful:
-        if colorfulMessage is None:
-            terminalMessage = (logger.levels[level].messageTemplate or logger.messageTemplate).replace('%level', f'\033[{logger.levels[level].color}m{level}\033[0m' if logger.levels[level].color else level).replace('%timer', f'\033[2m{now.strftime(logger.levels[level].timerTemplate or logger.timerTemplate)}\033[0m').replace('%content', message).replace('\n', '\n    ')
+    if sys.stdout.isatty():
+        if logger.colorful:
+            terminalMessage = now.strftime((logger.levels[level].messageTemplate or logger.messageTemplate).replace('%level', f'\033[{logger.levels[level].color}m{level}\033[0m' if logger.levels[level].color else level).replace('%content', colorfulMessage or message).replace('\n', '\n    '))
         else:
-            terminalMessage = (logger.levels[level].messageTemplate or logger.messageTemplate).replace('%level', f'\033[{logger.levels[level].color}m{level}\033[0m' if logger.levels[level].color else level).replace('%timer', f'\033[2m{now.strftime(logger.levels[level].timerTemplate or logger.timerTemplate)}\033[0m').replace('%content', colorfulMessage).replace('\n', '\n    ')
-    else:
-        terminalMessage = (logger.levels[level].messageTemplate or logger.messageTemplate).replace('%level', level).replace('%timer', now.strftime(logger.levels[level].timerTemplate or logger.timerTemplate)).replace('%content', message).replace('\n', '\n    ')
-    print(terminalMessage)
+            terminalMessage = now.strftime((logger.levels[level].messageTemplate or logger.messageTemplate).replace('%level', level).replace('%content', message).replace('\n', '\n    '))
+        print(terminalMessage)
 
     ''' Log file writter '''
     if logger.filePath is not None:
         if not logger.is_alive():
             logger.start()
         logger._queue.put((level, now, message))
```

### Comparing `CheeseLog-0.0.2/CheeseLog.egg-info/PKG-INFO` & `CheeseLog-0.0.3/CheeseLog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CheeseLog
-Version: 0.0.2
+Version: 0.0.3
 Summary: 日志系统。可在控制台输出一定格式的、可选颜色的内容，并支持写入指定的日志文件。
 Home-page: https://github.com/CheeseUnknown/CheeseLog
 Author: Cheese Unknown
 Author-email: cheese@cheese.ren
 License: MIT
 Keywords: log
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `CheeseLog-0.0.2/LICENSE` & `CheeseLog-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `CheeseLog-0.0.2/PKG-INFO` & `CheeseLog-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CheeseLog
-Version: 0.0.2
+Version: 0.0.3
 Summary: 日志系统。可在控制台输出一定格式的、可选颜色的内容，并支持写入指定的日志文件。
 Home-page: https://github.com/CheeseUnknown/CheeseLog
 Author: Cheese Unknown
 Author-email: cheese@cheese.ren
 License: MIT
 Keywords: log
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `CheeseLog-0.0.2/README.md` & `CheeseLog-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `CheeseLog-0.0.2/setup.py` & `CheeseLog-0.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('./README.md', 'r', encoding = 'utf-8') as f:
     longDescription = f.read()
 
 setuptools.setup(
     name = 'CheeseLog',
-    version = '0.0.2',
+    version = '0.0.3',
     author = 'Cheese Unknown',
     author_email = 'cheese@cheese.ren',
     description = '日志系统。可在控制台输出一定格式的、可选颜色的内容，并支持写入指定的日志文件。',
     long_description = longDescription,
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/CheeseUnknown/CheeseLog',
     license = 'MIT',
```

