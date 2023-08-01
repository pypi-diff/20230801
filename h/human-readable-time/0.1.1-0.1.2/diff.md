# Comparing `tmp/human_readable_time-0.1.1.tar.gz` & `tmp/human_readable_time-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "human_readable_time-0.1.1.tar", last modified: Tue Aug  1 10:18:33 2023, max compression
+gzip compressed data, was "human_readable_time-0.1.2.tar", last modified: Tue Aug  1 10:27:14 2023, max compression
```

## Comparing `human_readable_time-0.1.1.tar` & `human_readable_time-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 10:18:33.159853 human_readable_time-0.1.1/
--rw-rw-rw-   0        0        0     3469 2023-08-01 10:18:33.063848 human_readable_time-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2079 2023-07-31 17:27:26.000000 human_readable_time-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 10:18:31.434847 human_readable_time-0.1.1/human_readable_time/
--rw-rw-rw-   0        0        0      422 2023-07-31 17:26:38.000000 human_readable_time-0.1.1/human_readable_time/human_readable_time.py
-drwxrwxrwx   0        0        0        0 2023-08-01 10:18:33.051847 human_readable_time-0.1.1/human_readable_time.egg-info/
--rw-rw-rw-   0        0        0     3469 2023-08-01 10:18:29.000000 human_readable_time-0.1.1/human_readable_time.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-08-01 10:18:30.000000 human_readable_time-0.1.1/human_readable_time.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 10:18:29.000000 human_readable_time-0.1.1/human_readable_time.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-08-01 10:18:29.000000 human_readable_time-0.1.1/human_readable_time.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 10:18:33.160846 human_readable_time-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     3608 2023-08-01 10:18:14.000000 human_readable_time-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 10:27:14.076198 human_readable_time-0.1.2/
+-rw-rw-rw-   0        0        0     3505 2023-08-01 10:27:14.072202 human_readable_time-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2115 2023-08-01 10:26:19.000000 human_readable_time-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 10:27:12.633195 human_readable_time-0.1.2/human_readable_time/
+-rw-rw-rw-   0        0        0      422 2023-07-31 17:26:38.000000 human_readable_time-0.1.2/human_readable_time/human_readable_time.py
+drwxrwxrwx   0        0        0        0 2023-08-01 10:27:14.069204 human_readable_time-0.1.2/human_readable_time.egg-info/
+-rw-rw-rw-   0        0        0     3505 2023-08-01 10:27:10.000000 human_readable_time-0.1.2/human_readable_time.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-08-01 10:27:11.000000 human_readable_time-0.1.2/human_readable_time.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 10:27:10.000000 human_readable_time-0.1.2/human_readable_time.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-08-01 10:27:10.000000 human_readable_time-0.1.2/human_readable_time.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 10:27:14.126202 human_readable_time-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     3644 2023-08-01 10:27:04.000000 human_readable_time-0.1.2/setup.py
```

### Comparing `human_readable_time-0.1.1/PKG-INFO` & `human_readable_time-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: human_readable_time
-Version: 0.1.1
+Version: 0.1.2
 Summary: A utility package for human-readable time conversion.
 Home-page: https://github.com/MuGhasemi/human_readable_time
 Author: Muhammad Ghasemi
 Author-email: mughasemi2008@email.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -20,21 +20,21 @@
                     # زمان خوانا
 
                       این یک تابع پایتون است که عددی غیر منفی (ثانیه) را به عنوان ورودی می‌گیرد و زمان را با فرمت خوانا (ساعت:دقیقه:ثانیه) برمی‌گرداند.
 
                       ## چگونه استفاده کنیم
 
                       1. مخزن را در دستگاه محلی خود کلون کنید.
-                      2. تابع `make_readable` را از ماژول `time_utils` وارد کنید.
+                      2. تابع `make_readable` را از ماژول `human_readable_time` وارد کنید.
                       3. تابع `make_readable` را فراخوانی کنید و تعداد ثانیه‌ها را به عنوان آرگومان ارسال کنید.
 
                       مثال:
 
                       ```python
-                      from time_utils import make_readable1 #OR make_readable2
+                      from human_readable_time import make_readable1 #OR make_readable2
 
                       seconds = 3661
                       result = make_readable1(seconds)
                       print(result)  # خروجی: 01:01:01
                       ```
 
                       ## جزئیات تابع
@@ -44,21 +44,21 @@
                       # Human Readable Time
 
                       This is a Python function that takes a non-negative integer representing the number of seconds and returns the time in a human-readable format (HH:MM:SS).
 
                       ## How to Use
 
                       1. Clone the repository to your local machine.
-                      2. Import the `make_readable` function from the `time_utils` module.
+                      2. Import the `make_readable` function from the `human_readable_time` module.
                       3. Call the `make_readable` function and pass the number of seconds as an argument.
 
                       Example:
 
                       ```python
-                      from time_utils import make_readable #OR make_readable2
+                      from human_readable_time import make_readable #OR make_readable2
 
                       seconds = 3661
                       result = make_readable1(seconds)
                       print(result)  # Output: 01:01:01
                       ```
 
                       ## Function Details
```

### Comparing `human_readable_time-0.1.1/README.md` & `human_readable_time-0.1.2/human_readable_time.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,69 @@
-# زمان خوانا
+Metadata-Version: 2.1
+Name: human-readable-time
+Version: 0.1.2
+Summary: A utility package for human-readable time conversion.
+Home-page: https://github.com/MuGhasemi/human_readable_time
+Author: Muhammad Ghasemi
+Author-email: mughasemi2008@email.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/plain
 
-این یک تابع پایتون است که عددی غیر منفی (ثانیه) را به عنوان ورودی می‌گیرد و زمان را با فرمت خوانا (ساعت:دقیقه:ثانیه) برمی‌گرداند.
 
-## چگونه استفاده کنیم
+                    # زمان خوانا
 
-1. مخزن را در دستگاه محلی خود کلون کنید.
-2. تابع `make_readable` را از ماژول `time_utils` وارد کنید.
-3. تابع `make_readable` را فراخوانی کنید و تعداد ثانیه‌ها را به عنوان آرگومان ارسال کنید.
+                      این یک تابع پایتون است که عددی غیر منفی (ثانیه) را به عنوان ورودی می‌گیرد و زمان را با فرمت خوانا (ساعت:دقیقه:ثانیه) برمی‌گرداند.
 
-مثال:
+                      ## چگونه استفاده کنیم
 
-```python
-from time_utils import make_readable1 #OR make_readable2
+                      1. مخزن را در دستگاه محلی خود کلون کنید.
+                      2. تابع `make_readable` را از ماژول `human_readable_time` وارد کنید.
+                      3. تابع `make_readable` را فراخوانی کنید و تعداد ثانیه‌ها را به عنوان آرگومان ارسال کنید.
 
-seconds = 3661
-result = make_readable1(seconds)
-print(result)  # خروجی: 01:01:01
-```
+                      مثال:
 
-## جزئیات تابع
+                      ```python
+                      from human_readable_time import make_readable1 #OR make_readable2
 
-تابع `make_readable` ساعت، دقیقه و ثانیه را از تعداد داده شده ثانیه‌ها محاسبه کرده و آن‌ها را با رشته‌ی خوانا فرمت می‌کند. این تابع از تابع `divmod()` برای محاسبه کارآمد و f-string برای فرمت‌بندی خروجی با صفر اولیه استفاده می‌کند.
+                      seconds = 3661
+                      result = make_readable1(seconds)
+                      print(result)  # خروجی: 01:01:01
+                      ```
 
-# Human Readable Time
+                      ## جزئیات تابع
 
-This is a Python function that takes a non-negative integer representing the number of seconds and returns the time in a human-readable format (HH:MM:SS).
+                      تابع `make_readable` ساعت، دقیقه و ثانیه را از تعداد داده شده ثانیه‌ها محاسبه کرده و آن‌ها را با رشته‌ی خوانا فرمت می‌کند. این تابع از تابع `divmod()` برای محاسبه کارآمد و f-string برای فرمت‌بندی خروجی با صفر اولیه استفاده می‌کند.
 
-## How to Use
+                      # Human Readable Time
 
-1. Clone the repository to your local machine.
-2. Import the `make_readable` function from the `time_utils` module.
-3. Call the `make_readable` function and pass the number of seconds as an argument.
+                      This is a Python function that takes a non-negative integer representing the number of seconds and returns the time in a human-readable format (HH:MM:SS).
 
-Example:
+                      ## How to Use
 
-```python
-from time_utils import make_readable #OR make_readable2
+                      1. Clone the repository to your local machine.
+                      2. Import the `make_readable` function from the `human_readable_time` module.
+                      3. Call the `make_readable` function and pass the number of seconds as an argument.
 
-seconds = 3661
-result = make_readable1(seconds)
-print(result)  # Output: 01:01:01
-```
+                      Example:
 
-## Function Details
+                      ```python
+                      from human_readable_time import make_readable #OR make_readable2
+
+                      seconds = 3661
+                      result = make_readable1(seconds)
+                      print(result)  # Output: 01:01:01
+                      ```
+
+                      ## Function Details
+
+                      The `make_readable` function calculates the hours, minutes, and seconds from the given number of seconds and formats them in a human-readable string. It uses the `divmod()` function for efficient calculation and f-string for formatting the output with leading zeros.
+                      .
+                        
 
-The `make_readable` function calculates the hours, minutes, and seconds from the given number of seconds and formats them in a human-readable string. It uses the `divmod()` function for efficient calculation and f-string for formatting the output with leading zeros.
```

### Comparing `human_readable_time-0.1.1/human_readable_time.egg-info/PKG-INFO` & `human_readable_time-0.1.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,28 @@
-Metadata-Version: 2.1
-Name: human-readable-time
-Version: 0.1.1
-Summary: A utility package for human-readable time conversion.
-Home-page: https://github.com/MuGhasemi/human_readable_time
-Author: Muhammad Ghasemi
-Author-email: mughasemi2008@email.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/plain
-
+from setuptools import setup
 
+setup(
+    name='human_readable_time',
+    version='0.1.2',
+    description='A utility package for human-readable time conversion.',
+    long_description='''
                     # زمان خوانا
 
                       این یک تابع پایتون است که عددی غیر منفی (ثانیه) را به عنوان ورودی می‌گیرد و زمان را با فرمت خوانا (ساعت:دقیقه:ثانیه) برمی‌گرداند.
 
                       ## چگونه استفاده کنیم
 
                       1. مخزن را در دستگاه محلی خود کلون کنید.
-                      2. تابع `make_readable` را از ماژول `time_utils` وارد کنید.
+                      2. تابع `make_readable` را از ماژول `human_readable_time` وارد کنید.
                       3. تابع `make_readable` را فراخوانی کنید و تعداد ثانیه‌ها را به عنوان آرگومان ارسال کنید.
 
                       مثال:
 
                       ```python
-                      from time_utils import make_readable1 #OR make_readable2
+                      from human_readable_time import make_readable1 #OR make_readable2
 
                       seconds = 3661
                       result = make_readable1(seconds)
                       print(result)  # خروجی: 01:01:01
                       ```
 
                       ## جزئیات تابع
@@ -44,26 +32,41 @@
                       # Human Readable Time
 
                       This is a Python function that takes a non-negative integer representing the number of seconds and returns the time in a human-readable format (HH:MM:SS).
 
                       ## How to Use
 
                       1. Clone the repository to your local machine.
-                      2. Import the `make_readable` function from the `time_utils` module.
+                      2. Import the `make_readable` function from the `human_readable_time` module.
                       3. Call the `make_readable` function and pass the number of seconds as an argument.
 
                       Example:
 
                       ```python
-                      from time_utils import make_readable #OR make_readable2
+                      from human_readable_time import make_readable #OR make_readable2
 
                       seconds = 3661
                       result = make_readable1(seconds)
                       print(result)  # Output: 01:01:01
                       ```
 
                       ## Function Details
 
                       The `make_readable` function calculates the hours, minutes, and seconds from the given number of seconds and formats them in a human-readable string. It uses the `divmod()` function for efficient calculation and f-string for formatting the output with leading zeros.
                       .
-                        
-
+                        ''',
+    long_description_content_type = "text/plain",
+    author='Muhammad Ghasemi',
+    author_email='mughasemi2008@email.com',
+    url='https://github.com/MuGhasemi/human_readable_time',
+    packages=['human_readable_time'],
+    install_requires=[],
+    classifiers=[
+        'Development Status :: 3 - Alpha',
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+    ],
+)
```

