# Comparing `tmp/djangocms_leaflet-0.0.2.tar.gz` & `tmp/djangocms_leaflet-0.0.3b1.tar.gz`

## Comparing `djangocms_leaflet-0.0.2.tar` & `djangocms_leaflet-0.0.3b1.tar`

### file list

```diff
@@ -1,56 +1,57 @@
--rw-r--r--   0        0        0    58673 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/package-lock.json
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/package.json
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/webpack.config.js
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/assets/src/leaflet.js
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/__about__.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/__init__.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/apps.py
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/cms_plugins.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/models.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/migrations/0001_initial.py
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/migrations/0002_auto_20200310_2328.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/migrations/__init__.py
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/djangocms_leaflet/images/layers-2x.png
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/djangocms_leaflet/images/layers.png
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-icon-2x.png
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-icon.png
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-shadow.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-black.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-black.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-blue.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-blue.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-gold.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-gold.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-green.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-green.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-grey.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-grey.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-orange.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-orange.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-red.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-red.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-violet.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-violet.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-yellow.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-yellow.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-black.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-black.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-blue.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-blue.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-gold.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-gold.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-green.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-green.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-grey.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-grey.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-orange.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-orange.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-red.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-red.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-violet.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-violet.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-yellow.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-yellow.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-shadow.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-shadow.png
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/djangocms_leaflet/webpack/2b3e1faf89f94a483539.png
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/djangocms_leaflet/webpack/416d91365b44e4b4f477.png
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/djangocms_leaflet/webpack/8f2c4d11474275fbc161.png
--rw-r--r--   0        0        0   169468 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/djangocms_leaflet/webpack/leaflet.bundle.js
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/djangocms_leaflet/webpack/leaflet.bundle.js.LICENSE.txt
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/webpack/2b3e1faf89f94a483539.png
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/webpack/416d91365b44e4b4f477.png
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/webpack/8f2c4d11474275fbc161.png
--rw-r--r--   0        0        0   174912 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/webpack/leaflet.bundle.js
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/webpack/leaflet.bundle.js.LICENSE.txt
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/templates/djangocms_leaflet/map.html
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/src/djangocms_leaflet/templates/djangocms_leaflet/marker.html
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/.gitignore
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/README.md
--rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    58673 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/package-lock.json
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/package.json
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/webpack.config.js
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/assets/src/leaflet.js
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/__about__.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/__init__.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/apps.py
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/cms_plugins.py
+-rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/models.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/migrations/0001_initial.py
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/migrations/0002_auto_20200310_2328.py
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/migrations/0003_map_location_search_term_marker_location_search_term_and_more.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/migrations/__init__.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/layers-2x.png
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/layers.png
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-icon-2x.png
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-icon.png
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-shadow.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-black.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-black.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-blue.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-blue.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-gold.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-gold.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-green.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-green.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-grey.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-grey.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-orange.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-orange.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-red.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-red.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-violet.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-violet.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-yellow.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-yellow.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-black.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-black.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-blue.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-blue.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-gold.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-gold.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-green.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-green.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-grey.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-grey.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-orange.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-orange.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-red.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-red.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-violet.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-violet.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-yellow.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-yellow.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-shadow.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-shadow.png
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/webpack/2b3e1faf89f94a483539.png
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/webpack/416d91365b44e4b4f477.png
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/webpack/8f2c4d11474275fbc161.png
+-rw-r--r--   0        0        0   169468 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/webpack/leaflet.bundle.js
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/webpack/leaflet.bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/webpack/2b3e1faf89f94a483539.png
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/webpack/416d91365b44e4b4f477.png
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/webpack/8f2c4d11474275fbc161.png
+-rw-r--r--   0        0        0   174912 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/webpack/leaflet.bundle.js
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/webpack/leaflet.bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/templates/djangocms_leaflet/map.html
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/templates/djangocms_leaflet/marker.html
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/tests/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/.gitignore
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/LICENSE.txt
+-rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/README.md
+-rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/pyproject.toml
+-rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.3b1/PKG-INFO
```

### Comparing `djangocms_leaflet-0.0.2/package-lock.json` & `djangocms_leaflet-0.0.3b1/package-lock.json`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2/src/djangocms_leaflet/cms_plugins.py` & `djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2/src/djangocms_leaflet/locale/de/LC_MESSAGES/django.mo` & `djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2/src/djangocms_leaflet/locale/de/LC_MESSAGES/django.po` & `djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2/src/djangocms_leaflet/migrations/0001_initial.py` & `djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2/src/djangocms_leaflet/migrations/0002_auto_20200310_2328.py` & `djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/migrations/0002_auto_20200310_2328.py`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/djangocms_leaflet/images/layers-2x.png` & `djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/layers-2x.png`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/djangocms_leaflet/images/layers.png` & `djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/layers.png`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-icon-2x.png` & `djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-icon-2x.png`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-icon.png` & `djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-icon.png`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-shadow.png` & `djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-shadow.png`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/djangocms_leaflet/webpack/2b3e1faf89f94a483539.png` & `djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/webpack/2b3e1faf89f94a483539.png`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/djangocms_leaflet/webpack/416d91365b44e4b4f477.png` & `djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/webpack/416d91365b44e4b4f477.png`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/djangocms_leaflet/webpack/8f2c4d11474275fbc161.png` & `djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/webpack/8f2c4d11474275fbc161.png`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/djangocms_leaflet/webpack/leaflet.bundle.js` & `djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/djangocms_leaflet/webpack/leaflet.bundle.js`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/webpack/2b3e1faf89f94a483539.png` & `djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/webpack/2b3e1faf89f94a483539.png`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/webpack/416d91365b44e4b4f477.png` & `djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/webpack/416d91365b44e4b4f477.png`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/webpack/8f2c4d11474275fbc161.png` & `djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/webpack/8f2c4d11474275fbc161.png`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2/src/djangocms_leaflet/static/webpack/leaflet.bundle.js` & `djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/static/webpack/leaflet.bundle.js`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2/src/djangocms_leaflet/templates/djangocms_leaflet/map.html` & `djangocms_leaflet-0.0.3b1/src/djangocms_leaflet/templates/djangocms_leaflet/map.html`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2/LICENSE.txt` & `djangocms_leaflet-0.0.3b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2/README.md` & `djangocms_leaflet-0.0.3b1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -13,21 +13,45 @@
 - [License](#license)
 
 ## Installation
 
 ```console
 pip install djangocms-leaflet
 ```
+
+or add `djangocms-leaflet` to the dependencies of your project, e. g. in `pyprojet.toml`:
+```toml
+dependencies = [
+    # …
+    'djangocms-leaflet',
+    # …
+]
+```
+
+
+Add it to `INSTALLED_APPS` in the settings::
+
+```python
+INSTALLED_APPS: list[str] = [
+    # …
+    'djangocms_leaflet',
+    # …
+]
+```
 ## Usage
 
 Add a map plugin to a placeholder and fill in the form. Add markers as sub plugins if needed.
 In the template `src/djangocms_leaflet/templates/djangocms_leaflet/map.html` the tile server
 of the OpenStreetMap website is defined. Make sure you comply with their usage policy or
 use another tile server by replacing the tile server’s URL.
 
+You can either specify latitude and longitude of the map or marker or enter a search term.
+If no coordinates are entered, they will be searched with Nominatim and the first hit in the result list location will
+be used as coordinates.
+
 ## License
 
 `djangocms-leaflet` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
 
 ## Integrated library
 
 | Name                                                   | Description                | License                                                                       |
```

### Comparing `djangocms_leaflet-0.0.2/pyproject.toml` & `djangocms_leaflet-0.0.3b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "Django>=3.2",
   "django-cms>=3.11",
+  "requests>=2.31"
 ]
 
 [project.urls]
 Documentation = "https://github.com/MacLake/djangocms-leaflet#readme"
 Issues = "https://github.com/MacLake/djangocms-leaflet/issues"
 Source = "https://github.com/MacLake/djangocms-leaflet"
```

### Comparing `djangocms_leaflet-0.0.2/PKG-INFO` & `djangocms_leaflet-0.0.3b1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-leaflet
-Version: 0.0.2
+Version: 0.0.3b1
 Summary: django CMS plug-ins for the JavaScript map library Leaflet
 Project-URL: Documentation, https://github.com/MacLake/djangocms-leaflet#readme
 Project-URL: Issues, https://github.com/MacLake/djangocms-leaflet/issues
 Project-URL: Source, https://github.com/MacLake/djangocms-leaflet
 Author-email: Jens-Erik Weber <Jens-Erik.Weber@passiv.de>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9
 Requires-Dist: django-cms>=3.11
 Requires-Dist: django>=3.2
+Requires-Dist: requests>=2.31
 Description-Content-Type: text/markdown
 
 # djangocms-leaflet
 
 This app provides plug-ins for the JavaScript map library [Leaflet](https://leafletjs.com/).
 
 [![PyPI - Version](https://img.shields.io/pypi/v/djangocms-leaflet.svg)](https://pypi.org/project/djangocms-leaflet)
@@ -36,21 +37,45 @@
 - [License](#license)
 
 ## Installation
 
 ```console
 pip install djangocms-leaflet
 ```
+
+or add `djangocms-leaflet` to the dependencies of your project, e. g. in `pyprojet.toml`:
+```toml
+dependencies = [
+    # …
+    'djangocms-leaflet',
+    # …
+]
+```
+
+
+Add it to `INSTALLED_APPS` in the settings::
+
+```python
+INSTALLED_APPS: list[str] = [
+    # …
+    'djangocms_leaflet',
+    # …
+]
+```
 ## Usage
 
 Add a map plugin to a placeholder and fill in the form. Add markers as sub plugins if needed.
 In the template `src/djangocms_leaflet/templates/djangocms_leaflet/map.html` the tile server
 of the OpenStreetMap website is defined. Make sure you comply with their usage policy or
 use another tile server by replacing the tile server’s URL.
 
+You can either specify latitude and longitude of the map or marker or enter a search term.
+If no coordinates are entered, they will be searched with Nominatim and the first hit in the result list location will
+be used as coordinates.
+
 ## License
 
 `djangocms-leaflet` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
 
 ## Integrated library
 
 | Name                                                   | Description                | License                                                                       |
```

