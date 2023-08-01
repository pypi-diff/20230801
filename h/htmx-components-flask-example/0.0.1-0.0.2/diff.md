# Comparing `tmp/htmx-components-flask-example-0.0.1.tar.gz` & `tmp/htmx-components-flask-example-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htmx-components-flask-example-0.0.1.tar", last modified: Wed Jul 26 00:13:40 2023, max compression
+gzip compressed data, was "htmx-components-flask-example-0.0.2.tar", last modified: Tue Aug  1 21:47:18 2023, max compression
```

## Comparing `htmx-components-flask-example-0.0.1.tar` & `htmx-components-flask-example-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-07-26 00:13:40.685448 htmx-components-flask-example-0.0.1/
--rw-rw-r--   0 neil      (1000) neil      (1000)       29 2023-07-25 23:05:20.000000 htmx-components-flask-example-0.0.1/.gitignore
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-07-26 00:13:40.673448 htmx-components-flask-example-0.0.1/.vscode/
--rw-rw-r--   0 neil      (1000) neil      (1000)       68 2023-07-25 23:02:53.000000 htmx-components-flask-example-0.0.1/.vscode/settings.json
--rw-rw-r--   0 neil      (1000) neil      (1000)     1070 2023-07-25 22:55:43.000000 htmx-components-flask-example-0.0.1/LICENSE
--rw-rw-r--   0 neil      (1000) neil      (1000)      256 2023-07-26 00:13:40.685448 htmx-components-flask-example-0.0.1/PKG-INFO
--rw-rw-r--   0 neil      (1000) neil      (1000)       31 2023-07-25 22:55:43.000000 htmx-components-flask-example-0.0.1/README.md
--rw-rw-r--   0 neil      (1000) neil      (1000)     2310 2023-07-25 23:51:19.000000 htmx-components-flask-example-0.0.1/app.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     3364 2023-07-25 23:47:06.000000 htmx-components-flask-example-0.0.1/form.py
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-07-26 00:13:40.677448 htmx-components-flask-example-0.0.1/htmx_components_flask_example.egg-info/
--rw-rw-r--   0 neil      (1000) neil      (1000)      256 2023-07-26 00:13:40.000000 htmx-components-flask-example-0.0.1/htmx_components_flask_example.egg-info/PKG-INFO
--rw-rw-r--   0 neil      (1000) neil      (1000)      451 2023-07-26 00:13:40.000000 htmx-components-flask-example-0.0.1/htmx_components_flask_example.egg-info/SOURCES.txt
--rw-rw-r--   0 neil      (1000) neil      (1000)        1 2023-07-26 00:13:40.000000 htmx-components-flask-example-0.0.1/htmx_components_flask_example.egg-info/dependency_links.txt
--rw-rw-r--   0 neil      (1000) neil      (1000)       83 2023-07-26 00:13:40.000000 htmx-components-flask-example-0.0.1/htmx_components_flask_example.egg-info/requires.txt
--rw-rw-r--   0 neil      (1000) neil      (1000)        1 2023-07-26 00:13:40.000000 htmx-components-flask-example-0.0.1/htmx_components_flask_example.egg-info/top_level.txt
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-07-26 00:13:40.677448 htmx-components-flask-example-0.0.1/instance/
--rw-rw-r--   0 neil      (1000) neil      (1000)   942080 2023-07-25 23:31:34.000000 htmx-components-flask-example-0.0.1/instance/northwind.db
--rw-rw-r--   0 neil      (1000) neil      (1000)      469 2023-07-26 00:13:02.000000 htmx-components-flask-example-0.0.1/pyproject.toml
--rw-rw-r--   0 neil      (1000) neil      (1000)       38 2023-07-26 00:13:40.685448 htmx-components-flask-example-0.0.1/setup.cfg
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-07-26 00:13:40.685448 htmx-components-flask-example-0.0.1/templates/
--rw-rw-r--   0 neil      (1000) neil      (1000)      887 2023-07-25 23:40:00.000000 htmx-components-flask-example-0.0.1/templates/base.html
--rw-rw-r--   0 neil      (1000) neil      (1000)      179 2023-07-25 23:52:58.000000 htmx-components-flask-example-0.0.1/templates/form.html
--rw-rw-r--   0 neil      (1000) neil      (1000)      128 2023-07-25 23:53:10.000000 htmx-components-flask-example-0.0.1/templates/index.html
--rw-rw-r--   0 neil      (1000) neil      (1000)      115 2023-07-25 23:14:39.000000 htmx-components-flask-example-0.0.1/templates/viewgrid.html
+drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-08-01 21:47:18.568792 htmx-components-flask-example-0.0.2/
+-rw-rw-r--   0 neil      (1000) neil      (1000)       36 2023-07-26 00:13:50.000000 htmx-components-flask-example-0.0.2/.gitignore
+drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-08-01 21:47:18.544792 htmx-components-flask-example-0.0.2/.vscode/
+-rw-rw-r--   0 neil      (1000) neil      (1000)       68 2023-07-25 23:02:53.000000 htmx-components-flask-example-0.0.2/.vscode/settings.json
+-rw-rw-r--   0 neil      (1000) neil      (1000)     1070 2023-07-25 22:55:43.000000 htmx-components-flask-example-0.0.2/LICENSE
+-rw-rw-r--   0 neil      (1000) neil      (1000)      659 2023-08-01 21:47:18.568792 htmx-components-flask-example-0.0.2/PKG-INFO
+-rw-rw-r--   0 neil      (1000) neil      (1000)      349 2023-08-01 20:49:16.000000 htmx-components-flask-example-0.0.2/README.md
+-rw-rw-r--   0 neil      (1000) neil      (1000)     3109 2023-08-01 20:10:57.000000 htmx-components-flask-example-0.0.2/app.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)     3364 2023-07-25 23:47:06.000000 htmx-components-flask-example-0.0.2/form.py
+drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-08-01 21:47:18.548792 htmx-components-flask-example-0.0.2/htmx_components_flask_example.egg-info/
+-rw-rw-r--   0 neil      (1000) neil      (1000)      659 2023-08-01 21:47:18.000000 htmx-components-flask-example-0.0.2/htmx_components_flask_example.egg-info/PKG-INFO
+-rw-rw-r--   0 neil      (1000) neil      (1000)      475 2023-08-01 21:47:18.000000 htmx-components-flask-example-0.0.2/htmx_components_flask_example.egg-info/SOURCES.txt
+-rw-rw-r--   0 neil      (1000) neil      (1000)        1 2023-08-01 21:47:18.000000 htmx-components-flask-example-0.0.2/htmx_components_flask_example.egg-info/dependency_links.txt
+-rw-rw-r--   0 neil      (1000) neil      (1000)       83 2023-08-01 21:47:18.000000 htmx-components-flask-example-0.0.2/htmx_components_flask_example.egg-info/requires.txt
+-rw-rw-r--   0 neil      (1000) neil      (1000)        1 2023-08-01 21:47:18.000000 htmx-components-flask-example-0.0.2/htmx_components_flask_example.egg-info/top_level.txt
+drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-08-01 21:47:18.548792 htmx-components-flask-example-0.0.2/instance/
+-rw-rw-r--   0 neil      (1000) neil      (1000)   950272 2023-07-26 17:18:33.000000 htmx-components-flask-example-0.0.2/instance/northwind.db
+-rw-rw-r--   0 neil      (1000) neil      (1000)      574 2023-08-01 21:46:38.000000 htmx-components-flask-example-0.0.2/pyproject.toml
+-rw-rw-r--   0 neil      (1000) neil      (1000)       38 2023-08-01 21:47:18.568792 htmx-components-flask-example-0.0.2/setup.cfg
+drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-08-01 21:47:18.564792 htmx-components-flask-example-0.0.2/templates/
+-rw-rw-r--   0 neil      (1000) neil      (1000)      947 2023-08-01 20:11:20.000000 htmx-components-flask-example-0.0.2/templates/base.html
+-rw-rw-r--   0 neil      (1000) neil      (1000)      184 2023-08-01 20:04:15.000000 htmx-components-flask-example-0.0.2/templates/form.html
+-rw-rw-r--   0 neil      (1000) neil      (1000)      176 2023-08-01 20:15:21.000000 htmx-components-flask-example-0.0.2/templates/gridview.html
+-rw-rw-r--   0 neil      (1000) neil      (1000)      165 2023-08-01 20:08:59.000000 htmx-components-flask-example-0.0.2/templates/index.html
+-rw-rw-r--   0 neil      (1000) neil      (1000)      181 2023-08-01 20:12:51.000000 htmx-components-flask-example-0.0.2/templates/treeview.html
```

### Comparing `htmx-components-flask-example-0.0.1/LICENSE` & `htmx-components-flask-example-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `htmx-components-flask-example-0.0.1/form.py` & `htmx-components-flask-example-0.0.2/form.py`

 * *Files identical despite different names*

### Comparing `htmx-components-flask-example-0.0.1/instance/northwind.db` & `htmx-components-flask-example-0.0.2/instance/northwind.db`

 * *Files 0% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -5417,14 +5417,48 @@
 INSERT INTO Orders_FTS_docsize VALUES(826,X'0101010303000102030503020101');
 INSERT INTO Orders_FTS_docsize VALUES(827,X'0101010303000102020201020101');
 INSERT INTO Orders_FTS_docsize VALUES(828,X'0101010303000102020201020101');
 INSERT INTO Orders_FTS_docsize VALUES(829,X'0101010303000102020401020101');
 INSERT INTO Orders_FTS_docsize VALUES(830,X'0101010303000102030301020101');
 CREATE TABLE IF NOT EXISTS 'Orders_FTS_config'(k PRIMARY KEY, v) WITHOUT ROWID;
 INSERT INTO Orders_FTS_config VALUES('version',4);
+CREATE TABLE georegions (
+  id smallint primary key,
+  name text not null,
+  parent_id smallint null references georegions(id)
+);
+INSERT INTO georegions VALUES(1,'World',NULL);
+INSERT INTO georegions VALUES(2,'Africa',1);
+INSERT INTO georegions VALUES(5,'South America',419);
+INSERT INTO georegions VALUES(9,'Oceania',1);
+INSERT INTO georegions VALUES(11,'Western Africa',2);
+INSERT INTO georegions VALUES(13,'Central America',419);
+INSERT INTO georegions VALUES(14,'Eastern Africa',2);
+INSERT INTO georegions VALUES(15,'Northern Africa',2);
+INSERT INTO georegions VALUES(17,'Middle Africa',2);
+INSERT INTO georegions VALUES(18,'Southern Africa',2);
+INSERT INTO georegions VALUES(19,'Americas',1);
+INSERT INTO georegions VALUES(21,'Northern America',19);
+INSERT INTO georegions VALUES(29,'Caribbean',419);
+INSERT INTO georegions VALUES(30,'Eastern Asia',142);
+INSERT INTO georegions VALUES(34,'Southern Asia',142);
+INSERT INTO georegions VALUES(35,'South-Eastern Asia',142);
+INSERT INTO georegions VALUES(39,'Southern Europe',150);
+INSERT INTO georegions VALUES(53,'Australia and New Zealand',9);
+INSERT INTO georegions VALUES(54,'Melanesia',9);
+INSERT INTO georegions VALUES(57,'Micronesia',9);
+INSERT INTO georegions VALUES(61,'Polynesia',9);
+INSERT INTO georegions VALUES(142,'Asia',1);
+INSERT INTO georegions VALUES(143,'Central Asia',142);
+INSERT INTO georegions VALUES(145,'Western Asia',142);
+INSERT INTO georegions VALUES(150,'Europe',1);
+INSERT INTO georegions VALUES(151,'Eastern Europe',150);
+INSERT INTO georegions VALUES(154,'Northern Europe',150);
+INSERT INTO georegions VALUES(155,'Western Europe',150);
+INSERT INTO georegions VALUES(419,'Latin America and the Caribbean',19);
 DELETE FROM sqlite_sequence;
 INSERT INTO sqlite_sequence VALUES('Categories',8);
 INSERT INTO sqlite_sequence VALUES('Employees',9);
 INSERT INTO sqlite_sequence VALUES('Orders',11077);
 INSERT INTO sqlite_sequence VALUES('Products',77);
 INSERT INTO sqlite_sequence VALUES('Shippers',3);
 INSERT INTO sqlite_sequence VALUES('Suppliers',29);
```

### Comparing `htmx-components-flask-example-0.0.1/templates/base.html` & `htmx-components-flask-example-0.0.2/templates/base.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 <!doctype html>
 <html>
 
 <head>
   <meta charset="utf-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <meta name="htmx-config" content='{"defaultSwapStyle":"outerHTML", "useTemplateFragments":true}'>
-  <title>HTMX Components Flask Example</title>
+  <title>HTMX Components Flask Examples</title>
   <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet"
     integrity="sha384-9ndCyUaIbzAi2FUVXJi0CjmCapSmO7SnpJef0486qhLnuZ2cdeRhO02iuK6FUUVM" crossorigin="anonymous">
   <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.5/font/bootstrap-icons.css">
 </head>
 
 <body>
   <div class="container mt-3">
     {% block content %}{% endblock %}
   </div>
+
+  {% if request.args.get("nohx") is none %}
   <script src="https://unpkg.com/htmx.org@1.9.4"
     integrity="sha384-zUfuhFKKZCbHTY6aRR46gxiqszMk5tcHjsVFxnUo8VMus4kHGVdIYVbOYYNlKmHV"
     crossorigin="anonymous"></script>
+  {% endif %}
 
 </body>
 
 </html>
```

#### html2text {}

```diff
@@ -1,4 +1,6 @@
 
 
 
 {% block content %}{% endblock %}
+{% if request.args.get("nohx") is none %}
+ {% endif %}
```

