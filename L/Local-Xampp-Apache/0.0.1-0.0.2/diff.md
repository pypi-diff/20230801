# Comparing `tmp/Local_Xampp_Apache-0.0.1.tar.gz` & `tmp/Local_Xampp_Apache-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Local_Xampp_Apache-0.0.1.tar", last modified: Tue Aug  1 16:44:25 2023, max compression
+gzip compressed data, was "Local_Xampp_Apache-0.0.2.tar", last modified: Tue Aug  1 17:04:54 2023, max compression
```

## Comparing `Local_Xampp_Apache-0.0.1.tar` & `Local_Xampp_Apache-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 16:44:25.562987 Local_Xampp_Apache-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-08-01 16:44:25.545969 Local_Xampp_Apache-0.0.1/Local_Xampp_Apache.egg-info/
--rw-rw-rw-   0        0        0      325 2023-08-01 16:44:25.000000 Local_Xampp_Apache-0.0.1/Local_Xampp_Apache.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      340 2023-08-01 16:44:25.000000 Local_Xampp_Apache-0.0.1/Local_Xampp_Apache.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 16:44:25.000000 Local_Xampp_Apache-0.0.1/Local_Xampp_Apache.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-08-01 16:44:25.000000 Local_Xampp_Apache-0.0.1/Local_Xampp_Apache.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       51 2023-08-01 16:44:25.000000 Local_Xampp_Apache-0.0.1/Local_Xampp_Apache.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-08-01 16:44:25.000000 Local_Xampp_Apache-0.0.1/Local_Xampp_Apache.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      325 2023-08-01 16:44:25.561974 Local_Xampp_Apache-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-08-01 16:22:15.000000 Local_Xampp_Apache-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-08-01 16:44:25.563978 Local_Xampp_Apache-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      759 2023-08-01 16:32:36.000000 Local_Xampp_Apache-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 16:44:25.551971 Local_Xampp_Apache-0.0.1/src/
--rw-rw-rw-   0        0        0        0 2023-08-01 16:21:41.000000 Local_Xampp_Apache-0.0.1/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 16:44:25.556967 Local_Xampp_Apache-0.0.1/src/lib/
--rw-rw-rw-   0        0        0     1148 2023-08-01 14:50:59.000000 Local_Xampp_Apache-0.0.1/src/lib/Commands.py
--rw-rw-rw-   0        0        0        0 2023-08-01 16:22:02.000000 Local_Xampp_Apache-0.0.1/src/lib/__init__.py
--rw-rw-rw-   0        0        0     1350 2023-08-01 16:42:20.000000 Local_Xampp_Apache-0.0.1/src/main.py
+drwxrwxrwx   0        0        0        0 2023-08-01 17:04:54.144462 Local_Xampp_Apache-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-08-01 17:04:54.126877 Local_Xampp_Apache-0.0.2/Local_Xampp_Apache.egg-info/
+-rw-rw-rw-   0        0        0      325 2023-08-01 17:04:53.000000 Local_Xampp_Apache-0.0.2/Local_Xampp_Apache.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-08-01 17:04:53.000000 Local_Xampp_Apache-0.0.2/Local_Xampp_Apache.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 17:04:53.000000 Local_Xampp_Apache-0.0.2/Local_Xampp_Apache.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-08-01 17:04:53.000000 Local_Xampp_Apache-0.0.2/Local_Xampp_Apache.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       51 2023-08-01 17:04:53.000000 Local_Xampp_Apache-0.0.2/Local_Xampp_Apache.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-08-01 17:04:53.000000 Local_Xampp_Apache-0.0.2/Local_Xampp_Apache.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      325 2023-08-01 17:04:54.143464 Local_Xampp_Apache-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-08-01 16:22:15.000000 Local_Xampp_Apache-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-01 17:04:54.144462 Local_Xampp_Apache-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      759 2023-08-01 17:04:49.000000 Local_Xampp_Apache-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 17:04:54.131203 Local_Xampp_Apache-0.0.2/src/
+-rw-rw-rw-   0        0        0        0 2023-08-01 16:21:41.000000 Local_Xampp_Apache-0.0.2/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 17:04:54.141459 Local_Xampp_Apache-0.0.2/src/lib/
+-rw-rw-rw-   0        0        0     1148 2023-08-01 14:50:59.000000 Local_Xampp_Apache-0.0.2/src/lib/Commands.py
+-rw-rw-rw-   0        0        0        0 2023-08-01 16:22:02.000000 Local_Xampp_Apache-0.0.2/src/lib/__init__.py
+-rw-rw-rw-   0        0        0     1721 2023-08-01 17:04:00.000000 Local_Xampp_Apache-0.0.2/src/main.py
```

### Comparing `Local_Xampp_Apache-0.0.1/setup.py` & `Local_Xampp_Apache-0.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open("requirements.txt") as f:
     required_packages = f.read().splitlines()
 
 
 
 setup(
     name="Local_Xampp_Apache",
-    version="0.0.1",
+    version="0.0.2",
     author="Sridhar",
     author_email="sridhardscv@gmail.com",
     description="Access the Windows XamPP Apache Server via Command lines",
     # long_description="A longer description or README for your package",
     long_description_content_type="text/markdown",
     url="https://git.selfmade.ninja/SRIDHARDSCV/automate_xampp_windows",
     packages=find_packages(),
```

### Comparing `Local_Xampp_Apache-0.0.1/src/lib/Commands.py` & `Local_Xampp_Apache-0.0.2/src/lib/Commands.py`

 * *Files identical despite different names*

### Comparing `Local_Xampp_Apache-0.0.1/src/main.py` & `Local_Xampp_Apache-0.0.2/src/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -39,9 +39,21 @@
     elif args.command == "Is_run":
         Is_Apache_run()
     elif args.command == "Stop":
         Apache_stop()
     else:
         print("Invalid command. Available commands: Start_Apache,Is_Apache_run,Stop_Apache")
 
+
+def is_xampp_installed():
+    try:
+        output = subprocess.check_output("where xampp-control.exe", shell=True, text=True)
+        return True
+    except subprocess.CalledProcessError:
+        return False
+
+
 if __name__ == "__main__":
-    main()
+    if is_xampp_installed():
+        main()
+    else:
+        raise Exception("Xampp is Not installed in our System ..\nINstall the Default path of the Xampp")
```

