# Comparing `tmp/wfsx-1.5-py3-none-any.whl.zip` & `tmp/wfsx-1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 32603 bytes, number of entries: 20
+Zip file size: 32675 bytes, number of entries: 20
 -rw-rw-rw-  2.0 fat      413 b- defN 23-Jun-06 11:13 wfsx/CONST_j.py
 -rw-rw-rw-  2.0 fat     5163 b- defN 23-Jul-28 14:45 wfsx/Excel_x.py
 -rw-rw-rw-  2.0 fat     5280 b- defN 23-Jul-28 14:45 wfsx/Report.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-06 11:13 wfsx/__init__.py
 -rw-rw-rw-  2.0 fat     6310 b- defN 23-Jul-28 14:31 wfsx/api.py
 -rw-rw-rw-  2.0 fat     6019 b- defN 23-Jun-15 14:25 wfsx/apivalid.py
 -rw-rw-rw-  2.0 fat    16574 b- defN 23-Jul-28 14:41 wfsx/apivalidation.py
 -rw-rw-rw-  2.0 fat    20705 b- defN 23-Jul-28 16:02 wfsx/common.py
--rw-rw-rw-  2.0 fat    11989 b- defN 23-Jul-31 15:00 wfsx/dataextract.py
+-rw-rw-rw-  2.0 fat    12479 b- defN 23-Aug-01 14:37 wfsx/dataextract.py
 -rw-rw-rw-  2.0 fat     2808 b- defN 23-Jun-06 11:13 wfsx/excel_json_reader.py
 -rw-rw-rw-  2.0 fat     4189 b- defN 23-Jun-16 15:41 wfsx/ghelper.py
 -rw-rw-rw-  2.0 fat     5407 b- defN 23-Jun-06 11:13 wfsx/parseexcel.py
 -rw-rw-rw-  2.0 fat     7022 b- defN 23-Jun-13 11:44 wfsx/plite.py
 -rw-rw-rw-  2.0 fat    23242 b- defN 23-Jul-28 14:45 wfsx/results_validate.py
 -rw-rw-rw-  2.0 fat     4322 b- defN 23-Jul-27 11:01 wfsx/inix/endpointapi.ini
--rw-rw-rw-  2.0 fat    11365 b- defN 23-Jul-31 15:02 wfsx-1.5.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1260 b- defN 23-Jul-31 15:02 wfsx-1.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-31 15:02 wfsx-1.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 23-Jul-31 15:02 wfsx-1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1477 b- defN 23-Jul-31 15:02 wfsx-1.5.dist-info/RECORD
-20 files, 133642 bytes uncompressed, 30271 bytes compressed:  77.3%
+-rw-rw-rw-  2.0 fat    11365 b- defN 23-Aug-01 14:40 wfsx-1.6.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1260 b- defN 23-Aug-01 14:40 wfsx-1.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-01 14:40 wfsx-1.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-Aug-01 14:40 wfsx-1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1477 b- defN 23-Aug-01 14:40 wfsx-1.6.dist-info/RECORD
+20 files, 134132 bytes uncompressed, 30343 bytes compressed:  77.4%
```

## zipnote {}

```diff
@@ -39,23 +39,23 @@
 
 Filename: wfsx/results_validate.py
 Comment: 
 
 Filename: wfsx/inix/endpointapi.ini
 Comment: 
 
-Filename: wfsx-1.5.dist-info/LICENSE
+Filename: wfsx-1.6.dist-info/LICENSE
 Comment: 
 
-Filename: wfsx-1.5.dist-info/METADATA
+Filename: wfsx-1.6.dist-info/METADATA
 Comment: 
 
-Filename: wfsx-1.5.dist-info/WHEEL
+Filename: wfsx-1.6.dist-info/WHEEL
 Comment: 
 
-Filename: wfsx-1.5.dist-info/top_level.txt
+Filename: wfsx-1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: wfsx-1.5.dist-info/RECORD
+Filename: wfsx-1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wfsx/dataextract.py

```diff
@@ -207,15 +207,15 @@
     except Exception as e:
         return str(e)
 
 
 def get_defined_data(apipoint, ddata):
     # Use regular expressions to find the string inside the braces
     try:
-        global dResults, extnurl
+        global dResults, extnurl, gtxa
         if '$' in ddata:
             xid = []
             match = re.findall(r'\$(.*?)\$', ddata)
             gnx = 0
             for variable in match:
                 if '|' in variable:
                     dfile, dxt, appoint, gtxa = variable.split('|')
@@ -243,21 +243,28 @@
                         apipoint = apipoint
                     # print(dfile,dxt, apipoint, gtxa)
                 exresults, gnx, gxa = extractedValue(tdata=extracted_string, apipoint=apipoint)
                 # print(exresults, gnx, gxa)
                 if gxa in ['S1', 'S2']:
                     dResults = exresults
                 else:
-                    if type(exresults[0]) == list:
-                        dResults = []
-                        for xresults in exresults[0]:
-                            dResults.append(str(xresults))
-                        dResults = '-'.join(dResults)
-                    else:
-                        dResults = exresults[0]
+                    if type(exresults) == list:
+                        if gtxa == '*':
+                            dResults = ','.join(str(item) for item in exresults)
+                        else:
+                            splgtxa = gtxa.split('*')
+                            if splgtxa[1].isdigit():
+                                itemsx = random.sample(exresults, int(splgtxa[1]))
+                                dResults = ','.join(str(item) for item in itemsx)
+                            else:
+                                splgtxa = gtxa.split('**')
+                                if splgtxa[1].isdigit():
+                                    dResults = random.sample(exresults, int(splgtxa[1]))
+                                else:
+                                    dResults = exresults
                 replaced_string = ddata.replace('{' + extracted_string + '}', str(dResults))
                 return replaced_string
             else:
                 return ddata
     except Exception as e:
         return ddata
 
@@ -282,13 +289,13 @@
             apipoint = '_'.join(abx)
         else:
             apipoint = str(xpoint[0])
     tbname = apipoint + '_' + tbname
     getresult = engConnect(rindex=tbname, getdata=query, dbname=str(dbname) + '.db')
     return getresult
 
-def getbaseUrl(ddata, urlString):
+def get_base_Url(ddata, urlString):
     match = re.search(r'{(.*?)}', ddata)
     if match:
         extracted_string = match.group(1)
         replaced_string = ddata.replace(str('{' + extracted_string + '}'), str(urlString))
         return replaced_string
```

## Comparing `wfsx-1.5.dist-info/LICENSE` & `wfsx-1.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `wfsx-1.5.dist-info/METADATA` & `wfsx-1.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wfsx
-Version: 1.5
+Version: 1.6
 Summary: api automation testing framework based on unittest.
 Home-page: https://github.com/saasaa831/wfsx/
 Author: saasaa
 Author-email: saasaa@saa.com
 License: Apache 2.0
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: MacOS :: MacOS X
```

## Comparing `wfsx-1.5.dist-info/RECORD` & `wfsx-1.6.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 wfsx/Excel_x.py,sha256=-RhqrKWTi2ias2f8sMpembEYSectGn6zvhlDEaGIkIc,5163
 wfsx/Report.py,sha256=kbydYbBv0YmoOdgCQ2y92nuBNUZmYcwq4gbajGUbKMc,5280
 wfsx/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 wfsx/api.py,sha256=4RvVwxzel6i3jpIWOw8pzM_LOCc9P9lqk8QKrvOJGXM,6310
 wfsx/apivalid.py,sha256=OZz8aFjH9BSmrvJNY7XwV1yjUYHpd7Fa6pyO-X0z0G8,6019
 wfsx/apivalidation.py,sha256=Hl6G6bv66BVnlN6iZjxATfe19LyB7yfvSHQQZ_Ue0Sg,16574
 wfsx/common.py,sha256=JMA43pYw9PAaAotrKs9wTiPUdqbKeti_MqEmVqCpqmo,20705
-wfsx/dataextract.py,sha256=eVQQq4EPney1Twcjqs2FRY6C8abMLclK304AksyyjR8,11989
+wfsx/dataextract.py,sha256=G_jlT6quSalZb77_bOPQ9yWigUnwCOJrZRh56i8GPEk,12479
 wfsx/excel_json_reader.py,sha256=z4vQkNRLKCO7x3UAeI8EVd9vjY5GDTEYDOVTj2jqICA,2808
 wfsx/ghelper.py,sha256=oYgGDv8YZOKAX6vg4gel0kjpaAwZ40137AQhAFDFnW8,4189
 wfsx/parseexcel.py,sha256=uXXUcI9AiDHqdaKd8oGAxu_3OXFmuw66CLRXvJRXHtc,5407
 wfsx/plite.py,sha256=d2yNK_XkO17OFQbr4Ecf_OSkDgys9vzdefnm03Lm3Ck,7022
 wfsx/results_validate.py,sha256=Jzx6xUHcbrTQuKhc9q48vKR7BXmSrEbD8T7SB45c_NM,23242
 wfsx/inix/endpointapi.ini,sha256=0NfMZyTdLlBseaPlWWtzLFShX2qGODskfJ7PVUVnK34,4322
-wfsx-1.5.dist-info/LICENSE,sha256=O6YYwBy5W9D4kClOvrHiQlSfu479SgduHM03YRmz8mE,11365
-wfsx-1.5.dist-info/METADATA,sha256=JKGeOs6_hTqgYIFLmNh-wqfJe1n2587A0iA_7cBDL2A,1260
-wfsx-1.5.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-wfsx-1.5.dist-info/top_level.txt,sha256=ylpSMw0AVSmfULYBvc6iiXmLKtra7xinB3IPH0sBALs,5
-wfsx-1.5.dist-info/RECORD,,
+wfsx-1.6.dist-info/LICENSE,sha256=O6YYwBy5W9D4kClOvrHiQlSfu479SgduHM03YRmz8mE,11365
+wfsx-1.6.dist-info/METADATA,sha256=Rz1jjJ9dugv_cIA-TvKoiGmMBAY9foePKzQgjRJxnPY,1260
+wfsx-1.6.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+wfsx-1.6.dist-info/top_level.txt,sha256=ylpSMw0AVSmfULYBvc6iiXmLKtra7xinB3IPH0sBALs,5
+wfsx-1.6.dist-info/RECORD,,
```

