# Comparing `tmp/logbt-0.3.0.tar.gz` & `tmp/logbt-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logbt-0.3.0.tar", max compression
+gzip compressed data, was "logbt-0.4.0.tar", max compression
```

## Comparing `logbt-0.3.0.tar` & `logbt-0.4.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      539 2023-08-01 11:47:14.707983 logbt-0.3.0/README.md
--rw-r--r--   0        0        0     1828 2023-08-01 11:47:05.191974 logbt-0.3.0/logbt/__init__.py
--rw-r--r--   0        0        0      276 2023-08-01 11:47:44.920009 logbt-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1150 1970-01-01 00:00:00.000000 logbt-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      539 2023-08-01 11:47:14.707983 logbt-0.4.0/README.md
+-rw-r--r--   0        0        0     2094 2023-08-01 12:10:02.301408 logbt-0.4.0/logbt/__init__.py
+-rw-r--r--   0        0        0      276 2023-08-01 12:10:20.053429 logbt-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1150 1970-01-01 00:00:00.000000 logbt-0.4.0/PKG-INFO
```

### Comparing `logbt-0.3.0/README.md` & `logbt-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `logbt-0.3.0/logbt/__init__.py` & `logbt-0.4.0/logbt/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -56,38 +56,49 @@
 
 def colorize(record):
     record["level"].name = f'[{record["level"].name}]'.ljust(10)
     record["module"] = random_color(f'[{record["module"]}]'.ljust(15))
     record["function"] = f'[{record["function"]}]'.ljust(10)
 
 
-def config(level="INFO", splitter=" "):
+def config(
+    level="INFO",
+    splitter=" ",
+    show_function: bool = False,
+) -> None:
     splitter *= 3
+    format_list = [
+        "SPLITTER[{time:YYYY-MM-DD HH:mm:ss}]",
+        "SPLITTER<level>{level}</level>",
+        "SPLITTER{module}",
+    ]
+    if show_function:
+        format_list.append("SPLITTER{function}")
+    format_list.append("SPLITTER{message} :: ({file}:{line})")
     logger.add(
         sys.stdout,
         colorize=True,
         level=level,
-        format="SPLITTER[{time:YYYY-MM-DD HH:mm:ss}]"
-        "SPLITTER<level>{level}</level>"
-        "SPLITTER{module}"
-        "SPLITTER{function}"
-        "SPLITTER{message} :: ({file}:{line})".replace("SPLITTER", splitter),
+        format="".join(format_list).replace("SPLITTER", splitter),
     )
 
 
 class InjectLoguruHandler(logging.Handler):
     def emit(self, record: logging.LogRecord) -> None:
         logger.log(record.levelname, self.format(record))
 
 
 def inject_loguru_to_logging(
     name: str,
+    remove_handlers: bool = True,
 ):
     handler = InjectLoguruHandler()
     handler.setLevel(logging.NOTSET)
     logging_logger = logging.getLogger(name)
+    if remove_handlers:
+        logging_logger.handlers.clear()
     logging_logger.addHandler(handler)
 
 
 logger = loguru.logger
 logger.remove()
 logger = logger.patch(colorize)
```

### Comparing `logbt-0.3.0/PKG-INFO` & `logbt-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logbt
-Version: 0.3.0
+Version: 0.4.0
 Summary: 
 Author: SmsS4
 Author-email: smss.lite@gmail.com
 Requires-Python: >=3.5
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
```

