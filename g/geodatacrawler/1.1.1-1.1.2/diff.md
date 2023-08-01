# Comparing `tmp/geodatacrawler-1.1.1.tar.gz` & `tmp/geodatacrawler-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geodatacrawler-1.1.1.tar", max compression
+gzip compressed data, was "geodatacrawler-1.1.2.tar", max compression
```

## Comparing `geodatacrawler-1.1.1.tar` & `geodatacrawler-1.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rwxr-xr-x   0        0        0     1096 2023-06-20 07:37:01.011896 geodatacrawler-1.1.1/LICENSE
--rwxr-xr-x   0        0        0     3756 2023-07-31 14:47:49.815210 geodatacrawler-1.1.1/README.md
--rwxr-xr-x   0        0        0       23 2023-06-20 07:37:01.153896 geodatacrawler-1.1.1/geodatacrawler/__init__.py
--rwxr-xr-x   0        0        0      220 2023-06-20 07:37:01.153896 geodatacrawler-1.1.1/geodatacrawler/etl.py
--rwxr-xr-x   0        0        0    16594 2023-06-20 07:37:01.154895 geodatacrawler-1.1.1/geodatacrawler/mapfile.py
--rwxr-xr-x   0        0        0    30264 2023-07-31 15:02:18.986787 geodatacrawler-1.1.1/geodatacrawler/metadata.py
--rwxr-xr-x   0        0        0     7379 2023-06-20 07:37:01.156897 geodatacrawler-1.1.1/geodatacrawler/schemas/iso19139/__init__.py
--rwxr-xr-x   0        0        0     3603 2023-07-31 12:57:52.922404 geodatacrawler-1.1.1/geodatacrawler/schemas/iso19139/contact.j2
--rwxr-xr-x   0        0        0    21854 2023-07-31 12:57:52.930840 geodatacrawler-1.1.1/geodatacrawler/schemas/iso19139/main.j2
--rwxr-xr-x   0        0        0      307 2023-07-31 12:57:52.942960 geodatacrawler-1.1.1/geodatacrawler/templates/PGM.tpl
--rwxr-xr-x   0        0        0       21 2023-06-20 07:37:01.159894 geodatacrawler-1.1.1/geodatacrawler/templates/__init__.py
--rwxr-xr-x   0        0        0      118 2023-06-20 07:37:01.160911 geodatacrawler-1.1.1/geodatacrawler/templates/class-line.tpl
--rwxr-xr-x   0        0        0      118 2023-06-20 07:37:01.161895 geodatacrawler-1.1.1/geodatacrawler/templates/class-point.tpl
--rwxr-xr-x   0        0        0      137 2023-06-20 07:37:01.161895 geodatacrawler-1.1.1/geodatacrawler/templates/class-polygon.tpl
--rwxr-xr-x   0        0        0     6622 2023-06-20 07:37:01.162898 geodatacrawler-1.1.1/geodatacrawler/templates/class-raster.tpl
--rwxr-xr-x   0        0        0     2112 2023-06-20 07:37:01.163900 geodatacrawler-1.1.1/geodatacrawler/templates/csv.j2
--rwxr-xr-x   0        0        0     2860 2023-06-20 07:37:01.164899 geodatacrawler-1.1.1/geodatacrawler/templates/default.map
--rwxr-xr-x   0        0        0    12288 2023-06-20 07:37:01.164899 geodatacrawler-1.1.1/geodatacrawler/templates/index.sqlite
--rwxr-xr-x   0        0        0      722 2023-06-20 07:37:01.165896 geodatacrawler-1.1.1/geodatacrawler/templates/layer.tpl
--rwxr-xr-x   0        0        0     6686 2023-06-20 07:37:01.166897 geodatacrawler-1.1.1/geodatacrawler/upload.py
--rwxr-xr-x   0        0        0    17081 2023-06-20 07:37:01.167895 geodatacrawler-1.1.1/geodatacrawler/upload_wosis.py
--rwxr-xr-x   0        0        0    21760 2023-07-31 12:57:52.959935 geodatacrawler-1.1.1/geodatacrawler/utils.py
--rwxr-xr-x   0        0        0     1031 2023-07-31 15:03:15.148183 geodatacrawler-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     4890 1970-01-01 00:00:00.000000 geodatacrawler-1.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1096 2023-07-31 15:10:48.256791 geodatacrawler-1.1.2/LICENSE
+-rwxr-xr-x   0        0        0     3756 2023-07-31 15:13:12.659044 geodatacrawler-1.1.2/README.md
+-rwxr-xr-x   0        0        0       23 2023-06-20 07:37:01.153896 geodatacrawler-1.1.2/geodatacrawler/__init__.py
+-rwxr-xr-x   0        0        0      220 2023-06-20 07:37:01.153896 geodatacrawler-1.1.2/geodatacrawler/etl.py
+-rwxr-xr-x   0        0        0    16594 2023-06-20 07:37:01.154895 geodatacrawler-1.1.2/geodatacrawler/mapfile.py
+-rwxr-xr-x   0        0        0    30420 2023-08-01 11:26:35.949350 geodatacrawler-1.1.2/geodatacrawler/metadata.py
+-rwxr-xr-x   0        0        0     7379 2023-06-20 07:37:01.156897 geodatacrawler-1.1.2/geodatacrawler/schemas/iso19139/__init__.py
+-rwxr-xr-x   0        0        0     3646 2023-08-01 11:56:59.605365 geodatacrawler-1.1.2/geodatacrawler/schemas/iso19139/contact.j2
+-rwxr-xr-x   0        0        0    21873 2023-08-01 11:29:38.737869 geodatacrawler-1.1.2/geodatacrawler/schemas/iso19139/main.j2
+-rwxr-xr-x   0        0        0      307 2023-07-31 15:13:12.663046 geodatacrawler-1.1.2/geodatacrawler/templates/PGM.tpl
+-rwxr-xr-x   0        0        0       21 2023-06-20 07:37:01.159894 geodatacrawler-1.1.2/geodatacrawler/templates/__init__.py
+-rwxr-xr-x   0        0        0      118 2023-06-20 07:37:01.160911 geodatacrawler-1.1.2/geodatacrawler/templates/class-line.tpl
+-rwxr-xr-x   0        0        0      118 2023-06-20 07:37:01.161895 geodatacrawler-1.1.2/geodatacrawler/templates/class-point.tpl
+-rwxr-xr-x   0        0        0      137 2023-06-20 07:37:01.161895 geodatacrawler-1.1.2/geodatacrawler/templates/class-polygon.tpl
+-rwxr-xr-x   0        0        0     6622 2023-06-20 07:37:01.162898 geodatacrawler-1.1.2/geodatacrawler/templates/class-raster.tpl
+-rwxr-xr-x   0        0        0     2112 2023-06-20 07:37:01.163900 geodatacrawler-1.1.2/geodatacrawler/templates/csv.j2
+-rwxr-xr-x   0        0        0     2860 2023-06-20 07:37:01.164899 geodatacrawler-1.1.2/geodatacrawler/templates/default.map
+-rwxr-xr-x   0        0        0    12288 2023-06-20 07:37:01.164899 geodatacrawler-1.1.2/geodatacrawler/templates/index.sqlite
+-rwxr-xr-x   0        0        0      722 2023-06-20 07:37:01.165896 geodatacrawler-1.1.2/geodatacrawler/templates/layer.tpl
+-rwxr-xr-x   0        0        0     6686 2023-06-20 07:37:01.166897 geodatacrawler-1.1.2/geodatacrawler/upload.py
+-rwxr-xr-x   0        0        0    17081 2023-06-20 07:37:01.167895 geodatacrawler-1.1.2/geodatacrawler/upload_wosis.py
+-rwxr-xr-x   0        0        0    22229 2023-08-01 11:23:06.692596 geodatacrawler-1.1.2/geodatacrawler/utils.py
+-rwxr-xr-x   0        0        0     1031 2023-08-01 11:04:36.489404 geodatacrawler-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4890 1970-01-01 00:00:00.000000 geodatacrawler-1.1.2/PKG-INFO
```

### Comparing `geodatacrawler-1.1.1/LICENSE` & `geodatacrawler-1.1.2/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 paul van genuchten
+Copyright (c) 2023 paul van genuchten
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `geodatacrawler-1.1.1/README.md` & `geodatacrawler-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `geodatacrawler-1.1.1/geodatacrawler/mapfile.py` & `geodatacrawler-1.1.2/geodatacrawler/mapfile.py`

 * *Files identical despite different names*

### Comparing `geodatacrawler-1.1.1/geodatacrawler/metadata.py` & `geodatacrawler-1.1.2/geodatacrawler/metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from . import templates
 from hashlib import md5
 
 webdavUrl = os.getenv('pgdc_webdav_url')
 canonicalUrl = os.getenv('pgdc_canonical_url')
 schemaPath = os.getenv('pgdc_schema_path')
 if not schemaPath:
-    schemaPath = "/mnt/c/Users/genuc003/Projects/geopython/pyGeoDataCrawler/geodatacrawler/schemas"
+    schemaPath = os.path.join(os.path.dirname(__file__),"schemas")
 
 # for supported formats, see apache tika - http://tika.apache.org/1.4/formats.html
 TEXT_FILE_TYPES = ['xls', 'xlsx', 'geojson', 'sqlite', 'db', 'csv']
 GRID_FILE_TYPES = ['tif', 'grib2', 'nc']
 VECTOR_FILE_TYPES = ['shp', 'mvt', 'dxf', 'dwg', 'fgdb', 'gml', 'kml', 'geojson', 'vrt', 'gpkg', 'kmz']
 SPATIAL_FILE_TYPES = GRID_FILE_TYPES + VECTOR_FILE_TYPES
 INDEX_FILE_TYPES = SPATIAL_FILE_TYPES + TEXT_FILE_TYPES
@@ -56,32 +56,34 @@
 @click.option('--db', nargs=1, required=False, help="a db to export to")           
 @click.option('--map', nargs=1, required=False, help="a mappingfile for csv")
 @click.option('--sep', nargs=1, required=False, help="which separator is used on csv, default:,")
 @click.option('--cluster', nargs=1, required=False, help="Use a field to cluster records in a folder, default:none")
 def indexDir(dir, dir_out, dir_out_mode, mode, dbtype, profile, db, map, sep, cluster):
     if not dir:
         dir = "./"
-    if dir[-1] != "/":
-        dir += "/"
+    if dir[-1] == os.sep:
+        dir = dir[:-1]
     if not dir_out:
         dir_out = dir
+    elif dir_out[-1] == os.sep:
+        dir_out = dir_out[:-1]
     if not dir_out_mode or dir_out_mode not in ["flat","nested"]:
         dir_out_mode = "flat"
     if not mode:
         mode = "init"
     elif  mode not in ["init","update","export","import-csv"]:
         print('valid modes are init, update, export, import-csv')
         exit()
     if not dbtype or dbtype not in ["path","sqlite","postgres"]:
         dbtype = "path"
     if not db:
         db = dir   
     if not profile or profile not in ["iso19139","dcat"]:
         profile = "iso19139"    
-    print(mode + ' metadata in ' + dir + ' as ' + profile + ' in ' + db)
+    print(mode + ' metadata in ' + dir + ' to ' + dir_out)
 
     if mode=="export":
         if dbtype == 'sqlite':   
             dir_out = os.path.join(dir_out, db)
             createIndexIfDoesntExist(dir_out)
         elif dbtype == "path":
             if not os.path.exists(dir_out): 
@@ -110,22 +112,24 @@
             print('process path: '+ str(file))
             processPath(str(file), deepcopy(coreMetadata), mode, dbtype, dir_out, dir_out_mode, root)
         else:
             # process the file
             fname = str(file)
             if '.' in str(file):
                 base, extension = str(file).rsplit('.', 1)
-                relPath=os.sep.join(base.replace(root,'').split(os.sep)[:-1])
-                fn = base.split('/').pop()
+                relPath = os.path.relpath(os.path.dirname(file), root)
+                if relPath == '1':
+                    relPath == ''
+                fn = base.split(os.sep).pop()
                 #relPath=base.replace(root,'')
                 if extension.lower() in ["yml","yaml","mcf"] and fn != "index":
                     if mode == "export":
                         ### export a file
-                        try:
-                            #if 1==1:
+                        #try:
+                        if 1==1:
                             with open(fname, mode="r", encoding="utf-8") as f:
                                 cnf = yaml.load(f, Loader=SafeLoader)
                                 if not cnf:
                                     cnf = { 'metadata':{ 'identifier': fn } }
                                 elif 'metadata' not in cnf or cnf['metadata'] is None: 
                                     cnf['metadata'] = { 'identifier': fn }
                                 elif 'identifier' not in cnf['metadata'] or cnf['metadata']['identifier'] in [None,""]:
@@ -159,20 +163,20 @@
                                     xml_string = iso_os.write(md)
                                 if dbtype == 'sqlite' or dbtype=='postgres':
                                     insert_or_update(target, dir_out)
                                 elif dbtype == "path":
                                     if dir_out_mode == "flat":
                                         pth = os.path.join(dir_out,safeFileName(md['metadata']['identifier'])+'.xml')
                                     else:
-                                        pth = os.path.join(target_path,os.sep,safeFileName(md['metadata']['identifier'])+'.xml')
+                                        pth = os.path.join(target_path,safeFileName(md['metadata']['identifier'])+'.xml')
                                     with open(pth, 'w+') as ff:
                                         ff.write(xml_string)
                                         print('iso19139 xml generated at '+pth)    
-                        except Exception as e:
-                            print('Failed to create xml:',target_path,os.sep,base+'.xml',e)
+                        #except Exception as e:
+                        #    print('Failed to create xml:',os.path.join(target_path,base+'.xml'),e)
                     elif mode=='update':
                         # a yml should already exist for each spatial file, so only check yml's, not index
                         with open(str(file), mode="r", encoding="utf-8") as f:
                             orig = yaml.load(f, Loader=SafeLoader)
                         # todo: if this fails, we give a warning, or initialise the file again??
                         if not orig:
                             orig = {}
@@ -313,17 +317,17 @@
                             except Exception as e:
                                 print('Failed to dump yaml:',e)
 
                 # mode==init
                 elif extension.lower() in INDEX_FILE_TYPES:
                     print ('Indexing file ' + fname)
                     if (dir_out_mode=='flat'):
-                        outBase = dir_out+os.sep+fn
+                        outBase = os.path.join(dir_out,fn)
                     else:    
-                        outBase = dir_out+os.sep+relPath+os.sep+fn
+                        outBase = os.path.join(dir_out,relPath,fn)
 
                     yf = os.path.join(outBase+'.yml')
                     if not os.path.exists(yf): # only if yml not exists yet
                         # mode init for spatial files without metadata or update
                         cnt = indexSpatialFile(fname, extension) 
                         md = asPGM(cnt)
                     
@@ -340,17 +344,17 @@
                         if len(md['distribution'].keys()) == 0:
                             if webdavUrl:
                                 lnk = webdavUrl+os.sep+relPath+os.sep+fn+'.'+extension
                             else:
                                 lnk = str(file)
                             md['distribution']['local'] = { 'url':lnk, 'type': 'WWW:LINK', 'name':fn+'.'+extension }
 
-                        if not os.path.exists(dir_out+os.sep+relPath):
-                            os.makedirs(dir_out+os.sep+relPath)
-                            print('create folder',dir_out+os.sep+relPath)
+                        if not os.path.exists(os.path.join(dir_out,relPath)):
+                            os.makedirs(os.path.join(dir_out,relPath))
+                            print('create folder',os.path.join(dir_out,relPath))
                         # write yf
                         try:
                             with open(yf, 'w') as f: # todo: use identifier from metadata? if it were extracted from xml for example
                                 yaml.dump(md, f, sort_keys=False)
                         except Exception as e:
                             print('Failed to dump yaml:',e)
                 else:
@@ -400,15 +404,15 @@
                     print('Failed substituting',md,e)    
                 if yMcf:
                     
                     # which folder to write to?
                     fldr = dir_out
                     if cluster not in [None,""] and cluster in md.keys():
                         # todo, safe string, re.sub('[^A-Za-z0-9]+', '', cluster)
-                        fldr += md[cluster] + os.sep
+                        fldr = os.path.join(fldr, md[cluster])
                     if not os.path.isdir(fldr):
                         os.makedirs(fldr)
                         print('folder',fldr,'created')
                     # which id to use
                     # check identifier
                     if not 'metadata' in yMcf:
                         yMcf['metadata'] = {}
@@ -425,16 +429,16 @@
                         for d in domains:
                             myid = myid.split(d+'/')[-1]
 
                     myid = safeFileName(myid)
                     yMcf['metadata']['identifier'] = myid
 
                     # write out the yml
-                    print("Save to file",fldr+myid+'.yml')
-                    with open(fldr+myid+'.yml', 'w+') as f:
+                    print("Save to file",os.path.join(fldr,myid+'.yml'))
+                    with open(os.path.join(fldr,myid+'.yml'), 'w+') as f:
                         yaml.dump(yMcf, f, sort_keys=False)
 
 def insert_or_update(content, db, dbtype):
     """ run a query """
     try:
         if dbtype == 'sqlite':
             conn = sqlite3.connect(db)
```

### Comparing `geodatacrawler-1.1.1/geodatacrawler/schemas/iso19139/__init__.py` & `geodatacrawler-1.1.2/geodatacrawler/schemas/iso19139/__init__.py`

 * *Files identical despite different names*

### Comparing `geodatacrawler-1.1.1/geodatacrawler/schemas/iso19139/contact.j2` & `geodatacrawler-1.1.2/geodatacrawler/schemas/iso19139/contact.j2`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+{% if contact and not contact is string %}
 <gmd:CI_ResponsibleParty>
-  {{ cs.get_freetext('individualName', record['metadata']['language_alternate'], get_charstring(contact.get('individualname'), record['metadata']['language'], record['metadata']['language_alternate'])) }}
-  {{ cs.get_freetext('organisationName', record['metadata']['language_alternate'], get_charstring(contact.get('organization'), record['metadata']['language'], record['metadata']['language_alternate'])) }}
-  {{ cs.get_freetext('positionName', record['metadata']['language_alternate'], get_charstring(contact.get('positionname'), record['metadata']['language'], record['metadata']['language_alternate'])) }}
+  {{ cs.get_freetext('individualName', record['metadata']['language_alternate'], get_charstring(contact['individualname'], record['metadata']['language'], record['metadata']['language_alternate'])) }}
+  {{ cs.get_freetext('organisationName', record['metadata']['language_alternate'], get_charstring(contact['organization'], record['metadata']['language'], record['metadata']['language_alternate'])) }}
+  {{ cs.get_freetext('positionName', record['metadata']['language_alternate'], get_charstring(contact['positionname'], record['metadata']['language'], record['metadata']['language_alternate'])) }}
   <gmd:contactInfo>
     <gmd:CI_Contact>
       {% if contact['phone'] %}
       <gmd:phone>
         <gmd:CI_Telephone>
           {% if contact['phone'] %}
           <gmd:voice>
@@ -47,7 +48,8 @@
       {{ cs.get_freetext('contactInstructions', record['metadata']['language_alternate'], get_charstring(contact.get('contactinstructions'), record['metadata']['language'], record['metadata']['language_alternate'])) }}
     </gmd:CI_Contact>
   </gmd:contactInfo>
   <gmd:role>
     <gmd:CI_RoleCode codeList="http://www.isotc211.org/2005/resources/Codelist/gmxCodelists.xml#CI_RoleCode" codeSpace="ISOTC211/19115" codeListValue="{{ role.split('_') | first }}">{{ role }}</gmd:CI_RoleCode>
   </gmd:role>
 </gmd:CI_ResponsibleParty>
+{% endif %}
```

### Comparing `geodatacrawler-1.1.1/geodatacrawler/schemas/iso19139/main.j2` & `geodatacrawler-1.1.2/geodatacrawler/schemas/iso19139/main.j2`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
   <gmd:hierarchyLevel>
     <gmd:MD_ScopeCode codeList="http://www.isotc211.org/2005/resources/Codelist/gmxCodelists.xml#MD_ScopeCode" codeSpace="ISOTC211/19115" codeListValue="{{ record['metadata']['hierarchylevel'] }}">{{ record['metadata']['hierarchylevel'] }}</gmd:MD_ScopeCode>
   </gmd:hierarchyLevel>
   {% for key, value in record['contact'].items() %}
   {% if key in ['distributor', 'pointOfContact'] %}
   <gmd:contact>
     {% set contact = value %}
-    {% set role = key %}
+    {% set role = contact['role'] or key %}
     {% include "contact.j2" %}
   </gmd:contact>
   {% endif %}
   {% endfor %}
   <gmd:dateStamp>
     {% set datestamp = record['metadata']['datestamp']|normalize_datestring %}
     {% if datestamp|length > 11 %}
```

### Comparing `geodatacrawler-1.1.1/geodatacrawler/templates/class-raster.tpl` & `geodatacrawler-1.1.2/geodatacrawler/templates/class-raster.tpl`

 * *Files identical despite different names*

### Comparing `geodatacrawler-1.1.1/geodatacrawler/templates/csv.j2` & `geodatacrawler-1.1.2/geodatacrawler/templates/csv.j2`

 * *Files identical despite different names*

### Comparing `geodatacrawler-1.1.1/geodatacrawler/templates/default.map` & `geodatacrawler-1.1.2/geodatacrawler/templates/default.map`

 * *Files identical despite different names*

### Comparing `geodatacrawler-1.1.1/geodatacrawler/templates/index.sqlite` & `geodatacrawler-1.1.2/geodatacrawler/templates/index.sqlite`

 * *Files identical despite different names*

### Comparing `geodatacrawler-1.1.1/geodatacrawler/templates/layer.tpl` & `geodatacrawler-1.1.2/geodatacrawler/templates/layer.tpl`

 * *Files identical despite different names*

### Comparing `geodatacrawler-1.1.1/geodatacrawler/upload.py` & `geodatacrawler-1.1.2/geodatacrawler/upload.py`

 * *Files identical despite different names*

### Comparing `geodatacrawler-1.1.1/geodatacrawler/upload_wosis.py` & `geodatacrawler-1.1.2/geodatacrawler/upload_wosis.py`

 * *Files identical despite different names*

### Comparing `geodatacrawler-1.1.1/geodatacrawler/utils.py` & `geodatacrawler-1.1.2/geodatacrawler/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,18 +159,20 @@
 
 
 def wkt2epsg(wkt, epsg='/usr/local/share/proj/epsg', forceProj4=False):
     try:
         crs = CRS.from_wkt(wkt)
         epsg = crs.to_epsg()
     except Exception as e:
-        print('Invalid src (wkt) provided: ', e)
+        print('Invalid src (wkt) provided: ', e,'proj:', wkt)
     if not epsg:
-        if (wkt == 'PROJCS["unnamed",GEOGCS["WGS 84",DATUM["WGS_1984",SPHEROID["WGS 84",6378137,298.257223563,AUTHORITY["EPSG","7030"]],AUTHORITY["EPSG","6326"]],PRIMEM["Greenwich",0],UNIT["degree",0.0174532925199433,AUTHORITY["EPSG","9122"]],AUTHORITY["EPSG","4326"]],PROJECTION["Lambert_Azimuthal_Equal_Area"],PARAMETER["latitude_of_center",5],PARAMETER["longitude_of_center",20],PARAMETER["false_easting",0],PARAMETER["false_northing",0],UNIT["metre",1],AXIS["Easting",EAST],AXIS["Northing",NORTH]]'):
+        if ('GEOGCS["WGS 84",DATUM["WGS_1984",SPHEROID["WGS 84",6378137,298.257223563,AUTHORITY["EPSG","7030"]],AUTHORITY["EPSG","6326"]],PRIMEM["Greenwich",0],UNIT["degree",0.0174532925199433,AUTHORITY["EPSG","9122"]],AUTHORITY["EPSG","4326"]],PROJECTION["Lambert_Azimuthal_Equal_Area"],PARAMETER["latitude_of_center",5],PARAMETER["longitude_of_center",20],PARAMETER["false_easting",0],PARAMETER["false_northing",0],UNIT["metre",1],AXIS["Easting",EAST],AXIS["Northing",NORTH]' in wkt):
             return "epsg:42106"
+        elif ('GEOGCS["GCS_WGS_1984_ellipse",DATUM["WGS_1984",SPHEROID["WGS 84",6378137,298.257223563,AUTHORITY["EPSG","7030"]],AUTHORITY["EPSG","6326"]],PRIMEM["Greenwich",0],UNIT["Degree",0.0174532925199433]],PROJECTION["Interrupted_Goode_Homolosine"],PARAMETER["central_meridian",0],PARAMETER["false_easting",0],PARAMETER["false_northing",0],UNIT["metre",1,AUTHORITY["EPSG","9001"]],AXIS["Easting",EAST],AXIS["Northing",NORTH]' in wkt):
+            return "epsg:54052"
         print('Unable to identify: ' + wkt)
     else:
         return "epsg:" + str(epsg) 
 
 def isDistributionLocal(url, path):
     parsed = urlparse(url, allow_fragments=False)
     fn = str(parsed.path).split('/').pop()
```

### Comparing `geodatacrawler-1.1.1/pyproject.toml` & `geodatacrawler-1.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geodatacrawler"
-version = "1.1.1"
+version = "1.1.2"
 license = "MIT"
 description = "a crawler script to extract and author metadata of spatial datasets"
 authors = ["Paul van Genuchten <genuchten@yahoo.com>"]
 readme = "README.md"
 repository = "https://github.com/pvgenuchten/pyGeoDataCrawler"
 packages = [
     { include = "geodatacrawler" },
```

### Comparing `geodatacrawler-1.1.1/PKG-INFO` & `geodatacrawler-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geodatacrawler
-Version: 1.1.1
+Version: 1.1.2
 Summary: a crawler script to extract and author metadata of spatial datasets
 Home-page: https://github.com/pvgenuchten/pyGeoDataCrawler
 License: MIT
 Author: Paul van Genuchten
 Author-email: genuchten@yahoo.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

