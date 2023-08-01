# Comparing `tmp/glass-2023.6.tar.gz` & `tmp/glass-2023.7.tar.gz`

## Comparing `glass-2023.6.tar` & `glass-2023.7.tar`

### file list

```diff
@@ -1,70 +1,71 @@
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 glass-2023.6/.commitlint.rules.js
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 glass-2023.6/.flake8
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 glass-2023.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 glass-2023.6/.readthedocs.yml
--rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 glass-2023.6/CHANGELOG.md
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 glass-2023.6/CITATION.md
--rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 glass-2023.6/CONTRIBUTING.md
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 glass-2023.6/.github/dependabot.yml
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 glass-2023.6/.github/test-constraints.txt
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 glass-2023.6/.github/workflows/pull_request.yml
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 glass-2023.6/.github/workflows/pull_request_review.yml
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 glass-2023.6/.github/workflows/release.yml
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 glass-2023.6/.github/workflows/test.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 glass-2023.6/docs/Makefile
--rw-r--r--   0        0        0     6272 2020-02-02 00:00:00.000000 glass-2023.6/docs/conf.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 glass-2023.6/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 glass-2023.6/docs/make.bat
--rw-r--r--   0        0        0    94661 2020-02-02 00:00:00.000000 glass-2023.6/docs/_static/android-chrome-192x192.png
--rw-r--r--   0        0        0   704232 2020-02-02 00:00:00.000000 glass-2023.6/docs/_static/android-chrome-512x512.png
--rw-r--r--   0        0        0    85486 2020-02-02 00:00:00.000000 glass-2023.6/docs/_static/apple-touch-icon.png
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 glass-2023.6/docs/_static/favicon-16x16.png
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 glass-2023.6/docs/_static/favicon-32x32.png
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 glass-2023.6/docs/_static/favicon.ico
--rw-r--r--   0        0        0   867495 2020-02-02 00:00:00.000000 glass-2023.6/docs/_static/logo.png
--rw-r--r--   0        0        0   623526 2020-02-02 00:00:00.000000 glass-2023.6/docs/_static/spheres.png
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 glass-2023.6/docs/manual/extensions.rst
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 glass-2023.6/docs/manual/first-steps.rst
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 glass-2023.6/docs/manual/get-in-touch.rst
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 glass-2023.6/docs/manual/index.rst
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 glass-2023.6/docs/manual/installation.rst
--rw-r--r--   0        0        0     4573 2020-02-02 00:00:00.000000 glass-2023.6/docs/manual/releases.rst
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 glass-2023.6/docs/reference/fields.rst
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 glass-2023.6/docs/reference/galaxies.rst
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 glass-2023.6/docs/reference/index.rst
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 glass-2023.6/docs/reference/lensing.rst
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 glass-2023.6/docs/reference/observations.rst
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 glass-2023.6/docs/reference/points.rst
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 glass-2023.6/docs/reference/shapes.rst
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 glass-2023.6/docs/reference/shells.rst
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 glass-2023.6/docs/reference/user.rst
--rw-r--r--   0        0        0     2875 2020-02-02 00:00:00.000000 glass-2023.6/docs/user/definitions.rst
--rw-r--r--   0        0        0     6997 2020-02-02 00:00:00.000000 glass-2023.6/docs/user/how-glass-works.rst
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 glass-2023.6/docs/user/index.rst
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 glass-2023.6/docs/user/publications.rst
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 glass-2023.6/glass/__init__.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 glass-2023.6/glass/_version.py
--rw-r--r--   0        0        0     9341 2020-02-02 00:00:00.000000 glass-2023.6/glass/fields.py
--rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 glass-2023.6/glass/galaxies.py
--rw-r--r--   0        0        0    12328 2020-02-02 00:00:00.000000 glass-2023.6/glass/lensing.py
--rw-r--r--   0        0        0     9132 2020-02-02 00:00:00.000000 glass-2023.6/glass/observations.py
--rw-r--r--   0        0        0     9280 2020-02-02 00:00:00.000000 glass-2023.6/glass/points.py
--rw-r--r--   0        0        0     8335 2020-02-02 00:00:00.000000 glass-2023.6/glass/shapes.py
--rw-r--r--   0        0        0     8290 2020-02-02 00:00:00.000000 glass-2023.6/glass/shells.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 glass-2023.6/glass/user.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 glass-2023.6/glass/core/__init__.py
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 glass-2023.6/glass/core/array.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 glass-2023.6/glass/core/constants.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glass-2023.6/glass/core/test/__init__.py
--rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 glass-2023.6/glass/core/test/test_array.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 glass-2023.6/glass/ext/__init__.py
--rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 glass-2023.6/glass/test/test_galaxies.py
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 glass-2023.6/glass/test/test_lensing.py
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 glass-2023.6/glass/test/test_points.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 glass-2023.6/glass/test/test_shapes.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 glass-2023.6/glass/test/test_shells.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 glass-2023.6/.gitignore
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 glass-2023.6/LICENSE
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 glass-2023.6/README.md
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 glass-2023.6/pyproject.toml
--rw-r--r--   0        0        0     4821 2020-02-02 00:00:00.000000 glass-2023.6/PKG-INFO
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 glass-2023.7/.commitlint.rules.js
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 glass-2023.7/.flake8
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 glass-2023.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 glass-2023.7/.readthedocs.yml
+-rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 glass-2023.7/CHANGELOG.md
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 glass-2023.7/CITATION.md
+-rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 glass-2023.7/CONTRIBUTING.md
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 glass-2023.7/.github/dependabot.yml
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 glass-2023.7/.github/test-constraints.txt
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 glass-2023.7/.github/workflows/pull_request.yml
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 glass-2023.7/.github/workflows/pull_request_review.yml
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 glass-2023.7/.github/workflows/release.yml
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 glass-2023.7/.github/workflows/test.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 glass-2023.7/docs/Makefile
+-rw-r--r--   0        0        0     6272 2020-02-02 00:00:00.000000 glass-2023.7/docs/conf.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 glass-2023.7/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 glass-2023.7/docs/make.bat
+-rw-r--r--   0        0        0    94661 2020-02-02 00:00:00.000000 glass-2023.7/docs/_static/android-chrome-192x192.png
+-rw-r--r--   0        0        0   704232 2020-02-02 00:00:00.000000 glass-2023.7/docs/_static/android-chrome-512x512.png
+-rw-r--r--   0        0        0    85486 2020-02-02 00:00:00.000000 glass-2023.7/docs/_static/apple-touch-icon.png
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 glass-2023.7/docs/_static/favicon-16x16.png
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 glass-2023.7/docs/_static/favicon-32x32.png
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 glass-2023.7/docs/_static/favicon.ico
+-rw-r--r--   0        0        0   867495 2020-02-02 00:00:00.000000 glass-2023.7/docs/_static/logo.png
+-rw-r--r--   0        0        0   623526 2020-02-02 00:00:00.000000 glass-2023.7/docs/_static/spheres.png
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 glass-2023.7/docs/manual/extensions.rst
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 glass-2023.7/docs/manual/first-steps.rst
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 glass-2023.7/docs/manual/get-in-touch.rst
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 glass-2023.7/docs/manual/index.rst
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 glass-2023.7/docs/manual/installation.rst
+-rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 glass-2023.7/docs/manual/releases.rst
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 glass-2023.7/docs/reference/fields.rst
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 glass-2023.7/docs/reference/galaxies.rst
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 glass-2023.7/docs/reference/index.rst
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 glass-2023.7/docs/reference/lensing.rst
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 glass-2023.7/docs/reference/observations.rst
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 glass-2023.7/docs/reference/points.rst
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 glass-2023.7/docs/reference/shapes.rst
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 glass-2023.7/docs/reference/shells.rst
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 glass-2023.7/docs/reference/user.rst
+-rw-r--r--   0        0        0     2875 2020-02-02 00:00:00.000000 glass-2023.7/docs/user/definitions.rst
+-rw-r--r--   0        0        0     8344 2020-02-02 00:00:00.000000 glass-2023.7/docs/user/how-glass-works.rst
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 glass-2023.7/docs/user/index.rst
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 glass-2023.7/docs/user/publications.rst
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 glass-2023.7/glass/__init__.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 glass-2023.7/glass/_version.py
+-rw-r--r--   0        0        0    10106 2020-02-02 00:00:00.000000 glass-2023.7/glass/fields.py
+-rw-r--r--   0        0        0     6780 2020-02-02 00:00:00.000000 glass-2023.7/glass/galaxies.py
+-rw-r--r--   0        0        0    12328 2020-02-02 00:00:00.000000 glass-2023.7/glass/lensing.py
+-rw-r--r--   0        0        0     9132 2020-02-02 00:00:00.000000 glass-2023.7/glass/observations.py
+-rw-r--r--   0        0        0     9280 2020-02-02 00:00:00.000000 glass-2023.7/glass/points.py
+-rw-r--r--   0        0        0     8335 2020-02-02 00:00:00.000000 glass-2023.7/glass/shapes.py
+-rw-r--r--   0        0        0    14871 2020-02-02 00:00:00.000000 glass-2023.7/glass/shells.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 glass-2023.7/glass/user.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 glass-2023.7/glass/core/__init__.py
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 glass-2023.7/glass/core/array.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 glass-2023.7/glass/core/constants.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glass-2023.7/glass/core/test/__init__.py
+-rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 glass-2023.7/glass/core/test/test_array.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 glass-2023.7/glass/ext/__init__.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 glass-2023.7/glass/test/test_fields.py
+-rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 glass-2023.7/glass/test/test_galaxies.py
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 glass-2023.7/glass/test/test_lensing.py
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 glass-2023.7/glass/test/test_points.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 glass-2023.7/glass/test/test_shapes.py
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 glass-2023.7/glass/test/test_shells.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 glass-2023.7/.gitignore
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 glass-2023.7/LICENSE
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 glass-2023.7/README.md
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 glass-2023.7/pyproject.toml
+-rw-r--r--   0        0        0     4821 2020-02-02 00:00:00.000000 glass-2023.7/PKG-INFO
```

### Comparing `glass-2023.6/.commitlint.rules.js` & `glass-2023.7/.commitlint.rules.js`

 * *Files identical despite different names*

### Comparing `glass-2023.6/CHANGELOG.md` & `glass-2023.7/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,32 @@
 Changelog
 =========
 
 All notable changes to the project are documented in this file.  The format is
 based on [Keep a Changelog](https://keepachangelog.com).
 
 
+[2023.7]  (1 Aug 2023)
+----------------------
+
+### Added
+
+* Function `getcl()` to return angular power spectra by index from
+  a list using GLASS ordering.
+* New `linear_windows()` and `cubic_windows()` window functions for
+  shells.
+
+### Changed
+
+* The `gaussian_phz()` function now accepts bounds using `lower=`
+  and `upper=` keyword parameters.
+* The `partition()` function now returns an array of weights to
+  approximate the given function by the windows.
+
+
 [2023.6]  (30 Jun 2023)
 -----------------------
 
 ### Added
 
 - `deflect()` applies deflections to positions
 - `from_convergence()` returns other lensing fields given the convergence
@@ -101,11 +119,12 @@
 ----------------------
 
 ### Added
 
 - Initial wide release for GLASS paper
 
 
+[2023.7]: https://github.com/glass-dev/glass/compare/v2023.6...v2023.7
 [2023.6]: https://github.com/glass-dev/glass/compare/v2023.5...v2023.6
 [2023.5]: https://github.com/glass-dev/glass/compare/v2023.2...v2023.5
 [2023.2]: https://github.com/glass-dev/glass/compare/v2023.1...v2023.2
 [2023.1]: https://github.com/glass-dev/glass/releases/tag/v2023.1
```

### Comparing `glass-2023.6/CITATION.md` & `glass-2023.7/CITATION.md`

 * *Files identical despite different names*

### Comparing `glass-2023.6/CONTRIBUTING.md` & `glass-2023.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `glass-2023.6/.github/workflows/pull_request.yml` & `glass-2023.7/.github/workflows/pull_request.yml`

 * *Files identical despite different names*

### Comparing `glass-2023.6/.github/workflows/test.yml` & `glass-2023.7/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `glass-2023.6/docs/Makefile` & `glass-2023.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `glass-2023.6/docs/conf.py` & `glass-2023.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `glass-2023.6/docs/index.rst` & `glass-2023.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `glass-2023.6/docs/make.bat` & `glass-2023.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `glass-2023.6/docs/_static/android-chrome-192x192.png` & `glass-2023.7/docs/_static/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `glass-2023.6/docs/_static/android-chrome-512x512.png` & `glass-2023.7/docs/_static/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `glass-2023.6/docs/_static/apple-touch-icon.png` & `glass-2023.7/docs/_static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `glass-2023.6/docs/_static/favicon-16x16.png` & `glass-2023.7/docs/_static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `glass-2023.6/docs/_static/favicon-32x32.png` & `glass-2023.7/docs/_static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `glass-2023.6/docs/_static/favicon.ico` & `glass-2023.7/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `glass-2023.6/docs/_static/logo.png` & `glass-2023.7/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `glass-2023.6/docs/_static/spheres.png` & `glass-2023.7/docs/_static/spheres.png`

 * *Files identical despite different names*

### Comparing `glass-2023.6/docs/manual/installation.rst` & `glass-2023.7/docs/manual/installation.rst`

 * *Files identical despite different names*

### Comparing `glass-2023.6/docs/manual/releases.rst` & `glass-2023.7/docs/manual/releases.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,38 @@
 
 Release notes
 =============
 
 These notes document the changes between individual *GLASS* releases.
 
 
+2023.7 (1 Aug 2023)
+-------------------
+
+* New radial window functions :func:`~glass.shells.linear_windows()` and
+  :func:`~glass.shells.cubic_windows()`, which correspond to linear and cubic
+  spline interpolation of radial functions, respectively.  These are
+  overlapping window functions, and it has been difficult to obtain accurate
+  matter power spectra so far.
+
+* The :func:`~glass.shells.partition()` function now returns an array of
+  weights to approximate a given function by the window functions.  This is
+  necessary to obtain an accurate fit of redshift distributions by overlapping
+  window functions.  For example, to get the array of galaxy densities in each
+  shells from ``dndz``, one would now do::
+
+      ngal = partition(z, dndz, shells)
+
+* A new function :func:`~glass.fields.getcl()` was added to return angular
+  power spectra by index from a list using GLASS ordering.
+
+* The :func:`~glass.galaxies.gaussian_phz()` function now accepts bounds using
+  `lower=` and `upper=` keyword parameters.
+
+
 2023.6 (30 Jun 2023)
 --------------------
 
 - There is some support for simulating the deflections due to weak
   gravitational lensing:
 
   - The :func:`~glass.lensing.deflect` function applies deflections to
```

### Comparing `glass-2023.6/docs/user/definitions.rst` & `glass-2023.7/docs/user/definitions.rst`

 * *Files identical despite different names*

### Comparing `glass-2023.6/docs/user/how-glass-works.rst` & `glass-2023.7/docs/user/how-glass-works.rst`

 * *Files 13% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 
     # plot each window
     for i, (za, wa, zeff) in enumerate(ws):
         plt.plot(za, wa, c='k', lw=2)
         plt.fill_between(za, np.zeros_like(wa), wa, alpha=0.5)
         plt.annotate(f'shell {i+1}', (zeff, 0.5), ha='center', va='center')
 
-    plt.ylim(0., 2.)
     plt.xlabel('redshift $z$')
     plt.ylabel('window function $W(z)$')
     plt.tight_layout()
 
 Given such a sequence of window functions :math:`W_i`, *GLASS* discretises a
 continuous field :math:`F` (e.g. the matter density in the universe) by using
 each :math:`W_i` in turn to project :math:`F` onto the sphere,
@@ -59,14 +58,56 @@
 
 This results in the sequence :math:`F_1, F_2, \ldots` of integrated (projected)
 fields, which are :term:`spherical functions<spherical function>`.  *GLASS*
 then simulates the (radially) continuous field :math:`F(z)` as the (radially)
 discretised fields :math:`F_i`.
 
 
+.. _user-window-functions:
+
+Window functions
+^^^^^^^^^^^^^^^^
+
+*GLASS* supports arbitrary window functions (although the computation of
+:ref:`line-of-sight integrals <user-los-integrals>` makes some assumptions).
+The following :ref:`window functions <reference-window-functions>` are
+included:
+
+.. plot::
+
+    from glass.shells import (redshift_grid, tophat_windows, linear_windows,
+                              cubic_windows)
+
+    plot_windows = [tophat_windows, linear_windows,
+                    cubic_windows]
+    nr = (len(plot_windows)+1)//2
+
+    fig, axes = plt.subplots(nr, 2, figsize=(8, nr*3), layout="constrained",
+                             squeeze=False, sharex=False, sharey=True)
+
+    zs = redshift_grid(0., 0.5, dz=0.1)
+    zt = np.linspace(0., 0.5, 200)
+
+    for ax in axes.flat:
+        ax.axis(False)
+    for windows, ax in zip(plot_windows, axes.flat):
+        ws = windows(zs)
+        wt = np.zeros_like(zt)
+        ax.axis(True)
+        ax.set_title(windows.__name__)
+        for i, (za, wa, zeff) in enumerate(ws):
+            wt += np.interp(zt, za, wa, left=0., right=0.)
+            ax.fill_between(za, np.zeros_like(wa), wa, alpha=0.5)
+        ax.plot(zt, wt, c="k", lw=2)
+    for ax in axes.flat:
+        ax.set_xlabel("redshift $z$")
+    for ax in axes[:, 0]:
+        ax.set_ylabel("window function $W(z)$")
+
+
 Angular discretisation
 ----------------------
 
 The projected fields :math:`F_i` are still continuous functions on the sphere.
 They therefore require further discretisation, which turns :math:`F_i` into a
 spherical map of finite resolution.  In *GLASS*, this is done using the
 *HEALPix* [#healpix]_ discretisation of the sphere.
@@ -85,14 +126,16 @@
 field :math:`F_i` itself is sampled at the pixel centres.
 
 *GLASS* can simulate either kind of angular discretisation.  The only
 difference between the two is whether or not the pixel window function is
 applied to the spherical harmonic expansion of the fields.
 
 
+.. _user-los-integrals:
+
 Line-of-sight integrals
 -----------------------
 
 The `radial discretisation`_ determines how well the simulation can approximate
 line-of-sight integrals of the form
 
 .. math::
```

### Comparing `glass-2023.6/glass/fields.py` & `glass-2023.7/glass/fields.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,20 @@
 ---------
 
 .. autofunction:: gaussian_gls
 .. autofunction:: lognormal_gls
 .. autofunction:: generate_gaussian
 .. autofunction:: generate_lognormal
 
+
+Utility functions
+-----------------
+
+.. autofunction:: getcl
+
 '''
 
 import warnings
 import numpy as np
 import healpy as hp
 from gaussiancl import gaussiancl
 
@@ -281,7 +287,36 @@
 
         # lognormal shift, unless unity
         if shift != 1:
             m *= shift
 
         # yield the lognormal map
         yield m
+
+
+def getcl(cls, i, j, lmax=None):
+    """Return a specific angular power spectrum from an array.
+
+    Return the angular power spectrum for indices *i* and *j* from an
+    array in *GLASS* ordering.
+
+    Parameters
+    ----------
+    cls : list of array_like
+        List of angular power spectra in *GLASS* ordering.
+    i, j : int
+        Combination of indices to return.
+    lmax : int, optional
+        Truncate the returned spectrum at this mode number.
+
+    Returns
+    -------
+    cl : array_like
+        The angular power spectrum for indices *i* and *j*.
+
+    """
+    if j > i:
+        i, j = j, i
+    cl = cls[i*(i+1)//2+i-j]
+    if lmax is not None:
+        cl = cl[:lmax+1]
+    return cl
```

### Comparing `glass-2023.6/glass/galaxies.py` & `glass-2023.7/glass/galaxies.py`

 * *Files 15% similar despite different names*

```diff
@@ -141,37 +141,47 @@
     else:
         # simple sum of shears
         g += eps
 
     return g
 
 
-def gaussian_phz(z: ArrayLike, sigma_0: float | ArrayLike,
+def gaussian_phz(z: ArrayLike, sigma_0: float | ArrayLike, *,
+                 lower: ArrayLike | None = None,
+                 upper: ArrayLike | None = None,
                  rng: np.random.Generator | None = None) -> np.ndarray:
     r'''Photometric redshifts assuming a Gaussian error.
 
     A simple toy model of photometric redshift errors that assumes a
     Gaussian error with redshift-dependent standard deviation
     :math:`\sigma(z) = (1 + z) \sigma_0` [1]_.
 
     Parameters
     ----------
     z : array_like
         True redshifts.
     sigma_0 : float or array_like
         Redshift error in the tomographic binning at zero redshift.
+    lower, upper : float or array_like, optional
+        Bounds for the returned photometric redshifts.
     rng : :class:`~numpy.random.Generator`, optional
         Random number generator.  If not given, a default RNG is used.
 
     Returns
     -------
     phz : array_like
         Photometric redshifts assuming Gaussian errors, of the same
         shape as *z*.
 
+    Warnings
+    --------
+    The *lower* and *upper* bounds are implemented using plain rejection
+    sampling from the non-truncated normal distribution.  If bounds are
+    used, they should always contain significant probability mass.
+
     See Also
     --------
     glass.observations.tomo_nz_gausserr :
         Create tomographic redshift distributions assuming the same
         model.
 
     References
@@ -190,18 +200,27 @@
         rng = np.random.default_rng()
 
     sigma = np.add(1, z)*sigma_0
     dims = np.shape(sigma)
 
     zphot = rng.normal(z, sigma)
 
+    if lower is None:
+        lower = 0.
+    if upper is None:
+        upper = np.inf
+
+    if not np.all(lower < upper):
+        raise ValueError("requires lower < upper")
+
     if not dims:
-        while zphot < 0:
+        while zphot < lower or zphot > upper:
             zphot = rng.normal(z, sigma)
     else:
         z = np.broadcast_to(z, dims)
-        trunc = np.where(zphot < 0)[0]
+        trunc = np.where((zphot < lower) | (zphot > upper))[0]
         while trunc.size:
-            zphot[trunc] = rng.normal(z[trunc], sigma[trunc])
-            trunc = trunc[zphot[trunc] < 0]
+            znew = rng.normal(z[trunc], sigma[trunc])
+            zphot[trunc] = znew
+            trunc = trunc[(znew < lower) | (znew > upper)]
 
     return zphot
```

### Comparing `glass-2023.6/glass/lensing.py` & `glass-2023.7/glass/lensing.py`

 * *Files identical despite different names*

### Comparing `glass-2023.6/glass/observations.py` & `glass-2023.7/glass/observations.py`

 * *Files identical despite different names*

### Comparing `glass-2023.6/glass/points.py` & `glass-2023.7/glass/points.py`

 * *Files identical despite different names*

### Comparing `glass-2023.6/glass/shapes.py` & `glass-2023.7/glass/shapes.py`

 * *Files identical despite different names*

### Comparing `glass-2023.6/glass/user.py` & `glass-2023.7/glass/user.py`

 * *Files identical despite different names*

### Comparing `glass-2023.6/glass/core/array.py` & `glass-2023.7/glass/core/array.py`

 * *Files identical despite different names*

### Comparing `glass-2023.6/glass/core/test/test_array.py` & `glass-2023.7/glass/core/test/test_array.py`

 * *Files identical despite different names*

### Comparing `glass-2023.6/glass/test/test_galaxies.py` & `glass-2023.7/glass/test/test_galaxies.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,14 +93,25 @@
     sigma_0 = np.ones(100)
 
     phz = gaussian_phz(z, sigma_0)
 
     assert phz.shape == (100,)
     assert np.all(phz >= 0)
 
+    # case: upper and lower bound
+
+    z = 1.
+    sigma_0 = np.ones(100)
+
+    phz = gaussian_phz(z, sigma_0, lower=0.5, upper=1.5)
+
+    assert phz.shape == (100,)
+    assert np.all(phz >= 0.5)
+    assert np.all(phz <= 1.5)
+
     # test interface
 
     # case: scalar redshift, scalar sigma_0
 
     z = 1.
     sigma_0 = 0.
```

### Comparing `glass-2023.6/glass/test/test_lensing.py` & `glass-2023.7/glass/test/test_lensing.py`

 * *Files identical despite different names*

### Comparing `glass-2023.6/glass/test/test_points.py` & `glass-2023.7/glass/test/test_points.py`

 * *Files identical despite different names*

### Comparing `glass-2023.6/glass/test/test_shapes.py` & `glass-2023.7/glass/test/test_shapes.py`

 * *Files identical despite different names*

### Comparing `glass-2023.6/LICENSE` & `glass-2023.7/LICENSE`

 * *Files identical despite different names*

### Comparing `glass-2023.6/README.md` & `glass-2023.7/README.md`

 * *Files identical despite different names*

### Comparing `glass-2023.6/pyproject.toml` & `glass-2023.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `glass-2023.6/PKG-INFO` & `glass-2023.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glass
-Version: 2023.6
+Version: 2023.7
 Summary: Generator for Large Scale Structure
 Project-URL: Homepage, https://github.com/glass-dev/glass
 Project-URL: Documentation, https://glass.readthedocs.io/
 Project-URL: Issues, https://github.com/glass-dev/glass/issues
 Project-URL: Changelog, https://glass.readthedocs.io/en/stable/manual/releases.html
 Maintainer-email: Nicolas Tessore <n.tessore@ucl.ac.uk>
 License: MIT License
```

