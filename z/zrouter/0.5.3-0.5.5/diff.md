# Comparing `tmp/zrouter-0.5.3.tar.gz` & `tmp/zrouter-0.5.5.tar.gz`

## Comparing `zrouter-0.5.3.tar` & `zrouter-0.5.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 zrouter-0.5.3/src/zrouter/__init__.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 zrouter-0.5.3/src/zrouter/restful.py
--rw-r--r--   0        0        0     3450 2020-02-02 00:00:00.000000 zrouter-0.5.3/src/zrouter/router.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 zrouter-0.5.3/src/zrouter/exceptions/__init__.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 zrouter-0.5.3/src/zrouter/utils/json.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 zrouter-0.5.3/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zrouter-0.5.3/LICENSE
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 zrouter-0.5.3/README.md
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 zrouter-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 zrouter-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 zrouter-0.5.5/src/zrouter/__init__.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 zrouter-0.5.5/src/zrouter/restful.py
+-rw-r--r--   0        0        0     3648 2020-02-02 00:00:00.000000 zrouter-0.5.5/src/zrouter/router.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 zrouter-0.5.5/src/zrouter/exceptions/__init__.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 zrouter-0.5.5/src/zrouter/utils/json.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 zrouter-0.5.5/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zrouter-0.5.5/LICENSE
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 zrouter-0.5.5/README.md
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 zrouter-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 zrouter-0.5.5/PKG-INFO
```

### Comparing `zrouter-0.5.3/src/zrouter/restful.py` & `zrouter-0.5.5/src/zrouter/restful.py`

 * *Files identical despite different names*

### Comparing `zrouter-0.5.3/src/zrouter/router.py` & `zrouter-0.5.5/src/zrouter/router.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,23 +39,30 @@
     def verify_user(self):
         """用户验证，通过继承覆盖此方法实现具体逻辑"""
         return True
 
     def handle_error(self, e):
         """错误处理，通过继承覆盖此方法实现具体逻辑"""
         pass
-
+    
+    @staticmethod
+    def decorator(func):
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            return func(*args, **kwargs)
+        return wrapper
+    
     def wrap_view_func(self, func, direct=False, open=False):
         @wraps(func)
         def wrapper(*args, **kwargs):
             params = self.clean_params(self.get_params())
             if not self.verify_user() and not open:
                 return {'code': 401, 'msg': '用户无权限'}
             try:
-                data = func(**params)
+                data = self.decorator(func)(**params)
             except MessagePrompt as e:
                 return {'code': 500, 'msg': str(e)}
             except ValidationError as e:
                 return {'code': 400, 'msg': str(e)}
             except Exception as e:
                 self.handle_error(e)
                 raise e
```

### Comparing `zrouter-0.5.3/src/zrouter/utils/json.py` & `zrouter-0.5.5/src/zrouter/utils/json.py`

 * *Files identical despite different names*

### Comparing `zrouter-0.5.3/LICENSE` & `zrouter-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `zrouter-0.5.3/README.md` & `zrouter-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `zrouter-0.5.3/pyproject.toml` & `zrouter-0.5.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "zrouter"
-version = "0.5.3"
+version = "0.5.5"
 authors = [
   { name="inspirare6", email="inspirare6@163.com" },
 ]
 description = "zen router library"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `zrouter-0.5.3/PKG-INFO` & `zrouter-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zrouter
-Version: 0.5.3
+Version: 0.5.5
 Summary: zen router library
 Project-URL: Homepage, https://github.com/inspirare6/zrouter
 Project-URL: Bug Tracker, https://github.com/inspirare6/zrouter/issues
 Author-email: inspirare6 <inspirare6@163.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

