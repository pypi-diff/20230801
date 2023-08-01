# Comparing `tmp/icepapcms-3.4.1.tar.gz` & `tmp/icepapcms-3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/icepapcms-3.4.1.tar", last modified: Fri Mar 17 11:38:51 2023, max compression
+gzip compressed data, was "dist/icepapcms-3.4.2.tar", last modified: Tue Aug  1 09:48:11 2023, max compression
```

## Comparing `icepapcms-3.4.1.tar` & `icepapcms-3.4.2.tar`

### file list

```diff
@@ -1,231 +1,231 @@
-drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-03-17 11:38:51.000000 icepapcms-3.4.1/
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    21215 2023-03-17 11:37:04.000000 icepapcms-3.4.1/CHANGELOG.md
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     5483 2021-03-22 08:15:01.000000 icepapcms-3.4.1/CONTRIBUTING.md
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      956 2020-04-16 09:52:08.000000 icepapcms-3.4.1/LICENSE.txt
--rw-r--r--   0 rhoms     (1268) Computing  (1000)      475 2021-03-22 08:15:01.000000 icepapcms-3.4.1/MANIFEST.in
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     1409 2023-03-17 11:38:51.000000 icepapcms-3.4.1/PKG-INFO
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     1385 2021-04-09 15:17:01.000000 icepapcms-3.4.1/README.md
-drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-03-17 11:38:51.000000 icepapcms-3.4.1/distribute/
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      299 2020-04-16 09:52:08.000000 icepapcms-3.4.1/distribute/icepapcms.desktop
-drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-03-17 11:38:51.000000 icepapcms-3.4.1/icepapcms/
--rw-r--r--   0 rhoms     (1268) Computing  (1000)        0 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/__init__.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     4179 2023-03-17 11:37:04.000000 icepapcms-3.4.1/icepapcms/__main__.py
-drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-03-17 11:38:51.000000 icepapcms-3.4.1/icepapcms/db/
--rw-r--r--   0 rhoms     (1268) Computing  (1000)        0 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/db/__init__.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     3553 2021-03-25 15:42:51.000000 icepapcms-3.4.1/icepapcms/db/creates-mysql.sql
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     1731 2021-11-12 16:15:59.000000 icepapcms-3.4.1/icepapcms/db/creates_sqlite.sql
--rw-r--r--   0 rhoms     (1268) Computing  (1000)      118 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/db/db_notes.txt
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    88018 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/db/dbmodel.mwb
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      125 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/db/mysql-to-sqlite.sh
-drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-03-17 11:38:51.000000 icepapcms-3.4.1/icepapcms/doc/
--rw-r--r--   0 rhoms     (1268) Computing  (1000)   890238 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/doc/IcePAP_HardwareManual.pdf
--rw-r--r--   0 rhoms     (1268) Computing  (1000)  2318629 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/doc/IcePAP_UserManual-1.0b-150526-fw3.11+.pdf
--rw-r--r--   0 rhoms     (1268) Computing  (1000)  2318629 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/doc/IcePAP_UserManual.pdf
--rw-r--r--   0 rhoms     (1268) Computing  (1000)  1848816 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/doc/IcePAP_UserManual_last.pdf
--rw-r--r--   0 rhoms     (1268) Computing  (1000)   815208 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/doc/IcePAP_UserManual_working.pdf
--rw-r--r--   0 rhoms     (1268) Computing  (1000)   520534 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/doc/IcepapCMSUserManual.pdf
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     4735 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/doc/Icepapicon.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)        0 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/doc/__init__.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    13052 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/doc/remoteserver_setup.txt
-drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-03-17 11:38:51.000000 icepapcms-3.4.1/icepapcms/gui/
-drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-03-17 11:38:51.000000 icepapcms-3.4.1/icepapcms/gui/Led/
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     4301 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/Led/Led.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)       21 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/Led/__init__.py
-drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-03-17 11:38:51.000000 icepapcms-3.4.1/icepapcms/gui/Led/images24/
--rw-r--r--   0 rhoms     (1268) Computing  (1000)        0 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/Led/images24/__init__.py
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     1363 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/Led/images24/ledblue.png
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     1248 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/Led/images24/ledblueoff.png
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     1307 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/Led/images24/ledgreen.png
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     1244 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/Led/images24/ledgreenoff.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     1260 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/Led/images24/ledorange.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     1223 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/Led/images24/ledorangeoff.png
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     1165 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/Led/images24/ledred.png
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     1188 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/Led/images24/ledredoff.png
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     1257 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/Led/images24/ledyellow.png
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     1256 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/Led/images24/ledyellowoff.png
-drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-03-17 11:38:51.000000 icepapcms-3.4.1/icepapcms/gui/Led/images48/
--rw-r--r--   0 rhoms     (1268) Computing  (1000)        0 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/Led/images48/__init__.py
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     3370 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/Led/images48/ledblue.png
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     3102 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/Led/images48/ledblueoff.png
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     3152 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/Led/images48/ledgreen.png
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     3043 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/Led/images48/ledgreenoff.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     2935 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/Led/images48/ledorange.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     2981 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/Led/images48/ledorangeoff.png
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     2889 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/Led/images48/ledred.png
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     2793 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/Led/images48/ledredoff.png
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     3164 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/Led/images48/ledyellow.png
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     3119 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/Led/images48/ledyellowoff.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)       91 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/__init__.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     2450 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/dialogaddicepap.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     1419 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/dialogaddlocation.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     1878 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/dialogconflictdriver_expert.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     1942 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/dialogconflictdriver_nonexpert.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     5029 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/dialogdriverconflict.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     5908 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/dialoghomesrch.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     8115 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/dialogipapprogram.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     2430 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/dialognewdriver.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    11173 2021-11-12 16:15:59.000000 icepapcms-3.4.1/icepapcms/gui/dialogpreferences.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     3599 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/dialogsnapshot.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     7490 2021-04-23 14:38:32.000000 icepapcms-3.4.1/icepapcms/gui/dialogstatusinfo.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     5429 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/historiccfgwidget.py
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)    12918 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/icepap_treemodel.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    45714 2023-03-17 11:37:48.000000 icepapcms-3.4.1/icepapcms/gui/icepapcms.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     8453 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/icepapdriverwidget.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     1196 2023-03-17 11:37:04.000000 icepapcms-3.4.1/icepapcms/gui/ipapconsole.py
-drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-03-17 11:38:51.000000 icepapcms-3.4.1/icepapcms/gui/ldap/
--rw-r--r--   0 rhoms     (1268) Computing  (1000)        0 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ldap/__init__.py
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     4064 2021-05-14 07:12:13.000000 icepapcms-3.4.1/icepapcms/gui/ldap/login.py
-drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-03-17 11:38:51.000000 icepapcms-3.4.1/icepapcms/gui/ldap/ui/
--rw-r--r--   0 rhoms     (1268) Computing  (1000)       23 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ldap/ui/__init__.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)       86 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ldap/ui/login.qrc
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     3485 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ldap/ui/login.ui
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    26261 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ldap/ui/login_rc.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     6010 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ldap/ui/password.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     1448 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/messagedialogs.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    11557 2021-06-30 09:56:40.000000 icepapcms-3.4.1/icepapcms/gui/pageipapcrate.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    67225 2023-03-17 11:37:04.000000 icepapcms-3.4.1/icepapcms/gui/pageipapdriver.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    13791 2021-06-30 09:56:40.000000 icepapcms-3.4.1/icepapcms/gui/pageipapsystem.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     8064 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/pyconsoletext.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     2070 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/qvalidatelineedit.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     8309 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/templatescatalogwidget.py
-drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-03-17 11:38:51.000000 icepapcms-3.4.1/icepapcms/gui/ui/
--rw-r--r--   0 rhoms     (1268) Computing  (1000)       27 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/__init__.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    51603 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/axis.ui
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    22083 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/closedloop.ui
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    46937 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/dialogaddicepap.ui
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    17338 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/dialogaddlocation.ui
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     2461 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/dialogconflictdriver_expert.ui
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     2422 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/dialogconflictdriver_nonexpert.ui
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    29135 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/dialogdriverconflict.ui
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    22387 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/dialoghistoriccfg.ui
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    11862 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/dialoghomesrch.ui
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     9575 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/dialogipapprogram.ui
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     3140 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/dialognewdriver.ui
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    34397 2021-11-12 16:15:59.000000 icepapcms-3.4.1/icepapcms/gui/ui/dialogpreferences.ui
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     1685 2021-03-12 15:47:31.000000 icepapcms-3.4.1/icepapcms/gui/ui/dialogstatusinfo.ui
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    17671 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/dialogsystemscan.ui
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    49410 2021-05-06 10:12:05.000000 icepapcms-3.4.1/icepapcms/gui/ui/encoders.ui
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     8445 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/historiccfgwidget.ui
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    19172 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/homing.ui
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     3230 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icepapcms.qrc
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    23972 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icepapcms.ui
--rw-r--r--   0 rhoms     (1268) Computing  (1000)  1740723 2021-06-04 07:17:30.000000 icepapcms-3.4.1/icepapcms/gui/ui/icepapcms_rc.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    35795 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icepapdriverwidget.ui
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    33408 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icepapdriverwidgetsmall.ui
-drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-03-17 11:38:51.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    10998 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/Icepap.png
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)    63788 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/IcepapBig.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    25333 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/IcepapMed.png
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     3060 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/Icepapdriverpetit.png
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)    31136 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/Icepapicon.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)       65 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/__init__.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    28972 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/approved.gif
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    74725 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/axis.png
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     4067 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/backup.png
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     2733 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/calendar.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     3799 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/camera.svg
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     1633 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/close.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     6269 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/connect.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     3766 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/database.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     4795 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/disconnect.png
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     3449 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/emblem-keys.png
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     3390 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/emblem-people.png
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     2113 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/emblem-question.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    39822 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/encoder.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     3388 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/export.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     3371 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/file-roller.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     2159 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/folder-remote.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     2829 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/folder.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     4676 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/gconf-editor.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     2905 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/gnome-cpu.png
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     1764 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/gnome-dev-floppy.png
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     3706 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/gnome-dev-harddisk.png
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     3868 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/gnome-dev-network.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     2481 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/gnome-logout.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     2728 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/gnome-monitor.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     4798 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/gnome-nettool.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     1473 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/gnome-session-halt.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     3732 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/gnome-settings.png
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     4552 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/gnome-terminal.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     3717 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/gnome-workspace.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     2057 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/go-next.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     2034 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/go-previous.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     1917 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/go-up.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     3399 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/help-browser.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     3283 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/import.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     1186 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/ipapcrate.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     1080 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/ipapdriver.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     1073 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/ipapdrivercfg.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     1306 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/ipapdrivererror.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     1097 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/ipapdrivermodified.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     1265 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/ipapdrivermoved.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     1359 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/ipapdrivernew.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     1217 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/ipapdriverwarning.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)      840 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/ipapsys.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     1104 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/ipapsyserror.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)      833 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/ipapsysoffline.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     1059 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/ipapsyswarning.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     4205 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/keys.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     3948 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/ldap_icon.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)      891 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/list-add.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)      596 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/list-remove.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)      861 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/mysql.gif
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     1270 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/network-server.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     3735 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/notes.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     7880 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/oscilloscope.svg
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     2005 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/package-x-generic.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     3142 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/postgresql.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     3986 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/preferences-system.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     3110 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/quit.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)      155 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/redpixel.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     4367 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/sign.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     2599 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/sqlite.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     3498 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/system-users.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     3731 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/update-manager.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     4402 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/icons/view-refresh.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    35901 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/io.ui
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     5196 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/ipapconsole.ui
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    92770 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/ipaptestpage.ui
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    27406 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/motor.ui
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    87820 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/pageipapdriver.ui
-drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-03-17 11:38:51.000000 icepapcms-3.4.1/icepapcms/gui/ui/small_icons/
--rw-r--r--   0 rhoms     (1268) Computing  (1000)        0 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/small_icons/__init__.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)      940 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/small_icons/go-absolute.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)      930 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/small_icons/go-relative.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)      955 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/small_icons/go-relative2.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     1054 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/small_icons/historic.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)      386 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/small_icons/list-add.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)      252 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/small_icons/list-remove.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     1272 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/small_icons/process-stop.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)      787 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/small_icons/save.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)      773 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/small_icons/template.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     1047 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/small_icons/undo.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     1364 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/small_icons/view-refresh.png
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     2898 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/gui/ui/snapshot.ui
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     1248 2021-03-25 08:46:59.000000 icepapcms-3.4.1/icepapcms/helpers.py
-drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-03-17 11:38:51.000000 icepapcms-3.4.1/icepapcms/lib/
--rw-r--r--   0 rhoms     (1268) Computing  (1000)      213 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/lib/__init__.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     5376 2023-03-17 11:15:42.000000 icepapcms-3.4.1/icepapcms/lib/configmanager.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)      748 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/lib/conflict.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     4972 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/lib/icepapdriver.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     4444 2021-06-30 09:56:40.000000 icepapcms-3.4.1/icepapcms/lib/icepapdrivercfg.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    31937 2021-06-23 10:09:07.000000 icepapcms-3.4.1/icepapcms/lib/icepapsmanager.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    12538 2021-07-01 14:02:39.000000 icepapcms-3.4.1/icepapcms/lib/icepapsystem.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    24558 2021-03-25 15:42:51.000000 icepapcms-3.4.1/icepapcms/lib/mainmanager.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    11024 2021-03-25 15:42:51.000000 icepapcms-3.4.1/icepapcms/lib/sanpshot.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)      797 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/lib/singleton.py
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     7263 2021-11-12 16:15:59.000000 icepapcms-3.4.1/icepapcms/lib/stormmanager.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     8977 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/lib/stormmysql.py
-drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-03-17 11:38:51.000000 icepapcms-3.4.1/icepapcms/templates/
--rw-r--r--   0 rhoms     (1268) Computing  (1000)        0 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/templates/__init__.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     5558 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/templates/catalog.xml
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     7022 2021-03-22 08:15:01.000000 icepapcms-3.4.1/icepapcms/templates/driverparameters.xml
-drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-03-17 11:38:51.000000 icepapcms-3.4.1/icepapcms.egg-info/
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     1409 2023-03-17 11:38:51.000000 icepapcms-3.4.1/icepapcms.egg-info/PKG-INFO
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     7567 2023-03-17 11:38:51.000000 icepapcms-3.4.1/icepapcms.egg-info/SOURCES.txt
--rw-r--r--   0 rhoms     (1268) Computing  (1000)        1 2023-03-17 11:38:51.000000 icepapcms-3.4.1/icepapcms.egg-info/dependency_links.txt
--rw-r--r--   0 rhoms     (1268) Computing  (1000)       96 2023-03-17 11:38:51.000000 icepapcms-3.4.1/icepapcms.egg-info/entry_points.txt
--rw-r--r--   0 rhoms     (1268) Computing  (1000)       72 2023-03-17 11:38:51.000000 icepapcms-3.4.1/icepapcms.egg-info/requires.txt
--rw-r--r--   0 rhoms     (1268) Computing  (1000)       10 2023-03-17 11:38:51.000000 icepapcms-3.4.1/icepapcms.egg-info/top_level.txt
--rw-r--r--   0 rhoms     (1268) Computing  (1000)       38 2023-03-17 11:38:51.000000 icepapcms-3.4.1/setup.cfg
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     2131 2023-03-17 11:37:48.000000 icepapcms-3.4.1/setup.py
+drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-08-01 09:48:11.000000 icepapcms-3.4.2/
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    21511 2023-08-01 09:01:26.000000 icepapcms-3.4.2/CHANGELOG.md
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     5483 2021-03-22 08:15:01.000000 icepapcms-3.4.2/CONTRIBUTING.md
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      956 2020-04-16 09:52:08.000000 icepapcms-3.4.2/LICENSE.txt
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)      475 2021-03-22 08:15:01.000000 icepapcms-3.4.2/MANIFEST.in
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     1409 2023-08-01 09:48:11.000000 icepapcms-3.4.2/PKG-INFO
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     1385 2021-04-09 15:17:01.000000 icepapcms-3.4.2/README.md
+drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-08-01 09:48:11.000000 icepapcms-3.4.2/distribute/
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      299 2020-04-16 09:52:08.000000 icepapcms-3.4.2/distribute/icepapcms.desktop
+drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-08-01 09:48:11.000000 icepapcms-3.4.2/icepapcms/
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)        0 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/__init__.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     4179 2023-03-17 11:37:04.000000 icepapcms-3.4.2/icepapcms/__main__.py
+drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-08-01 09:48:11.000000 icepapcms-3.4.2/icepapcms/db/
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)        0 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/db/__init__.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     3553 2021-03-25 15:42:51.000000 icepapcms-3.4.2/icepapcms/db/creates-mysql.sql
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     1731 2021-11-12 16:15:59.000000 icepapcms-3.4.2/icepapcms/db/creates_sqlite.sql
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)      118 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/db/db_notes.txt
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    88018 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/db/dbmodel.mwb
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      125 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/db/mysql-to-sqlite.sh
+drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-08-01 09:48:11.000000 icepapcms-3.4.2/icepapcms/doc/
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)   890238 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/doc/IcePAP_HardwareManual.pdf
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)  2318629 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/doc/IcePAP_UserManual-1.0b-150526-fw3.11+.pdf
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)  2318629 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/doc/IcePAP_UserManual.pdf
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)  1848816 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/doc/IcePAP_UserManual_last.pdf
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)   815208 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/doc/IcePAP_UserManual_working.pdf
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)   520534 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/doc/IcepapCMSUserManual.pdf
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     4735 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/doc/Icepapicon.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)        0 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/doc/__init__.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    13052 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/doc/remoteserver_setup.txt
+drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-08-01 09:48:11.000000 icepapcms-3.4.2/icepapcms/gui/
+drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-08-01 09:48:11.000000 icepapcms-3.4.2/icepapcms/gui/Led/
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     4301 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/Led/Led.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)       21 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/Led/__init__.py
+drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-08-01 09:48:11.000000 icepapcms-3.4.2/icepapcms/gui/Led/images24/
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)        0 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/Led/images24/__init__.py
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     1363 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/Led/images24/ledblue.png
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     1248 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/Led/images24/ledblueoff.png
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     1307 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/Led/images24/ledgreen.png
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     1244 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/Led/images24/ledgreenoff.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     1260 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/Led/images24/ledorange.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     1223 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/Led/images24/ledorangeoff.png
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     1165 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/Led/images24/ledred.png
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     1188 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/Led/images24/ledredoff.png
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     1257 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/Led/images24/ledyellow.png
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     1256 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/Led/images24/ledyellowoff.png
+drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-08-01 09:48:11.000000 icepapcms-3.4.2/icepapcms/gui/Led/images48/
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)        0 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/Led/images48/__init__.py
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     3370 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/Led/images48/ledblue.png
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     3102 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/Led/images48/ledblueoff.png
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     3152 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/Led/images48/ledgreen.png
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     3043 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/Led/images48/ledgreenoff.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     2935 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/Led/images48/ledorange.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     2981 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/Led/images48/ledorangeoff.png
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     2889 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/Led/images48/ledred.png
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     2793 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/Led/images48/ledredoff.png
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     3164 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/Led/images48/ledyellow.png
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     3119 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/Led/images48/ledyellowoff.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)       91 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/__init__.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     2450 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/dialogaddicepap.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     1419 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/dialogaddlocation.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     1878 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/dialogconflictdriver_expert.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     1942 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/dialogconflictdriver_nonexpert.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     5029 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/dialogdriverconflict.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     5908 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/dialoghomesrch.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     8115 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/dialogipapprogram.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     2430 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/dialognewdriver.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    11173 2021-11-12 16:15:59.000000 icepapcms-3.4.2/icepapcms/gui/dialogpreferences.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     4040 2023-08-01 09:01:26.000000 icepapcms-3.4.2/icepapcms/gui/dialogsnapshot.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     7490 2021-04-23 14:38:32.000000 icepapcms-3.4.2/icepapcms/gui/dialogstatusinfo.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     5429 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/historiccfgwidget.py
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)    12918 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/icepap_treemodel.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    45714 2023-08-01 09:04:35.000000 icepapcms-3.4.2/icepapcms/gui/icepapcms.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     8453 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/icepapdriverwidget.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     1196 2023-03-17 11:37:04.000000 icepapcms-3.4.2/icepapcms/gui/ipapconsole.py
+drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-08-01 09:48:11.000000 icepapcms-3.4.2/icepapcms/gui/ldap/
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)        0 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ldap/__init__.py
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     4064 2021-05-14 07:12:13.000000 icepapcms-3.4.2/icepapcms/gui/ldap/login.py
+drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-08-01 09:48:11.000000 icepapcms-3.4.2/icepapcms/gui/ldap/ui/
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)       23 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ldap/ui/__init__.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)       86 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ldap/ui/login.qrc
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     3485 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ldap/ui/login.ui
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    26261 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ldap/ui/login_rc.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     6010 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ldap/ui/password.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     1448 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/messagedialogs.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    11557 2021-06-30 09:56:40.000000 icepapcms-3.4.2/icepapcms/gui/pageipapcrate.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    67225 2023-03-17 11:37:04.000000 icepapcms-3.4.2/icepapcms/gui/pageipapdriver.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    13791 2021-06-30 09:56:40.000000 icepapcms-3.4.2/icepapcms/gui/pageipapsystem.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     8064 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/pyconsoletext.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     2070 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/qvalidatelineedit.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     8309 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/templatescatalogwidget.py
+drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-08-01 09:48:11.000000 icepapcms-3.4.2/icepapcms/gui/ui/
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)       27 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/__init__.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    51603 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/axis.ui
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    22083 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/closedloop.ui
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    46937 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/dialogaddicepap.ui
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    17338 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/dialogaddlocation.ui
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     2461 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/dialogconflictdriver_expert.ui
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     2422 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/dialogconflictdriver_nonexpert.ui
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    29135 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/dialogdriverconflict.ui
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    22387 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/dialoghistoriccfg.ui
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    11862 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/dialoghomesrch.ui
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     9575 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/dialogipapprogram.ui
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     3140 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/dialognewdriver.ui
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    34397 2021-11-12 16:15:59.000000 icepapcms-3.4.2/icepapcms/gui/ui/dialogpreferences.ui
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     1685 2021-03-12 15:47:31.000000 icepapcms-3.4.2/icepapcms/gui/ui/dialogstatusinfo.ui
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    17671 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/dialogsystemscan.ui
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    49410 2021-05-06 10:12:05.000000 icepapcms-3.4.2/icepapcms/gui/ui/encoders.ui
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     8445 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/historiccfgwidget.ui
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    19172 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/homing.ui
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     3230 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icepapcms.qrc
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    23972 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icepapcms.ui
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)  1740723 2021-06-04 07:17:30.000000 icepapcms-3.4.2/icepapcms/gui/ui/icepapcms_rc.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    35795 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icepapdriverwidget.ui
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    33408 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icepapdriverwidgetsmall.ui
+drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-08-01 09:48:11.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    10998 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/Icepap.png
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)    63788 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/IcepapBig.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    25333 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/IcepapMed.png
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     3060 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/Icepapdriverpetit.png
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)    31136 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/Icepapicon.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)       65 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/__init__.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    28972 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/approved.gif
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    74725 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/axis.png
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     4067 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/backup.png
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     2733 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/calendar.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     3799 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/camera.svg
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     1633 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/close.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     6269 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/connect.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     3766 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/database.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     4795 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/disconnect.png
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     3449 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/emblem-keys.png
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     3390 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/emblem-people.png
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     2113 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/emblem-question.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    39822 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/encoder.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     3388 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/export.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     3371 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/file-roller.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     2159 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/folder-remote.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     2829 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/folder.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     4676 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/gconf-editor.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     2905 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/gnome-cpu.png
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     1764 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/gnome-dev-floppy.png
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     3706 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/gnome-dev-harddisk.png
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     3868 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/gnome-dev-network.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     2481 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/gnome-logout.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     2728 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/gnome-monitor.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     4798 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/gnome-nettool.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     1473 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/gnome-session-halt.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     3732 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/gnome-settings.png
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     4552 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/gnome-terminal.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     3717 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/gnome-workspace.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     2057 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/go-next.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     2034 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/go-previous.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     1917 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/go-up.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     3399 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/help-browser.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     3283 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/import.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     1186 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/ipapcrate.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     1080 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/ipapdriver.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     1073 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/ipapdrivercfg.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     1306 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/ipapdrivererror.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     1097 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/ipapdrivermodified.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     1265 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/ipapdrivermoved.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     1359 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/ipapdrivernew.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     1217 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/ipapdriverwarning.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)      840 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/ipapsys.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     1104 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/ipapsyserror.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)      833 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/ipapsysoffline.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     1059 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/ipapsyswarning.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     4205 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/keys.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     3948 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/ldap_icon.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)      891 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/list-add.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)      596 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/list-remove.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)      861 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/mysql.gif
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     1270 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/network-server.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     3735 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/notes.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     7880 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/oscilloscope.svg
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     2005 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/package-x-generic.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     3142 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/postgresql.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     3986 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/preferences-system.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     3110 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/quit.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)      155 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/redpixel.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     4367 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/sign.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     2599 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/sqlite.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     3498 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/system-users.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     3731 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/update-manager.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     4402 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/icons/view-refresh.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    35901 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/io.ui
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     5196 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/ipapconsole.ui
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    92770 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/ipaptestpage.ui
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    27406 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/motor.ui
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    87820 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/pageipapdriver.ui
+drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-08-01 09:48:11.000000 icepapcms-3.4.2/icepapcms/gui/ui/small_icons/
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)        0 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/small_icons/__init__.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)      940 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/small_icons/go-absolute.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)      930 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/small_icons/go-relative.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)      955 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/small_icons/go-relative2.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     1054 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/small_icons/historic.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)      386 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/small_icons/list-add.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)      252 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/small_icons/list-remove.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     1272 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/small_icons/process-stop.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)      787 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/small_icons/save.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)      773 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/small_icons/template.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     1047 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/small_icons/undo.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     1364 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/small_icons/view-refresh.png
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     2898 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/gui/ui/snapshot.ui
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     1248 2021-03-25 08:46:59.000000 icepapcms-3.4.2/icepapcms/helpers.py
+drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-08-01 09:48:11.000000 icepapcms-3.4.2/icepapcms/lib/
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)      213 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/lib/__init__.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     5376 2023-03-17 11:15:42.000000 icepapcms-3.4.2/icepapcms/lib/configmanager.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)      748 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/lib/conflict.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     4972 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/lib/icepapdriver.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     4444 2021-06-30 09:56:40.000000 icepapcms-3.4.2/icepapcms/lib/icepapdrivercfg.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    32309 2023-08-01 09:01:26.000000 icepapcms-3.4.2/icepapcms/lib/icepapsmanager.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    12538 2021-07-01 14:02:39.000000 icepapcms-3.4.2/icepapcms/lib/icepapsystem.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    24558 2021-03-25 15:42:51.000000 icepapcms-3.4.2/icepapcms/lib/mainmanager.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)      797 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/lib/singleton.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    11665 2023-08-01 09:01:26.000000 icepapcms-3.4.2/icepapcms/lib/snapshot.py
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     7263 2021-11-12 16:15:59.000000 icepapcms-3.4.2/icepapcms/lib/stormmanager.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     8977 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/lib/stormmysql.py
+drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-08-01 09:48:11.000000 icepapcms-3.4.2/icepapcms/templates/
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)        0 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/templates/__init__.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     5558 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/templates/catalog.xml
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     7022 2021-03-22 08:15:01.000000 icepapcms-3.4.2/icepapcms/templates/driverparameters.xml
+drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-08-01 09:48:11.000000 icepapcms-3.4.2/icepapcms.egg-info/
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     1409 2023-08-01 09:48:11.000000 icepapcms-3.4.2/icepapcms.egg-info/PKG-INFO
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     7567 2023-08-01 09:48:11.000000 icepapcms-3.4.2/icepapcms.egg-info/SOURCES.txt
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)        1 2023-08-01 09:48:11.000000 icepapcms-3.4.2/icepapcms.egg-info/dependency_links.txt
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)       96 2023-08-01 09:48:11.000000 icepapcms-3.4.2/icepapcms.egg-info/entry_points.txt
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)       72 2023-08-01 09:48:11.000000 icepapcms-3.4.2/icepapcms.egg-info/requires.txt
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)       10 2023-08-01 09:48:11.000000 icepapcms-3.4.2/icepapcms.egg-info/top_level.txt
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)       38 2023-08-01 09:48:11.000000 icepapcms-3.4.2/setup.cfg
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     2131 2023-08-01 09:04:35.000000 icepapcms-3.4.2/setup.py
```

### Comparing `icepapcms-3.4.1/CHANGELOG.md` & `icepapcms-3.4.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 IcepapCMS 3.4.x
 -------------------------------------------------------------------------
 Added:
 * Use icepapctl as new console for Linux
+* Include host on snapshot filename
+
 
 Fixed:
 * Console dialog fixed to xterm size
 * Fix wrong casting value for QSpinBox to support python >= 3.10
 * Exclude configobj 5.0.7 package because introduces a regression
 * Use correct configured log folder
+* Snapshot crashes with corrupted axis configuration
+* Show drives when there are corrupted axes configuration
+* Fix wrong casting value for QProgressBar to support python >= 3.10
+* Fix typo on snapshot module
  
 Removed:
 * Original QT console
 * Console Icon is disabled on Windows OS, the icepapctl console is not 
   supported
-
+* Snapshot of target, shaft and control enconders
 
 
 IcepapCMS 3.3.1
 -------------------------------------------------------------------------
 Added:
 * Allow to have a system-wide configuration file for all users.
 * Allow to use different configuration files.
```

### Comparing `icepapcms-3.4.1/CONTRIBUTING.md` & `icepapcms-3.4.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/LICENSE.txt` & `icepapcms-3.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/PKG-INFO` & `icepapcms-3.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: icepapcms
-Version: 3.4.1
+Version: 3.4.2
 Summary: Icepap Configuration Management System and Test Tool
 Home-page: https://github.com/ALBA-Synchrotron/IcepapCMS
 Author: Guifre Cuni et al.
 Author-email: ctbeamlines@cells.es
 License: GPLv3
 Description: 
         IcepapCMS is a graphical configuration and test tool for the Icepap motor
```

### Comparing `icepapcms-3.4.1/README.md` & `icepapcms-3.4.2/README.md`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/__main__.py` & `icepapcms-3.4.2/icepapcms/__main__.py`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/db/creates-mysql.sql` & `icepapcms-3.4.2/icepapcms/db/creates-mysql.sql`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/db/creates_sqlite.sql` & `icepapcms-3.4.2/icepapcms/db/creates_sqlite.sql`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/db/dbmodel.mwb` & `icepapcms-3.4.2/icepapcms/db/dbmodel.mwb`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/doc/IcePAP_HardwareManual.pdf` & `icepapcms-3.4.2/icepapcms/doc/IcePAP_HardwareManual.pdf`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/doc/IcePAP_UserManual-1.0b-150526-fw3.11+.pdf` & `icepapcms-3.4.2/icepapcms/doc/IcePAP_UserManual-1.0b-150526-fw3.11+.pdf`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/doc/IcePAP_UserManual.pdf` & `icepapcms-3.4.2/icepapcms/doc/IcePAP_UserManual.pdf`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/doc/IcePAP_UserManual_last.pdf` & `icepapcms-3.4.2/icepapcms/doc/IcePAP_UserManual_last.pdf`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/doc/IcePAP_UserManual_working.pdf` & `icepapcms-3.4.2/icepapcms/doc/IcePAP_UserManual_working.pdf`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/doc/IcepapCMSUserManual.pdf` & `icepapcms-3.4.2/icepapcms/doc/IcepapCMSUserManual.pdf`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/doc/Icepapicon.png` & `icepapcms-3.4.2/icepapcms/doc/Icepapicon.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/doc/remoteserver_setup.txt` & `icepapcms-3.4.2/icepapcms/doc/remoteserver_setup.txt`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/Led/Led.py` & `icepapcms-3.4.2/icepapcms/gui/Led/Led.py`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/Led/images24/ledblue.png` & `icepapcms-3.4.2/icepapcms/gui/Led/images24/ledblue.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/Led/images24/ledblueoff.png` & `icepapcms-3.4.2/icepapcms/gui/Led/images24/ledblueoff.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/Led/images24/ledgreen.png` & `icepapcms-3.4.2/icepapcms/gui/Led/images24/ledgreen.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/Led/images24/ledgreenoff.png` & `icepapcms-3.4.2/icepapcms/gui/Led/images24/ledgreenoff.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/Led/images24/ledorange.png` & `icepapcms-3.4.2/icepapcms/gui/Led/images24/ledorange.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/Led/images24/ledorangeoff.png` & `icepapcms-3.4.2/icepapcms/gui/Led/images24/ledorangeoff.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/Led/images24/ledred.png` & `icepapcms-3.4.2/icepapcms/gui/Led/images24/ledred.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/Led/images24/ledredoff.png` & `icepapcms-3.4.2/icepapcms/gui/Led/images24/ledredoff.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/Led/images24/ledyellow.png` & `icepapcms-3.4.2/icepapcms/gui/Led/images24/ledyellow.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/Led/images24/ledyellowoff.png` & `icepapcms-3.4.2/icepapcms/gui/Led/images24/ledyellowoff.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/Led/images48/ledblue.png` & `icepapcms-3.4.2/icepapcms/gui/Led/images48/ledblue.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/Led/images48/ledblueoff.png` & `icepapcms-3.4.2/icepapcms/gui/Led/images48/ledblueoff.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/Led/images48/ledgreen.png` & `icepapcms-3.4.2/icepapcms/gui/Led/images48/ledgreen.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/Led/images48/ledgreenoff.png` & `icepapcms-3.4.2/icepapcms/gui/Led/images48/ledgreenoff.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/Led/images48/ledorange.png` & `icepapcms-3.4.2/icepapcms/gui/Led/images48/ledorange.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/Led/images48/ledorangeoff.png` & `icepapcms-3.4.2/icepapcms/gui/Led/images48/ledorangeoff.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/Led/images48/ledred.png` & `icepapcms-3.4.2/icepapcms/gui/Led/images48/ledred.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/Led/images48/ledredoff.png` & `icepapcms-3.4.2/icepapcms/gui/Led/images48/ledredoff.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/Led/images48/ledyellow.png` & `icepapcms-3.4.2/icepapcms/gui/Led/images48/ledyellow.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/Led/images48/ledyellowoff.png` & `icepapcms-3.4.2/icepapcms/gui/Led/images48/ledyellowoff.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/dialogaddicepap.py` & `icepapcms-3.4.2/icepapcms/gui/dialogaddicepap.py`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/dialogaddlocation.py` & `icepapcms-3.4.2/icepapcms/gui/dialogaddlocation.py`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/dialogconflictdriver_expert.py` & `icepapcms-3.4.2/icepapcms/gui/dialogconflictdriver_expert.py`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/dialogconflictdriver_nonexpert.py` & `icepapcms-3.4.2/icepapcms/gui/dialogconflictdriver_nonexpert.py`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/dialogdriverconflict.py` & `icepapcms-3.4.2/icepapcms/gui/dialogdriverconflict.py`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/dialoghomesrch.py` & `icepapcms-3.4.2/icepapcms/gui/dialoghomesrch.py`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/dialogipapprogram.py` & `icepapcms-3.4.2/icepapcms/gui/dialogipapprogram.py`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/dialognewdriver.py` & `icepapcms-3.4.2/icepapcms/gui/dialognewdriver.py`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/dialogpreferences.py` & `icepapcms-3.4.2/icepapcms/gui/dialogpreferences.py`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/dialogsnapshot.py` & `icepapcms-3.4.2/icepapcms/gui/dialogsnapshot.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,17 +11,16 @@
 # -----------------------------------------------------------------------------
 
 
 from PyQt5 import QtWidgets, uic
 from pkg_resources import resource_filename
 import os
 import time
-import logging
 import threading
-from ..lib.sanpshot import IcepapSnapshot
+from ..lib.snapshot import IcepapSnapshot
 from ..lib.configmanager import ConfigManager
 from .messagedialogs import MessageDialogs
 
 
 class DialogSnapshot(QtWidgets.QDialog):
 
     def __init__(self, parent, host='', port=5000):
@@ -38,31 +37,36 @@
         self.set_filename()
 
         self.ui.browser.clicked.connect(self.set_filename)
         self.ui.take_snapshot.clicked.connect(self.take_snapshot_clicked)
 
     def set_filename(self):
         if self.ui.filename.text() == '':
-            name = 'snapshot_{}.yaml'.format(time.strftime('%Y%m%d_%H%M%S'))
+            host = self.ui.host.text()
+            str_time = time.strftime('%Y%m%d_%H%M%S')
+            if host:
+                name = '{}_snapshot_{}.yaml'.format(host, str_time)
+            else:
+                name = 'snapshot_{}.yaml'.format(str_time)
             snapshots_folder = \
                 self._config.config[self._config.icepap]['snapshots_folder']
             directory = os.path.join(snapshots_folder, name)
         else:
             directory = self.ui.filename.text()
         fn = QtWidgets.QFileDialog.getSaveFileName(
             self, "Take Snapshot",
             directory=directory,
             filter='*.yaml')[0]
         self.ui.filename.setText(fn)
 
     def update_progress_bar(self, ipap_snapshot):
         while ipap_snapshot.done != 100:
-            self.ui.progress_bar.setValue(ipap_snapshot.done)
+            self.ui.progress_bar.setValue(int(ipap_snapshot.done))
             time.sleep(1)
-        self.ui.progress_bar.setValue(ipap_snapshot.done)
+        self.ui.progress_bar.setValue(int(ipap_snapshot.done))
 
     def take_snapshot_clicked(self):
         try:
             host = self.ui.host.text()
             if host == '':
                 MessageDialogs.showErrorMessage(
                     self, 'Error', 'You should introduce a valid host')
@@ -83,16 +87,21 @@
                                                 str(e))
                 return
             thread = threading.Thread(target=self.update_progress_bar,
                                       args=[ipap_snapshot])
 
             self.ui.take_snapshot.setEnabled(False)
             thread.start()
-            ipap_snapshot.create_snapshot(filename)
+            axes_errors = ipap_snapshot.create_snapshot(filename)
             thread.join()
+            if axes_errors:
+               MessageDialogs.showErrorMessage(
+                    self, 'Error on reading values',
+                          'Check AxesError list on the file. Axes: {'
+                          '}'.format(axes_errors))
         finally:
             self.ui.take_snapshot.setEnabled(True)
 
 
 def main():
     import sys
     app = QtWidgets.QApplication(sys.argv)
```

### Comparing `icepapcms-3.4.1/icepapcms/gui/dialogstatusinfo.py` & `icepapcms-3.4.2/icepapcms/gui/dialogstatusinfo.py`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/historiccfgwidget.py` & `icepapcms-3.4.2/icepapcms/gui/historiccfgwidget.py`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/icepap_treemodel.py` & `icepapcms-3.4.2/icepapcms/gui/icepap_treemodel.py`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/icepapcms.py` & `icepapcms-3.4.2/icepapcms/gui/icepapcms.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 from .ipapconsole import IcepapConsole
 from .messagedialogs import MessageDialogs
 from .templatescatalogwidget import TemplatesCatalogWidget
 from ..helpers import loggingInfo
 from ..gui.ldap.login import DialogLdapLogin
 from icepap import IcePAPController
 
-__version__ = '3.4.1'
+__version__ = '3.4.2'
 
 
 class IcepapApp(QtWidgets.QApplication):
     log = logging.getLogger('{}.IcepapApp'.format(__name__))
 
     def __init__(self,parent=None):
         QtWidgets.QApplication.__init__(self, [])
```

### Comparing `icepapcms-3.4.1/icepapcms/gui/icepapdriverwidget.py` & `icepapcms-3.4.2/icepapcms/gui/icepapdriverwidget.py`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ipapconsole.py` & `icepapcms-3.4.2/icepapcms/gui/ipapconsole.py`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ldap/login.py` & `icepapcms-3.4.2/icepapcms/gui/ldap/login.py`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ldap/ui/login.ui` & `icepapcms-3.4.2/icepapcms/gui/ldap/ui/login.ui`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ldap/ui/login_rc.py` & `icepapcms-3.4.2/icepapcms/gui/ldap/ui/login_rc.py`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ldap/ui/password.png` & `icepapcms-3.4.2/icepapcms/gui/ldap/ui/password.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/messagedialogs.py` & `icepapcms-3.4.2/icepapcms/gui/messagedialogs.py`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/pageipapcrate.py` & `icepapcms-3.4.2/icepapcms/gui/pageipapcrate.py`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/pageipapdriver.py` & `icepapcms-3.4.2/icepapcms/gui/pageipapdriver.py`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/pageipapsystem.py` & `icepapcms-3.4.2/icepapcms/gui/pageipapsystem.py`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/pyconsoletext.py` & `icepapcms-3.4.2/icepapcms/gui/pyconsoletext.py`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/qvalidatelineedit.py` & `icepapcms-3.4.2/icepapcms/gui/qvalidatelineedit.py`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/templatescatalogwidget.py` & `icepapcms-3.4.2/icepapcms/gui/templatescatalogwidget.py`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/axis.ui` & `icepapcms-3.4.2/icepapcms/gui/ui/axis.ui`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/closedloop.ui` & `icepapcms-3.4.2/icepapcms/gui/ui/closedloop.ui`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/dialogaddicepap.ui` & `icepapcms-3.4.2/icepapcms/gui/ui/dialogaddicepap.ui`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/dialogaddlocation.ui` & `icepapcms-3.4.2/icepapcms/gui/ui/dialogaddlocation.ui`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/dialogconflictdriver_expert.ui` & `icepapcms-3.4.2/icepapcms/gui/ui/dialogconflictdriver_expert.ui`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/dialogconflictdriver_nonexpert.ui` & `icepapcms-3.4.2/icepapcms/gui/ui/dialogconflictdriver_nonexpert.ui`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/dialogdriverconflict.ui` & `icepapcms-3.4.2/icepapcms/gui/ui/dialogdriverconflict.ui`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/dialoghistoriccfg.ui` & `icepapcms-3.4.2/icepapcms/gui/ui/dialoghistoriccfg.ui`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/dialoghomesrch.ui` & `icepapcms-3.4.2/icepapcms/gui/ui/dialoghomesrch.ui`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/dialogipapprogram.ui` & `icepapcms-3.4.2/icepapcms/gui/ui/dialogipapprogram.ui`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/dialognewdriver.ui` & `icepapcms-3.4.2/icepapcms/gui/ui/dialognewdriver.ui`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/dialogpreferences.ui` & `icepapcms-3.4.2/icepapcms/gui/ui/dialogpreferences.ui`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/dialogstatusinfo.ui` & `icepapcms-3.4.2/icepapcms/gui/ui/dialogstatusinfo.ui`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/dialogsystemscan.ui` & `icepapcms-3.4.2/icepapcms/gui/ui/dialogsystemscan.ui`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/encoders.ui` & `icepapcms-3.4.2/icepapcms/gui/ui/encoders.ui`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/historiccfgwidget.ui` & `icepapcms-3.4.2/icepapcms/gui/ui/historiccfgwidget.ui`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/homing.ui` & `icepapcms-3.4.2/icepapcms/gui/ui/homing.ui`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icepapcms.qrc` & `icepapcms-3.4.2/icepapcms/gui/ui/icepapcms.qrc`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icepapcms.ui` & `icepapcms-3.4.2/icepapcms/gui/ui/icepapcms.ui`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icepapcms_rc.py` & `icepapcms-3.4.2/icepapcms/gui/ui/icepapcms_rc.py`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icepapdriverwidget.ui` & `icepapcms-3.4.2/icepapcms/gui/ui/icepapdriverwidget.ui`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icepapdriverwidgetsmall.ui` & `icepapcms-3.4.2/icepapcms/gui/ui/icepapdriverwidgetsmall.ui`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/Icepap.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/Icepap.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/IcepapBig.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/IcepapBig.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/IcepapMed.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/IcepapMed.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/Icepapdriverpetit.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/Icepapdriverpetit.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/Icepapicon.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/Icepapicon.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/approved.gif` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/approved.gif`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/axis.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/axis.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/backup.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/backup.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/calendar.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/calendar.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/camera.svg` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/camera.svg`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/close.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/close.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/connect.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/connect.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/database.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/database.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/disconnect.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/disconnect.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/emblem-keys.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/emblem-keys.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/emblem-people.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/emblem-people.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/emblem-question.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/emblem-question.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/encoder.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/encoder.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/export.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/export.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/file-roller.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/file-roller.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/folder-remote.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/folder-remote.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/folder.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/folder.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/gconf-editor.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/gconf-editor.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/gnome-cpu.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/gnome-cpu.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/gnome-dev-floppy.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/gnome-dev-floppy.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/gnome-dev-harddisk.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/gnome-dev-harddisk.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/gnome-dev-network.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/gnome-dev-network.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/gnome-logout.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/gnome-logout.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/gnome-monitor.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/gnome-monitor.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/gnome-nettool.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/gnome-nettool.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/gnome-session-halt.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/gnome-session-halt.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/gnome-settings.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/gnome-settings.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/gnome-terminal.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/gnome-terminal.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/gnome-workspace.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/gnome-workspace.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/go-next.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/go-next.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/go-previous.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/go-previous.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/go-up.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/go-up.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/help-browser.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/help-browser.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/import.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/import.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/ipapcrate.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/ipapcrate.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/ipapdriver.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/ipapdriver.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/ipapdrivercfg.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/ipapdrivercfg.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/ipapdrivererror.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/ipapdrivererror.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/ipapdrivermodified.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/ipapdrivermodified.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/ipapdrivermoved.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/ipapdrivermoved.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/ipapdrivernew.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/ipapdrivernew.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/ipapdriverwarning.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/ipapdriverwarning.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/ipapsys.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/ipapsys.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/ipapsyserror.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/ipapsyserror.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/ipapsysoffline.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/ipapsysoffline.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/ipapsyswarning.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/ipapsyswarning.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/keys.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/keys.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/ldap_icon.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/ldap_icon.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/list-add.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/list-add.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/list-remove.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/list-remove.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/mysql.gif` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/mysql.gif`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/network-server.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/network-server.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/notes.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/notes.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/oscilloscope.svg` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/oscilloscope.svg`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/package-x-generic.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/package-x-generic.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/postgresql.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/postgresql.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/preferences-system.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/preferences-system.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/quit.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/quit.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/sign.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/sign.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/sqlite.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/sqlite.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/system-users.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/system-users.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/update-manager.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/update-manager.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/icons/view-refresh.png` & `icepapcms-3.4.2/icepapcms/gui/ui/icons/view-refresh.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/io.ui` & `icepapcms-3.4.2/icepapcms/gui/ui/io.ui`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/ipapconsole.ui` & `icepapcms-3.4.2/icepapcms/gui/ui/ipapconsole.ui`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/ipaptestpage.ui` & `icepapcms-3.4.2/icepapcms/gui/ui/ipaptestpage.ui`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/motor.ui` & `icepapcms-3.4.2/icepapcms/gui/ui/motor.ui`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/pageipapdriver.ui` & `icepapcms-3.4.2/icepapcms/gui/ui/pageipapdriver.ui`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/small_icons/go-absolute.png` & `icepapcms-3.4.2/icepapcms/gui/ui/small_icons/go-absolute.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/small_icons/go-relative.png` & `icepapcms-3.4.2/icepapcms/gui/ui/small_icons/go-relative.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/small_icons/go-relative2.png` & `icepapcms-3.4.2/icepapcms/gui/ui/small_icons/go-relative2.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/small_icons/historic.png` & `icepapcms-3.4.2/icepapcms/gui/ui/small_icons/historic.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/small_icons/process-stop.png` & `icepapcms-3.4.2/icepapcms/gui/ui/small_icons/process-stop.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/small_icons/save.png` & `icepapcms-3.4.2/icepapcms/gui/ui/small_icons/save.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/small_icons/template.png` & `icepapcms-3.4.2/icepapcms/gui/ui/small_icons/template.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/small_icons/undo.png` & `icepapcms-3.4.2/icepapcms/gui/ui/small_icons/undo.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/small_icons/view-refresh.png` & `icepapcms-3.4.2/icepapcms/gui/ui/small_icons/view-refresh.png`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/gui/ui/snapshot.ui` & `icepapcms-3.4.2/icepapcms/gui/ui/snapshot.ui`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/helpers.py` & `icepapcms-3.4.2/icepapcms/helpers.py`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/lib/configmanager.py` & `icepapcms-3.4.2/icepapcms/lib/configmanager.py`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/lib/conflict.py` & `icepapcms-3.4.2/icepapcms/lib/conflict.py`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/lib/icepapdriver.py` & `icepapcms-3.4.2/icepapcms/lib/icepapdriver.py`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/lib/icepapdrivercfg.py` & `icepapcms-3.4.2/icepapcms/lib/icepapdrivercfg.py`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/lib/icepapsmanager.py` & `icepapcms-3.4.2/icepapcms/lib/icepapsmanager.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,25 @@
             axis_name = 'NON-ASCII_NAME'
             driver_cfg.setParameter("IPAPNAME", axis_name)
 
         # INSTEAD OF READING PARAM BY PARAM, WE SHOULD ASK THE ICEPAP FOR
         # ALL THE CONFIGURATION
         # WITH THE #N?:CFG COMMAND, USING SOME .getCfg() METHOD.
         axis = self.iPaps[icepap_name][driver_addr]
-        cfg = axis.get_cfg()
+
+        # TODO: Investigate how to mark the driver with error
+        try:
+            cfg = axis.get_cfg()
+        except Exception as e:
+            cfg = {}
+            msg = 'Can not read axis {} configuration: {}'.format(axis.axis, e)
+            self.log.error(msg)
+            MessageDialogs.showErrorMessage(None, 'Get Driver Configuration',
+                                            msg)
+
         for param_name, param_value in list(cfg.items()):
             driver_cfg.setParameter(str(param_name), param_value)
 
         return driver_cfg
 
     @loggingInfo
     def setDriverConfiguration(self, icepap_name, driver_addr, new_values,
```

### Comparing `icepapcms-3.4.1/icepapcms/lib/icepapsystem.py` & `icepapcms-3.4.2/icepapcms/lib/icepapsystem.py`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/lib/mainmanager.py` & `icepapcms-3.4.2/icepapcms/lib/mainmanager.py`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/lib/sanpshot.py` & `icepapcms-3.4.2/icepapcms/lib/snapshot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import yaml
 from icepap import IcePAPController
 import logging
 import time
 
+ERROR_VALUE = 'ERROR'
+
 
 class IcepapSnapshot:
     """
     Class to create/restore IcePAP backups based on Ethernet communication.
     """
 
     def __init__(self, host='', port=5000, timeout=3):
@@ -19,59 +21,72 @@
         self.done = 0
 
     def create_snapshot(self, filename):
         factor = 100 / (len(self._ipap.axes) + 2)
         _done = 0
         self.snapshot['Date'] = time.strftime('%Y/%m/%d %H:%M:%S +%z')
         self.snapshot['System'] = system = {}
+        self.snapshot['AxesErrors'] = axes_errors = []
         self.snapshot['Axes'] = axes = {}
         system['HOST'] = self._host
         system['PORT'] = self._port
         system['VER'] = self._ipap.ver['SYSTEM']['VER'][0]
         _done += 1
         self.done = _done * factor
+
         for axis in self._ipap.axes:
             axis_snapshot = AxisSnapshot(self._ipap[axis])
-            axis_snapshot.create_snapshot()
+            error = axis_snapshot.create_snapshot()
+            if error:
+                axes_errors.append(axis)
             axes[axis] = axis_snapshot.snapshot
             _done += 1
             self.done = _done * factor
         self._save(filename)
         self.done = 100
-
+        return axes_errors
     def _save(self, filename):
         with open(filename, 'w') as f:
             yaml.safe_dump(self.snapshot, f)
 
 
 class AxisSnapshot:
 
     def __init__(self, axis):
         self.axis = axis
         self.snapshot = {}
+        log_name = '{}.AxisSnapshot_({})'.format(__name__, axis)
+        self.log = logging.getLogger(log_name)
 
     def create_snapshot(self):
         drv_ver = self.axis.fver
         self.snapshot['VER'] = drv_ver
-
-
-        # Get Configuration
-        self.snapshot['Configuration'] = dict(self.axis.get_cfg())
+        flag_error = False
+        for i in range(3):
+            try:
+                # Get Configuration
+                value = dict(self.axis.get_cfg())
+                break
+            except Exception as e:
+                self.log.error('Error on reading configuration: {}'
+                               ''.format(e))
+                value = ERROR_VALUE
+
+        self.snapshot['Configuration'] = value
+        if value == ERROR_VALUE:
+            flag_error = True
 
         # Get Operation:
         self.snapshot['Operation'] = oper = {}
 
-        # Attributes can fail on reading, but we save it anyway with None
-        # value
+        # Basic operation attributes
         attrs = ['velocity', 'name', 'acctime', 'pcloop', 'indexer', 'infoa',
-                 'infob', 'infoc', 'pos', 'pos_measure', 'pos_shftenc',
-                 'pos_tgtenc', 'pos_ctrlenc', 'pos_encin', 'pos_inpos',
-                 'pos_absenc', 'pos_motor', 'pos_sync', 'enc', 'enc_measure',
-                 'enc_shftenc', 'enc_tgtenc', 'enc_ctrlenc', 'enc_encin',
-                 'enc_inpos', 'enc_absenc', 'enc_motor', 'enc_sync', 'id']
+                 'infob', 'infoc', 'pos', 'enc', 'pos_encin', 'enc_encin',
+                 'pos_inpos', 'enc_inpos', 'pos_absenc', 'enc_absenc',
+                 'pos_motor', 'enc_motor', 'pos_sync', 'enc_sync', 'id']
 
         # Attributes can fail on reading because they are on version 3.17
         # This attributes won on the backup file if the version is < 3
         v3_attrs = ['cswitch', 'velocity_min', 'velocity_max', 'ecam',
                     'outpos', 'outpaux', 'syncpos', 'syncaux']
 
         attrs += v3_attrs
@@ -81,25 +96,29 @@
             if attr in v3_attrs and drv_ver < 3:
                 continue
             for i in range(3):
                 try:
                     value = self.axis.__getattribute__(attr)
                     break
                 except Exception:
-                    value = None
+                    value = ERROR_VALUE
             oper[attr] = value
+            if value == ERROR_VALUE:
+                flag_error = True
 
         # External Disable. Valid for FW < 3
         if drv_ver < 3:
             try:
                 value = eval(self.axis.send_cmd('?DISDIS')[0])
             except Exception:
-                value = None
+                value = ERROR_VALUE
             oper['DISDIS'] = value
-
+            if value == ERROR_VALUE:
+                flag_error = True
+        return flag_error
 
     # def do_check(self, axes=[]):
     #     self._cfg_bkp.pop('GENERAL')
     #     sections = self._cfg_bkp.sections()
     #     sections.pop(sections.index('SYSTEM'))
     #     sections.pop(sections.index('CONTROLLER'))
     #     for axis in axes:
```

### Comparing `icepapcms-3.4.1/icepapcms/lib/singleton.py` & `icepapcms-3.4.2/icepapcms/lib/singleton.py`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/lib/stormmanager.py` & `icepapcms-3.4.2/icepapcms/lib/stormmanager.py`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/lib/stormmysql.py` & `icepapcms-3.4.2/icepapcms/lib/stormmysql.py`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/templates/catalog.xml` & `icepapcms-3.4.2/icepapcms/templates/catalog.xml`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms/templates/driverparameters.xml` & `icepapcms-3.4.2/icepapcms/templates/driverparameters.xml`

 * *Files identical despite different names*

### Comparing `icepapcms-3.4.1/icepapcms.egg-info/PKG-INFO` & `icepapcms-3.4.2/icepapcms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: icepapcms
-Version: 3.4.1
+Version: 3.4.2
 Summary: Icepap Configuration Management System and Test Tool
 Home-page: https://github.com/ALBA-Synchrotron/IcepapCMS
 Author: Guifre Cuni et al.
 Author-email: ctbeamlines@cells.es
 License: GPLv3
 Description: 
         IcepapCMS is a graphical configuration and test tool for the Icepap motor
```

### Comparing `icepapcms-3.4.1/icepapcms.egg-info/SOURCES.txt` & `icepapcms-3.4.2/icepapcms.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -199,14 +199,14 @@
 icepapcms/lib/configmanager.py
 icepapcms/lib/conflict.py
 icepapcms/lib/icepapdriver.py
 icepapcms/lib/icepapdrivercfg.py
 icepapcms/lib/icepapsmanager.py
 icepapcms/lib/icepapsystem.py
 icepapcms/lib/mainmanager.py
-icepapcms/lib/sanpshot.py
 icepapcms/lib/singleton.py
+icepapcms/lib/snapshot.py
 icepapcms/lib/stormmanager.py
 icepapcms/lib/stormmysql.py
 icepapcms/templates/__init__.py
 icepapcms/templates/catalog.xml
 icepapcms/templates/driverparameters.xml
```

### Comparing `icepapcms-3.4.1/setup.py` & `icepapcms-3.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 data base configuration. 
 
 The program includes one graphical console to communicate with raw commands.  
 """
 
 # The version is updated automatically with bumpversion
 # Do not update manually
-__version = '3.4.1'
+__version = '3.4.2'
 
 
 # Setup
 setup(
     name="icepapcms",
     version=__version,
     packages=find_packages(),
```

