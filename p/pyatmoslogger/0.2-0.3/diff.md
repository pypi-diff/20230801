# Comparing `tmp/pyatmoslogger-0.2.tar.gz` & `tmp/pyatmoslogger-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyatmoslogger-0.2.tar", max compression
+gzip compressed data, was "pyatmoslogger-0.3.tar", max compression
```

## Comparing `pyatmoslogger-0.2.tar` & `pyatmoslogger-0.3.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     1060 2023-07-12 08:26:48.057281 pyatmoslogger-0.2/LICENSE.txt
--rw-r--r--   0        0        0      760 2023-07-12 08:26:48.057281 pyatmoslogger-0.2/README.md
--rw-r--r--   0        0        0      146 2023-07-12 08:26:48.057281 pyatmoslogger-0.2/pyAtmosLogger/__init__.py
--rw-r--r--   0        0        0       71 2023-07-12 08:26:48.057281 pyatmoslogger-0.2/pyAtmosLogger/instruments/__init__.py
--rw-r--r--   0        0        0      184 2023-07-12 08:26:48.057281 pyatmoslogger-0.2/pyAtmosLogger/instruments/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    13479 2023-07-12 08:26:48.057281 pyatmoslogger-0.2/pyAtmosLogger/instruments/__pycache__/ott_parsivel2_default.cpython-39.pyc
--rw-r--r--   0        0        0     2225 2023-07-12 08:26:48.057281 pyatmoslogger-0.2/pyAtmosLogger/instruments/__pycache__/pyAtmosLogger_dummy_1.cpython-39.pyc
--rw-r--r--   0        0        0    20180 2023-07-12 08:26:48.057281 pyatmoslogger-0.2/pyAtmosLogger/instruments/ott_parsivel2_actris.py
--rw-r--r--   0        0        0     2939 2023-07-12 08:26:48.057281 pyatmoslogger-0.2/pyAtmosLogger/instruments/pyAtmosLogger_dummy_1.py
--rw-r--r--   0        0        0     1238 2023-07-12 08:26:48.057281 pyatmoslogger-0.2/pyAtmosLogger/pyAtmosLogger.py
--rw-r--r--   0        0        0       19 2023-07-12 08:26:48.057281 pyatmoslogger-0.2/pyAtmosLogger/utils/__init__.py
--rw-r--r--   0        0        0     1174 2023-07-12 08:26:48.061281 pyatmoslogger-0.2/pyAtmosLogger/utils/utils.py
--rw-r--r--   0        0        0      763 2023-07-12 08:26:48.061281 pyatmoslogger-0.2/pyproject.toml
--rw-r--r--   0        0        0     1766 1970-01-01 00:00:00.000000 pyatmoslogger-0.2/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-08-01 12:49:37.834036 pyatmoslogger-0.3/LICENSE.txt
+-rw-r--r--   0        0        0      924 2023-08-01 12:49:37.834036 pyatmoslogger-0.3/README.md
+-rw-r--r--   0        0        0        0 2023-08-01 12:49:37.838036 pyatmoslogger-0.3/pyAtmosLogger/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:49:37.838036 pyatmoslogger-0.3/pyAtmosLogger/instruments/__init__.py
+-rw-r--r--   0        0        0     4225 2023-08-01 12:49:37.838036 pyatmoslogger-0.3/pyAtmosLogger/instruments/bronkhorst_mfc_default.py
+-rw-r--r--   0        0        0    20114 2023-08-01 12:49:37.838036 pyatmoslogger-0.3/pyAtmosLogger/instruments/ott_parsivel2_actris.py
+-rw-r--r--   0        0        0     2939 2023-08-01 12:49:37.838036 pyatmoslogger-0.3/pyAtmosLogger/instruments/pyAtmosLogger_dummy_1.py
+-rw-r--r--   0        0        0    11147 2023-08-01 12:49:37.838036 pyatmoslogger-0.3/pyAtmosLogger/instruments/tsi_ops3330_default.py
+-rw-r--r--   0        0        0     1254 2023-08-01 12:49:37.838036 pyatmoslogger-0.3/pyAtmosLogger/pyAtmosLogger.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:49:37.838036 pyatmoslogger-0.3/pyAtmosLogger/utils/__init__.py
+-rw-r--r--   0        0        0     2413 2023-08-01 12:49:37.838036 pyatmoslogger-0.3/pyAtmosLogger/utils/utils.py
+-rw-r--r--   0        0        0      821 2023-08-01 12:49:37.838036 pyatmoslogger-0.3/pyproject.toml
+-rw-r--r--   0        0        0     2118 1970-01-01 00:00:00.000000 pyatmoslogger-0.3/PKG-INFO
```

### Comparing `pyatmoslogger-0.2/LICENSE.txt` & `pyatmoslogger-0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyatmoslogger-0.2/pyAtmosLogger/instruments/ott_parsivel2_actris.py` & `pyatmoslogger-0.3/pyAtmosLogger/instruments/ott_parsivel2_actris.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,18 +175,18 @@
  		                               'long_name': "velocity class width"}
         ds.dwidth.attrs              = {'units': "mm" ,
  		                               'long_name': "volume equivalent diameter class width"}
         
         for attr in self.configuration["attributes"]:
             ds.attrs[attr] = self.configuration["attributes"][attr]
         now = dt.datetime.now()
-        ds.attrs["Processing_date"] = now.strftime("%Y-%m-%d %H:%M:%S") 
-        ds.attrs["Processing_software"] = "pyAtmosLogger"
-        ds.attrs["Processing_software_version"] = "v0.1"
         ds.attrs["Instrument_serial_number"] = ds.serial_no[1]
+        dsAttributes = ds.attrs
+        dsAttributes.update(getPyAtmosLoggerAttributes())
+        ds.attrs = dsAttributes
         #save file
         ncFilePath = checkNcFolder(self.configuration, file)        
         ds.to_netcdf(ncFilePath, format="NETCDF4")
     def convertMultipleFiles(self):
          """Method to convert multiple-file csv-data to netCDF."""
          nDays = self.configuration["storage"]["ncConversionDays"]
          fileList = glob.glob(self.configuration["storage"]["csvStoragePath"]+'/**/*.csv', recursive=True)
```

### Comparing `pyatmoslogger-0.2/pyAtmosLogger/instruments/pyAtmosLogger_dummy_1.py` & `pyatmoslogger-0.3/pyAtmosLogger/instruments/pyAtmosLogger_dummy_1.py`

 * *Files identical despite different names*

### Comparing `pyatmoslogger-0.2/pyAtmosLogger/pyAtmosLogger.py` & `pyatmoslogger-0.3/pyAtmosLogger/pyAtmosLogger.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,16 +14,16 @@
     """
     parser = argparse.ArgumentParser(
         prog='python3 pyAtmosLogger.py',
         description='Python Package for automatic serial data logging to csv file and converting to netCDF',
     )
     parser.add_argument("-m", "--mode", help = "selct operation mode", choices=["log", "convert"], default="log")
     parser.add_argument("-p", "--path", help = "path to config file", required=True)
-    
     args = vars(parser.parse_args())
+    printCLIHeader()
     # select instrument class
     #instrumentFile = getInstrumentFile(args["path"])
     config = loadConfig(args["path"])
     #import instrument file
     moduleName = config["instrument"]["instrumentFile"][:-3]
     module = importlib.import_module("pyAtmosLogger.instruments."+moduleName)
     classObject = getattr(module, moduleName)
```

