# Comparing `tmp/hertz-1.0.0.tar.gz` & `tmp/hertz-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hertz-1.0.0.tar", last modified: Mon Jul 17 21:58:11 2023, max compression
+gzip compressed data, was "hertz-1.1.1.tar", last modified: Tue Aug  1 18:58:38 2023, max compression
```

## Comparing `hertz-1.0.0.tar` & `hertz-1.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 21:58:11.303758 hertz-1.0.0/
--rw-rw-rw-   0        0        0     1095 2023-07-17 21:52:01.000000 hertz-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      335 2023-07-17 21:58:11.303758 hertz-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-17 21:58:11.292785 hertz-1.0.0/hertz/
--rw-rw-rw-   0        0        0     3486 2023-07-17 21:57:32.000000 hertz-1.0.0/hertz/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 21:58:11.300765 hertz-1.0.0/hertz.egg-info/
--rw-rw-rw-   0        0        0      335 2023-07-17 21:58:11.000000 hertz-1.0.0/hertz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      150 2023-07-17 21:58:11.000000 hertz-1.0.0/hertz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 21:58:11.000000 hertz-1.0.0/hertz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-17 21:58:11.000000 hertz-1.0.0/hertz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 21:58:11.304753 hertz-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      576 2023-07-17 21:57:51.000000 hertz-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 18:58:38.564184 hertz-1.1.1/
+-rw-rw-rw-   0        0        0     1095 2023-07-17 21:52:01.000000 hertz-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0      334 2023-08-01 18:58:38.564184 hertz-1.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-01 18:58:38.555243 hertz-1.1.1/hertz/
+-rw-rw-rw-   0        0        0     3586 2023-08-01 18:58:04.000000 hertz-1.1.1/hertz/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 18:58:38.562190 hertz-1.1.1/hertz.egg-info/
+-rw-rw-rw-   0        0        0      334 2023-08-01 18:58:38.000000 hertz-1.1.1/hertz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      150 2023-08-01 18:58:38.000000 hertz-1.1.1/hertz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 18:58:38.000000 hertz-1.1.1/hertz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-08-01 18:58:38.000000 hertz-1.1.1/hertz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 18:58:38.565218 hertz-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      575 2023-07-26 23:20:53.000000 hertz-1.1.1/setup.py
```

### Comparing `hertz-1.0.0/LICENSE` & `hertz-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hertz-1.0.0/hertz/__init__.py` & `hertz-1.1.1/hertz/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,23 +10,24 @@
 foo += GHz('3')
 print(foo.in_ghz) # prints 3.001204
 """
 
 from functools import partial
 
 
-__version__ = '1.0.0'
+__version__ = '1.1.1'
+
 
 class Frequency(float):
     """Represents a generic frequency value.
     The constructor allows you to specify a unit, and you may access the value with convenience properties like in_khz.
     Directly accessing the value results in a megahertz value.
     """
     prefixes = {
-        '': 1e-6, 'k': 1e-3, 'm': 1, 'g': 1e3, 'p': 1e6
+        '': 1e-6, 'k': 1e-3, 'm': 1, 'g': 1e3, 't': 1e6
     }
 
     def __new__(cls, scalar, units: str = 'MHz'):
         """
         :param scalar: something you could pass to float()
         :param units: a string like "G" or "kHz". "MHz" and "mHz" both result in megahertz and not millihertz.
         """
@@ -73,14 +74,17 @@
 
     def __ceil__(self):
         return Frequency(super().__ceil__(), 'MHz')
 
     def __divmod__(self, other):
         return Frequency(super().__divmod__(other), 'MHz')
 
+    def __truediv__(self, other):
+        return Frequency(super().__truediv__(other), 'MHz')
+
     def __floor__(self):
         return Frequency(super().__floor__(), 'MHz')
 
     def __floordiv__(self, other):
         return Frequency(super().__floordiv__(other), 'MHz')
 
     def __mul__(self, other):
@@ -100,8 +104,8 @@
 
 
 '''Hz(5) is shorthand for Frequency(5, 'Hz')'''
 Hz = partial(Frequency, units='Hz')
 KHz = kHz = partial(Frequency, units='KHz')
 MHz = partial(Frequency, units='MHz')
 GHz = partial(Frequency, units='GHz')
-PHz = partial(Frequency, units='PHz')
+THz = partial(Frequency, units='THz')
```

### Comparing `hertz-1.0.0/setup.py` & `hertz-1.1.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import hertz
 
 
 if __name__ == '__main__':
     setuptools.setup(
         name="hertz",
         version=hertz.__version__,
-        author="Andrew Blomenberg",
+        author="Andrew and Izick",
         author_email="andrewBlomen@gmail.com",
         description="A simple, standard, and handy way to represent Hertz, kHz, GHz, etc",
         install_requires=[],
         packages=setuptools.find_packages(),
         classifiers=[
             "Programming Language :: Python :: 3",
         ],
```

