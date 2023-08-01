# Comparing `tmp/green_box-1.0.0.tar.gz` & `tmp/green_box-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "green_box-1.0.0.tar", max compression
+gzip compressed data, was "green_box-1.0.1.tar", max compression
```

## Comparing `green_box-1.0.0.tar` & `green_box-1.0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1585 2023-07-23 16:04:03.829480 green_box-1.0.0/README.md
--rw-r--r--   0        0        0       37 2023-07-23 16:04:03.829480 green_box-1.0.0/green_box/__init__.py
--rw-r--r--   0        0        0     1301 2023-07-23 16:04:03.829480 green_box-1.0.0/green_box/green_box.py
--rw-r--r--   0        0        0      394 2023-07-23 16:04:03.829480 green_box-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2052 1970-01-01 00:00:00.000000 green_box-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1560 2023-08-01 08:20:35.802328 green_box-1.0.1/README.md
+-rw-r--r--   0        0        0     1114 2023-08-01 08:20:35.802328 green_box-1.0.1/green_box/__init__.py
+-rw-r--r--   0        0        0     1275 2023-08-01 08:20:35.802328 green_box-1.0.1/green_box/green_box.py
+-rw-r--r--   0        0        0      394 2023-08-01 08:20:35.802328 green_box-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2027 1970-01-01 00:00:00.000000 green_box-1.0.1/PKG-INFO
```

### Comparing `green_box-1.0.0/README.md` & `green_box-1.0.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -9,21 +9,20 @@
 **PyPi**
 ```
 pip install green-box
 ```
 
 ## **Использование**
 Из всей ссылки берется только ID!
->https://docs.google.com/spreadsheets/d/***1O174ca048KT5YMYkDADzQvzIJEWUMADj_0ciLAQOt34***
-
+> <img src="https://imgur.com/wOMkbUe.png" width="" height="" />
 
 ```python
 from green_box import Table
 
-table = Table('1O174ca048KT5YMYkDADzQvzIJEWUMADj_0ciLAQOt34','Лист1').rows
+table = Table('1O174ca048KT5YMYkDADzQvzIJEWUMADj_0ciLAQOt34','Лист1').rows()
 
 ```
 ```
 ['Фамилия', 'Имя', 'Отчество', 'Адрес']
 ['Сидорова', 'Елена', 'Евгеньевна', 'пр. Победы, 10']
 ['Петров', 'Иван', 'Александрович', 'ул. Солнечная, 5']
 ['Васильева', 'Ирина', 'Александровна', 'ул. Парковая, 3']
```

### Comparing `green_box-1.0.0/green_box/green_box.py` & `green_box-1.0.1/green_box/green_box.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,22 +27,20 @@
     workbook = openpyxl.load_workbook(tmp_file)
     
     if isinstance(__worksheet, int):
       __worksheet = workbook.sheetnames[__worksheet]
     
     self.__worksheet = workbook[__worksheet]
 
-  @property
   def columns(self) -> Matrix:
     columns = []
     for column in self.__worksheet.iter_cols():
       column = [cell.value for cell in column]
       columns.append(column)
     return Matrix(columns)
   
-  @property
   def rows(self) -> Matrix:
     rows = []
     for row in self.__worksheet.iter_rows():
       row = [cell.value for cell in row]
       rows.append(row)
     return Matrix(rows)
```

### Comparing `green_box-1.0.0/PKG-INFO` & `green_box-1.0.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: green-box
-Version: 1.0.0
+Version: 1.0.1
 Summary: Simple data collection from Google Tables
 Author: QuoNaro
 Author-email: QuoNaro@mail.ru
 Requires-Python: >=3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -24,21 +24,20 @@
 **PyPi**
 ```
 pip install green-box
 ```
 
 ## **Использование**
 Из всей ссылки берется только ID!
->https://docs.google.com/spreadsheets/d/***1O174ca048KT5YMYkDADzQvzIJEWUMADj_0ciLAQOt34***
-
+> <img src="https://imgur.com/wOMkbUe.png" width="" height="" />
 
 ```python
 from green_box import Table
 
-table = Table('1O174ca048KT5YMYkDADzQvzIJEWUMADj_0ciLAQOt34','Лист1').rows
+table = Table('1O174ca048KT5YMYkDADzQvzIJEWUMADj_0ciLAQOt34','Лист1').rows()
 
 ```
 ```
 ['Фамилия', 'Имя', 'Отчество', 'Адрес']
 ['Сидорова', 'Елена', 'Евгеньевна', 'пр. Победы, 10']
 ['Петров', 'Иван', 'Александрович', 'ул. Солнечная, 5']
 ['Васильева', 'Ирина', 'Александровна', 'ул. Парковая, 3']
```

