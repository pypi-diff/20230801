# Comparing `tmp/blurhash-python-1.2.0.tar.gz` & `tmp/blurhash-python-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blurhash-python-1.2.0.tar", last modified: Tue Apr  4 10:43:08 2023, max compression
+gzip compressed data, was "blurhash-python-1.2.1.tar", last modified: Tue Aug  1 11:18:17 2023, max compression
```

## Comparing `blurhash-python-1.2.0.tar` & `blurhash-python-1.2.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 lautat    (1000) lautat    (1000)        0 2023-04-04 10:43:08.828248 blurhash-python-1.2.0/
--rw-r--r--   0 lautat    (1000) lautat    (1000)     1224 2023-04-04 07:14:33.000000 blurhash-python-1.2.0/.gitignore
--rw-r--r--   0 lautat    (1000) lautat    (1000)     1076 2023-04-04 07:14:33.000000 blurhash-python-1.2.0/LICENSE
--rw-r--r--   0 lautat    (1000) lautat    (1000)       30 2023-04-04 07:14:33.000000 blurhash-python-1.2.0/MANIFEST.in
--rw-r--r--   0 lautat    (1000) lautat    (1000)     2130 2023-04-04 10:43:08.828248 blurhash-python-1.2.0/PKG-INFO
--rw-r--r--   0 lautat    (1000) lautat    (1000)      194 2023-04-04 07:14:33.000000 blurhash-python-1.2.0/Pipfile
--rw-r--r--   0 lautat    (1000) lautat    (1000)     1388 2023-04-04 07:14:33.000000 blurhash-python-1.2.0/README.md
--rwxr-xr-x   0 lautat    (1000) lautat    (1000)      788 2023-04-04 10:36:25.000000 blurhash-python-1.2.0/build.sh
--rwxr-xr-x   0 lautat    (1000) lautat    (1000)      288 2023-04-04 10:39:59.000000 blurhash-python-1.2.0/docker-build.sh
--rw-r--r--   0 lautat    (1000) lautat    (1000)      100 2023-04-04 07:14:33.000000 blurhash-python-1.2.0/pyproject.toml
--rw-r--r--   0 lautat    (1000) lautat    (1000)       63 2023-04-04 10:43:08.828248 blurhash-python-1.2.0/setup.cfg
--rwxr-xr-x   0 lautat    (1000) lautat    (1000)     1370 2023-04-04 07:30:05.000000 blurhash-python-1.2.0/setup.py
-drwxr-xr-x   0 lautat    (1000) lautat    (1000)        0 2023-04-04 10:43:08.828248 blurhash-python-1.2.0/src/
-drwxr-xr-x   0 lautat    (1000) lautat    (1000)        0 2023-04-04 10:43:08.828248 blurhash-python-1.2.0/src/blurhash/
--rw-r--r--   0 lautat    (1000) lautat    (1000)     3473 2023-04-04 07:14:33.000000 blurhash-python-1.2.0/src/blurhash/__init__.py
--rw-r--r--   0 lautat    (1000) lautat    (1000)      160 2023-04-04 10:43:08.000000 blurhash-python-1.2.0/src/blurhash/_version.py
-drwxr-xr-x   0 lautat    (1000) lautat    (1000)        0 2023-04-04 10:43:08.828248 blurhash-python-1.2.0/src/blurhash_python.egg-info/
--rw-r--r--   0 lautat    (1000) lautat    (1000)     2130 2023-04-04 10:43:08.000000 blurhash-python-1.2.0/src/blurhash_python.egg-info/PKG-INFO
--rw-r--r--   0 lautat    (1000) lautat    (1000)      515 2023-04-04 10:43:08.000000 blurhash-python-1.2.0/src/blurhash_python.egg-info/SOURCES.txt
--rw-r--r--   0 lautat    (1000) lautat    (1000)        1 2023-04-04 10:43:08.000000 blurhash-python-1.2.0/src/blurhash_python.egg-info/dependency_links.txt
--rw-r--r--   0 lautat    (1000) lautat    (1000)       34 2023-04-04 10:43:08.000000 blurhash-python-1.2.0/src/blurhash_python.egg-info/requires.txt
--rw-r--r--   0 lautat    (1000) lautat    (1000)        9 2023-04-04 10:43:08.000000 blurhash-python-1.2.0/src/blurhash_python.egg-info/top_level.txt
--rw-r--r--   0 lautat    (1000) lautat    (1000)     2094 2023-04-04 07:14:33.000000 blurhash-python-1.2.0/src/build_blurhash.py
--rw-r--r--   0 lautat    (1000) lautat    (1000)      610 2023-04-04 07:14:33.000000 blurhash-python-1.2.0/src/common.h
--rw-r--r--   0 lautat    (1000) lautat    (1000)     4351 2023-04-04 07:14:33.000000 blurhash-python-1.2.0/src/decode.c
--rw-r--r--   0 lautat    (1000) lautat    (1000)     3837 2023-04-04 07:14:33.000000 blurhash-python-1.2.0/src/encode.c
-drwxr-xr-x   0 lautat    (1000) lautat    (1000)        0 2023-04-04 10:43:08.828248 blurhash-python-1.2.0/tests/
--rw-r--r--   0 lautat    (1000) lautat    (1000)   123718 2023-04-04 07:14:33.000000 blurhash-python-1.2.0/tests/pic2.png
--rw-r--r--   0 lautat    (1000) lautat    (1000)    42935 2023-04-04 07:14:33.000000 blurhash-python-1.2.0/tests/pic2_bw.png
--rw-r--r--   0 lautat    (1000) lautat    (1000)     1537 2023-04-04 07:14:33.000000 blurhash-python-1.2.0/tests/test_decode.py
--rw-r--r--   0 lautat    (1000) lautat    (1000)     1294 2023-04-04 07:14:33.000000 blurhash-python-1.2.0/tests/test_encode.py
--rw-r--r--   0 lautat    (1000) lautat    (1000)       90 2023-04-04 07:29:48.000000 blurhash-python-1.2.0/tox.ini
+drwxr-xr-x   0 lautat    (1000) lautat    (1000)        0 2023-08-01 11:18:17.601873 blurhash-python-1.2.1/
+-rw-r--r--   0 lautat    (1000) lautat    (1000)     1224 2023-04-04 07:14:33.000000 blurhash-python-1.2.1/.gitignore
+-rw-r--r--   0 lautat    (1000) lautat    (1000)     1076 2023-04-04 07:14:33.000000 blurhash-python-1.2.1/LICENSE
+-rw-r--r--   0 lautat    (1000) lautat    (1000)       30 2023-04-04 07:14:33.000000 blurhash-python-1.2.1/MANIFEST.in
+-rw-r--r--   0 lautat    (1000) lautat    (1000)     2130 2023-08-01 11:18:17.601873 blurhash-python-1.2.1/PKG-INFO
+-rw-r--r--   0 lautat    (1000) lautat    (1000)      194 2023-04-04 07:14:33.000000 blurhash-python-1.2.1/Pipfile
+-rw-r--r--   0 lautat    (1000) lautat    (1000)     1388 2023-04-04 07:14:33.000000 blurhash-python-1.2.1/README.md
+-rwxr-xr-x   0 lautat    (1000) lautat    (1000)      788 2023-04-04 10:36:25.000000 blurhash-python-1.2.1/build.sh
+-rwxr-xr-x   0 lautat    (1000) lautat    (1000)      288 2023-04-04 10:39:59.000000 blurhash-python-1.2.1/docker-build.sh
+-rw-r--r--   0 lautat    (1000) lautat    (1000)      100 2023-04-04 07:14:33.000000 blurhash-python-1.2.1/pyproject.toml
+-rw-r--r--   0 lautat    (1000) lautat    (1000)       63 2023-08-01 11:18:17.601873 blurhash-python-1.2.1/setup.cfg
+-rwxr-xr-x   0 lautat    (1000) lautat    (1000)     1370 2023-04-04 07:30:05.000000 blurhash-python-1.2.1/setup.py
+drwxr-xr-x   0 lautat    (1000) lautat    (1000)        0 2023-08-01 11:18:17.601873 blurhash-python-1.2.1/src/
+drwxr-xr-x   0 lautat    (1000) lautat    (1000)        0 2023-08-01 11:18:17.601873 blurhash-python-1.2.1/src/blurhash/
+-rw-r--r--   0 lautat    (1000) lautat    (1000)     3573 2023-08-01 10:59:59.000000 blurhash-python-1.2.1/src/blurhash/__init__.py
+-rw-r--r--   0 lautat    (1000) lautat    (1000)      160 2023-08-01 11:18:17.000000 blurhash-python-1.2.1/src/blurhash/_version.py
+drwxr-xr-x   0 lautat    (1000) lautat    (1000)        0 2023-08-01 11:18:17.601873 blurhash-python-1.2.1/src/blurhash_python.egg-info/
+-rw-r--r--   0 lautat    (1000) lautat    (1000)     2130 2023-08-01 11:18:17.000000 blurhash-python-1.2.1/src/blurhash_python.egg-info/PKG-INFO
+-rw-r--r--   0 lautat    (1000) lautat    (1000)      515 2023-08-01 11:18:17.000000 blurhash-python-1.2.1/src/blurhash_python.egg-info/SOURCES.txt
+-rw-r--r--   0 lautat    (1000) lautat    (1000)        1 2023-08-01 11:18:17.000000 blurhash-python-1.2.1/src/blurhash_python.egg-info/dependency_links.txt
+-rw-r--r--   0 lautat    (1000) lautat    (1000)       34 2023-08-01 11:18:17.000000 blurhash-python-1.2.1/src/blurhash_python.egg-info/requires.txt
+-rw-r--r--   0 lautat    (1000) lautat    (1000)        9 2023-08-01 11:18:17.000000 blurhash-python-1.2.1/src/blurhash_python.egg-info/top_level.txt
+-rw-r--r--   0 lautat    (1000) lautat    (1000)     2278 2023-08-01 11:01:51.000000 blurhash-python-1.2.1/src/build_blurhash.py
+-rw-r--r--   0 lautat    (1000) lautat    (1000)      610 2023-04-04 07:14:33.000000 blurhash-python-1.2.1/src/common.h
+-rw-r--r--   0 lautat    (1000) lautat    (1000)     4351 2023-04-04 07:14:33.000000 blurhash-python-1.2.1/src/decode.c
+-rw-r--r--   0 lautat    (1000) lautat    (1000)     3861 2023-08-01 11:05:10.000000 blurhash-python-1.2.1/src/encode.c
+drwxr-xr-x   0 lautat    (1000) lautat    (1000)        0 2023-08-01 11:18:17.601873 blurhash-python-1.2.1/tests/
+-rw-r--r--   0 lautat    (1000) lautat    (1000)   123718 2023-04-04 07:14:33.000000 blurhash-python-1.2.1/tests/pic2.png
+-rw-r--r--   0 lautat    (1000) lautat    (1000)    42935 2023-04-04 07:14:33.000000 blurhash-python-1.2.1/tests/pic2_bw.png
+-rw-r--r--   0 lautat    (1000) lautat    (1000)     1537 2023-04-04 07:14:33.000000 blurhash-python-1.2.1/tests/test_decode.py
+-rw-r--r--   0 lautat    (1000) lautat    (1000)     1294 2023-04-04 07:14:33.000000 blurhash-python-1.2.1/tests/test_encode.py
+-rw-r--r--   0 lautat    (1000) lautat    (1000)       90 2023-04-04 07:29:48.000000 blurhash-python-1.2.1/tox.ini
```

### Comparing `blurhash-python-1.2.0/.gitignore` & `blurhash-python-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `blurhash-python-1.2.0/LICENSE` & `blurhash-python-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `blurhash-python-1.2.0/PKG-INFO` & `blurhash-python-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blurhash-python
-Version: 1.2.0
+Version: 1.2.1
 Summary: BlurHash encoder implementation for Python
 Home-page: https://blurha.sh
 Author: Atte Lautanala
 Author-email: atte.lautanala@wolt.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `blurhash-python-1.2.0/README.md` & `blurhash-python-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `blurhash-python-1.2.0/build.sh` & `blurhash-python-1.2.1/build.sh`

 * *Files identical despite different names*

### Comparing `blurhash-python-1.2.0/setup.py` & `blurhash-python-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `blurhash-python-1.2.0/src/blurhash/__init__.py` & `blurhash-python-1.2.1/src/blurhash/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,17 +43,25 @@
 
     rgb = _ffi.new('uint8_t[]', rgb_data)
     bytes_per_row = _ffi.cast('size_t', width * 3)
     width = _ffi.cast('int', width)
     height = _ffi.cast('int', height)
     x_components = _ffi.cast('int', x_components)
     y_components = _ffi.cast('int', y_components)
+    destination = _ffi.new("char[]", 2 + 4 + (9 * 9 - 1) * 2 + 1)
 
-    result = _lib.create_hash_from_pixels(x_components, y_components, width,
-                                          height, rgb, bytes_per_row)
+    result = _lib.create_hash_from_pixels(
+        x_components,
+        y_components,
+        width,
+        height,
+        rgb,
+        bytes_per_row,
+        destination,
+    )
 
     if result == _ffi.NULL:
         raise ValueError('Invalid x_components or y_components')
 
     return _ffi.string(result).decode()
```

### Comparing `blurhash-python-1.2.0/src/blurhash_python.egg-info/PKG-INFO` & `blurhash-python-1.2.1/src/blurhash_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blurhash-python
-Version: 1.2.0
+Version: 1.2.1
 Summary: BlurHash encoder implementation for Python
 Home-page: https://blurha.sh
 Author: Atte Lautanala
 Author-email: atte.lautanala@wolt.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `blurhash-python-1.2.0/src/blurhash_python.egg-info/SOURCES.txt` & `blurhash-python-1.2.1/src/blurhash_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blurhash-python-1.2.0/src/build_blurhash.py` & `blurhash-python-1.2.1/src/build_blurhash.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,28 +8,30 @@
 ffibuilder.set_source('blurhash._functions', '''
     #include <stdbool.h>
 
     #include "common.h"
 
     const char* blurHashForPixels(int x_components, int y_components,
                                   int width, int height,
-                                  uint8_t * rgb, size_t bytesPerRow);
+                                  uint8_t * rgb, size_t bytesPerRow,
+                                  char* destination);
 
     int decodeToArray(const char* blurhash, int width, int height,
                       int punch, int n_channels,
                       uint8_t * pixel_array);
 
     bool isValidBlurhash(const char* blurhash);
 
 
     const char* create_hash_from_pixels(int x_components, int y_components,
                                         int width, int height, uint8_t* rgb,
-                                        size_t bytes_per_row) {
+                                        size_t bytes_per_row,
+                                        char* destination) {
         return blurHashForPixels(x_components, y_components, width, height,
-                                 rgb, bytes_per_row);
+                                 rgb, bytes_per_row, destination);
     }
 
     int create_pixels_from_blurhash(const char * blurhash, int width,
                                     int height, int punch, int n_channels,
                                     uint8_t * pixel_array){
         return decodeToArray(blurhash, width, height,
                              punch, n_channels, pixel_array);
@@ -42,15 +44,16 @@
         include_dirs=['src/'],
         extra_compile_args=['-std=gnu99'] if sys.platform != 'win32' else []
     )
 
 ffibuilder.cdef('''
     const char* create_hash_from_pixels(int x_components, int y_components,
                                         int width, int height, uint8_t* rgb,
-                                        size_t bytes_per_row);
+                                        size_t bytes_per_row,
+                                        char* destination);
     int create_pixels_from_blurhash(const char * blurhash, int width,
                                     int height, int punch, int nChannels,
                                     uint8_t * pixel_array);
 
     int is_valid_blurhash(const char * blurhash);
 
 ''')
```

### Comparing `blurhash-python-1.2.0/src/common.h` & `blurhash-python-1.2.1/src/common.h`

 * *Files identical despite different names*

### Comparing `blurhash-python-1.2.0/src/decode.c` & `blurhash-python-1.2.1/src/decode.c`

 * *Files identical despite different names*

### Comparing `blurhash-python-1.2.0/src/encode.c` & `blurhash-python-1.2.1/src/encode.c`

 * *Files 6% similar despite different names*

```diff
@@ -5,46 +5,50 @@
 
 #include "common.h"
 
 #ifndef M_PI
 #define M_PI 3.14159265358979323846
 #endif
 
-static float *multiplyBasisFunction(int xComponent, int yComponent, int width, int height, uint8_t *rgb, size_t bytesPerRow);
+struct RGB {
+	float r;
+	float g;
+	float b;
+};
+
+static struct RGB multiplyBasisFunction(int xComponent, int yComponent, int width, int height, uint8_t *rgb, size_t bytesPerRow);
 static char *encode_int(int value, int length, char *destination);
 
 static int encodeDC(float r, float g, float b);
 static int encodeAC(float r, float g, float b, float maximumValue);
 
-const char *blurHashForPixels(int xComponents, int yComponents, int width, int height, uint8_t *rgb, size_t bytesPerRow) {
-	static char buffer[2 + 4 + (9 * 9 - 1) * 2 + 1];
-
+const char *blurHashForPixels(int xComponents, int yComponents, int width, int height, uint8_t *rgb, size_t bytesPerRow, char *destination) {
 	if(xComponents < 1 || xComponents > 9) return NULL;
 	if(yComponents < 1 || yComponents > 9) return NULL;
 
 #ifndef _MSC_VER
 	float factors[yComponents * xComponents][3];
 #else
 	float factors[9 * 9][3];
 #endif
 	memset(factors, 0, sizeof(factors));
 
 	for(int y = 0; y < yComponents; y++) {
 		for(int x = 0; x < xComponents; x++) {
-			float *factor = multiplyBasisFunction(x, y, width, height, rgb, bytesPerRow);
-			factors[y * xComponents + x][0] = factor[0];
-			factors[y * xComponents + x][1] = factor[1];
-			factors[y * xComponents + x][2] = factor[2];
+			struct RGB factor = multiplyBasisFunction(x, y, width, height, rgb, bytesPerRow);
+			factors[y * xComponents + x][0] = factor.r;
+			factors[y * xComponents + x][1] = factor.g;
+			factors[y * xComponents + x][2] = factor.b;
 		}
 	}
 
 	float *dc = factors[0];
 	float *ac = dc + 3;
 	int acCount = xComponents * yComponents - 1;
-	char *ptr = buffer;
+	char *ptr = destination;
 
 	int sizeFlag = (xComponents - 1) + (yComponents - 1) * 9;
 	ptr = encode_int(sizeFlag, 1, ptr);
 
 	float maximumValue;
 	if(acCount > 0) {
 		float actualMaximumValue = 0;
@@ -64,36 +68,35 @@
 
 	for(int i = 0; i < acCount; i++) {
 		ptr = encode_int(encodeAC(ac[i * 3 + 0], ac[i * 3 + 1], ac[i * 3 + 2], maximumValue), 2, ptr);
 	}
 
 	*ptr = 0;
 
-	return buffer;
+	return destination;
 }
 
-static float *multiplyBasisFunction(int xComponent, int yComponent, int width, int height, uint8_t *rgb, size_t bytesPerRow) {
-	float r = 0, g = 0, b = 0;
+static struct RGB multiplyBasisFunction(int xComponent, int yComponent, int width, int height, uint8_t *rgb, size_t bytesPerRow) {
+	struct RGB result = { 0, 0, 0 };
 	float normalisation = (xComponent == 0 && yComponent == 0) ? 1 : 2;
 
 	for(int y = 0; y < height; y++) {
 		for(int x = 0; x < width; x++) {
 			float basis = cosf(M_PI * xComponent * x / width) * cosf(M_PI * yComponent * y / height);
-			r += basis * sRGBToLinear(rgb[3 * x + 0 + y * bytesPerRow]);
-			g += basis * sRGBToLinear(rgb[3 * x + 1 + y * bytesPerRow]);
-			b += basis * sRGBToLinear(rgb[3 * x + 2 + y * bytesPerRow]);
+			result.r += basis * sRGBToLinear(rgb[3 * x + 0 + y * bytesPerRow]);
+			result.g += basis * sRGBToLinear(rgb[3 * x + 1 + y * bytesPerRow]);
+			result.b += basis * sRGBToLinear(rgb[3 * x + 2 + y * bytesPerRow]);
 		}
 	}
 
 	float scale = normalisation / (width * height);
 
-	static float result[3];
-	result[0] = r * scale;
-	result[1] = g * scale;
-	result[2] = b * scale;
+	result.r *= scale;
+	result.g *= scale;
+	result.b *= scale;
 
 	return result;
 }
 
 static int encodeDC(float r, float g, float b) {
 	int roundedR = linearTosRGB(r);
 	int roundedG = linearTosRGB(g);
```

### Comparing `blurhash-python-1.2.0/tests/pic2.png` & `blurhash-python-1.2.1/tests/pic2.png`

 * *Files identical despite different names*

### Comparing `blurhash-python-1.2.0/tests/pic2_bw.png` & `blurhash-python-1.2.1/tests/pic2_bw.png`

 * *Files identical despite different names*

### Comparing `blurhash-python-1.2.0/tests/test_decode.py` & `blurhash-python-1.2.1/tests/test_decode.py`

 * *Files identical despite different names*

### Comparing `blurhash-python-1.2.0/tests/test_encode.py` & `blurhash-python-1.2.1/tests/test_encode.py`

 * *Files identical despite different names*

