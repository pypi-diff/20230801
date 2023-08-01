# Comparing `tmp/logbt-0.2.0.tar.gz` & `tmp/logbt-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logbt-0.2.0.tar", max compression
+gzip compressed data, was "logbt-0.3.0.tar", max compression
```

## Comparing `logbt-0.2.0.tar` & `logbt-0.3.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      317 2023-06-20 17:52:55.693151 logbt-0.2.0/README.md
--rw-r--r--   0        0        0     1368 2023-06-20 17:52:22.316515 logbt-0.2.0/logbt/__init__.py
--rw-r--r--   0        0        0      276 2023-06-20 17:52:33.088720 logbt-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      928 1970-01-01 00:00:00.000000 logbt-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      539 2023-08-01 11:47:14.707983 logbt-0.3.0/README.md
+-rw-r--r--   0        0        0     1828 2023-08-01 11:47:05.191974 logbt-0.3.0/logbt/__init__.py
+-rw-r--r--   0        0        0      276 2023-08-01 11:47:44.920009 logbt-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1150 1970-01-01 00:00:00.000000 logbt-0.3.0/PKG-INFO
```

### Comparing `logbt-0.2.0/logbt/__init__.py` & `logbt-0.3.0/logbt/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import logging
 import sys
 import zlib
-from pprint import pprint
 
 import loguru
 
 RESET = "\x1b[0m"
 FORMATS = {
     logging.DEBUG: "\u001b[38;5;247m",
     logging.WARNING: "\u001b[38;5;11m",
@@ -38,36 +37,57 @@
     192,
     201,
     210,
 ]
 
 
 def random_color(text: str) -> str:
-    color = (
-        "\u001b[38;5;" + str(COLORS[zlib.adler32(text.encode()) % len(COLORS)]) + "m"
+    """
+    Gets random color based on text hash
+    """
+    color = "".join(
+        [
+            "\u001b[38;5;",
+            str(COLORS[zlib.adler32(text.encode()) % len(COLORS)]),
+            "m",
+        ]
     )
     return f"{color}{text}{RESET}"
 
 
 def colorize(record):
     record["level"].name = f'[{record["level"].name}]'.ljust(10)
     record["module"] = random_color(f'[{record["module"]}]'.ljust(15))
     record["function"] = f'[{record["function"]}]'.ljust(10)
 
 
-def config(level="INFO"):
-    splitter = " " * 3
+def config(level="INFO", splitter=" "):
+    splitter *= 3
     logger.add(
         sys.stdout,
         colorize=True,
         level=level,
         format="SPLITTER[{time:YYYY-MM-DD HH:mm:ss}]"
         "SPLITTER<level>{level}</level>"
         "SPLITTER{module}"
         "SPLITTER{function}"
         "SPLITTER{message} :: ({file}:{line})".replace("SPLITTER", splitter),
     )
 
 
+class InjectLoguruHandler(logging.Handler):
+    def emit(self, record: logging.LogRecord) -> None:
+        logger.log(record.levelname, self.format(record))
+
+
+def inject_loguru_to_logging(
+    name: str,
+):
+    handler = InjectLoguruHandler()
+    handler.setLevel(logging.NOTSET)
+    logging_logger = logging.getLogger(name)
+    logging_logger.addHandler(handler)
+
+
 logger = loguru.logger
 logger.remove()
 logger = logger.patch(colorize)
```

