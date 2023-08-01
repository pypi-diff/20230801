# Comparing `tmp/forestadmin_agent_flask-1.0.0b4.tar.gz` & `tmp/forestadmin_agent_flask-1.0.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forestadmin_agent_flask-1.0.0b4.tar", max compression
+gzip compressed data, was "forestadmin_agent_flask-1.0.0b5.tar", max compression
```

## Comparing `forestadmin_agent_flask-1.0.0b4.tar` & `forestadmin_agent_flask-1.0.0b5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-07-31 15:38:20.291049 forestadmin_agent_flask-1.0.0b4/README.md
--rw-r--r--   0        0        0        0 2023-07-31 15:38:20.291049 forestadmin_agent_flask-1.0.0b4/forestadmin/flask_agent/__init__.py
--rw-r--r--   0        0        0     7601 2023-07-31 15:38:20.295050 forestadmin_agent_flask-1.0.0b4/forestadmin/flask_agent/agent.py
--rw-r--r--   0        0        0      125 2023-07-31 15:38:20.295050 forestadmin_agent_flask-1.0.0b4/forestadmin/flask_agent/exception.py
--rw-r--r--   0        0        0        0 2023-07-31 15:38:20.295050 forestadmin_agent_flask-1.0.0b4/forestadmin/flask_agent/utils/__init__.py
--rw-r--r--   0        0        0      581 2023-07-31 15:38:20.295050 forestadmin_agent_flask-1.0.0b4/forestadmin/flask_agent/utils/dispatcher.py
--rw-r--r--   0        0        0     1449 2023-07-31 15:38:20.295050 forestadmin_agent_flask-1.0.0b4/forestadmin/flask_agent/utils/requests.py
--rw-r--r--   0        0        0     1797 2023-07-31 15:38:42.206884 forestadmin_agent_flask-1.0.0b4/pyproject.toml
--rw-r--r--   0        0        0      907 1970-01-01 00:00:00.000000 forestadmin_agent_flask-1.0.0b4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-01 13:28:56.568983 forestadmin_agent_flask-1.0.0b5/README.md
+-rw-r--r--   0        0        0        0 2023-08-01 13:28:56.568983 forestadmin_agent_flask-1.0.0b5/forestadmin/flask_agent/__init__.py
+-rw-r--r--   0        0        0     7620 2023-08-01 13:28:56.568983 forestadmin_agent_flask-1.0.0b5/forestadmin/flask_agent/agent.py
+-rw-r--r--   0        0        0      125 2023-08-01 13:28:56.568983 forestadmin_agent_flask-1.0.0b5/forestadmin/flask_agent/exception.py
+-rw-r--r--   0        0        0        0 2023-08-01 13:28:56.568983 forestadmin_agent_flask-1.0.0b5/forestadmin/flask_agent/utils/__init__.py
+-rw-r--r--   0        0        0      581 2023-08-01 13:28:56.568983 forestadmin_agent_flask-1.0.0b5/forestadmin/flask_agent/utils/dispatcher.py
+-rw-r--r--   0        0        0     1449 2023-08-01 13:28:56.568983 forestadmin_agent_flask-1.0.0b5/forestadmin/flask_agent/utils/requests.py
+-rw-r--r--   0        0        0     1797 2023-08-01 13:29:22.465898 forestadmin_agent_flask-1.0.0b5/pyproject.toml
+-rw-r--r--   0        0        0      907 1970-01-01 00:00:00.000000 forestadmin_agent_flask-1.0.0b5/PKG-INFO
```

### Comparing `forestadmin_agent_flask-1.0.0b4/forestadmin/flask_agent/agent.py` & `forestadmin_agent_flask-1.0.0b5/forestadmin/flask_agent/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
     @blueprint.setter
     def blueprint(self, blueprint: Blueprint):
         self._blueprint = blueprint
 
     def register_blueprint(self, app: Flask):
         self.options["schema_path"] = os.path.join(app.root_path, ".forestadmin-schema.json")
-        app.register_blueprint(self.blueprint, url_prefix="/forest")
+        app.register_blueprint(self.blueprint, url_prefix=f'/{self.options["prefix"]}')
         self.loop.run_until_complete(self.start())
         ForestLogger.log("info", "Flask agent initialized")
 
 
 def build_agent(options: Options) -> Agent:
     agent = Agent(options)
     agent.blueprint = build_blueprint(agent)
```

### Comparing `forestadmin_agent_flask-1.0.0b4/forestadmin/flask_agent/utils/dispatcher.py` & `forestadmin_agent_flask-1.0.0b5/forestadmin/flask_agent/utils/dispatcher.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_flask-1.0.0b4/forestadmin/flask_agent/utils/requests.py` & `forestadmin_agent_flask-1.0.0b5/forestadmin/flask_agent/utils/requests.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_flask-1.0.0b4/pyproject.toml` & `forestadmin_agent_flask-1.0.0b5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "forestadmin-agent-flask"
-version = "1.0.0-beta.4"
+version = "1.0.0-beta.5"
 description = ""
 authors = [ "Valentin Monté <valentinm@forestadmin.com>",]
 readme = "README.md"
 [[tool.poetry.packages]]
 include = "forestadmin"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
 typing-extensions = "~=4.2"
 tzdata = "~=2022.6"
-forestadmin-agent-toolkit = "^1.0.0-beta.4"
-forestadmin-datasource-toolkit = "^1.0.0-beta.4"
+forestadmin-agent-toolkit = "^1.0.0-beta.5"
+forestadmin-datasource-toolkit = "^1.0.0-beta.5"
 Flask-Cors = "^3.0.8"
 
 [tool.poetry.dependencies.flask]
 extras = [ "async",]
 version = "^2.0.0"
 
 [tool.poetry.dependencies."backports.zoneinfo"]
```

### Comparing `forestadmin_agent_flask-1.0.0b4/PKG-INFO` & `forestadmin_agent_flask-1.0.0b5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: forestadmin-agent-flask
-Version: 1.0.0b4
+Version: 1.0.0b5
 Summary: 
 Author: Valentin Monté
 Author-email: valentinm@forestadmin.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Flask-Cors (>=3.0.8,<4.0.0)
 Requires-Dist: backports.zoneinfo[tzdata] (>=0.2.1,<0.3.0) ; python_version < "3.9"
 Requires-Dist: flask[async] (>=2.0.0,<3.0.0)
-Requires-Dist: forestadmin-agent-toolkit (>=1.0.0-beta.4,<2.0.0)
-Requires-Dist: forestadmin-datasource-toolkit (>=1.0.0-beta.4,<2.0.0)
+Requires-Dist: forestadmin-agent-toolkit (>=1.0.0-beta.5,<2.0.0)
+Requires-Dist: forestadmin-datasource-toolkit (>=1.0.0-beta.5,<2.0.0)
 Requires-Dist: typing-extensions (>=4.2,<5.0)
 Requires-Dist: tzdata (>=2022.6,<2023.0)
 Description-Content-Type: text/markdown
```

