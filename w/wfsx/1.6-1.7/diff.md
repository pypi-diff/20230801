# Comparing `tmp/wfsx-1.6-py3-none-any.whl.zip` & `tmp/wfsx-1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 32675 bytes, number of entries: 20
+Zip file size: 32679 bytes, number of entries: 20
 -rw-rw-rw-  2.0 fat      413 b- defN 23-Jun-06 11:13 wfsx/CONST_j.py
 -rw-rw-rw-  2.0 fat     5163 b- defN 23-Jul-28 14:45 wfsx/Excel_x.py
 -rw-rw-rw-  2.0 fat     5280 b- defN 23-Jul-28 14:45 wfsx/Report.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-06 11:13 wfsx/__init__.py
 -rw-rw-rw-  2.0 fat     6310 b- defN 23-Jul-28 14:31 wfsx/api.py
 -rw-rw-rw-  2.0 fat     6019 b- defN 23-Jun-15 14:25 wfsx/apivalid.py
 -rw-rw-rw-  2.0 fat    16574 b- defN 23-Jul-28 14:41 wfsx/apivalidation.py
--rw-rw-rw-  2.0 fat    20705 b- defN 23-Jul-28 16:02 wfsx/common.py
--rw-rw-rw-  2.0 fat    12479 b- defN 23-Aug-01 14:37 wfsx/dataextract.py
+-rw-rw-rw-  2.0 fat    20715 b- defN 23-Aug-01 15:36 wfsx/common.py
+-rw-rw-rw-  2.0 fat    12481 b- defN 23-Aug-01 15:32 wfsx/dataextract.py
 -rw-rw-rw-  2.0 fat     2808 b- defN 23-Jun-06 11:13 wfsx/excel_json_reader.py
 -rw-rw-rw-  2.0 fat     4189 b- defN 23-Jun-16 15:41 wfsx/ghelper.py
 -rw-rw-rw-  2.0 fat     5407 b- defN 23-Jun-06 11:13 wfsx/parseexcel.py
 -rw-rw-rw-  2.0 fat     7022 b- defN 23-Jun-13 11:44 wfsx/plite.py
 -rw-rw-rw-  2.0 fat    23242 b- defN 23-Jul-28 14:45 wfsx/results_validate.py
 -rw-rw-rw-  2.0 fat     4322 b- defN 23-Jul-27 11:01 wfsx/inix/endpointapi.ini
--rw-rw-rw-  2.0 fat    11365 b- defN 23-Aug-01 14:40 wfsx-1.6.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1260 b- defN 23-Aug-01 14:40 wfsx-1.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-01 14:40 wfsx-1.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 23-Aug-01 14:40 wfsx-1.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1477 b- defN 23-Aug-01 14:40 wfsx-1.6.dist-info/RECORD
-20 files, 134132 bytes uncompressed, 30343 bytes compressed:  77.4%
+-rw-rw-rw-  2.0 fat    11365 b- defN 23-Aug-01 15:36 wfsx-1.7.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1260 b- defN 23-Aug-01 15:36 wfsx-1.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-01 15:36 wfsx-1.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-Aug-01 15:36 wfsx-1.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1477 b- defN 23-Aug-01 15:36 wfsx-1.7.dist-info/RECORD
+20 files, 134144 bytes uncompressed, 30347 bytes compressed:  77.4%
```

## zipnote {}

```diff
@@ -39,23 +39,23 @@
 
 Filename: wfsx/results_validate.py
 Comment: 
 
 Filename: wfsx/inix/endpointapi.ini
 Comment: 
 
-Filename: wfsx-1.6.dist-info/LICENSE
+Filename: wfsx-1.7.dist-info/LICENSE
 Comment: 
 
-Filename: wfsx-1.6.dist-info/METADATA
+Filename: wfsx-1.7.dist-info/METADATA
 Comment: 
 
-Filename: wfsx-1.6.dist-info/WHEEL
+Filename: wfsx-1.7.dist-info/WHEEL
 Comment: 
 
-Filename: wfsx-1.6.dist-info/top_level.txt
+Filename: wfsx-1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: wfsx-1.6.dist-info/RECORD
+Filename: wfsx-1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wfsx/common.py

```diff
@@ -8,15 +8,15 @@
 from pathlib import Path
 from wfsx.parseexcel import ParseExcel
 from wfsx.apivalid import Validations
 from datetime import date
 from cdxg import testdata
 
 mypath = Path.cwd()  # .parent
-print(mypath)
+# print(mypath)
 config = configparser.ConfigParser()
 data_file_path = mypath / 'config.ini'
 config.read(mypath / 'config.ini')
 
 
 def dumpData(apiselect, getalljson):
     with open(apiselect, 'w', encoding='utf-8') as jsonfile:
@@ -91,15 +91,15 @@
         reportpath.write_cell_content_colored(get_total_rows + 1, 10, comments)
         reportpath.write_cell_content_colored(get_total_rows + 1, 11, elapsed_secs)
         reportpath.write_cell_content_colored(get_total_rows + 1, 12, sprints)
     except Exception as e:
         if ValueError:
             for xna in acResults:
                 reportpath.write_cell_content_colored(get_total_rows + 1, 5, xna)
-        print(str(e))
+        # print(str(e))
 
 
 def Create_New_Report(report):
     otime = time.strftime("%Y-%m-%d_%H%M%S", time.localtime())
     reportfolderpath = report + "_" + otime + ".xlsx"
     shutil.copy(mypath / 'reports' / 'api_results.xlsx', mypath / 'reports' / reportfolderpath)
     return mypath / 'reports' / reportfolderpath
@@ -162,15 +162,15 @@
                         if mxchars == '[]':
                             charsx = []
                         else:
                             charsx = str(mxchars)
                     get_data[str(gcspt[0])] = charsx
                 elif xSplit[xlenn] == 'Extract':
                     gcspt = pSplit[xlenn].split('=')
-                    print(gcspt)
+                    # print(gcspt)
                     gxdatax = getExtract(xdata=gcspt[1], tdata=tdata)
                     get_data[str(gcspt[0])] = gxdatax
                 elif xSplit[xlenn] == 'Dadd':
                     keyx, valuesx = pSplit[xlenn].split('=')
                     rpl = valuesx.replace('*', ',')
                     xType_dict = json.loads(rpl)
                     get_data[keyx] = xType_dict
@@ -285,15 +285,15 @@
                 f.write('\t\tconfig.read(mypath / "utils" / "endpointapi.ini")\n')
                 f.write("\t\tif '/' in xendpoint:\n")
                 f.write("\t\t\txpoint = str(xendpoint).split('/')\n")
                 f.write("\t\t\trolepoint = getepoint(xpoint)  # xpoint[len(xpoint)-1]\n")
                 f.write('\t\telse:\n')
                 f.write("\t\t\trolepoint = xendpoint\n")
                 f.write('\t\troles = config.get("apiEndpoint", rolepoint)\n')
-                f.write('\t\tprint(roles)\n')
+                # f.write('\t\tprint(roles)\n')
                 f.write("\t\troles, cxUrl = roles.split(',')\n")
                 f.write('\t\tif rtype != "skip" and rtype == get_tags(rtype) and rtype is not None:\n')
                 f.write("\t\t\tgetallx = None\n")
                 f.write("\t\t\tgtdata = get_sheetnames_excel(generate_test_ap, itemdata=depend, ustory=tcdef)\n")
                 f.write("\t\t\tfor xlen in range(0, len(gtdata)):\n")
                 f.write("\t\t\t\tgetallx = excel_row_data(gtdata[xlen][0], depend)\n")
                 f.write("\t\t\t\tif depend is not None:\n")
@@ -414,15 +414,15 @@
         datapack = Validations().get_json_string_results(xdata, getdata)
         getxdata = datapack[0]
     return getxdata
 
 
 def getExtract(xdata, tdata):
     fpath, aName, apiname, evalue = xdata.split('|')
-    print(fpath, aName, apiname, evalue)
+    # print(fpath, aName, apiname, evalue)
     apiname = str(apiname) + '.json'
     getfile = mypath / 'test_data' / 'json_data' / fpath / apiname
     getdata = data_required(datafile=getfile)
     datapack = Validations().get_json_string_results(aName, getdata)
     if evalue == '':
         return datapack
     else:
```

## wfsx/dataextract.py

```diff
@@ -112,15 +112,15 @@
 
 def extractedValue(tdata, apipoint, ePoint=None, eValue=None, dictdata=None, gnx=0):
     global random_value, value
     getx, gnx, gxa = None, 0, None
     if ePoint is None and dictdata is None:
         if tdata != 'None' and tdata != '':
             eHome, ePoint, apxpoint, eValue = str(tdata).split('|')
-            print(eHome, ePoint, apxpoint, eValue)
+            # print(eHome, ePoint, apxpoint, eValue)
             if eValue == '': eValue = None
             if eHome not in ['filterdata', 'mixdata'] and apxpoint == '':
                 xroles = config.get('apiEndpoint', apipoint)
                 xroles, cxUrl = xroles.split(',')
             elif eHome not in ['filterdata', 'mixdata'] and apxpoint != '':
                 xroles = config.get('apiEndpoint', apxpoint)
                 xroles, cxUrl = xroles.split(',')
```

## Comparing `wfsx-1.6.dist-info/LICENSE` & `wfsx-1.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `wfsx-1.6.dist-info/METADATA` & `wfsx-1.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wfsx
-Version: 1.6
+Version: 1.7
 Summary: api automation testing framework based on unittest.
 Home-page: https://github.com/saasaa831/wfsx/
 Author: saasaa
 Author-email: saasaa@saa.com
 License: Apache 2.0
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: MacOS :: MacOS X
```

## Comparing `wfsx-1.6.dist-info/RECORD` & `wfsx-1.7.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 wfsx/CONST_j.py,sha256=K1qp18BcG4QXmeYaMLqd8j6-_rnMj1kQ67RmtsWMFvw,413
 wfsx/Excel_x.py,sha256=-RhqrKWTi2ias2f8sMpembEYSectGn6zvhlDEaGIkIc,5163
 wfsx/Report.py,sha256=kbydYbBv0YmoOdgCQ2y92nuBNUZmYcwq4gbajGUbKMc,5280
 wfsx/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 wfsx/api.py,sha256=4RvVwxzel6i3jpIWOw8pzM_LOCc9P9lqk8QKrvOJGXM,6310
 wfsx/apivalid.py,sha256=OZz8aFjH9BSmrvJNY7XwV1yjUYHpd7Fa6pyO-X0z0G8,6019
 wfsx/apivalidation.py,sha256=Hl6G6bv66BVnlN6iZjxATfe19LyB7yfvSHQQZ_Ue0Sg,16574
-wfsx/common.py,sha256=JMA43pYw9PAaAotrKs9wTiPUdqbKeti_MqEmVqCpqmo,20705
-wfsx/dataextract.py,sha256=G_jlT6quSalZb77_bOPQ9yWigUnwCOJrZRh56i8GPEk,12479
+wfsx/common.py,sha256=g4wdM0P_O3Uw4WV5jLzD4-koqIgIrWPD4CsHzXNwLoY,20715
+wfsx/dataextract.py,sha256=L_F7JAB5Z-TzpFWLlPHx8VJF_4Jr6FPbKBPTxBCy_3Y,12481
 wfsx/excel_json_reader.py,sha256=z4vQkNRLKCO7x3UAeI8EVd9vjY5GDTEYDOVTj2jqICA,2808
 wfsx/ghelper.py,sha256=oYgGDv8YZOKAX6vg4gel0kjpaAwZ40137AQhAFDFnW8,4189
 wfsx/parseexcel.py,sha256=uXXUcI9AiDHqdaKd8oGAxu_3OXFmuw66CLRXvJRXHtc,5407
 wfsx/plite.py,sha256=d2yNK_XkO17OFQbr4Ecf_OSkDgys9vzdefnm03Lm3Ck,7022
 wfsx/results_validate.py,sha256=Jzx6xUHcbrTQuKhc9q48vKR7BXmSrEbD8T7SB45c_NM,23242
 wfsx/inix/endpointapi.ini,sha256=0NfMZyTdLlBseaPlWWtzLFShX2qGODskfJ7PVUVnK34,4322
-wfsx-1.6.dist-info/LICENSE,sha256=O6YYwBy5W9D4kClOvrHiQlSfu479SgduHM03YRmz8mE,11365
-wfsx-1.6.dist-info/METADATA,sha256=Rz1jjJ9dugv_cIA-TvKoiGmMBAY9foePKzQgjRJxnPY,1260
-wfsx-1.6.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-wfsx-1.6.dist-info/top_level.txt,sha256=ylpSMw0AVSmfULYBvc6iiXmLKtra7xinB3IPH0sBALs,5
-wfsx-1.6.dist-info/RECORD,,
+wfsx-1.7.dist-info/LICENSE,sha256=O6YYwBy5W9D4kClOvrHiQlSfu479SgduHM03YRmz8mE,11365
+wfsx-1.7.dist-info/METADATA,sha256=c4F0LkrtEUnrDvF8r40Ehk2LI0IxM60DuMgtUOzIPGk,1260
+wfsx-1.7.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+wfsx-1.7.dist-info/top_level.txt,sha256=ylpSMw0AVSmfULYBvc6iiXmLKtra7xinB3IPH0sBALs,5
+wfsx-1.7.dist-info/RECORD,,
```

