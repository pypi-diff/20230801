# Comparing `tmp/abinitostudio-1.0.0.tar.gz` & `tmp/abinitostudio-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\abinitostudio-1.0.0.tar", last modified: Mon Jul 31 14:21:58 2023, max compression
+gzip compressed data, was "dist\abinitostudio-1.0.1.tar", last modified: Tue Aug  1 14:48:28 2023, max compression
```

## Comparing `abinitostudio-1.0.0.tar` & `abinitostudio-1.0.1.tar`

### file list

```diff
@@ -1,88 +1,89 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 14:21:58.000000 abinitostudio-1.0.0/
--rw-rw-rw-   0        0        0       96 2021-08-03 14:08:19.000000 abinitostudio-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0      383 2023-07-31 14:21:58.000000 abinitostudio-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1134 2021-08-06 03:05:42.000000 abinitostudio-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 14:21:57.000000 abinitostudio-1.0.0/abinitostudio/
--rw-rw-rw-   0        0        0        0 2020-01-08 01:57:09.000000 abinitostudio-1.0.0/abinitostudio/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 14:21:57.000000 abinitostudio-1.0.0/abinitostudio/calculation/
--rw-rw-rw-   0        0        0        0 2020-01-08 01:57:09.000000 abinitostudio-1.0.0/abinitostudio/calculation/__init__.py
--rw-rw-rw-   0        0        0    25840 2021-08-02 00:55:16.000000 abinitostudio-1.0.0/abinitostudio/calculation/vasp_calculation.py
-drwxrwxrwx   0        0        0        0 2023-07-31 14:21:57.000000 abinitostudio-1.0.0/abinitostudio/io/
--rw-rw-rw-   0        0        0        0 2020-01-08 01:57:09.000000 abinitostudio-1.0.0/abinitostudio/io/__init__.py
--rw-rw-rw-   0        0        0    20951 2023-07-26 23:35:53.000000 abinitostudio-1.0.0/abinitostudio/io/vasp_io.py
--rw-rw-rw-   0        0        0    59876 2023-07-26 23:10:00.000000 abinitostudio-1.0.0/abinitostudio/myMainWindow.py
-drwxrwxrwx   0        0        0        0 2023-07-31 14:21:57.000000 abinitostudio-1.0.0/abinitostudio/plot/
--rw-rw-rw-   0        0        0        0 2020-01-08 01:57:09.000000 abinitostudio-1.0.0/abinitostudio/plot/__init__.py
--rw-rw-rw-   0        0        0      679 2021-08-05 03:39:45.000000 abinitostudio-1.0.0/abinitostudio/plot/plot_field.py
--rw-rw-rw-   0        0        0     2330 2023-07-27 00:58:33.000000 abinitostudio-1.0.0/abinitostudio/plot/plot_vasp.py
-drwxrwxrwx   0        0        0        0 2023-07-31 14:21:57.000000 abinitostudio-1.0.0/abinitostudio/structure/
--rw-rw-rw-   0        0        0        0 2020-01-08 01:57:09.000000 abinitostudio-1.0.0/abinitostudio/structure/__init__.py
--rw-rw-rw-   0        0        0    35274 2023-07-26 23:37:48.000000 abinitostudio-1.0.0/abinitostudio/structure/plot_structure.py
--rw-rw-rw-   0        0        0     3343 2021-08-02 00:55:55.000000 abinitostudio-1.0.0/abinitostudio/structure/tabdialog.py
-drwxrwxrwx   0        0        0        0 2023-07-31 14:21:57.000000 abinitostudio-1.0.0/abinitostudio/ui/
--rw-rw-rw-   0        0        0    17334 2021-08-02 07:37:44.000000 abinitostudio-1.0.0/abinitostudio/ui/Dialog_DOS.py
--rw-rw-rw-   0        0        0    38630 2021-08-02 08:21:52.000000 abinitostudio-1.0.0/abinitostudio/ui/Dialog_PB.py
--rw-rw-rw-   0        0        0     7633 2021-07-13 07:37:22.000000 abinitostudio-1.0.0/abinitostudio/ui/Dialog_band.py
--rw-rw-rw-   0        0        0    13745 2023-07-26 22:49:46.000000 abinitostudio-1.0.0/abinitostudio/ui/UI.py
--rw-rw-rw-   0        0        0    12159 2021-08-02 08:18:40.000000 abinitostudio-1.0.0/abinitostudio/ui/UI_setting.py
--rw-rw-rw-   0        0        0     8922 2021-08-02 08:20:50.000000 abinitostudio-1.0.0/abinitostudio/ui/UI_test.py
--rw-rw-rw-   0        0        0    31919 2021-08-02 08:20:32.000000 abinitostudio-1.0.0/abinitostudio/ui/UI_vasp_DOS.py
--rw-rw-rw-   0        0        0    32252 2021-08-02 08:20:44.000000 abinitostudio-1.0.0/abinitostudio/ui/UI_vasp_band.py
--rw-rw-rw-   0        0        0    31944 2021-08-02 08:20:38.000000 abinitostudio-1.0.0/abinitostudio/ui/UI_vasp_band_noncal.py
--rw-rw-rw-   0        0        0    25099 2021-08-02 08:20:25.000000 abinitostudio-1.0.0/abinitostudio/ui/UI_vasp_phonon.py
--rw-rw-rw-   0        0        0    22764 2021-08-02 08:20:19.000000 abinitostudio-1.0.0/abinitostudio/ui/UI_vasp_scf.py
--rw-rw-rw-   0        0        0    22785 2021-08-02 08:20:11.000000 abinitostudio-1.0.0/abinitostudio/ui/UI_vasp_scf_noncal.py
--rw-rw-rw-   0        0        0     4585 2021-08-02 08:20:03.000000 abinitostudio-1.0.0/abinitostudio/ui/UI_vasp_supercell.py
--rw-rw-rw-   0        0        0    21153 2021-08-02 08:19:54.000000 abinitostudio-1.0.0/abinitostudio/ui/UI_vasp_wannier.py
--rw-rw-rw-   0        0        0        0 2020-01-08 01:57:09.000000 abinitostudio-1.0.0/abinitostudio/ui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 14:21:57.000000 abinitostudio-1.0.0/abinitostudio.egg-info/
--rw-rw-rw-   0        0        0      383 2023-07-31 14:21:56.000000 abinitostudio-1.0.0/abinitostudio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1835 2023-07-31 14:21:57.000000 abinitostudio-1.0.0/abinitostudio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 14:21:56.000000 abinitostudio-1.0.0/abinitostudio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      205 2023-07-31 14:21:56.000000 abinitostudio-1.0.0/abinitostudio.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2023-07-31 14:21:56.000000 abinitostudio-1.0.0/abinitostudio.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      881 2021-08-02 08:06:44.000000 abinitostudio-1.0.0/appMain.py
-drwxrwxrwx   0        0        0        0 2023-07-31 14:21:58.000000 abinitostudio-1.0.0/doc/
--rw-rw-rw-   0        0        0   325819 2021-07-30 12:49:48.000000 abinitostudio-1.0.0/doc/启动图片.pptx
--rw-rw-rw-   0        0        0    10870 2023-07-25 03:39:28.000000 abinitostudio-1.0.0/doc/程序bug.docx
--rw-rw-rw-   0        0        0   553988 2021-07-30 08:12:44.000000 abinitostudio-1.0.0/doc/说明文档.docx
--rw-rw-rw-   0        0        0   756022 2021-07-30 07:37:10.000000 abinitostudio-1.0.0/doc/说明文档.pdf
-drwxrwxrwx   0        0        0        0 2023-07-31 14:21:58.000000 abinitostudio-1.0.0/examples/
--rw-rw-rw-   0        0        0 12582333 2021-08-01 03:29:39.000000 abinitostudio-1.0.0/examples/CHGCAR
--rw-rw-rw-   0        0        0   300593 2020-07-30 07:58:04.000000 abinitostudio-1.0.0/examples/DOSCAR
--rw-rw-rw-   0        0        0   132487 2019-11-19 12:21:46.000000 abinitostudio-1.0.0/examples/EIGENVAL_CdCl
--rw-rw-rw-   0        0        0     1321 2023-04-21 12:57:23.000000 abinitostudio-1.0.0/examples/POSCAR
--rw-rw-rw-   0        0        0  2888368 2019-11-19 12:21:46.000000 abinitostudio-1.0.0/examples/PROCAR _CdCl
--rw-rw-rw-   0        0        0      291 2021-08-01 03:08:04.000000 abinitostudio-1.0.0/examples/text_ip.txt
-drwxrwxrwx   0        0        0        0 2023-07-31 14:21:58.000000 abinitostudio-1.0.0/images/
--rw-rw-rw-   0        0        0     7946 2021-07-08 05:28:12.000000 abinitostudio-1.0.0/images/3d可视.png
--rw-rw-rw-   0        0        0     7103 2021-07-27 09:09:04.000000 abinitostudio-1.0.0/images/DOS.png
--rw-rw-rw-   0        0        0     2541 2021-07-11 06:18:08.000000 abinitostudio-1.0.0/images/band.png
--rw-rw-rw-   0        0        0     3332 2021-07-27 09:08:38.000000 abinitostudio-1.0.0/images/band_noncal.png
--rw-rw-rw-   0        0        0     2218 2021-07-27 09:08:58.000000 abinitostudio-1.0.0/images/phonin.png
--rw-rw-rw-   0        0        0     3762 2021-07-27 09:08:22.000000 abinitostudio-1.0.0/images/scf.png
--rw-rw-rw-   0        0        0     2830 2021-07-27 09:08:28.000000 abinitostudio-1.0.0/images/scf_noncal.png
--rw-rw-rw-   0        0        0    87766 2021-07-30 08:31:34.000000 abinitostudio-1.0.0/images/startup.jpg
--rw-rw-rw-   0        0        0     6280 2021-07-10 11:22:50.000000 abinitostudio-1.0.0/images/vasp.png
--rw-rw-rw-   0        0        0     2468 2021-07-27 09:09:24.000000 abinitostudio-1.0.0/images/wannier.png
--rw-rw-rw-   0        0        0     5090 2021-06-28 05:59:22.000000 abinitostudio-1.0.0/images/关于.png
--rw-rw-rw-   0        0        0     7333 2021-06-28 05:43:40.000000 abinitostudio-1.0.0/images/关闭.png
--rw-rw-rw-   0        0        0     3636 2021-07-08 07:06:54.000000 abinitostudio-1.0.0/images/层级.png
--rw-rw-rw-   0        0        0     2981 2021-06-28 07:05:38.000000 abinitostudio-1.0.0/images/态密度.png
--rw-rw-rw-   0        0        0     5788 2021-07-08 06:57:38.000000 abinitostudio-1.0.0/images/扩胞.png
--rw-rw-rw-   0        0        0     2034 2021-06-28 07:04:50.000000 abinitostudio-1.0.0/images/投影能带.png
--rw-rw-rw-   0        0        0     6657 2021-07-10 04:25:24.000000 abinitostudio-1.0.0/images/测试.png
--rw-rw-rw-   0        0        0     9896 2021-06-28 07:27:34.000000 abinitostudio-1.0.0/images/结构.png
--rw-rw-rw-   0        0        0     2229 2021-06-28 07:04:44.000000 abinitostudio-1.0.0/images/能带.png
--rw-rw-rw-   0        0        0    22484 2021-08-01 09:49:20.000000 abinitostudio-1.0.0/images/能带图.png
--rw-rw-rw-   0        0        0     7906 2021-07-10 04:23:36.000000 abinitostudio-1.0.0/images/设置.png
--rw-rw-rw-   0        0        0     2434 2021-06-28 06:32:52.000000 abinitostudio-1.0.0/images/说明.png
--rw-rw-rw-   0        0        0      308 2021-08-05 05:45:24.000000 abinitostudio-1.0.0/install.py
-drwxrwxrwx   0        0        0        0 2023-07-31 14:21:58.000000 abinitostudio-1.0.0/scripts/
--rw-rw-rw-   0        0        0     8707 2021-08-01 03:49:29.000000 abinitostudio-1.0.0/scripts/cal_vasp_single.py
--rw-rw-rw-   0        0        0       42 2023-07-31 14:21:58.000000 abinitostudio-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1930 2023-07-31 14:21:50.000000 abinitostudio-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 14:21:58.000000 abinitostudio-1.0.0/test/
--rw-rw-rw-   0        0        0     3496 2021-08-06 13:31:27.000000 abinitostudio-1.0.0/test/test_CHGCAR.py
--rw-rw-rw-   0        0        0     1751 2021-08-05 01:56:11.000000 abinitostudio-1.0.0/test/test_multiply_scene.py
--rw-rw-rw-   0        0        0     2556 2021-08-04 04:01:50.000000 abinitostudio-1.0.0/test/test_pick.py
+drwxrwxrwx   0        0        0        0 2023-08-01 14:48:28.000000 abinitostudio-1.0.1/
+-rw-rw-rw-   0        0        0     1084 2023-07-31 13:26:19.000000 abinitostudio-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       96 2021-08-03 14:08:19.000000 abinitostudio-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      383 2023-08-01 14:48:28.000000 abinitostudio-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1134 2021-08-06 03:05:42.000000 abinitostudio-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 14:48:28.000000 abinitostudio-1.0.1/abinitostudio/
+-rw-rw-rw-   0        0        0        0 2020-01-08 01:57:09.000000 abinitostudio-1.0.1/abinitostudio/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 14:48:28.000000 abinitostudio-1.0.1/abinitostudio/calculation/
+-rw-rw-rw-   0        0        0        0 2020-01-08 01:57:09.000000 abinitostudio-1.0.1/abinitostudio/calculation/__init__.py
+-rw-rw-rw-   0        0        0    25840 2021-08-02 00:55:16.000000 abinitostudio-1.0.1/abinitostudio/calculation/vasp_calculation.py
+drwxrwxrwx   0        0        0        0 2023-08-01 14:48:28.000000 abinitostudio-1.0.1/abinitostudio/io/
+-rw-rw-rw-   0        0        0        0 2020-01-08 01:57:09.000000 abinitostudio-1.0.1/abinitostudio/io/__init__.py
+-rw-rw-rw-   0        0        0    20951 2023-07-26 23:35:53.000000 abinitostudio-1.0.1/abinitostudio/io/vasp_io.py
+-rw-rw-rw-   0        0        0    59876 2023-07-26 23:10:00.000000 abinitostudio-1.0.1/abinitostudio/myMainWindow.py
+drwxrwxrwx   0        0        0        0 2023-08-01 14:48:28.000000 abinitostudio-1.0.1/abinitostudio/plot/
+-rw-rw-rw-   0        0        0        0 2020-01-08 01:57:09.000000 abinitostudio-1.0.1/abinitostudio/plot/__init__.py
+-rw-rw-rw-   0        0        0      679 2021-08-05 03:39:45.000000 abinitostudio-1.0.1/abinitostudio/plot/plot_field.py
+-rw-rw-rw-   0        0        0     2330 2023-07-27 00:58:33.000000 abinitostudio-1.0.1/abinitostudio/plot/plot_vasp.py
+drwxrwxrwx   0        0        0        0 2023-08-01 14:48:28.000000 abinitostudio-1.0.1/abinitostudio/structure/
+-rw-rw-rw-   0        0        0        0 2020-01-08 01:57:09.000000 abinitostudio-1.0.1/abinitostudio/structure/__init__.py
+-rw-rw-rw-   0        0        0    35274 2023-07-26 23:37:48.000000 abinitostudio-1.0.1/abinitostudio/structure/plot_structure.py
+-rw-rw-rw-   0        0        0     3343 2021-08-02 00:55:55.000000 abinitostudio-1.0.1/abinitostudio/structure/tabdialog.py
+drwxrwxrwx   0        0        0        0 2023-08-01 14:48:28.000000 abinitostudio-1.0.1/abinitostudio/ui/
+-rw-rw-rw-   0        0        0    17334 2021-08-02 07:37:44.000000 abinitostudio-1.0.1/abinitostudio/ui/Dialog_DOS.py
+-rw-rw-rw-   0        0        0    38630 2021-08-02 08:21:52.000000 abinitostudio-1.0.1/abinitostudio/ui/Dialog_PB.py
+-rw-rw-rw-   0        0        0     7633 2021-07-13 07:37:22.000000 abinitostudio-1.0.1/abinitostudio/ui/Dialog_band.py
+-rw-rw-rw-   0        0        0    13745 2023-07-26 22:49:46.000000 abinitostudio-1.0.1/abinitostudio/ui/UI.py
+-rw-rw-rw-   0        0        0    12159 2021-08-02 08:18:40.000000 abinitostudio-1.0.1/abinitostudio/ui/UI_setting.py
+-rw-rw-rw-   0        0        0     8922 2021-08-02 08:20:50.000000 abinitostudio-1.0.1/abinitostudio/ui/UI_test.py
+-rw-rw-rw-   0        0        0    31919 2021-08-02 08:20:32.000000 abinitostudio-1.0.1/abinitostudio/ui/UI_vasp_DOS.py
+-rw-rw-rw-   0        0        0    32252 2021-08-02 08:20:44.000000 abinitostudio-1.0.1/abinitostudio/ui/UI_vasp_band.py
+-rw-rw-rw-   0        0        0    31944 2021-08-02 08:20:38.000000 abinitostudio-1.0.1/abinitostudio/ui/UI_vasp_band_noncal.py
+-rw-rw-rw-   0        0        0    25099 2021-08-02 08:20:25.000000 abinitostudio-1.0.1/abinitostudio/ui/UI_vasp_phonon.py
+-rw-rw-rw-   0        0        0    22764 2021-08-02 08:20:19.000000 abinitostudio-1.0.1/abinitostudio/ui/UI_vasp_scf.py
+-rw-rw-rw-   0        0        0    22785 2021-08-02 08:20:11.000000 abinitostudio-1.0.1/abinitostudio/ui/UI_vasp_scf_noncal.py
+-rw-rw-rw-   0        0        0     4585 2021-08-02 08:20:03.000000 abinitostudio-1.0.1/abinitostudio/ui/UI_vasp_supercell.py
+-rw-rw-rw-   0        0        0    21153 2021-08-02 08:19:54.000000 abinitostudio-1.0.1/abinitostudio/ui/UI_vasp_wannier.py
+-rw-rw-rw-   0        0        0        0 2020-01-08 01:57:09.000000 abinitostudio-1.0.1/abinitostudio/ui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 14:48:28.000000 abinitostudio-1.0.1/abinitostudio.egg-info/
+-rw-rw-rw-   0        0        0      383 2023-08-01 14:48:28.000000 abinitostudio-1.0.1/abinitostudio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1847 2023-08-01 14:48:28.000000 abinitostudio-1.0.1/abinitostudio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 14:48:28.000000 abinitostudio-1.0.1/abinitostudio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      175 2023-08-01 14:48:28.000000 abinitostudio-1.0.1/abinitostudio.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2023-08-01 14:48:28.000000 abinitostudio-1.0.1/abinitostudio.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      881 2021-08-02 08:06:44.000000 abinitostudio-1.0.1/appMain.py
+drwxrwxrwx   0        0        0        0 2023-08-01 14:48:28.000000 abinitostudio-1.0.1/doc/
+-rw-rw-rw-   0        0        0   325819 2021-07-30 12:49:48.000000 abinitostudio-1.0.1/doc/启动图片.pptx
+-rw-rw-rw-   0        0        0    10870 2023-07-25 03:39:28.000000 abinitostudio-1.0.1/doc/程序bug.docx
+-rw-rw-rw-   0        0        0   553988 2021-07-30 08:12:44.000000 abinitostudio-1.0.1/doc/说明文档.docx
+-rw-rw-rw-   0        0        0   756022 2021-07-30 07:37:10.000000 abinitostudio-1.0.1/doc/说明文档.pdf
+drwxrwxrwx   0        0        0        0 2023-08-01 14:48:28.000000 abinitostudio-1.0.1/examples/
+-rw-rw-rw-   0        0        0 12582333 2021-08-01 03:29:39.000000 abinitostudio-1.0.1/examples/CHGCAR
+-rw-rw-rw-   0        0        0   300593 2020-07-30 07:58:04.000000 abinitostudio-1.0.1/examples/DOSCAR
+-rw-rw-rw-   0        0        0   132487 2019-11-19 12:21:46.000000 abinitostudio-1.0.1/examples/EIGENVAL_CdCl
+-rw-rw-rw-   0        0        0     1321 2023-04-21 12:57:23.000000 abinitostudio-1.0.1/examples/POSCAR
+-rw-rw-rw-   0        0        0  2888368 2019-11-19 12:21:46.000000 abinitostudio-1.0.1/examples/PROCAR _CdCl
+-rw-rw-rw-   0        0        0      291 2021-08-01 03:08:04.000000 abinitostudio-1.0.1/examples/text_ip.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 14:48:28.000000 abinitostudio-1.0.1/images/
+-rw-rw-rw-   0        0        0     7946 2021-07-08 05:28:12.000000 abinitostudio-1.0.1/images/3d可视.png
+-rw-rw-rw-   0        0        0     7103 2021-07-27 09:09:04.000000 abinitostudio-1.0.1/images/DOS.png
+-rw-rw-rw-   0        0        0     2541 2021-07-11 06:18:08.000000 abinitostudio-1.0.1/images/band.png
+-rw-rw-rw-   0        0        0     3332 2021-07-27 09:08:38.000000 abinitostudio-1.0.1/images/band_noncal.png
+-rw-rw-rw-   0        0        0     2218 2021-07-27 09:08:58.000000 abinitostudio-1.0.1/images/phonin.png
+-rw-rw-rw-   0        0        0     3762 2021-07-27 09:08:22.000000 abinitostudio-1.0.1/images/scf.png
+-rw-rw-rw-   0        0        0     2830 2021-07-27 09:08:28.000000 abinitostudio-1.0.1/images/scf_noncal.png
+-rw-rw-rw-   0        0        0    87766 2021-07-30 08:31:34.000000 abinitostudio-1.0.1/images/startup.jpg
+-rw-rw-rw-   0        0        0     6280 2021-07-10 11:22:50.000000 abinitostudio-1.0.1/images/vasp.png
+-rw-rw-rw-   0        0        0     2468 2021-07-27 09:09:24.000000 abinitostudio-1.0.1/images/wannier.png
+-rw-rw-rw-   0        0        0     5090 2021-06-28 05:59:22.000000 abinitostudio-1.0.1/images/关于.png
+-rw-rw-rw-   0        0        0     7333 2021-06-28 05:43:40.000000 abinitostudio-1.0.1/images/关闭.png
+-rw-rw-rw-   0        0        0     3636 2021-07-08 07:06:54.000000 abinitostudio-1.0.1/images/层级.png
+-rw-rw-rw-   0        0        0     2981 2021-06-28 07:05:38.000000 abinitostudio-1.0.1/images/态密度.png
+-rw-rw-rw-   0        0        0     5788 2021-07-08 06:57:38.000000 abinitostudio-1.0.1/images/扩胞.png
+-rw-rw-rw-   0        0        0     2034 2021-06-28 07:04:50.000000 abinitostudio-1.0.1/images/投影能带.png
+-rw-rw-rw-   0        0        0     6657 2021-07-10 04:25:24.000000 abinitostudio-1.0.1/images/测试.png
+-rw-rw-rw-   0        0        0     9896 2021-06-28 07:27:34.000000 abinitostudio-1.0.1/images/结构.png
+-rw-rw-rw-   0        0        0     2229 2021-06-28 07:04:44.000000 abinitostudio-1.0.1/images/能带.png
+-rw-rw-rw-   0        0        0    22484 2021-08-01 09:49:20.000000 abinitostudio-1.0.1/images/能带图.png
+-rw-rw-rw-   0        0        0     7906 2021-07-10 04:23:36.000000 abinitostudio-1.0.1/images/设置.png
+-rw-rw-rw-   0        0        0     2434 2021-06-28 06:32:52.000000 abinitostudio-1.0.1/images/说明.png
+-rw-rw-rw-   0        0        0      308 2021-08-05 05:45:24.000000 abinitostudio-1.0.1/install.py
+drwxrwxrwx   0        0        0        0 2023-08-01 14:48:28.000000 abinitostudio-1.0.1/scripts/
+-rw-rw-rw-   0        0        0     8707 2021-08-01 03:49:29.000000 abinitostudio-1.0.1/scripts/cal_vasp_single.py
+-rw-rw-rw-   0        0        0       42 2023-08-01 14:48:28.000000 abinitostudio-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1890 2023-08-01 14:46:34.000000 abinitostudio-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 14:48:28.000000 abinitostudio-1.0.1/test/
+-rw-rw-rw-   0        0        0     3496 2021-08-06 13:31:27.000000 abinitostudio-1.0.1/test/test_CHGCAR.py
+-rw-rw-rw-   0        0        0     1751 2021-08-05 01:56:11.000000 abinitostudio-1.0.1/test/test_multiply_scene.py
+-rw-rw-rw-   0        0        0     2556 2021-08-04 04:01:50.000000 abinitostudio-1.0.1/test/test_pick.py
```

### Comparing `abinitostudio-1.0.0/README.md` & `abinitostudio-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/abinitostudio/calculation/vasp_calculation.py` & `abinitostudio-1.0.1/abinitostudio/calculation/vasp_calculation.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/abinitostudio/io/vasp_io.py` & `abinitostudio-1.0.1/abinitostudio/io/vasp_io.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/abinitostudio/myMainWindow.py` & `abinitostudio-1.0.1/abinitostudio/myMainWindow.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/abinitostudio/plot/plot_field.py` & `abinitostudio-1.0.1/abinitostudio/plot/plot_field.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/abinitostudio/plot/plot_vasp.py` & `abinitostudio-1.0.1/abinitostudio/plot/plot_vasp.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/abinitostudio/structure/plot_structure.py` & `abinitostudio-1.0.1/abinitostudio/structure/plot_structure.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/abinitostudio/structure/tabdialog.py` & `abinitostudio-1.0.1/abinitostudio/structure/tabdialog.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/abinitostudio/ui/Dialog_DOS.py` & `abinitostudio-1.0.1/abinitostudio/ui/Dialog_DOS.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/abinitostudio/ui/Dialog_PB.py` & `abinitostudio-1.0.1/abinitostudio/ui/Dialog_PB.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/abinitostudio/ui/Dialog_band.py` & `abinitostudio-1.0.1/abinitostudio/ui/Dialog_band.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/abinitostudio/ui/UI.py` & `abinitostudio-1.0.1/abinitostudio/ui/UI.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/abinitostudio/ui/UI_setting.py` & `abinitostudio-1.0.1/abinitostudio/ui/UI_setting.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/abinitostudio/ui/UI_test.py` & `abinitostudio-1.0.1/abinitostudio/ui/UI_test.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/abinitostudio/ui/UI_vasp_DOS.py` & `abinitostudio-1.0.1/abinitostudio/ui/UI_vasp_DOS.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/abinitostudio/ui/UI_vasp_band.py` & `abinitostudio-1.0.1/abinitostudio/ui/UI_vasp_band.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/abinitostudio/ui/UI_vasp_band_noncal.py` & `abinitostudio-1.0.1/abinitostudio/ui/UI_vasp_band_noncal.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/abinitostudio/ui/UI_vasp_phonon.py` & `abinitostudio-1.0.1/abinitostudio/ui/UI_vasp_phonon.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/abinitostudio/ui/UI_vasp_scf.py` & `abinitostudio-1.0.1/abinitostudio/ui/UI_vasp_scf.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/abinitostudio/ui/UI_vasp_scf_noncal.py` & `abinitostudio-1.0.1/abinitostudio/ui/UI_vasp_scf_noncal.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/abinitostudio/ui/UI_vasp_supercell.py` & `abinitostudio-1.0.1/abinitostudio/ui/UI_vasp_supercell.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/abinitostudio/ui/UI_vasp_wannier.py` & `abinitostudio-1.0.1/abinitostudio/ui/UI_vasp_wannier.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/abinitostudio.egg-info/SOURCES.txt` & `abinitostudio-1.0.1/abinitostudio.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.txt
 MANIFEST.in
 README.md
 appMain.py
 install.py
 setup.py
 abinitostudio/__init__.py
 abinitostudio/myMainWindow.py
```

### Comparing `abinitostudio-1.0.0/appMain.py` & `abinitostudio-1.0.1/appMain.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/doc/启动图片.pptx` & `abinitostudio-1.0.1/doc/启动图片.pptx`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/doc/程序bug.docx` & `abinitostudio-1.0.1/doc/程序bug.docx`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/doc/说明文档.docx` & `abinitostudio-1.0.1/doc/说明文档.docx`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/doc/说明文档.pdf` & `abinitostudio-1.0.1/doc/说明文档.pdf`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/examples/CHGCAR` & `abinitostudio-1.0.1/examples/CHGCAR`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/examples/DOSCAR` & `abinitostudio-1.0.1/examples/DOSCAR`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/examples/EIGENVAL_CdCl` & `abinitostudio-1.0.1/examples/EIGENVAL_CdCl`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/examples/POSCAR` & `abinitostudio-1.0.1/examples/POSCAR`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/examples/PROCAR _CdCl` & `abinitostudio-1.0.1/examples/PROCAR _CdCl`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/images/3d可视.png` & `abinitostudio-1.0.1/images/3d可视.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/images/DOS.png` & `abinitostudio-1.0.1/images/DOS.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/images/band.png` & `abinitostudio-1.0.1/images/band.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/images/band_noncal.png` & `abinitostudio-1.0.1/images/band_noncal.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/images/phonin.png` & `abinitostudio-1.0.1/images/phonin.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/images/scf.png` & `abinitostudio-1.0.1/images/scf.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/images/scf_noncal.png` & `abinitostudio-1.0.1/images/scf_noncal.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/images/startup.jpg` & `abinitostudio-1.0.1/images/startup.jpg`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/images/vasp.png` & `abinitostudio-1.0.1/images/vasp.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/images/wannier.png` & `abinitostudio-1.0.1/images/wannier.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/images/关于.png` & `abinitostudio-1.0.1/images/关于.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/images/关闭.png` & `abinitostudio-1.0.1/images/关闭.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/images/层级.png` & `abinitostudio-1.0.1/images/层级.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/images/态密度.png` & `abinitostudio-1.0.1/images/态密度.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/images/扩胞.png` & `abinitostudio-1.0.1/images/扩胞.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/images/投影能带.png` & `abinitostudio-1.0.1/images/投影能带.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/images/测试.png` & `abinitostudio-1.0.1/images/测试.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/images/结构.png` & `abinitostudio-1.0.1/images/结构.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/images/能带.png` & `abinitostudio-1.0.1/images/能带.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/images/能带图.png` & `abinitostudio-1.0.1/images/能带图.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/images/设置.png` & `abinitostudio-1.0.1/images/设置.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/images/说明.png` & `abinitostudio-1.0.1/images/说明.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/scripts/cal_vasp_single.py` & `abinitostudio-1.0.1/scripts/cal_vasp_single.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/setup.py` & `abinitostudio-1.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
                     'abinitostudio.plot', 
                     'abinitostudio.structure', 
                     'abinitostudio.ui']
 abinito_scripts = ['scripts/cal_vasp_single.py']
 
 setup(name="abinitostudio",
     # pypi中的名称，pip或者easy_install安装时使用的名称，或生成egg文件的名称
-    version="1.0.0",
+    version="1.0.1",
     description="A studio for first-principles calculations.",
     long_description="This is a long description.",
     author="Pan Zhou, Xin Lu and Li Zhongsun",
     author_email="zhoupan71234@xtu.edu.cn",
     classifiers=["Development Status :: 3 - Alpha",'Programming Language :: Python',],
     # 需要打包的目录列表
     packages=['abinitostudio',
@@ -29,23 +29,21 @@
     # 需要安装的依赖
     install_requires=[
 		'paramiko==2.7.1',
 		'jumpssh==1.6.5',
 		'pyxtal==0.3.0',
 		'ase==3.19.1',
 		'pymatgen==2020.4.2',
+		'traits==6.0.0',
+		'traitsui==7.0.0',
 		'PyQt5==5.11.2',
-		'traits==4.6.0',
-		'traitsui==6.0.0',
 		'pyface==6.1.2',
 		'envisage==4.9.2',
 		'vtk==8.1.2',
 		'mayavi==4.7.1',
-		'traits==6.0.0',
-		'traitsui==7.0.0',
     ]
     # # 安装过程中，需要安装的静态文件，如配置文件、service文件、图片等
     # data_files=[
     #     ('', ['conf/*.conf']),
     #     ('/usr/lib/systemd/system/', ['bin/*.service']),
     # ],
     # # 希望被打包的文件
```

### Comparing `abinitostudio-1.0.0/test/test_CHGCAR.py` & `abinitostudio-1.0.1/test/test_CHGCAR.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/test/test_multiply_scene.py` & `abinitostudio-1.0.1/test/test_multiply_scene.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.0/test/test_pick.py` & `abinitostudio-1.0.1/test/test_pick.py`

 * *Files identical despite different names*

