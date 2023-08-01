# Comparing `tmp/aqtinstall-3.1.6.tar.gz` & `tmp/aqtinstall-3.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aqtinstall-3.1.6.tar", last modified: Thu May  4 23:47:10 2023, max compression
+gzip compressed data, was "aqtinstall-3.1.7.tar", last modified: Tue Aug  1 07:25:41 2023, max compression
```

## Comparing `aqtinstall-3.1.6.tar` & `aqtinstall-3.1.7.tar`

### file list

```diff
@@ -1,144 +1,146 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 23:47:10.876622 aqtinstall-3.1.6/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/.flake8
--rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      567 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9826 2023-05-04 23:47:10.876622 aqtinstall-3.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     8587 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 23:47:10.848619 aqtinstall-3.1.6/aqt/
--rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/aqt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1220 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/aqt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)    25241 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/aqt/archives.py
--rw-r--r--   0 runner    (1001) docker     (122)    26751 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/aqt/combinations.json
--rw-r--r--   0 runner    (1001) docker     (122)     3553 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/aqt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    19294 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/aqt/helper.py
--rw-r--r--   0 runner    (1001) docker     (122)    56222 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/aqt/installer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/aqt/logging.ini
--rw-r--r--   0 runner    (1001) docker     (122)    42338 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/aqt/metadata.py
--rw-r--r--   0 runner    (1001) docker     (122)    13217 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/aqt/settings.ini
--rw-r--r--   0 runner    (1001) docker     (122)    15062 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/aqt/updater.py
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-04 23:47:10.000000 aqtinstall-3.1.6/aqt/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 23:47:10.848619 aqtinstall-3.1.6/aqtinstall.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9826 2023-05-04 23:47:10.000000 aqtinstall-3.1.6/aqtinstall.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3909 2023-05-04 23:47:10.000000 aqtinstall-3.1.6/aqtinstall.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-04 23:47:10.000000 aqtinstall-3.1.6/aqtinstall.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-05-04 23:47:10.000000 aqtinstall-3.1.6/aqtinstall.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      452 2023-05-04 23:47:10.000000 aqtinstall-3.1.6/aqtinstall.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        4 2023-05-04 23:47:10.000000 aqtinstall-3.1.6/aqtinstall.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 23:47:10.852620 aqtinstall-3.1.6/ci/
--rw-r--r--   0 runner    (1001) docker     (122)     3846 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/ci/accelbubble.7z
--rw-r--r--   0 runner    (1001) docker     (122)    16872 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/ci/generate_azure_pipelines_matrices.py
--rw-r--r--   0 runner    (1001) docker     (122)     7223 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/ci/generate_combinations.py
--rw-r--r--   0 runner    (1001) docker     (122)      439 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/ci/helloworld.7z
--rw-r--r--   0 runner    (1001) docker     (122)  1213852 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/ci/jom_1_1_3.zip
--rw-r--r--   0 runner    (1001) docker     (122)      801 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/ci/logging.ini
--rw-r--r--   0 runner    (1001) docker     (122)     3134 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/ci/openglwindow.7z
--rw-r--r--   0 runner    (1001) docker     (122)     2513 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/ci/openglwindow_qt6.7z
--rw-r--r--   0 runner    (1001) docker     (122)     3890 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/ci/redditclient.7z
--rw-r--r--   0 runner    (1001) docker     (122)      791 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/ci/settings.ini
--rw-r--r--   0 runner    (1001) docker     (122)    18931 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/ci/steps.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 23:47:10.856620 aqtinstall-3.1.6/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     6132 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)     5708 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1002 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/CONTRIBUTE.rst
--rw-r--r--   0 runner    (1001) docker     (122)     7672 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      504 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/SECURITY.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1506 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (122)    32418 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (122)     9830 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     6244 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (122)    26591 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (122)      319 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2588 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 23:47:10.844619 aqtinstall-3.1.6/docs/locale/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 23:47:10.844619 aqtinstall-3.1.6/docs/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 23:47:10.860620 aqtinstall-3.1.6/docs/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     8165 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/locale/ja/LC_MESSAGES/CODE_OF_CONDUCT.po
--rw-r--r--   0 runner    (1001) docker     (122)     3215 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/locale/ja/LC_MESSAGES/CONTRIBUTE.po
--rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/locale/ja/LC_MESSAGES/SECURITY.po
--rw-r--r--   0 runner    (1001) docker     (122)     3980 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/locale/ja/LC_MESSAGES/authors.po
--rw-r--r--   0 runner    (1001) docker     (122)    41059 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/locale/ja/LC_MESSAGES/changes.po
--rw-r--r--   0 runner    (1001) docker     (122)    39387 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/locale/ja/LC_MESSAGES/cli.po
--rw-r--r--   0 runner    (1001) docker     (122)    14457 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/locale/ja/LC_MESSAGES/configuration.po
--rw-r--r--   0 runner    (1001) docker     (122)    46696 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/locale/ja/LC_MESSAGES/getting_started.po
--rw-r--r--   0 runner    (1001) docker     (122)      912 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/locale/ja/LC_MESSAGES/index.po
--rw-r--r--   0 runner    (1001) docker     (122)     3905 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/locale/ja/LC_MESSAGES/installation.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 23:47:10.864621 aqtinstall-3.1.6/docs/locale/pot/
--rw-r--r--   0 runner    (1001) docker     (122)     7867 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/locale/pot/CODE_OF_CONDUCT.pot
--rw-r--r--   0 runner    (1001) docker     (122)     2120 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/locale/pot/CONTRIBUTE.pot
--rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/locale/pot/SECURITY.pot
--rw-r--r--   0 runner    (1001) docker     (122)     3343 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/locale/pot/authors.pot
--rw-r--r--   0 runner    (1001) docker     (122)    40934 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/locale/pot/changes.pot
--rw-r--r--   0 runner    (1001) docker     (122)    20318 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/locale/pot/cli.pot
--rw-r--r--   0 runner    (1001) docker     (122)     7649 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/locale/pot/configuration.pot
--rw-r--r--   0 runner    (1001) docker     (122)    22725 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/locale/pot/getting_started.pot
--rw-r--r--   0 runner    (1001) docker     (122)      893 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/locale/pot/index.pot
--rw-r--r--   0 runner    (1001) docker     (122)     2894 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/locale/pot/installation.pot
--rw-r--r--   0 runner    (1001) docker     (122)     6994 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (122)    25779 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/previous_changes.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6004 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-04 23:47:10.876622 aqtinstall-3.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 23:47:10.864621 aqtinstall-3.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      274 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 23:47:10.876622 aqtinstall-3.1.6/tests/data/
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (122)     1468 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/linux-android-expect.json
--rw-r--r--   0 runner    (1001) docker     (122)    18093 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/linux-android.html
--rw-r--r--   0 runner    (1001) docker     (122)     2304 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/linux-desktop-expect.json
--rw-r--r--   0 runner    (1001) docker     (122)    30760 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/linux-desktop.html
--rw-r--r--   0 runner    (1001) docker     (122)     1468 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/mac-android-expect.json
--rw-r--r--   0 runner    (1001) docker     (122)    16521 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/mac-android.html
--rw-r--r--   0 runner    (1001) docker     (122)     2336 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/mac-desktop-expect.json
--rw-r--r--   0 runner    (1001) docker     (122)      202 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/mac-desktop-tools_cmake-expect.json
--rw-r--r--   0 runner    (1001) docker     (122)      961 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/mac-desktop-tools_cmake-update.xml
--rw-r--r--   0 runner    (1001) docker     (122)      361 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/mac-desktop-tools_ifw-expect.json
--rw-r--r--   0 runner    (1001) docker     (122)      918 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/mac-desktop-tools_ifw-update.xml
--rw-r--r--   0 runner    (1001) docker     (122)     2593 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/mac-desktop-tools_qtcreator-expect.json
--rw-r--r--   0 runner    (1001) docker     (122)     2072 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/mac-desktop-tools_qtcreator-update.xml
--rw-r--r--   0 runner    (1001) docker     (122)     1979 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/mac-desktop-tools_qtdesignstudio-expect.json
--rw-r--r--   0 runner    (1001) docker     (122)     1504 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/mac-desktop-tools_qtdesignstudio-update.xml
--rw-r--r--   0 runner    (1001) docker     (122)    28650 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/mac-desktop.html
--rw-r--r--   0 runner    (1001) docker     (122)      839 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/mac-ios-expect.json
--rw-r--r--   0 runner    (1001) docker     (122)    11401 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/mac-ios.html
--rw-r--r--   0 runner    (1001) docker     (122)     1920 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/mirror-expect.json
--rw-r--r--   0 runner    (1001) docker     (122)    19653 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/mirror-first-td.html
--rw-r--r--   0 runner    (1001) docker     (122)    17200 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/mirror-pre-a.html
--rw-r--r--   0 runner    (1001) docker     (122)    23047 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/mirror-table-before-pre-a.html
--rw-r--r--   0 runner    (1001) docker     (122)    76947 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/mirror-tag-in-a.html
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/settings.ini
--rw-r--r--   0 runner    (1001) docker     (122)    12460 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/settings_no_concurrency.ini
--rw-r--r--   0 runner    (1001) docker     (122)    79658 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-5140-expect.json
--rw-r--r--   0 runner    (1001) docker     (122)    72606 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-5140-update.xml
--rw-r--r--   0 runner    (1001) docker     (122)      285 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-5140-wasm-expect.json
--rw-r--r--   0 runner    (1001) docker     (122)    16692 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-5140-wasm-update.xml
--rw-r--r--   0 runner    (1001) docker     (122)     1494 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-5150-expect.json
--rw-r--r--   0 runner    (1001) docker     (122)   120616 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-5150-update.xml
--rw-r--r--   0 runner    (1001) docker     (122)     3914 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-5152-src-doc-example-expect.json
--rw-r--r--   0 runner    (1001) docker     (122)    18932 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-5152-src-doc-example-update.xml
--rw-r--r--   0 runner    (1001) docker     (122)    35906 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-620-android-armv7-update.xml
--rw-r--r--   0 runner    (1001) docker     (122)     1703 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-620-expect.json
--rw-r--r--   0 runner    (1001) docker     (122)    84709 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-620-update.xml
--rw-r--r--   0 runner    (1001) docker     (122)      469 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-650-wasm-multi-expect.json
--rw-r--r--   0 runner    (1001) docker     (122)    14238 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-650-wasm-multi-update.xml
--rw-r--r--   0 runner    (1001) docker     (122)      471 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-650-wasm-single-expect.json
--rw-r--r--   0 runner    (1001) docker     (122)    14534 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-650-wasm-single-update.xml
--rw-r--r--   0 runner    (1001) docker     (122)     1468 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-android-expect.json
--rw-r--r--   0 runner    (1001) docker     (122)    16533 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-android.html
--rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-desktop-expect.json
--rw-r--r--   0 runner    (1001) docker     (122)     6580 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-desktop-tools-mingw-updates.xml
--rw-r--r--   0 runner    (1001) docker     (122)     2833 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-desktop-tools-qtcreator-updates.xml
--rw-r--r--   0 runner    (1001) docker     (122)     6115 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-desktop-tools_vcredist-expect.json
--rw-r--r--   0 runner    (1001) docker     (122)     5916 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-desktop-tools_vcredist-update.xml
--rw-r--r--   0 runner    (1001) docker     (122)    30718 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-desktop.html
--rw-r--r--   0 runner    (1001) docker     (122)      817 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-winrt-expect.json
--rw-r--r--   0 runner    (1001) docker     (122)    10501 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-winrt.html
--rw-r--r--   0 runner    (1001) docker     (122)    24466 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/test_archives.py
--rw-r--r--   0 runner    (1001) docker     (122)    19640 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     1619 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (122)     1805 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/test_doc_archives.py
--rw-r--r--   0 runner    (1001) docker     (122)    15284 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (122)    62437 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/test_install.py
--rw-r--r--   0 runner    (1001) docker     (122)    50103 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/test_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     2416 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/test_updater.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 23:47:10.876622 aqtinstall-3.1.6/tools/
--rw-r--r--   0 runner    (1001) docker     (122)      893 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tools/build_standalone.py
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tools/launch_aqt.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 07:25:41.276274 aqtinstall-3.1.7/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/.flake8
+-rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      567 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9826 2023-08-01 07:25:41.276274 aqtinstall-3.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     8587 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 07:25:41.256274 aqtinstall-3.1.7/aqt/
+-rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/aqt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1220 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/aqt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25241 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/aqt/archives.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29231 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/aqt/combinations.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3553 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/aqt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19294 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/aqt/helper.py
+-rw-r--r--   0 runner    (1001) docker     (122)    56232 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/aqt/installer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/aqt/logging.ini
+-rw-r--r--   0 runner    (1001) docker     (122)    42535 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/aqt/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13217 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/aqt/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (122)    15062 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/aqt/updater.py
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-08-01 07:25:41.000000 aqtinstall-3.1.7/aqt/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 07:25:41.256274 aqtinstall-3.1.7/aqtinstall.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9826 2023-08-01 07:25:41.000000 aqtinstall-3.1.7/aqtinstall.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3994 2023-08-01 07:25:41.000000 aqtinstall-3.1.7/aqtinstall.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-01 07:25:41.000000 aqtinstall-3.1.7/aqtinstall.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-08-01 07:25:41.000000 aqtinstall-3.1.7/aqtinstall.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      452 2023-08-01 07:25:41.000000 aqtinstall-3.1.7/aqtinstall.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        4 2023-08-01 07:25:41.000000 aqtinstall-3.1.7/aqtinstall.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 07:25:41.260274 aqtinstall-3.1.7/ci/
+-rw-r--r--   0 runner    (1001) docker     (122)     3846 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/ci/accelbubble.7z
+-rw-r--r--   0 runner    (1001) docker     (122)    16872 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/ci/generate_azure_pipelines_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7223 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/ci/generate_combinations.py
+-rw-r--r--   0 runner    (1001) docker     (122)      439 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/ci/helloworld.7z
+-rw-r--r--   0 runner    (1001) docker     (122)  1213852 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/ci/jom_1_1_3.zip
+-rw-r--r--   0 runner    (1001) docker     (122)      801 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/ci/logging.ini
+-rw-r--r--   0 runner    (1001) docker     (122)     3134 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/ci/openglwindow.7z
+-rw-r--r--   0 runner    (1001) docker     (122)     2513 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/ci/openglwindow_qt6.7z
+-rw-r--r--   0 runner    (1001) docker     (122)     3890 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/ci/redditclient.7z
+-rw-r--r--   0 runner    (1001) docker     (122)      791 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/ci/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (122)    18931 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/ci/steps.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 07:25:41.264274 aqtinstall-3.1.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     6556 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/docs/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5708 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/docs/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1002 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/docs/CONTRIBUTE.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7672 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      504 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/docs/SECURITY.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1506 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    32406 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     9830 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6246 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    26591 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/docs/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      319 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2588 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/docs/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 07:25:41.252274 aqtinstall-3.1.7/docs/locale/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 07:25:41.252274 aqtinstall-3.1.7/docs/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 07:25:41.264274 aqtinstall-3.1.7/docs/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     8165 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/docs/locale/ja/LC_MESSAGES/CODE_OF_CONDUCT.po
+-rw-r--r--   0 runner    (1001) docker     (122)     3215 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/docs/locale/ja/LC_MESSAGES/CONTRIBUTE.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/docs/locale/ja/LC_MESSAGES/SECURITY.po
+-rw-r--r--   0 runner    (1001) docker     (122)     3980 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/docs/locale/ja/LC_MESSAGES/authors.po
+-rw-r--r--   0 runner    (1001) docker     (122)    41059 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/docs/locale/ja/LC_MESSAGES/changes.po
+-rw-r--r--   0 runner    (1001) docker     (122)    39387 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/docs/locale/ja/LC_MESSAGES/cli.po
+-rw-r--r--   0 runner    (1001) docker     (122)    14457 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/docs/locale/ja/LC_MESSAGES/configuration.po
+-rw-r--r--   0 runner    (1001) docker     (122)    46696 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/docs/locale/ja/LC_MESSAGES/getting_started.po
+-rw-r--r--   0 runner    (1001) docker     (122)      912 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/docs/locale/ja/LC_MESSAGES/index.po
+-rw-r--r--   0 runner    (1001) docker     (122)     3905 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/docs/locale/ja/LC_MESSAGES/installation.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 07:25:41.264274 aqtinstall-3.1.7/docs/locale/pot/
+-rw-r--r--   0 runner    (1001) docker     (122)     7867 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/docs/locale/pot/CODE_OF_CONDUCT.pot
+-rw-r--r--   0 runner    (1001) docker     (122)     2120 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/docs/locale/pot/CONTRIBUTE.pot
+-rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/docs/locale/pot/SECURITY.pot
+-rw-r--r--   0 runner    (1001) docker     (122)     3343 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/docs/locale/pot/authors.pot
+-rw-r--r--   0 runner    (1001) docker     (122)    40934 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/docs/locale/pot/changes.pot
+-rw-r--r--   0 runner    (1001) docker     (122)    20318 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/docs/locale/pot/cli.pot
+-rw-r--r--   0 runner    (1001) docker     (122)     7649 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/docs/locale/pot/configuration.pot
+-rw-r--r--   0 runner    (1001) docker     (122)    22725 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/docs/locale/pot/getting_started.pot
+-rw-r--r--   0 runner    (1001) docker     (122)      893 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/docs/locale/pot/index.pot
+-rw-r--r--   0 runner    (1001) docker     (122)     2894 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/docs/locale/pot/installation.pot
+-rw-r--r--   0 runner    (1001) docker     (122)     6994 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)    25779 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/docs/previous_changes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6004 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-01 07:25:41.276274 aqtinstall-3.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 07:25:41.268274 aqtinstall-3.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      274 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 07:25:41.276274 aqtinstall-3.1.7/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (122)     1468 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/linux-android-expect.json
+-rw-r--r--   0 runner    (1001) docker     (122)    18093 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/linux-android.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2319 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/linux-desktop-expect.json
+-rw-r--r--   0 runner    (1001) docker     (122)    30922 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/linux-desktop.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1468 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/mac-android-expect.json
+-rw-r--r--   0 runner    (1001) docker     (122)    16521 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/mac-android.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2351 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/mac-desktop-expect.json
+-rw-r--r--   0 runner    (1001) docker     (122)      196 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/mac-desktop-sdktool-expect.json
+-rw-r--r--   0 runner    (1001) docker     (122)      795 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/mac-desktop-sdktool-update.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      202 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/mac-desktop-tools_cmake-expect.json
+-rw-r--r--   0 runner    (1001) docker     (122)      961 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/mac-desktop-tools_cmake-update.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      361 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/mac-desktop-tools_ifw-expect.json
+-rw-r--r--   0 runner    (1001) docker     (122)      918 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/mac-desktop-tools_ifw-update.xml
+-rw-r--r--   0 runner    (1001) docker     (122)     2593 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/mac-desktop-tools_qtcreator-expect.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2072 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/mac-desktop-tools_qtcreator-update.xml
+-rw-r--r--   0 runner    (1001) docker     (122)     1979 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/mac-desktop-tools_qtdesignstudio-expect.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1504 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/mac-desktop-tools_qtdesignstudio-update.xml
+-rw-r--r--   0 runner    (1001) docker     (122)    28812 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/mac-desktop.html
+-rw-r--r--   0 runner    (1001) docker     (122)      839 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/mac-ios-expect.json
+-rw-r--r--   0 runner    (1001) docker     (122)    11401 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/mac-ios.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1920 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/mirror-expect.json
+-rw-r--r--   0 runner    (1001) docker     (122)    19653 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/mirror-first-td.html
+-rw-r--r--   0 runner    (1001) docker     (122)    17200 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/mirror-pre-a.html
+-rw-r--r--   0 runner    (1001) docker     (122)    23047 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/mirror-table-before-pre-a.html
+-rw-r--r--   0 runner    (1001) docker     (122)    76947 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/mirror-tag-in-a.html
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (122)    12460 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/settings_no_concurrency.ini
+-rw-r--r--   0 runner    (1001) docker     (122)    79658 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/windows-5140-expect.json
+-rw-r--r--   0 runner    (1001) docker     (122)    72606 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/windows-5140-update.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      285 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/windows-5140-wasm-expect.json
+-rw-r--r--   0 runner    (1001) docker     (122)    16692 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/windows-5140-wasm-update.xml
+-rw-r--r--   0 runner    (1001) docker     (122)     1494 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/windows-5150-expect.json
+-rw-r--r--   0 runner    (1001) docker     (122)   120616 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/windows-5150-update.xml
+-rw-r--r--   0 runner    (1001) docker     (122)     3914 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/windows-5152-src-doc-example-expect.json
+-rw-r--r--   0 runner    (1001) docker     (122)    18932 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/windows-5152-src-doc-example-update.xml
+-rw-r--r--   0 runner    (1001) docker     (122)    35906 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/windows-620-android-armv7-update.xml
+-rw-r--r--   0 runner    (1001) docker     (122)     1703 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/windows-620-expect.json
+-rw-r--r--   0 runner    (1001) docker     (122)    84709 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/windows-620-update.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      469 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/windows-650-wasm-multi-expect.json
+-rw-r--r--   0 runner    (1001) docker     (122)    14238 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/windows-650-wasm-multi-update.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      471 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/windows-650-wasm-single-expect.json
+-rw-r--r--   0 runner    (1001) docker     (122)    14534 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/windows-650-wasm-single-update.xml
+-rw-r--r--   0 runner    (1001) docker     (122)     1468 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/windows-android-expect.json
+-rw-r--r--   0 runner    (1001) docker     (122)    16533 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/windows-android.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2557 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/windows-desktop-expect.json
+-rw-r--r--   0 runner    (1001) docker     (122)     6580 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/windows-desktop-tools-mingw-updates.xml
+-rw-r--r--   0 runner    (1001) docker     (122)     2833 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/windows-desktop-tools-qtcreator-updates.xml
+-rw-r--r--   0 runner    (1001) docker     (122)     6115 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/windows-desktop-tools_vcredist-expect.json
+-rw-r--r--   0 runner    (1001) docker     (122)     5916 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/windows-desktop-tools_vcredist-update.xml
+-rw-r--r--   0 runner    (1001) docker     (122)    30880 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/windows-desktop.html
+-rw-r--r--   0 runner    (1001) docker     (122)      817 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/windows-winrt-expect.json
+-rw-r--r--   0 runner    (1001) docker     (122)    10501 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/data/windows-winrt.html
+-rw-r--r--   0 runner    (1001) docker     (122)    24466 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/test_archives.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19640 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1619 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1805 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/test_doc_archives.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15284 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (122)    63173 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/test_install.py
+-rw-r--r--   0 runner    (1001) docker     (122)    50353 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2416 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tests/test_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 07:25:41.276274 aqtinstall-3.1.7/tools/
+-rw-r--r--   0 runner    (1001) docker     (122)      893 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tools/build_standalone.py
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-08-01 07:25:22.000000 aqtinstall-3.1.7/tools/launch_aqt.py
```

### Comparing `aqtinstall-3.1.6/LICENSE` & `aqtinstall-3.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/MANIFEST.in` & `aqtinstall-3.1.7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/PKG-INFO` & `aqtinstall-3.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqtinstall
-Version: 3.1.6
+Version: 3.1.7
 Summary: Another unofficial Qt installer
 Author-email: Hiroshi Miura <miurahr@linux.com>
 License: MIT License
 Project-URL: Documentation, https://aqtinstall.readthedocs.io/
 Project-URL: Bug Tracker, https://github.com/miurahr/aqtinstall/issues
 Project-URL: Wiki, https://github.com/miurahr/aqtinstall/wiki
 Project-URL: Source, https://github.com/miurahr/aqtinstall
```

### Comparing `aqtinstall-3.1.6/README.rst` & `aqtinstall-3.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/aqt/__init__.py` & `aqtinstall-3.1.7/aqt/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/aqt/__main__.py` & `aqtinstall-3.1.7/aqt/__main__.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/aqt/archives.py` & `aqtinstall-3.1.7/aqt/archives.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/aqt/combinations.json` & `aqtinstall-3.1.7/aqt/combinations.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9784302896416298%*

 * *Differences: {'0': "{'modules': {insert: [(13, OrderedDict([('modules', ['debug_info', 'qt3d', 'qt5compat', "*

 * *      "'qtcharts', 'qtconnectivity', 'qtdatavis3d', 'qtgraphs', 'qtgrpc', 'qthttpserver', "*

 * *      "'qtimageformats', 'qtlanguageserver', 'qtlocation', 'qtlottie', 'qtmultimedia', "*

 * *      "'qtnetworkauth', 'qtpdf', 'qtpositioning', 'qtquick3d', 'qtquick3dphysics', "*

 * *      "'qtquickeffectmaker', 'qtquicktimeline', 'qtremoteobjects', 'qtscxml', 'qtsensors', "*

 * *      "'qtserialbus', 'qtserialport', 'qtshadertools', ' […]*

```diff
@@ -268,14 +268,53 @@
                     "qtwaylandcompositor",
                     "qtwebchannel",
                     "qtwebengine",
                     "qtwebsockets",
                     "qtwebview"
                 ],
                 "qt_version": "6.5"
+            },
+            {
+                "modules": [
+                    "debug_info",
+                    "qt3d",
+                    "qt5compat",
+                    "qtcharts",
+                    "qtconnectivity",
+                    "qtdatavis3d",
+                    "qtgraphs",
+                    "qtgrpc",
+                    "qthttpserver",
+                    "qtimageformats",
+                    "qtlanguageserver",
+                    "qtlocation",
+                    "qtlottie",
+                    "qtmultimedia",
+                    "qtnetworkauth",
+                    "qtpdf",
+                    "qtpositioning",
+                    "qtquick3d",
+                    "qtquick3dphysics",
+                    "qtquickeffectmaker",
+                    "qtquicktimeline",
+                    "qtremoteobjects",
+                    "qtscxml",
+                    "qtsensors",
+                    "qtserialbus",
+                    "qtserialport",
+                    "qtshadertools",
+                    "qtspeech",
+                    "qtvirtualkeyboard",
+                    "qtwaylandcompositor",
+                    "qtwebchannel",
+                    "qtwebengine",
+                    "qtwebsockets",
+                    "qtwebview"
+                ],
+                "qt_version": "6.6"
             }
         ],
         "new_archive": [
             "5.1.0",
             "5.2",
             "5.3.0",
             "5.3.1",
@@ -543,14 +582,20 @@
                 "arch": "win64_msvc2019_winrt_x86",
                 "os_name": "windows",
                 "target": "winrt"
             }
         ],
         "tools": [
             {
+                "arch": "qt.tools.qtcreator",
+                "os_name": "linux",
+                "target": "desktop",
+                "tool_name": "sdktool"
+            },
+            {
                 "arch": "qt.tools.cmake",
                 "os_name": "linux",
                 "target": "desktop",
                 "tool_name": "tools_cmake"
             },
             {
                 "arch": "qt.tools.conan",
@@ -567,15 +612,15 @@
             {
                 "arch": "qt.tools.sdktools.doc",
                 "os_name": "linux",
                 "target": "desktop",
                 "tool_name": "tools_generic"
             },
             {
-                "arch": "qt.tools.ifw.45",
+                "arch": "qt.tools.ifw.46",
                 "os_name": "linux",
                 "target": "desktop",
                 "tool_name": "tools_ifw"
             },
             {
                 "arch": "qt.tools.maintenance",
                 "os_name": "linux",
@@ -669,26 +714,44 @@
             {
                 "arch": "qt.tools.qtdesignstudio",
                 "os_name": "linux",
                 "target": "desktop",
                 "tool_name": "tools_qtdesignstudio_generation2"
             },
             {
+                "arch": "qtdesignstudio.lts",
+                "os_name": "linux",
+                "target": "desktop",
+                "tool_name": "tools_qtdesignstudio_generation2_lts"
+            },
+            {
                 "arch": "qt.tools.qtcreator.telemetry",
                 "os_name": "linux",
                 "target": "desktop",
                 "tool_name": "tools_telemetry"
             },
             {
+                "arch": "qt.tools.qtcreator_gui.telemetry_evaluator",
+                "os_name": "linux",
+                "target": "desktop",
+                "tool_name": "tools_telemetry_eval_gui"
+            },
+            {
                 "arch": "qt.tools.qtcreator_gui.telemetry",
                 "os_name": "linux",
                 "target": "desktop",
                 "tool_name": "tools_telemetry_gui"
             },
             {
+                "arch": "qt.tools.qtcreator",
+                "os_name": "mac",
+                "target": "desktop",
+                "tool_name": "sdktool"
+            },
+            {
                 "arch": "qt.tools.cmake",
                 "os_name": "mac",
                 "target": "desktop",
                 "tool_name": "tools_cmake"
             },
             {
                 "arch": "qt.tools.conan",
@@ -705,15 +768,15 @@
             {
                 "arch": "qt.tools.sdktools.doc",
                 "os_name": "mac",
                 "target": "desktop",
                 "tool_name": "tools_generic"
             },
             {
-                "arch": "qt.tools.ifw.45",
+                "arch": "qt.tools.ifw.46",
                 "os_name": "mac",
                 "target": "desktop",
                 "tool_name": "tools_ifw"
             },
             {
                 "arch": "qt.tools.maintenance",
                 "os_name": "mac",
@@ -777,26 +840,44 @@
             {
                 "arch": "qt.tools.qtdesignstudio",
                 "os_name": "mac",
                 "target": "desktop",
                 "tool_name": "tools_qtdesignstudio_generation2"
             },
             {
+                "arch": "qtdesignstudio.lts",
+                "os_name": "mac",
+                "target": "desktop",
+                "tool_name": "tools_qtdesignstudio_generation2_lts"
+            },
+            {
                 "arch": "qt.tools.qtcreator.telemetry",
                 "os_name": "mac",
                 "target": "desktop",
                 "tool_name": "tools_telemetry"
             },
             {
+                "arch": "qt.tools.qtcreator_gui.telemetry_evaluator",
+                "os_name": "mac",
+                "target": "desktop",
+                "tool_name": "tools_telemetry_eval_gui"
+            },
+            {
                 "arch": "qt.tools.qtcreator_gui.telemetry",
                 "os_name": "mac",
                 "target": "desktop",
                 "tool_name": "tools_telemetry_gui"
             },
             {
+                "arch": "qt.tools.qtcreator",
+                "os_name": "windows",
+                "target": "desktop",
+                "tool_name": "sdktool"
+            },
+            {
                 "arch": "qt.tools.cmake",
                 "os_name": "windows",
                 "target": "desktop",
                 "tool_name": "tools_cmake"
             },
             {
                 "arch": "qt.tools.conan",
@@ -813,15 +894,15 @@
             {
                 "arch": "qt.tools.sdktools.doc",
                 "os_name": "windows",
                 "target": "desktop",
                 "tool_name": "tools_generic"
             },
             {
-                "arch": "qt.tools.ifw.45",
+                "arch": "qt.tools.ifw.46",
                 "os_name": "windows",
                 "target": "desktop",
                 "tool_name": "tools_ifw"
             },
             {
                 "arch": "qt.tools.maintenance",
                 "os_name": "windows",
@@ -999,20 +1080,32 @@
             {
                 "arch": "qt.tools.qtdesignstudio",
                 "os_name": "windows",
                 "target": "desktop",
                 "tool_name": "tools_qtdesignstudio_generation2"
             },
             {
+                "arch": "qtdesignstudio.lts",
+                "os_name": "windows",
+                "target": "desktop",
+                "tool_name": "tools_qtdesignstudio_generation2_lts"
+            },
+            {
                 "arch": "qt.tools.qtcreator.telemetry",
                 "os_name": "windows",
                 "target": "desktop",
                 "tool_name": "tools_telemetry"
             },
             {
+                "arch": "qt.tools.qtcreator_gui.telemetry_evaluator",
+                "os_name": "windows",
+                "target": "desktop",
+                "tool_name": "tools_telemetry_eval_gui"
+            },
+            {
                 "arch": "qt.tools.qtcreator_gui.telemetry",
                 "os_name": "windows",
                 "target": "desktop",
                 "tool_name": "tools_telemetry_gui"
             },
             {
                 "arch": "qt.tools.vcredist",
@@ -1131,11 +1224,14 @@
             "6.3.0",
             "6.3.1",
             "6.3.2",
             "6.4.0",
             "6.4.1",
             "6.4.2",
             "6.4.3",
-            "6.5.0"
+            "6.5.0",
+            "6.5.1",
+            "6.5.2",
+            "6.6.0"
         ]
     }
 ]
```

### Comparing `aqtinstall-3.1.6/aqt/exceptions.py` & `aqtinstall-3.1.7/aqt/exceptions.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/aqt/helper.py` & `aqtinstall-3.1.7/aqt/helper.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/aqt/installer.py` & `aqtinstall-3.1.7/aqt/installer.py`

 * *Files 0% similar despite different names*

```diff
@@ -911,19 +911,19 @@
 
     def _make_list_tool_parser(self, subparsers: argparse._SubParsersAction):
         """Creates a subparser that works with the MetadataFactory, and adds it to the `subparsers` parameter"""
         list_parser: ListArgumentParser = subparsers.add_parser(
             "list-tool",
             formatter_class=argparse.RawDescriptionHelpFormatter,
             epilog="Examples:\n"
-            "$ aqt list-tool mac desktop                 # print all tools for mac desktop\n"
-            "$ aqt list-tool mac desktop tools_ifw       # print all tool variant names for QtIFW\n"
-            "$ aqt list-tool mac desktop ifw             # print all tool variant names for QtIFW\n"
-            "$ aqt list-tool mac desktop -l tools_ifw    # print tool variant names with metadata for QtIFW\n"
-            "$ aqt list-tool mac desktop -l ifw          # print tool variant names with metadata for QtIFW\n",
+            "$ aqt list-tool mac desktop                   # print all tools for mac desktop\n"
+            "$ aqt list-tool mac desktop tools_ifw         # print all tool variant names for QtIFW\n"
+            "$ aqt list-tool mac desktop ifw               # print all tool variant names for QtIFW\n"
+            "$ aqt list-tool mac desktop tools_ifw --long  # print tool variant names with metadata for QtIFW\n"
+            "$ aqt list-tool mac desktop ifw --long        # print tool variant names with metadata for QtIFW\n",
         )
         list_parser.add_argument("host", choices=["linux", "mac", "windows"], help="host os name")
         list_parser.add_argument(
             "target",
             nargs="?",
             default=None,
             choices=["desktop", "winrt", "android", "ios"],
```

### Comparing `aqtinstall-3.1.6/aqt/logging.ini` & `aqtinstall-3.1.7/aqt/logging.ini`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/aqt/metadata.py` & `aqtinstall-3.1.7/aqt/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -539,15 +539,18 @@
         self.logger = getLogger("aqt.metadata")
         self.archive_id = archive_id
         self.spec = spec
         self.base_url = base_url
 
         if archive_id.is_tools():
             if tool_name is not None:
-                _tool_name: str = "tools_" + tool_name if not tool_name.startswith("tools_") else tool_name
+                if not tool_name.startswith("tools_") and tool_name != "sdktool":
+                    _tool_name = f"tools_{tool_name}"
+                else:
+                    _tool_name = tool_name
                 if is_long_listing:
                     self.request_type = "tool long listing"
                     self._action: MetadataFactory.Action = lambda: self.fetch_tool_long_listing(_tool_name)
                 else:
                     self.request_type = "tool variant names"
                     self._action = lambda: self.fetch_tool_modules(_tool_name)
             else:
@@ -729,14 +732,16 @@
             soup: bs4.BeautifulSoup = bs4.BeautifulSoup(html_doc, "html.parser")
             for link in soup.find_all("a"):
                 folder: str = link_to_folder(link)
                 if not folder:
                     continue
                 if folder.startswith(filter_category):
                     yield folder
+                if filter_category == "tools" and folder == "sdktool":
+                    yield folder
         except Exception as e:
             raise ArchiveConnectionError(
                 f"Failed to retrieve the expected HTML page at {html_url}",
                 suggested_action=[
                     "Check your network connection.",
                     f"Make sure that you can access {html_url} in your web browser.",
                 ],
```

### Comparing `aqtinstall-3.1.6/aqt/settings.ini` & `aqtinstall-3.1.7/aqt/settings.ini`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/aqt/updater.py` & `aqtinstall-3.1.7/aqt/updater.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/aqtinstall.egg-info/PKG-INFO` & `aqtinstall-3.1.7/aqtinstall.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqtinstall
-Version: 3.1.6
+Version: 3.1.7
 Summary: Another unofficial Qt installer
 Author-email: Hiroshi Miura <miurahr@linux.com>
 License: MIT License
 Project-URL: Documentation, https://aqtinstall.readthedocs.io/
 Project-URL: Bug Tracker, https://github.com/miurahr/aqtinstall/issues
 Project-URL: Wiki, https://github.com/miurahr/aqtinstall/wiki
 Project-URL: Source, https://github.com/miurahr/aqtinstall
```

### Comparing `aqtinstall-3.1.6/aqtinstall.egg-info/SOURCES.txt` & `aqtinstall-3.1.7/aqtinstall.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,16 @@
 tests/data/linux-android-expect.json
 tests/data/linux-android.html
 tests/data/linux-desktop-expect.json
 tests/data/linux-desktop.html
 tests/data/mac-android-expect.json
 tests/data/mac-android.html
 tests/data/mac-desktop-expect.json
+tests/data/mac-desktop-sdktool-expect.json
+tests/data/mac-desktop-sdktool-update.xml
 tests/data/mac-desktop-tools_cmake-expect.json
 tests/data/mac-desktop-tools_cmake-update.xml
 tests/data/mac-desktop-tools_ifw-expect.json
 tests/data/mac-desktop-tools_ifw-update.xml
 tests/data/mac-desktop-tools_qtcreator-expect.json
 tests/data/mac-desktop-tools_qtcreator-update.xml
 tests/data/mac-desktop-tools_qtdesignstudio-expect.json
```

### Comparing `aqtinstall-3.1.6/ci/accelbubble.7z` & `aqtinstall-3.1.7/ci/accelbubble.7z`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/ci/generate_azure_pipelines_matrices.py` & `aqtinstall-3.1.7/ci/generate_azure_pipelines_matrices.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/ci/generate_combinations.py` & `aqtinstall-3.1.7/ci/generate_combinations.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/ci/jom_1_1_3.zip` & `aqtinstall-3.1.7/ci/jom_1_1_3.zip`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/ci/logging.ini` & `aqtinstall-3.1.7/ci/logging.ini`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/ci/openglwindow.7z` & `aqtinstall-3.1.7/ci/openglwindow.7z`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/ci/openglwindow_qt6.7z` & `aqtinstall-3.1.7/ci/openglwindow_qt6.7z`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/ci/redditclient.7z` & `aqtinstall-3.1.7/ci/redditclient.7z`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/ci/settings.ini` & `aqtinstall-3.1.7/ci/settings.ini`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/ci/steps.yml` & `aqtinstall-3.1.7/ci/steps.yml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/docs/CHANGELOG.rst` & `aqtinstall-3.1.7/docs/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,33 @@
 ==========
 
 All notable changes to this project will be documented in this file.
 
 `Unreleased`_
 =============
 
+`v3.1.7`_ (1, Aug. 2023)
+========================
+
+Added
+-----
+Add support for standalone sdktool installation(#677)
+
+Fixed
+-----
+- Fixed command to check tools_mingw90 (#680)
+- Fixed help text for list-tool
+
+Changed
+-------
+* Add Qt 6.6.0, 6.5.2 and 6.5.1 as known version(#685,#698)
+* Default blacklist setting(#689)
+* Add test for sdktool(#678)
+
+
 `v3.1.6`_ (4, May, 2023)
 ========================
 
 Added
 -----
 * Add opensslv3 as known module (#674)
 * Add code signature for standalone binary
@@ -223,15 +242,16 @@
 --------
 * Use secrets for secure random numbers(#498)
 * Use defusedxml to parse Updates.xml file to avoid attack(#498)
 * Improve get_hash function(#504)
 * Check Update.xml file with SHA256 hash (#493)
 
 
-.. _Unreleased: https://github.com/miurahr/aqtinstall/compare/v3.1.6...HEAD
+.. _Unreleased: https://github.com/miurahr/aqtinstall/compare/v3.1.7...HEAD
+.. _v3.1.7: https://github.com/miurahr/aqtinstall/compare/v3.1.6...v3.1.7
 .. _v3.1.6: https://github.com/miurahr/aqtinstall/compare/v3.1.5...v3.1.6
 .. _v3.1.5: https://github.com/miurahr/aqtinstall/compare/v3.1.4...v3.1.5
 .. _v3.1.4: https://github.com/miurahr/aqtinstall/compare/v3.1.3...v3.1.4
 .. _v3.1.3: https://github.com/miurahr/aqtinstall/compare/v3.1.2...v3.1.3
 .. _v3.1.2: https://github.com/miurahr/aqtinstall/compare/v3.1.1...v3.1.2
 .. _v3.1.1: https://github.com/miurahr/aqtinstall/compare/v3.1.0...v3.1.1
 .. _v3.1.0: https://github.com/miurahr/aqtinstall/compare/v3.0.2...v3.1.0
```

### Comparing `aqtinstall-3.1.6/docs/CODE_OF_CONDUCT.rst` & `aqtinstall-3.1.7/docs/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/docs/CONTRIBUTE.rst` & `aqtinstall-3.1.7/docs/CONTRIBUTE.rst`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/docs/Makefile` & `aqtinstall-3.1.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/docs/authors.rst` & `aqtinstall-3.1.7/docs/authors.rst`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/docs/cli.rst` & `aqtinstall-3.1.7/docs/cli.rst`

 * *Files 1% similar despite different names*

```diff
@@ -383,15 +383,15 @@
     In the past, our users have had success using 7-zip_ on Windows, Linux and Mac.
     You can install 7-zip on Windows with Choco_.
     The Linux/Mac port of 7-zip is called ``p7zip``, and you can install it with brew_ on Mac,
     or on Linux with your package manager.
 
 .. _py7zr: https://pypi.org/project/py7zr/
 .. _7-zip: https://www.7-zip.org/
-.. _Choco: https://community.chocolatey.org/packages/7zip/19.0
+.. _Choco: https://community.chocolatey.org/packages/7zip/
 .. _brew: https://formulae.brew.sh/formula/p7zip
 
 .. option:: --internal
 
     Use the internal extractor, py7zr_
 
 .. option:: --keep, -k
@@ -939,15 +939,15 @@
     set PATH=C:\Qt\Tools\mingw1120_64\bin
 
 .. note::
 
     This is not a typo; it is a mislabelled tool name!
     ``tools_mingw90`` and the tool variant ``qt.tools.win64_mingw900``
     do not contain MinGW 9.0.0; they actually contain MinGW 11.2.0!
-    Verify with ``aqt list-tool windows desktop --long-modules tools_mingw90``
+    Verify with ``aqt list-tool --long windows desktop tools_mingw90``
     in a wide terminal.
 
 
 Example: Show help message
 
 .. code-block:: console
```

### Comparing `aqtinstall-3.1.6/docs/conf.py` & `aqtinstall-3.1.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/docs/configuration.rst` & `aqtinstall-3.1.7/docs/configuration.rst`

 * *Files 5% similar despite different names*

```diff
@@ -152,14 +152,14 @@
     ``aqtinstall`` uses the SHA-256 algorithm to perform this check.
 
 blacklist:
     It is a list of URL where is a problematic mirror site.
     Some mirror sites ignore a connection from IP addresses out of their preffered one.
     It will cause connection error or connection timeout.
     There are some known mirror sites in default.
-    When you are happy with the default sites,
-    you can override with your custom settings.
+    If you are not happy with the default sites,
+    you can override them with custom settings.
 
 fallbacks:
     It is a list of URL where is a good for access.
     When mirror site cause an error, aqt use fallbacks when possible.
     You can find a list of mirrors at: https://download.qt.io/static/mirrorlist/
```

### Comparing `aqtinstall-3.1.6/docs/getting_started.rst` & `aqtinstall-3.1.7/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/docs/installation.rst` & `aqtinstall-3.1.7/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/docs/locale/ja/LC_MESSAGES/CODE_OF_CONDUCT.po` & `aqtinstall-3.1.7/docs/locale/ja/LC_MESSAGES/CODE_OF_CONDUCT.po`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/docs/locale/ja/LC_MESSAGES/CONTRIBUTE.po` & `aqtinstall-3.1.7/docs/locale/ja/LC_MESSAGES/CONTRIBUTE.po`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/docs/locale/ja/LC_MESSAGES/SECURITY.po` & `aqtinstall-3.1.7/docs/locale/ja/LC_MESSAGES/SECURITY.po`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/docs/locale/ja/LC_MESSAGES/authors.po` & `aqtinstall-3.1.7/docs/locale/ja/LC_MESSAGES/authors.po`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/docs/locale/ja/LC_MESSAGES/changes.po` & `aqtinstall-3.1.7/docs/locale/ja/LC_MESSAGES/changes.po`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/docs/locale/ja/LC_MESSAGES/cli.po` & `aqtinstall-3.1.7/docs/locale/ja/LC_MESSAGES/cli.po`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/docs/locale/ja/LC_MESSAGES/configuration.po` & `aqtinstall-3.1.7/docs/locale/ja/LC_MESSAGES/configuration.po`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/docs/locale/ja/LC_MESSAGES/getting_started.po` & `aqtinstall-3.1.7/docs/locale/ja/LC_MESSAGES/getting_started.po`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/docs/locale/ja/LC_MESSAGES/index.po` & `aqtinstall-3.1.7/docs/locale/ja/LC_MESSAGES/index.po`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/docs/locale/ja/LC_MESSAGES/installation.po` & `aqtinstall-3.1.7/docs/locale/ja/LC_MESSAGES/installation.po`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/docs/locale/pot/CODE_OF_CONDUCT.pot` & `aqtinstall-3.1.7/docs/locale/pot/CODE_OF_CONDUCT.pot`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/docs/locale/pot/CONTRIBUTE.pot` & `aqtinstall-3.1.7/docs/locale/pot/CONTRIBUTE.pot`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/docs/locale/pot/SECURITY.pot` & `aqtinstall-3.1.7/docs/locale/pot/SECURITY.pot`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/docs/locale/pot/authors.pot` & `aqtinstall-3.1.7/docs/locale/pot/authors.pot`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/docs/locale/pot/changes.pot` & `aqtinstall-3.1.7/docs/locale/pot/changes.pot`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/docs/locale/pot/cli.pot` & `aqtinstall-3.1.7/docs/locale/pot/cli.pot`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/docs/locale/pot/configuration.pot` & `aqtinstall-3.1.7/docs/locale/pot/configuration.pot`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/docs/locale/pot/getting_started.pot` & `aqtinstall-3.1.7/docs/locale/pot/getting_started.pot`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/docs/locale/pot/index.pot` & `aqtinstall-3.1.7/docs/locale/pot/index.pot`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/docs/locale/pot/installation.pot` & `aqtinstall-3.1.7/docs/locale/pot/installation.pot`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/docs/make.bat` & `aqtinstall-3.1.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/docs/previous_changes.rst` & `aqtinstall-3.1.7/docs/previous_changes.rst`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/pyproject.toml` & `aqtinstall-3.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tests/data/linux-android-expect.json` & `aqtinstall-3.1.7/tests/data/linux-android-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tests/data/linux-android.html` & `aqtinstall-3.1.7/tests/data/linux-android.html`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tests/data/linux-desktop-expect.json` & `aqtinstall-3.1.7/tests/data/linux-desktop-expect.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9919354838709677%*

 * *Differences: {"'tools'": "{insert: [(30, 'sdktool')]}"}*

```diff
@@ -79,10 +79,11 @@
         "tools_ninja",
         "tools_maintenance_update_reminder",
         "tools_maintenance_early_access",
         "tools_maintenance",
         "tools_ifw",
         "tools_generic",
         "tools_conan",
-        "tools_cmake"
+        "tools_cmake",
+        "sdktool"
     ]
 }
```

### Comparing `aqtinstall-3.1.6/tests/data/linux-desktop.html` & `aqtinstall-3.1.7/tests/data/linux-desktop.html`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 <tr><td valign="top">&nbsp;</td><td><a href="tools_maintenance_update_reminder/">tools_maintenance_update_reminder/</a></td><td align="right">02-Feb-2018 10:00  </td><td align="right">  - </td><td>&nbsp;</td></tr>
 <tr><td valign="top">&nbsp;</td><td><a href="tools_maintenance_early_access/">tools_maintenance_early_access/</a></td><td align="right">30-Sep-2020 12:48  </td><td align="right">  - </td><td>&nbsp;</td></tr>
 <tr><td valign="top">&nbsp;</td><td><a href="tools_maintenance/">tools_maintenance/</a></td><td align="right">13-Apr-2021 14:41  </td><td align="right">  - </td><td>&nbsp;</td></tr>
 <tr><td valign="top">&nbsp;</td><td><a href="tools_ifw/">tools_ifw/</a></td><td align="right">13-Apr-2021 14:58  </td><td align="right">  - </td><td>&nbsp;</td></tr>
 <tr><td valign="top">&nbsp;</td><td><a href="tools_generic/">tools_generic/</a></td><td align="right">13-Apr-2021 14:39  </td><td align="right">  - </td><td>&nbsp;</td></tr>
 <tr><td valign="top">&nbsp;</td><td><a href="tools_conan/">tools_conan/</a></td><td align="right">15-Feb-2021 12:14  </td><td align="right">  - </td><td>&nbsp;</td></tr>
 <tr><td valign="top">&nbsp;</td><td><a href="tools_cmake/">tools_cmake/</a></td><td align="right">07-Jan-2021 14:22  </td><td align="right">  - </td><td>&nbsp;</td></tr>
+<tr><td valign="top">&nbsp;</td><td><a href="sdktool/">sdktool/</a></td><td align="right">05-May-2023 10:53  </td><td align="right">  - </td><td>&nbsp;</td></tr>
 <tr><td valign="top">&nbsp;</td><td><a href="qt6_650_wasm_singlethread/">qt6_650_wasm_singlethread/</a></td><td align="right">01-Jan-2023 00:00 </td><td align="right">  - </td><td>&nbsp;</td></tr>
 <tr><td valign="top">&nbsp;</td><td><a href="qt6_650_wasm_multithread/">qt6_650_wasm_multithread/</a></td><td align="right">01-Jan-2023 00:00   </td><td align="right">  - </td><td>&nbsp;</td></tr>
 <tr><td valign="top">&nbsp;</td><td><a href="qt6_650_src_doc_examples/">qt6_650_src_doc_examples/</a></td><td align="right">01-Jan-2023 00:00   </td><td align="right">  - </td><td>&nbsp;</td></tr>
 <tr><td valign="top">&nbsp;</td><td><a href="qt6_650/">qt6_650/</a></td><td align="right">01-Jan-2023 00:00  </td><td align="right">  - </td><td>&nbsp;</td></tr>
 <tr><td valign="top">&nbsp;</td><td><a href="qt6_620_wasm/">qt6_620_wasm/</a></td><td align="right">29-Sep-2021 12:46  </td><td align="right">  - </td><td>&nbsp;</td></tr>
 <tr><td valign="top">&nbsp;</td><td><a href="qt6_620_src_doc_examples/">qt6_620_src_doc_examples/</a></td><td align="right">29-Sep-2021 12:43  </td><td align="right">  - </td><td>&nbsp;</td></tr>
 <tr><td valign="top">&nbsp;</td><td><a href="qt6_620/">qt6_620/</a></td><td align="right">29-Sep-2021 12:34  </td><td align="right">  - </td><td>&nbsp;</td></tr>
```

#### html2text {}

```diff
@@ -28,14 +28,15 @@
  tools_maintenance_update_reminder/            02-Feb-2018 10:00    -  
  tools_maintenance_early_access/               30-Sep-2020 12:48    -  
  tools_maintenance/                            13-Apr-2021 14:41    -  
  tools_ifw/                                    13-Apr-2021 14:58    -  
  tools_generic/                                13-Apr-2021 14:39    -  
  tools_conan/                                  15-Feb-2021 12:14    -  
  tools_cmake/                                  07-Jan-2021 14:22    -  
+ sdktool/                                      05-May-2023 10:53    -  
  qt6_650_wasm_singlethread/                    01-Jan-2023 00:00    -  
  qt6_650_wasm_multithread/                     01-Jan-2023 00:00    -  
  qt6_650_src_doc_examples/                     01-Jan-2023 00:00    -  
  qt6_650/                                      01-Jan-2023 00:00    -  
  qt6_620_wasm/                                 29-Sep-2021 12:46    -  
  qt6_620_src_doc_examples/                     29-Sep-2021 12:43    -  
  qt6_620/                                      29-Sep-2021 12:34    -
```

### Comparing `aqtinstall-3.1.6/tests/data/mac-android-expect.json` & `aqtinstall-3.1.7/tests/data/mac-android-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tests/data/mac-android.html` & `aqtinstall-3.1.7/tests/data/mac-android.html`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tests/data/mac-desktop-expect.json` & `aqtinstall-3.1.7/tests/data/mac-desktop-expect.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9919354838709677%*

 * *Differences: {"'tools'": "{insert: [(30, 'sdktool')]}"}*

```diff
@@ -80,10 +80,11 @@
         "tools_ninja",
         "tools_maintenance_update_reminder",
         "tools_maintenance_early_access",
         "tools_maintenance",
         "tools_ifw",
         "tools_generic",
         "tools_conan",
-        "tools_cmake"
+        "tools_cmake",
+        "sdktool"
     ]
 }
```

### Comparing `aqtinstall-3.1.6/tests/data/mac-desktop-tools_cmake-update.xml` & `aqtinstall-3.1.7/tests/data/mac-desktop-tools_cmake-update.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tests/data/mac-desktop-tools_ifw-update.xml` & `aqtinstall-3.1.7/tests/data/mac-desktop-tools_ifw-update.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tests/data/mac-desktop-tools_qtcreator-expect.json` & `aqtinstall-3.1.7/tests/data/mac-desktop-tools_qtcreator-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tests/data/mac-desktop-tools_qtcreator-update.xml` & `aqtinstall-3.1.7/tests/data/mac-desktop-tools_qtcreator-update.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tests/data/mac-desktop-tools_qtdesignstudio-expect.json` & `aqtinstall-3.1.7/tests/data/mac-desktop-tools_qtdesignstudio-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tests/data/mac-desktop-tools_qtdesignstudio-update.xml` & `aqtinstall-3.1.7/tests/data/mac-desktop-tools_qtdesignstudio-update.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tests/data/mac-desktop.html` & `aqtinstall-3.1.7/tests/data/mac-desktop.html`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 <tr><td valign="top">&nbsp;</td><td><a href="tools_maintenance_update_reminder/">tools_maintenance_update_reminder/</a></td><td align="right">02-Feb-2018 10:00  </td><td align="right">  - </td><td>&nbsp;</td></tr>
 <tr><td valign="top">&nbsp;</td><td><a href="tools_maintenance_early_access/">tools_maintenance_early_access/</a></td><td align="right">30-Sep-2020 12:48  </td><td align="right">  - </td><td>&nbsp;</td></tr>
 <tr><td valign="top">&nbsp;</td><td><a href="tools_maintenance/">tools_maintenance/</a></td><td align="right">13-Apr-2021 14:41  </td><td align="right">  - </td><td>&nbsp;</td></tr>
 <tr><td valign="top">&nbsp;</td><td><a href="tools_ifw/">tools_ifw/</a></td><td align="right">13-Apr-2021 14:58  </td><td align="right">  - </td><td>&nbsp;</td></tr>
 <tr><td valign="top">&nbsp;</td><td><a href="tools_generic/">tools_generic/</a></td><td align="right">13-Apr-2021 14:39  </td><td align="right">  - </td><td>&nbsp;</td></tr>
 <tr><td valign="top">&nbsp;</td><td><a href="tools_conan/">tools_conan/</a></td><td align="right">15-Feb-2021 12:15  </td><td align="right">  - </td><td>&nbsp;</td></tr>
 <tr><td valign="top">&nbsp;</td><td><a href="tools_cmake/">tools_cmake/</a></td><td align="right">07-Jan-2021 14:22  </td><td align="right">  - </td><td>&nbsp;</td></tr>
+<tr><td valign="top">&nbsp;</td><td><a href="sdktool/">sdktool/</a></td><td align="right">05-May-2023 10:53  </td><td align="right">  - </td><td>&nbsp;</td></tr>
 <tr><td valign="top">&nbsp;</td><td><a href="qt6_650_wasm_singlethread/">qt6_650_wasm_singlethread/</a></td><td align="right">01-Jan-2023 00:00 </td><td align="right">  - </td><td>&nbsp;</td></tr>
 <tr><td valign="top">&nbsp;</td><td><a href="qt6_650_wasm_multithread/">qt6_650_wasm_multithread/</a></td><td align="right">01-Jan-2023 00:00   </td><td align="right">  - </td><td>&nbsp;</td></tr>
 <tr><td valign="top">&nbsp;</td><td><a href="qt6_650_src_doc_examples/">qt6_650_src_doc_examples/</a></td><td align="right">01-Jan-2023 00:00   </td><td align="right">  - </td><td>&nbsp;</td></tr>
 <tr><td valign="top">&nbsp;</td><td><a href="qt6_650/">qt6_650/</a></td><td align="right">01-Jan-2023 00:00  </td><td align="right">  - </td><td>&nbsp;</td></tr>
 <tr><td valign="top">&nbsp;</td><td><a href="qt6_620_wasm/">qt6_620_wasm/</a></td><td align="right">29-Sep-2021 12:46  </td><td align="right">  - </td><td>&nbsp;</td></tr>
 <tr><td valign="top">&nbsp;</td><td><a href="qt6_620_src_doc_examples/">qt6_620_src_doc_examples/</a></td><td align="right">29-Sep-2021 12:43  </td><td align="right">  - </td><td>&nbsp;</td></tr>
 <tr><td valign="top">&nbsp;</td><td><a href="qt6_620/">qt6_620/</a></td><td align="right">29-Sep-2021 12:34  </td><td align="right">  - </td><td>&nbsp;</td></tr>
```

#### html2text {}

```diff
@@ -28,14 +28,15 @@
  tools_maintenance_update_reminder/            02-Feb-2018 10:00    -  
  tools_maintenance_early_access/               30-Sep-2020 12:48    -  
  tools_maintenance/                            13-Apr-2021 14:41    -  
  tools_ifw/                                    13-Apr-2021 14:58    -  
  tools_generic/                                13-Apr-2021 14:39    -  
  tools_conan/                                  15-Feb-2021 12:15    -  
  tools_cmake/                                  07-Jan-2021 14:22    -  
+ sdktool/                                      05-May-2023 10:53    -  
  qt6_650_wasm_singlethread/                    01-Jan-2023 00:00    -  
  qt6_650_wasm_multithread/                     01-Jan-2023 00:00    -  
  qt6_650_src_doc_examples/                     01-Jan-2023 00:00    -  
  qt6_650/                                      01-Jan-2023 00:00    -  
  qt6_620_wasm/                                 29-Sep-2021 12:46    -  
  qt6_620_src_doc_examples/                     29-Sep-2021 12:43    -  
  qt6_620/                                      29-Sep-2021 12:34    -
```

### Comparing `aqtinstall-3.1.6/tests/data/mac-ios-expect.json` & `aqtinstall-3.1.7/tests/data/mac-ios-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tests/data/mac-ios.html` & `aqtinstall-3.1.7/tests/data/mac-ios.html`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tests/data/mirror-expect.json` & `aqtinstall-3.1.7/tests/data/mirror-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tests/data/mirror-first-td.html` & `aqtinstall-3.1.7/tests/data/mirror-first-td.html`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tests/data/mirror-pre-a.html` & `aqtinstall-3.1.7/tests/data/mirror-pre-a.html`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tests/data/mirror-table-before-pre-a.html` & `aqtinstall-3.1.7/tests/data/mirror-table-before-pre-a.html`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tests/data/mirror-tag-in-a.html` & `aqtinstall-3.1.7/tests/data/mirror-tag-in-a.html`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tests/data/settings_no_concurrency.ini` & `aqtinstall-3.1.7/tests/data/settings_no_concurrency.ini`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tests/data/windows-5140-expect.json` & `aqtinstall-3.1.7/tests/data/windows-5140-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tests/data/windows-5140-update.xml` & `aqtinstall-3.1.7/tests/data/windows-5140-update.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tests/data/windows-5140-wasm-update.xml` & `aqtinstall-3.1.7/tests/data/windows-5140-wasm-update.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tests/data/windows-5150-expect.json` & `aqtinstall-3.1.7/tests/data/windows-5150-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tests/data/windows-5150-update.xml` & `aqtinstall-3.1.7/tests/data/windows-5150-update.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tests/data/windows-5152-src-doc-example-expect.json` & `aqtinstall-3.1.7/tests/data/windows-5152-src-doc-example-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tests/data/windows-5152-src-doc-example-update.xml` & `aqtinstall-3.1.7/tests/data/windows-5152-src-doc-example-update.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tests/data/windows-620-android-armv7-update.xml` & `aqtinstall-3.1.7/tests/data/windows-620-android-armv7-update.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tests/data/windows-620-expect.json` & `aqtinstall-3.1.7/tests/data/windows-620-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tests/data/windows-620-update.xml` & `aqtinstall-3.1.7/tests/data/windows-620-update.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tests/data/windows-650-wasm-multi-update.xml` & `aqtinstall-3.1.7/tests/data/windows-650-wasm-multi-update.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tests/data/windows-650-wasm-single-update.xml` & `aqtinstall-3.1.7/tests/data/windows-650-wasm-single-update.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tests/data/windows-android-expect.json` & `aqtinstall-3.1.7/tests/data/windows-android-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tests/data/windows-android.html` & `aqtinstall-3.1.7/tests/data/windows-android.html`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tests/data/windows-desktop-expect.json` & `aqtinstall-3.1.7/tests/data/windows-desktop-expect.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9930555555555556%*

 * *Differences: {"'tools'": "{insert: [(35, 'sdktool')]}"}*

```diff
@@ -91,10 +91,11 @@
         "tools_mingw",
         "tools_maintenance_update_reminder",
         "tools_maintenance_early_access",
         "tools_maintenance",
         "tools_ifw",
         "tools_generic",
         "tools_conan",
-        "tools_cmake"
+        "tools_cmake",
+        "sdktool"
     ]
 }
```

### Comparing `aqtinstall-3.1.6/tests/data/windows-desktop-tools-mingw-updates.xml` & `aqtinstall-3.1.7/tests/data/windows-desktop-tools-mingw-updates.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tests/data/windows-desktop-tools-qtcreator-updates.xml` & `aqtinstall-3.1.7/tests/data/windows-desktop-tools-qtcreator-updates.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tests/data/windows-desktop-tools_vcredist-expect.json` & `aqtinstall-3.1.7/tests/data/windows-desktop-tools_vcredist-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tests/data/windows-desktop-tools_vcredist-update.xml` & `aqtinstall-3.1.7/tests/data/windows-desktop-tools_vcredist-update.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tests/data/windows-desktop.html` & `aqtinstall-3.1.7/tests/data/windows-desktop.html`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 <tr><td valign="top">&nbsp;</td><td><a href="tools_maintenance_update_reminder/">tools_maintenance_update_reminder/</a></td><td align="right">02-Feb-2018 10:00  </td><td align="right">  - </td><td>&nbsp;</td></tr>
 <tr><td valign="top">&nbsp;</td><td><a href="tools_maintenance_early_access/">tools_maintenance_early_access/</a></td><td align="right">30-Sep-2020 12:48  </td><td align="right">  - </td><td>&nbsp;</td></tr>
 <tr><td valign="top">&nbsp;</td><td><a href="tools_maintenance/">tools_maintenance/</a></td><td align="right">13-Apr-2021 14:41  </td><td align="right">  - </td><td>&nbsp;</td></tr>
 <tr><td valign="top">&nbsp;</td><td><a href="tools_ifw/">tools_ifw/</a></td><td align="right">13-Apr-2021 14:58  </td><td align="right">  - </td><td>&nbsp;</td></tr>
 <tr><td valign="top">&nbsp;</td><td><a href="tools_generic/">tools_generic/</a></td><td align="right">13-Apr-2021 14:39  </td><td align="right">  - </td><td>&nbsp;</td></tr>
 <tr><td valign="top">&nbsp;</td><td><a href="tools_conan/">tools_conan/</a></td><td align="right">15-Feb-2021 12:15  </td><td align="right">  - </td><td>&nbsp;</td></tr>
 <tr><td valign="top">&nbsp;</td><td><a href="tools_cmake/">tools_cmake/</a></td><td align="right">07-Jan-2021 14:22  </td><td align="right">  - </td><td>&nbsp;</td></tr>
+<tr><td valign="top">&nbsp;</td><td><a href="sdktool/">sdktool/</a></td><td align="right">05-May-2023 10:53  </td><td align="right">  - </td><td>&nbsp;</td></tr>
 <tr><td valign="top">&nbsp;</td><td><a href="qt6_650_wasm_singlethread/">qt6_650_wasm_singlethread/</a></td><td align="right">01-Jan-2023 00:00 </td><td align="right">  - </td><td>&nbsp;</td></tr>
 <tr><td valign="top">&nbsp;</td><td><a href="qt6_650_wasm_multithread/">qt6_650_wasm_multithread/</a></td><td align="right">01-Jan-2023 00:00   </td><td align="right">  - </td><td>&nbsp;</td></tr>
 <tr><td valign="top">&nbsp;</td><td><a href="qt6_650_src_doc_examples/">qt6_650_src_doc_examples/</a></td><td align="right">01-Jan-2023 00:00   </td><td align="right">  - </td><td>&nbsp;</td></tr>
 <tr><td valign="top">&nbsp;</td><td><a href="qt6_650/">qt6_650/</a></td><td align="right">01-Jan-2023 00:00  </td><td align="right">  - </td><td>&nbsp;</td></tr>
 <tr><td valign="top">&nbsp;</td><td><a href="qt6_620_wasm/">qt6_620_wasm/</a></td><td align="right">29-Sep-2021 12:46  </td><td align="right">  - </td><td>&nbsp;</td></tr>
 <tr><td valign="top">&nbsp;</td><td><a href="qt6_620_src_doc_examples/">qt6_620_src_doc_examples/</a></td><td align="right">29-Sep-2021 12:43  </td><td align="right">  - </td><td>&nbsp;</td></tr>
 <tr><td valign="top">&nbsp;</td><td><a href="qt6_620/">qt6_620/</a></td><td align="right">29-Sep-2021 12:34  </td><td align="right">  - </td><td>&nbsp;</td></tr>
```

#### html2text {}

```diff
@@ -33,14 +33,15 @@
  tools_maintenance_update_reminder/            02-Feb-2018 10:00    -  
  tools_maintenance_early_access/               30-Sep-2020 12:48    -  
  tools_maintenance/                            13-Apr-2021 14:41    -  
  tools_ifw/                                    13-Apr-2021 14:58    -  
  tools_generic/                                13-Apr-2021 14:39    -  
  tools_conan/                                  15-Feb-2021 12:15    -  
  tools_cmake/                                  07-Jan-2021 14:22    -  
+ sdktool/                                      05-May-2023 10:53    -  
  qt6_650_wasm_singlethread/                    01-Jan-2023 00:00    -  
  qt6_650_wasm_multithread/                     01-Jan-2023 00:00    -  
  qt6_650_src_doc_examples/                     01-Jan-2023 00:00    -  
  qt6_650/                                      01-Jan-2023 00:00    -  
  qt6_620_wasm/                                 29-Sep-2021 12:46    -  
  qt6_620_src_doc_examples/                     29-Sep-2021 12:43    -  
  qt6_620/                                      29-Sep-2021 12:34    -
```

### Comparing `aqtinstall-3.1.6/tests/data/windows-winrt-expect.json` & `aqtinstall-3.1.7/tests/data/windows-winrt-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tests/data/windows-winrt.html` & `aqtinstall-3.1.7/tests/data/windows-winrt.html`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tests/test_archives.py` & `aqtinstall-3.1.7/tests/test_archives.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tests/test_cli.py` & `aqtinstall-3.1.7/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tests/test_connection.py` & `aqtinstall-3.1.7/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tests/test_doc_archives.py` & `aqtinstall-3.1.7/tests/test_doc_archives.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tests/test_helper.py` & `aqtinstall-3.1.7/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tests/test_install.py` & `aqtinstall-3.1.7/tests/test_install.py`

 * *Files 2% similar despite different names*

```diff
@@ -308,14 +308,31 @@
                 r"INFO    : Downloading qt.tools.qtcreator...\n"
                 r"Finished installation of tools_qtcreator-linux-qt.tools.qtcreator.7z in .*\n"
                 r"INFO    : Finished installation\n"
                 r"INFO    : Time elapsed: .* second"
             ),
         ),
         (
+            "install-tool linux desktop sdktool qt.tools.qtcreator".split(),
+            "linux",
+            "desktop",
+            "10.0.1-0-202305050734",
+            {"std": ""},
+            {"std": ""},
+            {"std": "linux_x64/desktop/sdktool/Updates.xml"},
+            {"std": [tool_archive("linux", "sdktool", "qt.tools.qtcreator")]},
+            re.compile(
+                r"^INFO    : aqtinstall\(aqt\) v.* on Python 3.*\n"
+                r"INFO    : Downloading qt.tools.qtcreator...\n"
+                r"Finished installation of sdktool-linux-qt.tools.qtcreator.7z in .*\n"
+                r"INFO    : Finished installation\n"
+                r"INFO    : Time elapsed: .* second"
+            ),
+        ),
+        (
             "tool linux tools_qtcreator 1.2.3-0-197001020304 qt.tools.qtcreator".split(),
             "linux",
             "desktop",
             "1.2.3",
             {"std": ""},
             {"std": ""},
             {"std": "linux_x64/desktop/tools_qtcreator/Updates.xml"},
```

### Comparing `aqtinstall-3.1.6/tests/test_list.py` & `aqtinstall-3.1.7/tests/test_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1062,15 +1062,21 @@
     for variant_name, *values in raw_tooldata:
         assert len(keys) == len(values)
         tools[variant_name] = {k: v for k, v in zip(keys, values)}
 
     return ToolData(tools)
 
 
-@pytest.mark.parametrize("host, target, tool_name", (("mac", "desktop", "tools_cmake"),))
+@pytest.mark.parametrize(
+    "host, target, tool_name",
+    (
+        ("mac", "desktop", "tools_cmake"),
+        ("mac", "desktop", "sdktool"),
+    ),
+)
 def test_list_tool_cli(monkeypatch, capsys, host: str, target: str, tool_name: str):
     html_file = f"{host}-{target}.html"
     xml_file = f"{host}-{target}-{tool_name}-update.xml"
     html_expect = f"{host}-{target}-expect.json"
     xml_expect = f"{host}-{target}-{tool_name}-expect.json"
     htmltext, xmltext, htmljson, xmljson = [
         (Path(__file__).parent / "data" / filename).read_text("utf-8")
@@ -1080,43 +1086,47 @@
     xml_data = json.loads(xmljson)
     expected_tool_modules = set(xml_data["modules"])
 
     def _mock_fetch_http(_, rest_of_url, *args, **kwargs: str) -> str:
         if not rest_of_url.endswith("Updates.xml"):
             return htmltext
         folder = urlparse(rest_of_url).path.split("/")[-2]
-        assert folder.startswith("tools_")
+        assert folder.startswith("tools_") or folder in ["sdktool"]
         return xmltext
 
     monkeypatch.setattr(MetadataFactory, "fetch_http", _mock_fetch_http)
 
     cli = Cli()
     cli.run(["list-tool", host, target])
     out, err = capsys.readouterr()
+    assert not err
     output_set = set(out.strip().split())
     assert output_set == expected_tools
 
     cli.run(["list-tool", host, target, tool_name])
     out, err = capsys.readouterr()
+    assert not err
     output_set = set(out.strip().split())
     assert output_set == expected_tool_modules
 
     # Test abbreviated tool name: "aqt list-tool mac desktop ifw"
-    assert tool_name.startswith("tools_")
-    short_tool_name = tool_name[6:]
+    assert tool_name.startswith("tools_") or tool_name in ["sdktool"]
+    short_tool_name = tool_name[6:] if tool_name.startswith("tools_") else tool_name
     cli.run(["list-tool", host, target, short_tool_name])
     out, err = capsys.readouterr()
+    assert not err
     output_set = set(out.strip().split())
     assert output_set == expected_tool_modules
 
     cli.run(["list-tool", host, target, tool_name, "-l"])
     out, err = capsys.readouterr()
+    assert not err
 
     expected_tooldata = format(fetch_expected_tooldata(xml_expect))
-    assert out.strip() == expected_tooldata
+    assert out.strip() == expected_tooldata.strip()
 
 
 def test_fetch_http_ok(monkeypatch):
     html_content = b"some_html_content"
     base_url = "https://alt.baseurl.com"
 
     def mock_getUrl(url: str, *args, **kwargs) -> str:
```

### Comparing `aqtinstall-3.1.6/tests/test_updater.py` & `aqtinstall-3.1.7/tests/test_updater.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.6/tools/build_standalone.py` & `aqtinstall-3.1.7/tools/build_standalone.py`

 * *Files identical despite different names*

