# Comparing `tmp/directdb-1.0.0.tar.gz` & `tmp/directdb-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "directdb-1.0.0.tar", last modified: Mon Jul 31 14:03:11 2023, max compression
+gzip compressed data, was "directdb-1.0.1.tar", last modified: Tue Aug  1 16:36:11 2023, max compression
```

## Comparing `directdb-1.0.0.tar` & `directdb-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 14:03:11.434096 directdb-1.0.0/
--rw-rw-rw-   0        0        0    35182 2023-07-31 07:28:41.000000 directdb-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     2515 2023-07-31 14:03:11.433100 directdb-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1796 2023-07-31 14:02:18.000000 directdb-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 14:03:11.427097 directdb-1.0.0/directdb/
--rw-rw-rw-   0        0        0       30 2023-07-31 13:36:43.000000 directdb-1.0.0/directdb/__init__.py
--rw-rw-rw-   0        0        0     1865 2023-07-31 06:56:02.000000 directdb-1.0.0/directdb/exceptions.py
--rw-rw-rw-   0        0        0     4598 2023-07-31 13:51:44.000000 directdb-1.0.0/directdb/main.py
-drwxrwxrwx   0        0        0        0 2023-07-31 14:03:11.432099 directdb-1.0.0/directdb.egg-info/
--rw-rw-rw-   0        0        0     2515 2023-07-31 14:03:11.000000 directdb-1.0.0/directdb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-07-31 14:03:11.000000 directdb-1.0.0/directdb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 14:03:11.000000 directdb-1.0.0/directdb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-31 14:03:11.000000 directdb-1.0.0/directdb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-31 14:03:11.000000 directdb-1.0.0/directdb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 14:03:11.434096 directdb-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1117 2023-07-31 14:02:49.000000 directdb-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 16:36:11.407807 directdb-1.0.1/
+-rw-rw-rw-   0        0        0    35182 2023-07-31 07:28:41.000000 directdb-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2525 2023-08-01 16:36:11.406811 directdb-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1806 2023-08-01 16:32:26.000000 directdb-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 16:36:11.397810 directdb-1.0.1/directdb/
+-rw-rw-rw-   0        0        0      536 2023-08-01 16:35:34.000000 directdb-1.0.1/directdb/__init__.py
+-rw-rw-rw-   0        0        0     2371 2023-08-01 16:35:28.000000 directdb-1.0.1/directdb/exceptions.py
+-rw-rw-rw-   0        0        0     5223 2023-08-01 16:35:16.000000 directdb-1.0.1/directdb/main.py
+drwxrwxrwx   0        0        0        0 2023-08-01 16:36:11.404807 directdb-1.0.1/directdb.egg-info/
+-rw-rw-rw-   0        0        0     2525 2023-08-01 16:36:11.000000 directdb-1.0.1/directdb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-08-01 16:36:11.000000 directdb-1.0.1/directdb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 16:36:11.000000 directdb-1.0.1/directdb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-08-01 16:36:11.000000 directdb-1.0.1/directdb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-01 16:36:11.000000 directdb-1.0.1/directdb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 16:36:11.407807 directdb-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1117 2023-08-01 14:43:36.000000 directdb-1.0.1/setup.py
```

### Comparing `directdb-1.0.0/LICENSE` & `directdb-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `directdb-1.0.0/PKG-INFO` & `directdb-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: directdb
-Version: 1.0.0
+Version: 1.0.1
 Summary: An async package that makes database handling extremely easy!
 Author: Cannonball Chris
 Author-email: cannonballchris8@gmail.com
 Keywords: db,bot,discord bot,database,postgresql,asyncpg,async,pgutils,nosql,sqlite
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -34,15 +34,15 @@
 ## License
 
 [GPL-3.0](https://choosealicense.com/licenses/gpl-3.0/)
 
 
 ## Documentation
 
-[Documentation](https://linktodocumentation)
+[Documentation](https://indigodev.gitbook.io/directdb)
 
 
 ## Usage/Examples
 
 Using the library with a discord bot
 
 ```py
```

### Comparing `directdb-1.0.0/README.md` & `directdb-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ## License
 
 [GPL-3.0](https://choosealicense.com/licenses/gpl-3.0/)
 
 
 ## Documentation
 
-[Documentation](https://linktodocumentation)
+[Documentation](https://indigodev.gitbook.io/directdb)
 
 
 ## Usage/Examples
 
 Using the library with a discord bot
 
 ```py
```

### Comparing `directdb-1.0.0/directdb/exceptions.py` & `directdb-1.0.1/directdb/exceptions.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+# LICENSE
+# -----------------------------------------------------------------------
+# directdb is distributed under the terms of the GNU Affero General Public License (AGPL).
+# You can find a copy of the license in the LICENSE file included with this distribution.
+# The AGPL is a copyleft license that ensures the freedom to use, modify, and distribute the library's code, even in the case of web-based services.
+# By using directdb, you agree to comply with the terms and conditions of the AGPL.
+
 import datetime
 
 class DatabaseInsertionException(Exception):
 	"""Class for exceptions when insertion into database fails.
 	
 	Parameters
 	----------
```

### Comparing `directdb-1.0.0/directdb/main.py` & `directdb-1.0.1/directdb/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,21 @@
+# LICENSE
+# -----------------------------------------------------------------------
+# directdb is distributed under the terms of the GNU Affero General Public License (AGPL).
+# You can find a copy of the license in the LICENSE file included with this distribution.
+# The AGPL is a copyleft license that ensures the freedom to use, modify, and distribute the library's code, even in the case of web-based services.
+# By using directdb, you agree to comply with the terms and conditions of the AGPL.
+
 import asyncio
 
 import asyncpg
 
 from .exceptions import *
 
-class Postgresql:	
+class Postgresql:
 	""" A class to handle all database related tasks efficiently.
 	
 	Parameters
 	----------
 	host: str
 		The host of the database.
 	user: str
@@ -26,28 +33,30 @@
 
 	def __init__(self, host, user, password, database, port):
 		self.host = host
 		self.user = user
 		self.password = password
 		self.database = database
 		self.port = port
-	
+
 
 	async def connect(self) -> asyncpg.Pool:
 		""" Connects to the database. 
 		
 		Returns
 		-------
 		Class
 			The custom database handler class.
 
 		"""
-		self.pool = await asyncpg.create_pool(host=self.host, user=self.user, password=self.password, database=self.database, port=self.port)
+		self.pool = await asyncpg.create_pool(
+			host=self.host, user=self.user, password=self.password, database=self.database, port=self.port
+		)
 		return self.pool
-	
+
 	async def create_table(self, tables:list) -> None:
 		""" Creates table(s) in the database.
 		
 		Parameters
 		----------
 		tables: list
 			A list in format of [{'table_name': {'column_name:'datatype'}}]
@@ -93,75 +102,75 @@
 		try:
 			columns = ', '.join(data.keys())
 			values = ', '.join(['${}'.format(i + 1) for i in range(len(data))])
 			query = 'INSERT INTO {} ({}) VALUES ({})'.format(table, columns, values)
 			await self.pool.execute(query, *data.values())
 		except Exception as e:
 			raise DatabaseInsertionException(e)
-	
-	async def fetch(self, table:str, *, filter:dict = None) -> list:
+
+	async def fetch(self, table:str, *, data_filter:dict = None) -> list:
 		""" Fetches data from the database.
 		
 		Parameters
 		----------
 		table: str
 			The table to fetch data from.
-		filter: dict [Optional]
-			The filter to use in format {'column name':data}.
+		data_filter: dict [Optional]
+			The data_filter to use in format {'column name':data}.
 
 		Returns
 		-------
 		list
 			A list of data fetched from the database.
 
 		"""
 		try:
-			if not filter:
+			if not data_filter:
 				query = 'SELECT * FROM {}'.format(table)
 				return await self.pool.fetch(query)
 			else:
-				filters = ' AND '.join(['{} = ${}'.format(column, i + 1) for i, column in enumerate(filter)])
-				query = 'SELECT * FROM {} WHERE {}'.format(table, filters)
-				return await self.pool.fetch(query, *filter.values())
+				data_filters = ' AND '.join(['{} = ${}'.format(column, i + 1) for i, column in enumerate(data_filter)])
+				query = 'SELECT * FROM {} WHERE {}'.format(table, data_filters)
+				return await self.pool.fetch(query, *data_filter.values())
 
 		except Exception as e:
 			raise DatabaseFetchException(e)
-	
-	async def update(self, table:str, data:dict, filter:dict) -> None:
+
+	async def update(self, table:str, data:dict, data_filter:dict) -> None:
 		""" Updates data in the database.
 		
 		Parameters
 		----------
 		table: str
 			The table to update data in.
 		data: dict
 			The data to update in format {'column name':data}.
-		filter: dict
-			The filter to use in format {'column name':data}.
+		data_filter: dict
+			The data_filter to use in format {'column name':data}.
 
 		"""
 		try:
-			#Since $1, $2 etc are used in update data, we need to continue from there for filter data to avoid errors.
+			#Since $1, $2 etc are used in update data, we need to continue from there for data_filter data to avoid errors.
 			columns = ', '.join(['{} = ${}'.format(column, i + 1) for i, column in enumerate(data)])
-			filters = ' AND '.join(['{} = ${}'.format(column, i + len(data) + 1) for i, column in enumerate(filter)])
-			query = 'UPDATE {} SET {} WHERE {}'.format(table, columns, filters)
-			await self.pool.execute(query, *data.values(), *filter.values())
+			data_filters = ' AND '.join(['{} = ${}'.format(column, i + len(data) + 1) for i, column in enumerate(data_filter)])
+			query = 'UPDATE {} SET {} WHERE {}'.format(table, columns, data_filters)
+			await self.pool.execute(query, *data.values(), *data_filter.values())
 		except Exception as e:
 			raise DatabaseUpdateException(e)
 
-	async def delete(self, table:str, filter:dict) -> None:
+	async def delete(self, table:str, data_filter:dict) -> None:
 		""" Deletes data from the database.
 		
 		Parameters
 		----------
 		table: str
 			The table to delete data from.
-		filter: dict
-			The filter to use in format {'column name':data}.
+		data_filter: dict
+			The data_filter to use in format {'column name':data}.
 
 		"""
 		try:
-			filters = ' AND '.join(['{} = ${}'.format(column, i + 1) for i, column in enumerate(filter)])
-			query = 'DELETE FROM {} WHERE {}'.format(table, filters)
-			await self.pool.execute(query, *filter.values())
+			data_filters = ' AND '.join(['{} = ${}'.format(column, i + 1) for i, column in enumerate(data_filter)])
+			query = 'DELETE FROM {} WHERE {}'.format(table, data_filters)
+			await self.pool.execute(query, *data_filter.values())
 		except Exception as e:
 			raise DatabaseDeleteException(e)
```

### Comparing `directdb-1.0.0/directdb.egg-info/PKG-INFO` & `directdb-1.0.1/directdb.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: directdb
-Version: 1.0.0
+Version: 1.0.1
 Summary: An async package that makes database handling extremely easy!
 Author: Cannonball Chris
 Author-email: cannonballchris8@gmail.com
 Keywords: db,bot,discord bot,database,postgresql,asyncpg,async,pgutils,nosql,sqlite
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -34,15 +34,15 @@
 ## License
 
 [GPL-3.0](https://choosealicense.com/licenses/gpl-3.0/)
 
 
 ## Documentation
 
-[Documentation](https://linktodocumentation)
+[Documentation](https://indigodev.gitbook.io/directdb)
 
 
 ## Usage/Examples
 
 Using the library with a discord bot
 
 ```py
```

### Comparing `directdb-1.0.0/setup.py` & `directdb-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import codecs
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.0'
+VERSION = '1.0.1'
 DESCRIPTION = 'An async package that makes database handling extremely easy!'
 
 # Setting up
 setup(
     name="directdb",
     version=VERSION,
     author="Cannonball Chris",
```

