# Comparing `tmp/chardet-5.1.0.tar.gz` & `tmp/chardet-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chardet-5.1.0.tar", last modified: Thu Dec  1 22:33:22 2022, max compression
+gzip compressed data, was "chardet-5.2.0.tar", last modified: Tue Aug  1 19:20:08 2023, max compression
```

## Comparing `chardet-5.1.0.tar` & `chardet-5.2.0.tar`

### file list

```diff
@@ -1,559 +1,560 @@
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.751726 chardet-5.1.0/
--rw-r--r--   0 danblanchard   (501) staff       (20)    26530 2022-07-03 20:13:08.000000 chardet-5.1.0/LICENSE
--rw-r--r--   0 danblanchard   (501) staff       (20)      195 2022-07-03 20:13:08.000000 chardet-5.1.0/MANIFEST.in
--rw-r--r--   0 danblanchard   (501) staff       (20)     3773 2022-07-03 20:13:08.000000 chardet-5.1.0/NOTES.rst
--rw-r--r--   0 danblanchard   (501) staff       (20)     3418 2022-12-01 22:33:22.751814 chardet-5.1.0/PKG-INFO
--rw-r--r--   0 danblanchard   (501) staff       (20)     2011 2022-07-17 17:41:43.000000 chardet-5.1.0/README.rst
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.650295 chardet-5.1.0/chardet/
--rw-r--r--   0 danblanchard   (501) staff       (20)     4797 2022-12-01 21:25:39.000000 chardet-5.1.0/chardet/__init__.py
--rw-r--r--   0 danblanchard   (501) staff       (20)    31274 2022-07-03 20:13:08.000000 chardet-5.1.0/chardet/big5freq.py
--rw-r--r--   0 danblanchard   (501) staff       (20)     1763 2022-07-03 20:13:08.000000 chardet-5.1.0/chardet/big5prober.py
--rw-r--r--   0 danblanchard   (501) staff       (20)    10032 2022-07-03 20:13:08.000000 chardet-5.1.0/chardet/chardistribution.py
--rw-r--r--   0 danblanchard   (501) staff       (20)     3915 2022-07-03 20:13:08.000000 chardet-5.1.0/chardet/charsetgroupprober.py
--rw-r--r--   0 danblanchard   (501) staff       (20)     5420 2022-12-01 22:33:01.000000 chardet-5.1.0/chardet/charsetprober.py
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.651345 chardet-5.1.0/chardet/cli/
--rw-r--r--   0 danblanchard   (501) staff       (20)        0 2022-07-03 20:13:08.000000 chardet-5.1.0/chardet/cli/__init__.py
--rw-r--r--   0 danblanchard   (501) staff       (20)     3242 2022-07-22 19:51:29.000000 chardet-5.1.0/chardet/cli/chardetect.py
--rw-r--r--   0 danblanchard   (501) staff       (20)     3732 2022-07-03 20:13:08.000000 chardet-5.1.0/chardet/codingstatemachine.py
--rw-r--r--   0 danblanchard   (501) staff       (20)      542 2022-07-03 20:13:08.000000 chardet-5.1.0/chardet/codingstatemachinedict.py
--rw-r--r--   0 danblanchard   (501) staff       (20)     1860 2022-07-03 20:13:08.000000 chardet-5.1.0/chardet/cp949prober.py
--rw-r--r--   0 danblanchard   (501) staff       (20)     1683 2022-07-03 20:13:08.000000 chardet-5.1.0/chardet/enums.py
--rw-r--r--   0 danblanchard   (501) staff       (20)     4006 2022-07-03 20:13:08.000000 chardet-5.1.0/chardet/escprober.py
--rw-r--r--   0 danblanchard   (501) staff       (20)    12176 2022-07-03 20:13:08.000000 chardet-5.1.0/chardet/escsm.py
--rw-r--r--   0 danblanchard   (501) staff       (20)     3934 2022-07-03 20:13:08.000000 chardet-5.1.0/chardet/eucjpprober.py
--rw-r--r--   0 danblanchard   (501) staff       (20)    13566 2022-07-03 20:13:08.000000 chardet-5.1.0/chardet/euckrfreq.py
--rw-r--r--   0 danblanchard   (501) staff       (20)     1753 2022-07-03 20:13:08.000000 chardet-5.1.0/chardet/euckrprober.py
--rw-r--r--   0 danblanchard   (501) staff       (20)    36913 2022-07-03 20:13:08.000000 chardet-5.1.0/chardet/euctwfreq.py
--rw-r--r--   0 danblanchard   (501) staff       (20)     1753 2022-07-03 20:13:08.000000 chardet-5.1.0/chardet/euctwprober.py
--rw-r--r--   0 danblanchard   (501) staff       (20)    20735 2022-07-03 20:13:08.000000 chardet-5.1.0/chardet/gb2312freq.py
--rw-r--r--   0 danblanchard   (501) staff       (20)     1759 2022-07-03 20:13:08.000000 chardet-5.1.0/chardet/gb2312prober.py
--rw-r--r--   0 danblanchard   (501) staff       (20)    14537 2022-07-03 20:13:08.000000 chardet-5.1.0/chardet/hebrewprober.py
--rw-r--r--   0 danblanchard   (501) staff       (20)    25796 2022-07-03 20:13:08.000000 chardet-5.1.0/chardet/jisfreq.py
--rw-r--r--   0 danblanchard   (501) staff       (20)    42498 2022-07-03 20:13:08.000000 chardet-5.1.0/chardet/johabfreq.py
--rw-r--r--   0 danblanchard   (501) staff       (20)     1752 2022-07-03 20:13:08.000000 chardet-5.1.0/chardet/johabprober.py
--rw-r--r--   0 danblanchard   (501) staff       (20)    27055 2022-07-03 20:13:08.000000 chardet-5.1.0/chardet/jpcntx.py
--rw-r--r--   0 danblanchard   (501) staff       (20)   104550 2022-07-03 20:13:08.000000 chardet-5.1.0/chardet/langbulgarianmodel.py
--rw-r--r--   0 danblanchard   (501) staff       (20)    98472 2022-07-03 20:13:08.000000 chardet-5.1.0/chardet/langgreekmodel.py
--rw-r--r--   0 danblanchard   (501) staff       (20)    98184 2022-07-03 20:13:08.000000 chardet-5.1.0/chardet/langhebrewmodel.py
--rw-r--r--   0 danblanchard   (501) staff       (20)   101351 2022-07-03 20:13:08.000000 chardet-5.1.0/chardet/langhungarianmodel.py
--rw-r--r--   0 danblanchard   (501) staff       (20)   128023 2022-07-03 20:13:08.000000 chardet-5.1.0/chardet/langrussianmodel.py
--rw-r--r--   0 danblanchard   (501) staff       (20)   102762 2022-07-03 20:13:08.000000 chardet-5.1.0/chardet/langthaimodel.py
--rw-r--r--   0 danblanchard   (501) staff       (20)    95360 2022-07-03 20:13:08.000000 chardet-5.1.0/chardet/langturkishmodel.py
--rw-r--r--   0 danblanchard   (501) staff       (20)     5380 2022-07-03 20:13:08.000000 chardet-5.1.0/chardet/latin1prober.py
--rw-r--r--   0 danblanchard   (501) staff       (20)     6077 2022-07-03 20:13:08.000000 chardet-5.1.0/chardet/macromanprober.py
--rw-r--r--   0 danblanchard   (501) staff       (20)     3715 2022-07-03 20:13:08.000000 chardet-5.1.0/chardet/mbcharsetprober.py
--rw-r--r--   0 danblanchard   (501) staff       (20)     2131 2022-07-03 20:13:08.000000 chardet-5.1.0/chardet/mbcsgroupprober.py
--rw-r--r--   0 danblanchard   (501) staff       (20)    30391 2022-07-03 20:13:08.000000 chardet-5.1.0/chardet/mbcssm.py
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.651643 chardet-5.1.0/chardet/metadata/
--rw-r--r--   0 danblanchard   (501) staff       (20)        0 2022-07-03 20:13:08.000000 chardet-5.1.0/chardet/metadata/__init__.py
--rw-r--r--   0 danblanchard   (501) staff       (20)    13560 2022-07-17 17:41:43.000000 chardet-5.1.0/chardet/metadata/languages.py
--rw-r--r--   0 danblanchard   (501) staff       (20)        0 2022-07-03 20:13:08.000000 chardet-5.1.0/chardet/py.typed
--rw-r--r--   0 danblanchard   (501) staff       (20)      402 2022-12-01 21:24:44.000000 chardet-5.1.0/chardet/resultdict.py
--rw-r--r--   0 danblanchard   (501) staff       (20)     6400 2022-07-03 20:13:08.000000 chardet-5.1.0/chardet/sbcharsetprober.py
--rw-r--r--   0 danblanchard   (501) staff       (20)     4137 2022-07-03 20:13:08.000000 chardet-5.1.0/chardet/sbcsgroupprober.py
--rw-r--r--   0 danblanchard   (501) staff       (20)     4007 2022-07-03 20:13:08.000000 chardet-5.1.0/chardet/sjisprober.py
--rw-r--r--   0 danblanchard   (501) staff       (20)    14848 2022-12-01 22:33:01.000000 chardet-5.1.0/chardet/universaldetector.py
--rw-r--r--   0 danblanchard   (501) staff       (20)     8505 2022-07-03 20:13:08.000000 chardet-5.1.0/chardet/utf1632prober.py
--rw-r--r--   0 danblanchard   (501) staff       (20)     2812 2022-07-03 20:13:08.000000 chardet-5.1.0/chardet/utf8prober.py
--rw-r--r--   0 danblanchard   (501) staff       (20)      244 2022-12-01 21:29:39.000000 chardet-5.1.0/chardet/version.py
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.651078 chardet-5.1.0/chardet.egg-info/
--rw-r--r--   0 danblanchard   (501) staff       (20)     3418 2022-12-01 22:33:22.000000 chardet-5.1.0/chardet.egg-info/PKG-INFO
--rw-r--r--   0 danblanchard   (501) staff       (20)    18204 2022-12-01 22:33:22.000000 chardet-5.1.0/chardet.egg-info/SOURCES.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)        1 2022-12-01 22:33:22.000000 chardet-5.1.0/chardet.egg-info/dependency_links.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)       59 2022-12-01 22:33:22.000000 chardet-5.1.0/chardet.egg-info/entry_points.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)        8 2022-12-01 22:33:22.000000 chardet-5.1.0/chardet.egg-info/top_level.txt
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.653513 chardet-5.1.0/docs/
--rw-r--r--   0 danblanchard   (501) staff       (20)        7 2022-07-03 20:13:08.000000 chardet-5.1.0/docs/.gitignore
--rw-r--r--   0 danblanchard   (501) staff       (20)     6766 2022-07-03 20:13:08.000000 chardet-5.1.0/docs/Makefile
--rw-r--r--   0 danblanchard   (501) staff       (20)      127 2022-07-03 20:13:08.000000 chardet-5.1.0/docs/README.md
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.653886 chardet-5.1.0/docs/api/
--rw-r--r--   0 danblanchard   (501) staff       (20)     5786 2022-07-03 20:13:08.000000 chardet-5.1.0/docs/api/chardet.rst
--rw-r--r--   0 danblanchard   (501) staff       (20)       58 2022-07-03 20:13:08.000000 chardet-5.1.0/docs/api/modules.rst
--rw-r--r--   0 danblanchard   (501) staff       (20)     8770 2022-07-03 20:13:08.000000 chardet-5.1.0/docs/conf.py
--rw-r--r--   0 danblanchard   (501) staff       (20)     5186 2022-07-03 20:13:08.000000 chardet-5.1.0/docs/faq.rst
--rw-r--r--   0 danblanchard   (501) staff       (20)     8574 2022-07-03 20:13:08.000000 chardet-5.1.0/docs/how-it-works.rst
--rw-r--r--   0 danblanchard   (501) staff       (20)      324 2022-07-03 20:13:08.000000 chardet-5.1.0/docs/index.rst
--rw-r--r--   0 danblanchard   (501) staff       (20)     6461 2022-07-03 20:13:08.000000 chardet-5.1.0/docs/make.bat
--rw-r--r--   0 danblanchard   (501) staff       (20)     1304 2022-07-03 20:13:08.000000 chardet-5.1.0/docs/supported-encodings.rst
--rw-r--r--   0 danblanchard   (501) staff       (20)     2817 2022-07-03 20:13:08.000000 chardet-5.1.0/docs/usage.rst
--rw-r--r--   0 danblanchard   (501) staff       (20)       81 2022-07-03 20:13:08.000000 chardet-5.1.0/pyproject.toml
--rw-r--r--   0 danblanchard   (501) staff       (20)     1573 2022-12-01 22:33:22.752134 chardet-5.1.0/setup.cfg
--rw-r--r--   0 danblanchard   (501) staff       (20)     8142 2022-07-22 19:51:29.000000 chardet-5.1.0/test.py
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.654089 chardet-5.1.0/tests/
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.660984 chardet-5.1.0/tests/Big5/
--rw-r--r--   0 danblanchard   (501) staff       (20)    23616 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/Big5/0804.blogspot.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)      770 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/Big5/_chromium_Big5_with_no_encoding_specified.html
--rw-r--r--   0 danblanchard   (501) staff       (20)      743 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/Big5/_ude_1.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)    10233 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/Big5/blog.worren.net.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    17791 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/Big5/carbonxiv.blogspot.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    18147 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/Big5/catshadow.blogspot.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    18354 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/Big5/coolloud.org.tw.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     1343 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/Big5/digitalwall.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     4945 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/Big5/ebao.us.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    28525 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/Big5/fudesign.blogspot.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    13558 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/Big5/kafkatseng.blogspot.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    14599 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/Big5/ke207.blogspot.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    18471 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/Big5/leavesth.blogspot.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    66777 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/Big5/letterlego.blogspot.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    12547 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/Big5/linyijen.blogspot.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     6440 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/Big5/marilynwu.blogspot.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     1464 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/Big5/myblog.pchome.com.tw.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     2278 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/Big5/oui-design.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    67286 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/Big5/sanwenji.blogspot.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    10639 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/Big5/sinica.edu.tw.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    17028 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/Big5/sylvia1976.blogspot.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     7192 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/Big5/tlkkuo.blogspot.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    15769 2022-12-01 21:28:03.000000 chardet-5.1.0/tests/Big5/unoriginalblog.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    68305 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/Big5/upsaid.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    13437 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/Big5/willythecop.blogspot.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    54145 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/Big5/ytc.blogspot.com.xml
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.661765 chardet-5.1.0/tests/CP932/
--rw-r--r--   0 danblanchard   (501) staff       (20)    45871 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/CP932/hardsoft.at.webry.info.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     4420 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/CP932/www2.chuo-u.ac.jp-suishin.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    37856 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/CP932/y-moto.com.xml
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.662019 chardet-5.1.0/tests/CP949/
--rw-r--r--   0 danblanchard   (501) staff       (20)    35289 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/CP949/ricanet.com.xml
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.668248 chardet-5.1.0/tests/EUC-JP/
--rw-r--r--   0 danblanchard   (501) staff       (20)      737 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-JP/_mozilla_bug426271_text-euc-jp.html
--rw-r--r--   0 danblanchard   (501) staff       (20)       39 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-JP/_mozilla_bug431054_text.html
--rw-r--r--   0 danblanchard   (501) staff       (20)     1176 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-JP/_mozilla_bug620106_text.html
--rw-r--r--   0 danblanchard   (501) staff       (20)     1375 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-JP/_ude_1.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)    15308 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-JP/aivy.co.jp.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    34082 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-JP/akaname.main.jp.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    73993 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-JP/arclamp.jp.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    30931 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-JP/aristrist.s57.xrea.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     8855 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-JP/artifact-jp.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    19768 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-JP/atom.ycf.nanet.co.jp.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     8072 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-JP/azito.under.jp.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    15188 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-JP/azoz.org.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    20472 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-JP/blog.kabu-navi.com.atom.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    17527 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-JP/blog.kabu-navi.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     7808 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-JP/bphrs.net.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    22171 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-JP/ch.kitaguni.tv.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     8094 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-JP/club.h14m.org.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    11504 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-JP/contents-factory.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    14851 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-JP/furusatonoeki.cutegirl.jp.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     7471 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-JP/manana.moo.jp.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    12646 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-JP/mimizun.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    20052 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-JP/misuzilla.org.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    98950 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-JP/overcube.com.atom.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     8857 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-JP/overcube.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    19883 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-JP/pinkupa.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    10855 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-JP/rdf.ycf.nanet.co.jp.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)   122707 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-JP/siesta.co.jp.aozora.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    15158 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-JP/tls.org.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    11596 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-JP/yukiboh.moo.jp.xml
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.674380 chardet-5.1.0/tests/EUC-KR/
--rw-r--r--   0 danblanchard   (501) staff       (20)      746 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-KR/_chromium_windows-949_with_no_encoding_specified.html
--rw-r--r--   0 danblanchard   (501) staff       (20)      291 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-KR/_mozilla_bug9357_text.html
--rw-r--r--   0 danblanchard   (501) staff       (20)      387 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-KR/_ude_euc1.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)     1164 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-KR/_ude_euc2.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)    10865 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-KR/acnnewswire.net.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    10715 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-KR/alogblog.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    16157 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-KR/arts.egloos.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    11272 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-KR/birder.egloos.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     9146 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-KR/blog.bd-lab.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     1869 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-KR/blog.empas.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     4188 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-KR/blog.rss.naver.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    28099 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-KR/calmguy.egloos.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    71320 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-KR/chisato.info.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     9970 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-KR/console.linuxstudy.pe.kr.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     5986 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-KR/critique.or.kr.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     8486 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-KR/epitaph.egloos.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    26659 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-KR/ittrend.egloos.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    19721 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-KR/jely.egloos.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    20847 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-KR/jely.pe.kr.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    41204 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-KR/jowchung.oolim.net.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     8538 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-KR/kina.egloos.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     6122 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-KR/lennon81.egloos.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     6339 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-KR/oroll.egloos.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     6519 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-KR/poliplus.egloos.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    10320 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-KR/scarletkh2.egloos.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    12646 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-KR/siwoo.org.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     6828 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-KR/sparcs.kaist.ac.kr.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    19792 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-KR/tori02.egloos.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    21598 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-KR/willis.egloos.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    44107 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-KR/xenix.egloos.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    23344 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-KR/yunho.egloos.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    14754 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-KR/zangsalang.egloos.com.xml
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.674557 chardet-5.1.0/tests/EUC-TW/
--rw-r--r--   0 danblanchard   (501) staff       (20)      743 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/EUC-TW/_ude_euc-tw1.txt
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.680703 chardet-5.1.0/tests/GB2312/
--rw-r--r--   0 danblanchard   (501) staff       (20)    15445 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/GB2312/14.blog.westca.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    21264 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/GB2312/2.blog.westca.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)      990 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/GB2312/_chromium_gb18030_with_no_encoding_specified.html.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     1126 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/GB2312/_mozilla_bug171813_text.html
--rw-r--r--   0 danblanchard   (501) staff       (20)    10620 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/GB2312/acnnewswire.net.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    15536 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/GB2312/bbs.blogsome.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     7336 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/GB2312/cappuccinos.3322.org.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    15173 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/GB2312/chen56.blogcn.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    16608 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/GB2312/cindychen.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    26465 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/GB2312/cnblog.org.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    12095 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/GB2312/coverer.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    22083 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/GB2312/eighthday.blogspot.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     2628 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/GB2312/godthink.blogsome.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     9356 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/GB2312/jjgod.3322.org.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    38414 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/GB2312/lily.blogsome.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    20395 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/GB2312/luciferwang.blogcn.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     4479 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/GB2312/pda.blogsome.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    87552 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/GB2312/softsea.net.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     5646 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/GB2312/w3cn.org.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    19804 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/GB2312/xy15400.blogcn.com.xml
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.684336 chardet-5.1.0/tests/IBM855/
--rw-r--r--   0 danblanchard   (501) staff       (20)     1211 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/IBM855/_ude_1.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)     7815 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/IBM855/aif.ru.health.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)      621 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/IBM855/aug32.hole.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    44660 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/IBM855/aviaport.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     6449 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/IBM855/blog.mlmaster.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    24863 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/IBM855/forum.template-toolkit.ru.1.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    10730 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/IBM855/forum.template-toolkit.ru.4.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    32200 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/IBM855/forum.template-toolkit.ru.6.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    17744 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/IBM855/forum.template-toolkit.ru.8.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     2968 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/IBM855/forum.template-toolkit.ru.9.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     2948 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/IBM855/greek.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)      575 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/IBM855/intertat.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    18809 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/IBM855/janulalife.blogspot.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     7463 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/IBM855/kapranoff.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     7550 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/IBM855/money.rin.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     7866 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/IBM855/music.peeps.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    24099 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/IBM855/newsru.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     2059 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/IBM855/susu.ac.ru.xml
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.688992 chardet-5.1.0/tests/IBM866/
--rw-r--r--   0 danblanchard   (501) staff       (20)     1211 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/IBM866/_ude_1.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)     7815 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/IBM866/aif.ru.health.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)      621 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/IBM866/aug32.hole.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    26912 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/IBM866/aviaport.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     6449 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/IBM866/blog.mlmaster.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    24863 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/IBM866/forum.template-toolkit.ru.1.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    10730 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/IBM866/forum.template-toolkit.ru.4.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    32200 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/IBM866/forum.template-toolkit.ru.6.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    17744 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/IBM866/forum.template-toolkit.ru.8.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     2968 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/IBM866/forum.template-toolkit.ru.9.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     4267 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/IBM866/greek.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)      575 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/IBM866/intertat.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    18809 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/IBM866/janulalife.blogspot.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     7463 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/IBM866/kapranoff.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     7550 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/IBM866/money.rin.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     7866 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/IBM866/music.peeps.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    24099 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/IBM866/newsru.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     2059 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/IBM866/susu.ac.ru.xml
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.689582 chardet-5.1.0/tests/Johab/
--rw-r--r--   0 danblanchard   (501) staff       (20)     1541 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/Johab/hlpro-readme.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)    18649 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/Johab/iyagi-readme.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)    70536 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/Johab/mdir-doc.txt
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.694109 chardet-5.1.0/tests/KOI8-R/
--rw-r--r--   0 danblanchard   (501) staff       (20)      583 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/KOI8-R/_chromium_KOI8-R_with_no_encoding_specified.html
--rw-r--r--   0 danblanchard   (501) staff       (20)     1211 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/KOI8-R/_ude_1.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)     7966 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/KOI8-R/aif.ru.health.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)      634 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/KOI8-R/aug32.hole.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    61945 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/KOI8-R/aviaport.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     6455 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/KOI8-R/blog.mlmaster.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    24894 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/KOI8-R/forum.template-toolkit.ru.1.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    11051 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/KOI8-R/forum.template-toolkit.ru.4.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    32901 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/KOI8-R/forum.template-toolkit.ru.6.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    18265 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/KOI8-R/forum.template-toolkit.ru.8.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     2979 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/KOI8-R/forum.template-toolkit.ru.9.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     4271 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/KOI8-R/greek.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    66462 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/KOI8-R/intertat.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    18809 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/KOI8-R/janulalife.blogspot.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     7701 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/KOI8-R/kapranoff.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    25155 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/KOI8-R/koi.kinder.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     7582 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/KOI8-R/money.rin.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     7947 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/KOI8-R/music.peeps.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    24264 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/KOI8-R/newsru.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    13623 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/KOI8-R/susu.ac.ru.xml
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.698387 chardet-5.1.0/tests/MacCyrillic/
--rw-r--r--   0 danblanchard   (501) staff       (20)     1211 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/MacCyrillic/_ude_1.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)     7825 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/MacCyrillic/aif.ru.health.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)      631 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/MacCyrillic/aug32.hole.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    60037 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/MacCyrillic/aviaport.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     6459 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/MacCyrillic/blog.mlmaster.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    10740 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/MacCyrillic/forum.template-toolkit.ru.4.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    32210 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/MacCyrillic/forum.template-toolkit.ru.6.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    17754 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/MacCyrillic/forum.template-toolkit.ru.8.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     2978 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/MacCyrillic/forum.template-toolkit.ru.9.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     2063 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/MacCyrillic/greek.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)      585 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/MacCyrillic/intertat.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     7473 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/MacCyrillic/kapranoff.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     3656 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/MacCyrillic/koi.kinder.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     7560 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/MacCyrillic/money.rin.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     7876 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/MacCyrillic/music.peeps.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    24109 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/MacCyrillic/newsru.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     1216 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/MacCyrillic/susu.ac.ru.xml
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.698624 chardet-5.1.0/tests/MacRoman/
--rw-r--r--   0 danblanchard   (501) staff       (20)   748505 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/MacRoman/ioreg_output.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)      267 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/README.txt
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.706339 chardet-5.1.0/tests/SHIFT_JIS/
--rw-r--r--   0 danblanchard   (501) staff       (20)    49064 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/SHIFT_JIS/10e.org.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    55398 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/SHIFT_JIS/1affliate.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     1030 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/SHIFT_JIS/_chromium_Shift-JIS_with_no_encoding_specified.html
--rw-r--r--   0 danblanchard   (501) staff       (20)    24612 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/SHIFT_JIS/_ude_1.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)     1375 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/SHIFT_JIS/_ude_2.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)     1375 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/SHIFT_JIS/_ude_3.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)    34727 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/SHIFT_JIS/_ude_4.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)    13732 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/SHIFT_JIS/accessories-brand.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    58977 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/SHIFT_JIS/amefoot.net.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    11351 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/SHIFT_JIS/andore.com.inami.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    17236 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/SHIFT_JIS/andore.com.money.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     8325 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/SHIFT_JIS/andore.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    30255 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/SHIFT_JIS/blog.inkase.net.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    24859 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/SHIFT_JIS/blog.paseri.ne.jp.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    27219 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/SHIFT_JIS/bloglelife.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    17145 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/SHIFT_JIS/brag.zaka.to.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    47828 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/SHIFT_JIS/celeb.lalalu.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    18136 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/SHIFT_JIS/clickablewords.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    30840 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/SHIFT_JIS/do.beginnersrack.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    17767 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/SHIFT_JIS/dogsinn.jp.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    16953 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/SHIFT_JIS/grebeweb.net.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    34584 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/SHIFT_JIS/milliontimes.jp.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     7588 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/SHIFT_JIS/moon-light.ne.jp.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    21540 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/SHIFT_JIS/nextbeaut.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     2681 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/SHIFT_JIS/ooganemochi.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     3760 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/SHIFT_JIS/perth-on.net.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    51676 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/SHIFT_JIS/sakusaka-silk.net.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    48592 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/SHIFT_JIS/setsuzei119.jp.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    30148 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/SHIFT_JIS/tamuyou.haun.org.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     5431 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/SHIFT_JIS/yasuhisa.com.xml
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.708221 chardet-5.1.0/tests/TIS-620/
--rw-r--r--   0 danblanchard   (501) staff       (20)       70 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/TIS-620/_mozilla_bug488426_text.html
--rw-r--r--   0 danblanchard   (501) staff       (20)    14156 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/TIS-620/opentle.org.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    12082 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/TIS-620/pharmacy.kku.ac.th.analyse1.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     9540 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/TIS-620/pharmacy.kku.ac.th.centerlab.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    19707 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/TIS-620/pharmacy.kku.ac.th.healthinfo-ne.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    13027 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/TIS-620/trickspot.boxchart.com.xml
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.708651 chardet-5.1.0/tests/UTF-16/
--rw-r--r--   0 danblanchard   (501) staff       (20)     1714 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/UTF-16/bom-utf-16-be.srt
--rw-r--r--   0 danblanchard   (501) staff       (20)     1714 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/UTF-16/bom-utf-16-le.srt
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.709050 chardet-5.1.0/tests/UTF-16BE/
--rw-r--r--   0 danblanchard   (501) staff       (20)     1588 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/UTF-16BE/nobom-utf16be.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)    12504 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/UTF-16BE/plane1-utf-16be.html
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.709471 chardet-5.1.0/tests/UTF-16LE/
--rw-r--r--   0 danblanchard   (501) staff       (20)     1588 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/UTF-16LE/nobom-utf16le.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)    12504 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/UTF-16LE/plane1-utf-16le.html
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.709925 chardet-5.1.0/tests/UTF-32/
--rw-r--r--   0 danblanchard   (501) staff       (20)     3428 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/UTF-32/bom-utf-32-be.srt
--rw-r--r--   0 danblanchard   (501) staff       (20)     3428 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/UTF-32/bom-utf-32-le.srt
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.710436 chardet-5.1.0/tests/UTF-32BE/
--rw-r--r--   0 danblanchard   (501) staff       (20)     3176 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/UTF-32BE/nobom-utf32be.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)    24500 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/UTF-32BE/plane1-utf-32be.html
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.710926 chardet-5.1.0/tests/UTF-32LE/
--rw-r--r--   0 danblanchard   (501) staff       (20)     3176 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/UTF-32LE/nobom-utf32le.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)    24500 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/UTF-32LE/plane1-utf-32le.html
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.711630 chardet-5.1.0/tests/ascii/
--rw-r--r--   0 danblanchard   (501) staff       (20)      472 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/ascii/_chromium_iso-8859-1_with_no_encoding_specified.html
--rw-r--r--   0 danblanchard   (501) staff       (20)     1108 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/ascii/_mozilla_bug638318_text.html
--rw-r--r--   0 danblanchard   (501) staff       (20)     3419 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/ascii/howto.diveintomark.org.xml
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.711839 chardet-5.1.0/tests/iso-2022-jp/
--rw-r--r--   0 danblanchard   (501) staff       (20)     1561 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-2022-jp/_ude_1.txt
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.712276 chardet-5.1.0/tests/iso-2022-kr/
--rw-r--r--   0 danblanchard   (501) staff       (20)      501 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-2022-kr/_ude_iso1.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)     1460 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-2022-kr/_ude_iso2.txt
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.713521 chardet-5.1.0/tests/iso-8859-1/
--rw-r--r--   0 danblanchard   (501) staff       (20)     1648 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-1/_ude_1.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)     2010 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-1/_ude_2.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)     1495 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-1/_ude_3.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)     1222 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-1/_ude_4.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)     1639 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-1/_ude_5.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)     2189 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-1/_ude_6.txt
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.713717 chardet-5.1.0/tests/iso-8859-2-croatian/
--rw-r--r--   0 danblanchard   (501) staff       (20)     5976 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-2-croatian/_ude_1.txt
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.714103 chardet-5.1.0/tests/iso-8859-2-czech/
--rw-r--r--   0 danblanchard   (501) staff       (20)     2154 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-2-czech/_ude_1.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)     1646 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-2-czech/_ude_2.txt
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.716839 chardet-5.1.0/tests/iso-8859-2-hungarian/
--rw-r--r--   0 danblanchard   (501) staff       (20)     2696 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-2-hungarian/_ude_1.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)     1409 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-2-hungarian/_ude_2.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)     1409 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-2-hungarian/_ude_3.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)    20435 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-2-hungarian/auto-apro.hu.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     5447 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-2-hungarian/cigartower.hu.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    13696 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-2-hungarian/escience.hu.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     3510 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-2-hungarian/hirtv.hu.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     4275 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-2-hungarian/honositomuhely.hu.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     7095 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-2-hungarian/saraspatak.hu.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    11632 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-2-hungarian/shamalt.uw.hu.mk.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     4950 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-2-hungarian/shamalt.uw.hu.mr.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     8202 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-2-hungarian/shamalt.uw.hu.mv.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    12464 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-2-hungarian/shamalt.uw.hu.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    17772 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-2-hungarian/ugyanmar.blogspot.com.xml
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.717043 chardet-5.1.0/tests/iso-8859-2-polish/
--rw-r--r--   0 danblanchard   (501) staff       (20)     3413 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-2-polish/_ude_1.txt
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.717421 chardet-5.1.0/tests/iso-8859-2-slovak/
--rw-r--r--   0 danblanchard   (501) staff       (20)     3201 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-2-slovak/_ude_1.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)     1136 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-2-slovak/_ude_2.txt
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.717614 chardet-5.1.0/tests/iso-8859-2-slovene/
--rw-r--r--   0 danblanchard   (501) staff       (20)     3861 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-2-slovene/_ude_1.txt
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.721031 chardet-5.1.0/tests/iso-8859-5-bulgarian/
--rw-r--r--   0 danblanchard   (501) staff       (20)    11527 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-5-bulgarian/aero-bg.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    15247 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-5-bulgarian/bbc.co.uk.popshow.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    12151 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-5-bulgarian/bpm.cult.bg.2.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     5584 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-5-bulgarian/bpm.cult.bg.4.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    12433 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-5-bulgarian/bpm.cult.bg.9.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     5591 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-5-bulgarian/bpm.cult.bg.medusa.4.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     2932 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-5-bulgarian/bpm.cult.bg.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     2102 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-5-bulgarian/debian.gabrovo.com.news.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     1184 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-5-bulgarian/debian.gabrovo.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     4190 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-5-bulgarian/doncho.net.comments.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    13120 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-5-bulgarian/ecloga.cult.bg.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     2721 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-5-bulgarian/ide.li.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     3009 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-5-bulgarian/linux-bg.org.xml
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.724471 chardet-5.1.0/tests/iso-8859-5-russian/
--rw-r--r--   0 danblanchard   (501) staff       (20)      587 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-5-russian/_chromium_ISO-8859-5_with_no_encoding_specified.html
--rw-r--r--   0 danblanchard   (501) staff       (20)     7823 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-5-russian/aif.ru.health.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)      629 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-5-russian/aug32.hole.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    44668 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-5-russian/aviaport.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     6457 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-5-russian/blog.mlmaster.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    24871 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-5-russian/forum.template-toolkit.ru.1.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    10738 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-5-russian/forum.template-toolkit.ru.4.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    32208 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-5-russian/forum.template-toolkit.ru.6.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    17752 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-5-russian/forum.template-toolkit.ru.8.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     2976 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-5-russian/forum.template-toolkit.ru.9.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     2061 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-5-russian/greek.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)      583 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-5-russian/intertat.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    18817 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-5-russian/janulalife.blogspot.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     7471 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-5-russian/kapranoff.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     7558 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-5-russian/money.rin.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     7874 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-5-russian/music.peeps.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    24107 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-5-russian/newsru.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     1214 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-5-russian/susu.ac.ru.xml
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.724645 chardet-5.1.0/tests/iso-8859-6-arabic/
--rw-r--r--   0 danblanchard   (501) staff       (20)      605 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-6-arabic/_chromium_ISO-8859-6_with_no_encoding_specified.html
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.727132 chardet-5.1.0/tests/iso-8859-7-greek/
--rw-r--r--   0 danblanchard   (501) staff       (20)      339 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-7-greek/_chromium_ISO-8859-7_with_no_encoding_specified.html
--rw-r--r--   0 danblanchard   (501) staff       (20)     1639 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-7-greek/_ude_1.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)     1180 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-7-greek/_ude_2.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)      570 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-7-greek/_ude_3.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)      570 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-7-greek/_ude_greek.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)    10120 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-7-greek/disabled.gr.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     2051 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-7-greek/hotstation.gr.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     4505 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-7-greek/naftemporiki.gr.bus.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     4072 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-7-greek/naftemporiki.gr.cmm.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     4473 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-7-greek/naftemporiki.gr.fin.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     4317 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-7-greek/naftemporiki.gr.mrk.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     4523 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-7-greek/naftemporiki.gr.mrt.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     4372 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-7-greek/naftemporiki.gr.spo.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     4576 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-7-greek/naftemporiki.gr.wld.xml
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.727961 chardet-5.1.0/tests/iso-8859-9-turkish/
--rw-r--r--   0 danblanchard   (501) staff       (20)     1379 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-9-turkish/_ude_1.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)     2394 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-9-turkish/_ude_2.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)     5971 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-9-turkish/divxplanet.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     1440 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-9-turkish/subtitle.srt
--rw-r--r--   0 danblanchard   (501) staff       (20)     1840 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/iso-8859-9-turkish/wikitop_tr_ISO-8859-9.txt
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.731671 chardet-5.1.0/tests/utf-8/
--rw-r--r--   0 danblanchard   (501) staff       (20)      811 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/utf-8/_chromium_UTF-8_with_no_encoding_specified.html
--rw-r--r--   0 danblanchard   (501) staff       (20)      227 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/utf-8/_mozilla_bug306272_text.html
--rw-r--r--   0 danblanchard   (501) staff       (20)     1027 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/utf-8/_mozilla_bug426271_text-utf-8.html
--rw-r--r--   0 danblanchard   (501) staff       (20)      549 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/utf-8/_ude_1.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)     1628 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/utf-8/_ude_2.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)       49 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/utf-8/_ude_3.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)      407 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/utf-8/_ude_5.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)     1039 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/utf-8/_ude_greek.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)     1187 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/utf-8/_ude_he1.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)     2893 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/utf-8/_ude_he2.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)      612 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/utf-8/_ude_he3.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)     2209 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/utf-8/_ude_russian.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)    37858 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/utf-8/anitabee.blogspot.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    42993 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/utf-8/balatonblog.typepad.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    12982 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/utf-8/boobooo.blogspot.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    14178 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/utf-8/linuxbox.hu.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    16479 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/utf-8/pihgy.hu.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    12234 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/utf-8/weblabor.hu.2.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    10054 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/utf-8/weblabor.hu.xml
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.732052 chardet-5.1.0/tests/utf-8-sig/
--rw-r--r--   0 danblanchard   (501) staff       (20)     1729 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/utf-8-sig/_ude_4.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)      859 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/utf-8-sig/bom-utf-8.srt
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.732385 chardet-5.1.0/tests/windows-1250-croatian/
--rw-r--r--   0 danblanchard   (501) staff       (20)     5976 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1250-croatian/_ude_1.txt
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.732727 chardet-5.1.0/tests/windows-1250-czech/
--rw-r--r--   0 danblanchard   (501) staff       (20)     2154 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1250-czech/_ude_1.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)     1646 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1250-czech/_ude_2.txt
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.735733 chardet-5.1.0/tests/windows-1250-hungarian/
--rw-r--r--   0 danblanchard   (501) staff       (20)     1685 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1250-hungarian/_ude_1.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)     2348 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1250-hungarian/_ude_2.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)     2009 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1250-hungarian/_ude_3.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)    21564 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1250-hungarian/bbc.co.uk.hu.forum.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    18576 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1250-hungarian/bbc.co.uk.hu.learningenglish.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    17091 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1250-hungarian/bbc.co.uk.hu.pressreview.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    46615 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1250-hungarian/bbc.co.uk.hu.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    13417 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1250-hungarian/objektivhir.hu.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)   596838 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1250-hungarian/torokorszag.blogspot.com.xml
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.736987 chardet-5.1.0/tests/windows-1250-polish/
--rw-r--r--   0 danblanchard   (501) staff       (20)     3413 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1250-polish/_ude_1.txt
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.737206 chardet-5.1.0/tests/windows-1250-romanian/
--rw-r--r--   0 danblanchard   (501) staff       (20)     3964 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1250-romanian/_ude_1.txt
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.737767 chardet-5.1.0/tests/windows-1250-slovak/
--rw-r--r--   0 danblanchard   (501) staff       (20)     1293 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1250-slovak/_ude_1.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)     1136 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1250-slovak/_ude_2.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)     3201 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1250-slovak/_ude_3.txt
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.737995 chardet-5.1.0/tests/windows-1250-slovene/
--rw-r--r--   0 danblanchard   (501) staff       (20)     2535 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1250-slovene/_ude_1.txt
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.740695 chardet-5.1.0/tests/windows-1251-bulgarian/
--rw-r--r--   0 danblanchard   (501) staff       (20)    28125 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1251-bulgarian/bbc.co.uk.popshow.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    12193 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1251-bulgarian/bpm.cult.bg.2.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    11184 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1251-bulgarian/bpm.cult.bg.3.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    11873 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1251-bulgarian/bpm.cult.bg.4.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    12546 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1251-bulgarian/bpm.cult.bg.9.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    11880 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1251-bulgarian/bpm.cult.bg.medusa.4.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     6568 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1251-bulgarian/bpm.cult.bg.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     2115 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1251-bulgarian/debian.gabrovo.com.news.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     1197 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1251-bulgarian/debian.gabrovo.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     9587 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1251-bulgarian/doncho.net.comments.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     9177 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1251-bulgarian/doncho.net.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    13203 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1251-bulgarian/ecloga.cult.bg.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     3963 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1251-bulgarian/ide.li.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     2026 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1251-bulgarian/informator.org.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     3030 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1251-bulgarian/linux-bg.org.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     5559 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1251-bulgarian/rinennor.org.xml
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.744215 chardet-5.1.0/tests/windows-1251-russian/
--rw-r--r--   0 danblanchard   (501) staff       (20)      589 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1251-russian/_chromium_windows-1251_with_no_encoding_specified.html
--rw-r--r--   0 danblanchard   (501) staff       (20)     1211 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1251-russian/_ude_1.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)     7827 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1251-russian/aif.ru.health.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    10482 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1251-russian/anthropology.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)      633 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1251-russian/aug32.hole.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    60039 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1251-russian/aviaport.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     6461 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1251-russian/blog.mlmaster.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    24875 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1251-russian/forum.template-toolkit.ru.1.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    10742 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1251-russian/forum.template-toolkit.ru.4.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    32212 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1251-russian/forum.template-toolkit.ru.6.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    17756 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1251-russian/forum.template-toolkit.ru.8.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     2980 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1251-russian/forum.template-toolkit.ru.9.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     2065 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1251-russian/greek.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)      587 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1251-russian/intertat.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    18821 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1251-russian/janulalife.blogspot.com.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     7475 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1251-russian/kapranoff.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     7562 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1251-russian/money.rin.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     7878 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1251-russian/music.peeps.ru.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    24111 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1251-russian/newsru.com.xml
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.745071 chardet-5.1.0/tests/windows-1252/
--rw-r--r--   0 danblanchard   (501) staff       (20)      671 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1252/_mozilla_bug421271_text.html
--rw-r--r--   0 danblanchard   (501) staff       (20)      865 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1252/_ude_1.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)     2257 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1252/_ude_2.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)      136 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1252/github_bug_9.txt
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.745450 chardet-5.1.0/tests/windows-1254-turkish/
--rw-r--r--   0 danblanchard   (501) staff       (20)      340 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1254-turkish/_chromium_windows-1254_with_no_encoding_specified.html
--rw-r--r--   0 danblanchard   (501) staff       (20)     2088 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1254-turkish/_ude_1.txt
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.751395 chardet-5.1.0/tests/windows-1255-hebrew/
--rw-r--r--   0 danblanchard   (501) staff       (20)      602 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1255-hebrew/_chromium_ISO-8859-8_with_no_encoding_specified.html
--rw-r--r--   0 danblanchard   (501) staff       (20)      604 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1255-hebrew/_chromium_windows-1255_with_no_encoding_specified.html
--rw-r--r--   0 danblanchard   (501) staff       (20)      681 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1255-hebrew/_ude_he1.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)     1608 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1255-hebrew/_ude_he2.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)      340 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1255-hebrew/_ude_he3.txt
--rw-r--r--   0 danblanchard   (501) staff       (20)   142386 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1255-hebrew/carshops.co.il.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    11896 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1255-hebrew/exego.net.2.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     3687 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1255-hebrew/hagada.org.il.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    15049 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1255-hebrew/halemo.net.edoar.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     2111 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1255-hebrew/hevra.org.il.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    82358 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1255-hebrew/hydepark.hevre.co.il.7957.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     7980 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1255-hebrew/info.org.il.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     8119 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1255-hebrew/infomed.co.il.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     5477 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1255-hebrew/law.co.il.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     1835 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1255-hebrew/maakav.org.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     7245 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1255-hebrew/neviim.net.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    10945 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1255-hebrew/notes.co.il.50.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    10056 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1255-hebrew/notes.co.il.6.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     9972 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1255-hebrew/notes.co.il.7.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)    10860 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1255-hebrew/notes.co.il.8.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     1652 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1255-hebrew/pcplus.co.il.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     4949 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1255-hebrew/sharks.co.il.xml
--rw-r--r--   0 danblanchard   (501) staff       (20)     8755 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1255-hebrew/whatsup.org.il.xml
-drwxr-xr-x   0 danblanchard   (501) staff       (20)        0 2022-12-01 22:33:22.751579 chardet-5.1.0/tests/windows-1256-arabic/
--rw-r--r--   0 danblanchard   (501) staff       (20)      607 2022-07-03 20:13:08.000000 chardet-5.1.0/tests/windows-1256-arabic/_chromium_windows-1256_with_no_encoding_specified.html
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.735478 chardet-5.2.0/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    26530 2023-08-01 19:07:52.000000 chardet-5.2.0/LICENSE
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      195 2023-08-01 19:07:52.000000 chardet-5.2.0/MANIFEST.in
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     3773 2023-08-01 19:07:52.000000 chardet-5.2.0/NOTES.rst
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     3418 2023-08-01 19:20:08.735556 chardet-5.2.0/PKG-INFO
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     2011 2023-08-01 19:07:52.000000 chardet-5.2.0/README.rst
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.673650 chardet-5.2.0/chardet/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     4797 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/__init__.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      123 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/__main__.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    31274 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/big5freq.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1763 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/big5prober.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    10032 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/chardistribution.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     3915 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/charsetgroupprober.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     5420 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/charsetprober.py
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.674470 chardet-5.2.0/chardet/cli/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/cli/__init__.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     3242 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/cli/chardetect.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     3732 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/codingstatemachine.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      542 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/codingstatemachinedict.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1860 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/cp949prober.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1683 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/enums.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     4006 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/escprober.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    12176 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/escsm.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     3934 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/eucjpprober.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    13566 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/euckrfreq.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1753 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/euckrprober.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    36913 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/euctwfreq.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1753 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/euctwprober.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    20735 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/gb2312freq.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1759 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/gb2312prober.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    14537 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/hebrewprober.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    25796 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/jisfreq.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    42498 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/johabfreq.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1752 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/johabprober.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    27055 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/jpcntx.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)   104550 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/langbulgarianmodel.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    98472 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/langgreekmodel.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    98184 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/langhebrewmodel.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)   101351 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/langhungarianmodel.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)   128023 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/langrussianmodel.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)   102762 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/langthaimodel.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    95360 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/langturkishmodel.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     5380 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/latin1prober.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     6077 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/macromanprober.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     3715 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/mbcharsetprober.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     2131 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/mbcsgroupprober.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    30391 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/mbcssm.py
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.674692 chardet-5.2.0/chardet/metadata/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/metadata/__init__.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    13560 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/metadata/languages.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/py.typed
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      402 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/resultdict.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     6400 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/sbcharsetprober.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     4137 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/sbcsgroupprober.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     4007 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/sjisprober.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    14848 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/universaldetector.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     8505 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/utf1632prober.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     2812 2023-08-01 19:07:52.000000 chardet-5.2.0/chardet/utf8prober.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      244 2023-08-01 19:20:01.000000 chardet-5.2.0/chardet/version.py
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.674248 chardet-5.2.0/chardet.egg-info/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     3418 2023-08-01 19:20:08.000000 chardet-5.2.0/chardet.egg-info/PKG-INFO
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    18224 2023-08-01 19:20:08.000000 chardet-5.2.0/chardet.egg-info/SOURCES.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)        1 2023-08-01 19:20:08.000000 chardet-5.2.0/chardet.egg-info/dependency_links.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)       59 2023-08-01 19:20:08.000000 chardet-5.2.0/chardet.egg-info/entry_points.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)        8 2023-08-01 19:20:08.000000 chardet-5.2.0/chardet.egg-info/top_level.txt
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.675809 chardet-5.2.0/docs/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)        7 2023-08-01 19:07:52.000000 chardet-5.2.0/docs/.gitignore
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     6766 2023-08-01 19:07:52.000000 chardet-5.2.0/docs/Makefile
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      127 2023-08-01 19:07:52.000000 chardet-5.2.0/docs/README.md
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.676045 chardet-5.2.0/docs/api/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     5786 2023-08-01 19:07:52.000000 chardet-5.2.0/docs/api/chardet.rst
+-rw-r--r--   0 danielblanchard   (501) staff       (20)       58 2023-08-01 19:07:52.000000 chardet-5.2.0/docs/api/modules.rst
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     8770 2023-08-01 19:07:52.000000 chardet-5.2.0/docs/conf.py
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     5186 2023-08-01 19:07:52.000000 chardet-5.2.0/docs/faq.rst
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     8574 2023-08-01 19:07:52.000000 chardet-5.2.0/docs/how-it-works.rst
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      324 2023-08-01 19:07:52.000000 chardet-5.2.0/docs/index.rst
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     6461 2023-08-01 19:07:52.000000 chardet-5.2.0/docs/make.bat
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1304 2023-08-01 19:07:52.000000 chardet-5.2.0/docs/supported-encodings.rst
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     2817 2023-08-01 19:07:52.000000 chardet-5.2.0/docs/usage.rst
+-rw-r--r--   0 danielblanchard   (501) staff       (20)       81 2023-08-01 19:07:52.000000 chardet-5.2.0/pyproject.toml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1573 2023-08-01 19:20:08.735868 chardet-5.2.0/setup.cfg
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     8142 2023-08-01 19:07:52.000000 chardet-5.2.0/test.py
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.676169 chardet-5.2.0/tests/
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.679602 chardet-5.2.0/tests/Big5/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    23616 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/Big5/0804.blogspot.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      770 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/Big5/_chromium_Big5_with_no_encoding_specified.html
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      743 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/Big5/_ude_1.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    10233 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/Big5/blog.worren.net.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    17791 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/Big5/carbonxiv.blogspot.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    18147 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/Big5/catshadow.blogspot.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    18354 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/Big5/coolloud.org.tw.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1343 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/Big5/digitalwall.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     4945 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/Big5/ebao.us.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    28525 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/Big5/fudesign.blogspot.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    13558 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/Big5/kafkatseng.blogspot.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    14599 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/Big5/ke207.blogspot.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    18471 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/Big5/leavesth.blogspot.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    66777 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/Big5/letterlego.blogspot.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    12547 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/Big5/linyijen.blogspot.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     6440 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/Big5/marilynwu.blogspot.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1464 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/Big5/myblog.pchome.com.tw.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     2278 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/Big5/oui-design.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    67286 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/Big5/sanwenji.blogspot.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    10639 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/Big5/sinica.edu.tw.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    17028 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/Big5/sylvia1976.blogspot.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     7192 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/Big5/tlkkuo.blogspot.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    15769 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/Big5/unoriginalblog.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    68305 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/Big5/upsaid.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    13437 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/Big5/willythecop.blogspot.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    54145 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/Big5/ytc.blogspot.com.xml
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.680042 chardet-5.2.0/tests/CP932/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    45871 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/CP932/hardsoft.at.webry.info.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     4420 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/CP932/www2.chuo-u.ac.jp-suishin.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    37856 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/CP932/y-moto.com.xml
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.680196 chardet-5.2.0/tests/CP949/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    35289 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/CP949/ricanet.com.xml
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.684275 chardet-5.2.0/tests/EUC-JP/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      737 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-JP/_mozilla_bug426271_text-euc-jp.html
+-rw-r--r--   0 danielblanchard   (501) staff       (20)       39 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-JP/_mozilla_bug431054_text.html
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1176 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-JP/_mozilla_bug620106_text.html
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1375 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-JP/_ude_1.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    15308 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-JP/aivy.co.jp.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    34082 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-JP/akaname.main.jp.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    73993 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-JP/arclamp.jp.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    30931 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-JP/aristrist.s57.xrea.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     8855 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-JP/artifact-jp.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    19768 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-JP/atom.ycf.nanet.co.jp.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     8072 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-JP/azito.under.jp.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    15188 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-JP/azoz.org.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    20472 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-JP/blog.kabu-navi.com.atom.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    17527 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-JP/blog.kabu-navi.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     7808 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-JP/bphrs.net.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    22171 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-JP/ch.kitaguni.tv.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     8094 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-JP/club.h14m.org.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    11504 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-JP/contents-factory.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    14851 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-JP/furusatonoeki.cutegirl.jp.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     7471 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-JP/manana.moo.jp.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    12646 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-JP/mimizun.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    20052 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-JP/misuzilla.org.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    98950 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-JP/overcube.com.atom.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     8857 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-JP/overcube.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    19883 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-JP/pinkupa.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    10855 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-JP/rdf.ycf.nanet.co.jp.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)   122707 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-JP/siesta.co.jp.aozora.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    15158 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-JP/tls.org.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    11596 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-JP/yukiboh.moo.jp.xml
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.688635 chardet-5.2.0/tests/EUC-KR/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      746 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-KR/_chromium_windows-949_with_no_encoding_specified.html
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      291 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-KR/_mozilla_bug9357_text.html
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      387 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-KR/_ude_euc1.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1164 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-KR/_ude_euc2.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    10865 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-KR/acnnewswire.net.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    10715 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-KR/alogblog.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    16157 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-KR/arts.egloos.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    11272 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-KR/birder.egloos.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     9146 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-KR/blog.bd-lab.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1869 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-KR/blog.empas.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     4188 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-KR/blog.rss.naver.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    28099 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-KR/calmguy.egloos.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    71320 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-KR/chisato.info.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     9970 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-KR/console.linuxstudy.pe.kr.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     5986 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-KR/critique.or.kr.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     8486 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-KR/epitaph.egloos.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    26659 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-KR/ittrend.egloos.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    19721 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-KR/jely.egloos.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    20847 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-KR/jely.pe.kr.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    41204 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-KR/jowchung.oolim.net.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     8538 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-KR/kina.egloos.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     6122 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-KR/lennon81.egloos.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     6339 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-KR/oroll.egloos.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     6519 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-KR/poliplus.egloos.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    10320 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-KR/scarletkh2.egloos.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    12646 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-KR/siwoo.org.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     6828 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-KR/sparcs.kaist.ac.kr.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    19792 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-KR/tori02.egloos.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    21598 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-KR/willis.egloos.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    44107 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-KR/xenix.egloos.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    23344 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-KR/yunho.egloos.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    14754 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-KR/zangsalang.egloos.com.xml
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.688780 chardet-5.2.0/tests/EUC-TW/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      743 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/EUC-TW/_ude_euc-tw1.txt
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.691569 chardet-5.2.0/tests/GB2312/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    15445 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/GB2312/14.blog.westca.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    21264 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/GB2312/2.blog.westca.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      990 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/GB2312/_chromium_gb18030_with_no_encoding_specified.html.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1126 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/GB2312/_mozilla_bug171813_text.html
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    10620 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/GB2312/acnnewswire.net.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    15536 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/GB2312/bbs.blogsome.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     7336 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/GB2312/cappuccinos.3322.org.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    15173 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/GB2312/chen56.blogcn.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    16608 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/GB2312/cindychen.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    26465 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/GB2312/cnblog.org.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    12095 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/GB2312/coverer.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    22083 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/GB2312/eighthday.blogspot.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     2628 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/GB2312/godthink.blogsome.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     9356 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/GB2312/jjgod.3322.org.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    38414 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/GB2312/lily.blogsome.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    20395 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/GB2312/luciferwang.blogcn.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     4479 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/GB2312/pda.blogsome.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    87552 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/GB2312/softsea.net.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     5646 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/GB2312/w3cn.org.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    19804 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/GB2312/xy15400.blogcn.com.xml
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.693840 chardet-5.2.0/tests/IBM855/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1211 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/IBM855/_ude_1.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     7815 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/IBM855/aif.ru.health.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      621 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/IBM855/aug32.hole.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    44660 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/IBM855/aviaport.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     6449 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/IBM855/blog.mlmaster.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    24863 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/IBM855/forum.template-toolkit.ru.1.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    10730 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/IBM855/forum.template-toolkit.ru.4.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    32200 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/IBM855/forum.template-toolkit.ru.6.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    17744 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/IBM855/forum.template-toolkit.ru.8.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     2968 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/IBM855/forum.template-toolkit.ru.9.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     2948 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/IBM855/greek.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      575 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/IBM855/intertat.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    18809 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/IBM855/janulalife.blogspot.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     7463 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/IBM855/kapranoff.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     7550 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/IBM855/money.rin.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     7866 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/IBM855/music.peeps.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    24099 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/IBM855/newsru.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     2059 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/IBM855/susu.ac.ru.xml
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.696544 chardet-5.2.0/tests/IBM866/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1211 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/IBM866/_ude_1.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     7815 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/IBM866/aif.ru.health.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      621 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/IBM866/aug32.hole.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    26912 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/IBM866/aviaport.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     6449 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/IBM866/blog.mlmaster.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    24863 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/IBM866/forum.template-toolkit.ru.1.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    10730 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/IBM866/forum.template-toolkit.ru.4.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    32200 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/IBM866/forum.template-toolkit.ru.6.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    17744 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/IBM866/forum.template-toolkit.ru.8.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     2968 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/IBM866/forum.template-toolkit.ru.9.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     4267 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/IBM866/greek.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      575 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/IBM866/intertat.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    18809 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/IBM866/janulalife.blogspot.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     7463 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/IBM866/kapranoff.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     7550 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/IBM866/money.rin.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     7866 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/IBM866/music.peeps.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    24099 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/IBM866/newsru.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     2059 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/IBM866/susu.ac.ru.xml
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.696996 chardet-5.2.0/tests/Johab/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1541 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/Johab/hlpro-readme.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    18649 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/Johab/iyagi-readme.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    70536 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/Johab/mdir-doc.txt
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.699886 chardet-5.2.0/tests/KOI8-R/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      583 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/KOI8-R/_chromium_KOI8-R_with_no_encoding_specified.html
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1211 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/KOI8-R/_ude_1.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     7966 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/KOI8-R/aif.ru.health.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      634 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/KOI8-R/aug32.hole.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    61945 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/KOI8-R/aviaport.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     6455 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/KOI8-R/blog.mlmaster.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    24894 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/KOI8-R/forum.template-toolkit.ru.1.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    11051 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/KOI8-R/forum.template-toolkit.ru.4.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    32901 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/KOI8-R/forum.template-toolkit.ru.6.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    18265 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/KOI8-R/forum.template-toolkit.ru.8.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     2979 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/KOI8-R/forum.template-toolkit.ru.9.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     4271 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/KOI8-R/greek.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    66462 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/KOI8-R/intertat.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    18809 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/KOI8-R/janulalife.blogspot.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     7701 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/KOI8-R/kapranoff.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    25155 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/KOI8-R/koi.kinder.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     7582 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/KOI8-R/money.rin.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     7947 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/KOI8-R/music.peeps.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    24264 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/KOI8-R/newsru.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    13623 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/KOI8-R/susu.ac.ru.xml
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.702078 chardet-5.2.0/tests/MacCyrillic/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1211 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/MacCyrillic/_ude_1.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     7825 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/MacCyrillic/aif.ru.health.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      631 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/MacCyrillic/aug32.hole.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    60037 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/MacCyrillic/aviaport.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     6459 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/MacCyrillic/blog.mlmaster.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    10740 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/MacCyrillic/forum.template-toolkit.ru.4.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    32210 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/MacCyrillic/forum.template-toolkit.ru.6.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    17754 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/MacCyrillic/forum.template-toolkit.ru.8.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     2978 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/MacCyrillic/forum.template-toolkit.ru.9.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     2063 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/MacCyrillic/greek.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      585 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/MacCyrillic/intertat.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     7473 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/MacCyrillic/kapranoff.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     3656 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/MacCyrillic/koi.kinder.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     7560 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/MacCyrillic/money.rin.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     7876 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/MacCyrillic/music.peeps.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    24109 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/MacCyrillic/newsru.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1216 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/MacCyrillic/susu.ac.ru.xml
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.702198 chardet-5.2.0/tests/MacRoman/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)   748505 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/MacRoman/ioreg_output.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      267 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/README.txt
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.706950 chardet-5.2.0/tests/SHIFT_JIS/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    49064 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/SHIFT_JIS/10e.org.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    55398 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/SHIFT_JIS/1affliate.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1030 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/SHIFT_JIS/_chromium_Shift-JIS_with_no_encoding_specified.html
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    24612 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/SHIFT_JIS/_ude_1.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1375 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/SHIFT_JIS/_ude_2.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1375 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/SHIFT_JIS/_ude_3.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    34727 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/SHIFT_JIS/_ude_4.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    13732 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/SHIFT_JIS/accessories-brand.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    58977 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/SHIFT_JIS/amefoot.net.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    11351 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/SHIFT_JIS/andore.com.inami.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    17236 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/SHIFT_JIS/andore.com.money.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     8325 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/SHIFT_JIS/andore.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    30255 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/SHIFT_JIS/blog.inkase.net.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    24859 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/SHIFT_JIS/blog.paseri.ne.jp.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    27219 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/SHIFT_JIS/bloglelife.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    17145 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/SHIFT_JIS/brag.zaka.to.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    47828 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/SHIFT_JIS/celeb.lalalu.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    18136 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/SHIFT_JIS/clickablewords.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    30840 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/SHIFT_JIS/do.beginnersrack.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    17767 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/SHIFT_JIS/dogsinn.jp.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    16953 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/SHIFT_JIS/grebeweb.net.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    34584 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/SHIFT_JIS/milliontimes.jp.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     7588 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/SHIFT_JIS/moon-light.ne.jp.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    21540 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/SHIFT_JIS/nextbeaut.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     2681 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/SHIFT_JIS/ooganemochi.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     3760 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/SHIFT_JIS/perth-on.net.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    51676 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/SHIFT_JIS/sakusaka-silk.net.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    48592 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/SHIFT_JIS/setsuzei119.jp.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    30148 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/SHIFT_JIS/tamuyou.haun.org.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     5431 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/SHIFT_JIS/yasuhisa.com.xml
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.707805 chardet-5.2.0/tests/TIS-620/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)       70 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/TIS-620/_mozilla_bug488426_text.html
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    14156 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/TIS-620/opentle.org.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    12082 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/TIS-620/pharmacy.kku.ac.th.analyse1.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     9540 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/TIS-620/pharmacy.kku.ac.th.centerlab.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    19707 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/TIS-620/pharmacy.kku.ac.th.healthinfo-ne.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    13027 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/TIS-620/trickspot.boxchart.com.xml
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.708142 chardet-5.2.0/tests/UTF-16/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1714 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/UTF-16/bom-utf-16-be.srt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1714 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/UTF-16/bom-utf-16-le.srt
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.708441 chardet-5.2.0/tests/UTF-16BE/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1588 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/UTF-16BE/nobom-utf16be.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    12504 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/UTF-16BE/plane1-utf-16be.html
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.708704 chardet-5.2.0/tests/UTF-16LE/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1588 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/UTF-16LE/nobom-utf16le.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    12504 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/UTF-16LE/plane1-utf-16le.html
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.709001 chardet-5.2.0/tests/UTF-32/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     3428 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/UTF-32/bom-utf-32-be.srt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     3428 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/UTF-32/bom-utf-32-le.srt
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.709311 chardet-5.2.0/tests/UTF-32BE/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     3176 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/UTF-32BE/nobom-utf32be.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    24500 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/UTF-32BE/plane1-utf-32be.html
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.709632 chardet-5.2.0/tests/UTF-32LE/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     3176 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/UTF-32LE/nobom-utf32le.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    24500 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/UTF-32LE/plane1-utf-32le.html
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.710110 chardet-5.2.0/tests/ascii/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      472 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/ascii/_chromium_iso-8859-1_with_no_encoding_specified.html
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1108 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/ascii/_mozilla_bug638318_text.html
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     3419 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/ascii/howto.diveintomark.org.xml
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.710260 chardet-5.2.0/tests/iso-2022-jp/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1561 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-2022-jp/_ude_1.txt
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.710563 chardet-5.2.0/tests/iso-2022-kr/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      501 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-2022-kr/_ude_iso1.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1460 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-2022-kr/_ude_iso2.txt
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.711447 chardet-5.2.0/tests/iso-8859-1/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1648 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-1/_ude_1.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     2010 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-1/_ude_2.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1495 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-1/_ude_3.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1222 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-1/_ude_4.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1639 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-1/_ude_5.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     2189 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-1/_ude_6.txt
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.711602 chardet-5.2.0/tests/iso-8859-2-croatian/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     5976 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-2-croatian/_ude_1.txt
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.711887 chardet-5.2.0/tests/iso-8859-2-czech/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     2154 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-2-czech/_ude_1.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1646 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-2-czech/_ude_2.txt
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.713612 chardet-5.2.0/tests/iso-8859-2-hungarian/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     2696 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-2-hungarian/_ude_1.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1409 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-2-hungarian/_ude_2.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1409 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-2-hungarian/_ude_3.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    20435 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-2-hungarian/auto-apro.hu.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     5447 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-2-hungarian/cigartower.hu.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    13696 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-2-hungarian/escience.hu.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     3510 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-2-hungarian/hirtv.hu.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     4275 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-2-hungarian/honositomuhely.hu.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     7095 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-2-hungarian/saraspatak.hu.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    11632 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-2-hungarian/shamalt.uw.hu.mk.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     4950 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-2-hungarian/shamalt.uw.hu.mr.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     8202 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-2-hungarian/shamalt.uw.hu.mv.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    12464 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-2-hungarian/shamalt.uw.hu.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    17772 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-2-hungarian/ugyanmar.blogspot.com.xml
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.713759 chardet-5.2.0/tests/iso-8859-2-polish/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     3413 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-2-polish/_ude_1.txt
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.714020 chardet-5.2.0/tests/iso-8859-2-slovak/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     3201 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-2-slovak/_ude_1.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1136 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-2-slovak/_ude_2.txt
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.714149 chardet-5.2.0/tests/iso-8859-2-slovene/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     3861 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-2-slovene/_ude_1.txt
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.716109 chardet-5.2.0/tests/iso-8859-5-bulgarian/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    11527 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-5-bulgarian/aero-bg.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    15247 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-5-bulgarian/bbc.co.uk.popshow.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    12151 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-5-bulgarian/bpm.cult.bg.2.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     5584 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-5-bulgarian/bpm.cult.bg.4.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    12433 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-5-bulgarian/bpm.cult.bg.9.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     5591 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-5-bulgarian/bpm.cult.bg.medusa.4.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     2932 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-5-bulgarian/bpm.cult.bg.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     2102 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-5-bulgarian/debian.gabrovo.com.news.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1184 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-5-bulgarian/debian.gabrovo.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     4190 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-5-bulgarian/doncho.net.comments.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    13120 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-5-bulgarian/ecloga.cult.bg.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     2721 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-5-bulgarian/ide.li.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     3009 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-5-bulgarian/linux-bg.org.xml
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.718855 chardet-5.2.0/tests/iso-8859-5-russian/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      587 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-5-russian/_chromium_ISO-8859-5_with_no_encoding_specified.html
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     7823 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-5-russian/aif.ru.health.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      629 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-5-russian/aug32.hole.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    44668 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-5-russian/aviaport.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     6457 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-5-russian/blog.mlmaster.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    24871 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-5-russian/forum.template-toolkit.ru.1.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    10738 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-5-russian/forum.template-toolkit.ru.4.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    32208 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-5-russian/forum.template-toolkit.ru.6.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    17752 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-5-russian/forum.template-toolkit.ru.8.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     2976 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-5-russian/forum.template-toolkit.ru.9.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     2061 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-5-russian/greek.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      583 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-5-russian/intertat.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    18817 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-5-russian/janulalife.blogspot.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     7471 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-5-russian/kapranoff.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     7558 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-5-russian/money.rin.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     7874 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-5-russian/music.peeps.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    24107 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-5-russian/newsru.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1214 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-5-russian/susu.ac.ru.xml
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.718993 chardet-5.2.0/tests/iso-8859-6-arabic/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      605 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-6-arabic/_chromium_ISO-8859-6_with_no_encoding_specified.html
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.720895 chardet-5.2.0/tests/iso-8859-7-greek/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      339 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-7-greek/_chromium_ISO-8859-7_with_no_encoding_specified.html
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1639 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-7-greek/_ude_1.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1180 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-7-greek/_ude_2.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      570 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-7-greek/_ude_3.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      570 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-7-greek/_ude_greek.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    10120 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-7-greek/disabled.gr.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     2051 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-7-greek/hotstation.gr.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     4505 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-7-greek/naftemporiki.gr.bus.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     4072 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-7-greek/naftemporiki.gr.cmm.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     4473 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-7-greek/naftemporiki.gr.fin.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     4317 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-7-greek/naftemporiki.gr.mrk.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     4523 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-7-greek/naftemporiki.gr.mrt.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     4372 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-7-greek/naftemporiki.gr.spo.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     4576 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-7-greek/naftemporiki.gr.wld.xml
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.721548 chardet-5.2.0/tests/iso-8859-9-turkish/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1379 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-9-turkish/_ude_1.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     2394 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-9-turkish/_ude_2.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     5971 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-9-turkish/divxplanet.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1440 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-9-turkish/subtitle.srt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1840 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/iso-8859-9-turkish/wikitop_tr_ISO-8859-9.txt
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.724023 chardet-5.2.0/tests/utf-8/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      811 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/utf-8/_chromium_UTF-8_with_no_encoding_specified.html
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      227 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/utf-8/_mozilla_bug306272_text.html
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1027 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/utf-8/_mozilla_bug426271_text-utf-8.html
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      549 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/utf-8/_ude_1.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1628 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/utf-8/_ude_2.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)       49 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/utf-8/_ude_3.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      407 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/utf-8/_ude_5.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1039 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/utf-8/_ude_greek.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1187 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/utf-8/_ude_he1.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     2893 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/utf-8/_ude_he2.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      612 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/utf-8/_ude_he3.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     2209 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/utf-8/_ude_russian.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    37858 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/utf-8/anitabee.blogspot.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    42993 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/utf-8/balatonblog.typepad.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    12982 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/utf-8/boobooo.blogspot.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    14178 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/utf-8/linuxbox.hu.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    16479 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/utf-8/pihgy.hu.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    12234 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/utf-8/weblabor.hu.2.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    10054 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/utf-8/weblabor.hu.xml
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.724291 chardet-5.2.0/tests/utf-8-sig/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1729 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/utf-8-sig/_ude_4.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      859 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/utf-8-sig/bom-utf-8.srt
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.724409 chardet-5.2.0/tests/windows-1250-croatian/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     5976 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1250-croatian/_ude_1.txt
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.724647 chardet-5.2.0/tests/windows-1250-czech/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     2154 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1250-czech/_ude_1.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1646 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1250-czech/_ude_2.txt
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.725813 chardet-5.2.0/tests/windows-1250-hungarian/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1685 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1250-hungarian/_ude_1.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     2348 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1250-hungarian/_ude_2.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     2009 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1250-hungarian/_ude_3.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    21564 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1250-hungarian/bbc.co.uk.hu.forum.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    18576 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1250-hungarian/bbc.co.uk.hu.learningenglish.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    17091 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1250-hungarian/bbc.co.uk.hu.pressreview.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    46615 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1250-hungarian/bbc.co.uk.hu.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    13417 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1250-hungarian/objektivhir.hu.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)   596838 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1250-hungarian/torokorszag.blogspot.com.xml
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.726208 chardet-5.2.0/tests/windows-1250-polish/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     3413 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1250-polish/_ude_1.txt
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.726326 chardet-5.2.0/tests/windows-1250-romanian/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     3964 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1250-romanian/_ude_1.txt
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.726682 chardet-5.2.0/tests/windows-1250-slovak/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1293 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1250-slovak/_ude_1.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1136 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1250-slovak/_ude_2.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     3201 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1250-slovak/_ude_3.txt
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.726807 chardet-5.2.0/tests/windows-1250-slovene/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     2535 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1250-slovene/_ude_1.txt
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.728988 chardet-5.2.0/tests/windows-1251-bulgarian/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    28125 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1251-bulgarian/bbc.co.uk.popshow.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    12193 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1251-bulgarian/bpm.cult.bg.2.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    11184 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1251-bulgarian/bpm.cult.bg.3.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    11873 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1251-bulgarian/bpm.cult.bg.4.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    12546 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1251-bulgarian/bpm.cult.bg.9.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    11880 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1251-bulgarian/bpm.cult.bg.medusa.4.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     6568 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1251-bulgarian/bpm.cult.bg.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     2115 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1251-bulgarian/debian.gabrovo.com.news.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1197 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1251-bulgarian/debian.gabrovo.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     9587 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1251-bulgarian/doncho.net.comments.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     9177 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1251-bulgarian/doncho.net.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    13203 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1251-bulgarian/ecloga.cult.bg.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     3963 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1251-bulgarian/ide.li.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     2026 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1251-bulgarian/informator.org.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     3030 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1251-bulgarian/linux-bg.org.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     5559 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1251-bulgarian/rinennor.org.xml
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.731499 chardet-5.2.0/tests/windows-1251-russian/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      589 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1251-russian/_chromium_windows-1251_with_no_encoding_specified.html
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1211 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1251-russian/_ude_1.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     7827 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1251-russian/aif.ru.health.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    10482 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1251-russian/anthropology.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      633 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1251-russian/aug32.hole.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    60039 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1251-russian/aviaport.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     6461 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1251-russian/blog.mlmaster.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    24875 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1251-russian/forum.template-toolkit.ru.1.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    10742 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1251-russian/forum.template-toolkit.ru.4.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    32212 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1251-russian/forum.template-toolkit.ru.6.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    17756 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1251-russian/forum.template-toolkit.ru.8.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     2980 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1251-russian/forum.template-toolkit.ru.9.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     2065 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1251-russian/greek.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      587 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1251-russian/intertat.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    18821 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1251-russian/janulalife.blogspot.com.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     7475 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1251-russian/kapranoff.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     7562 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1251-russian/money.rin.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     7878 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1251-russian/music.peeps.ru.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    24111 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1251-russian/newsru.com.xml
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.731989 chardet-5.2.0/tests/windows-1252/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      671 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1252/_mozilla_bug421271_text.html
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      865 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1252/_ude_1.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     2257 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1252/_ude_2.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      136 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1252/github_bug_9.txt
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.732259 chardet-5.2.0/tests/windows-1254-turkish/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      340 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1254-turkish/_chromium_windows-1254_with_no_encoding_specified.html
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     2088 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1254-turkish/_ude_1.txt
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.735235 chardet-5.2.0/tests/windows-1255-hebrew/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      602 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1255-hebrew/_chromium_ISO-8859-8_with_no_encoding_specified.html
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      604 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1255-hebrew/_chromium_windows-1255_with_no_encoding_specified.html
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      681 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1255-hebrew/_ude_he1.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1608 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1255-hebrew/_ude_he2.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      340 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1255-hebrew/_ude_he3.txt
+-rw-r--r--   0 danielblanchard   (501) staff       (20)   142386 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1255-hebrew/carshops.co.il.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    11896 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1255-hebrew/exego.net.2.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     3687 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1255-hebrew/hagada.org.il.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    15049 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1255-hebrew/halemo.net.edoar.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     2111 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1255-hebrew/hevra.org.il.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    82358 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1255-hebrew/hydepark.hevre.co.il.7957.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     7980 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1255-hebrew/info.org.il.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     8119 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1255-hebrew/infomed.co.il.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     5477 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1255-hebrew/law.co.il.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1835 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1255-hebrew/maakav.org.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     7245 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1255-hebrew/neviim.net.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    10945 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1255-hebrew/notes.co.il.50.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    10056 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1255-hebrew/notes.co.il.6.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     9972 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1255-hebrew/notes.co.il.7.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)    10860 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1255-hebrew/notes.co.il.8.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     1652 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1255-hebrew/pcplus.co.il.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     4949 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1255-hebrew/sharks.co.il.xml
+-rw-r--r--   0 danielblanchard   (501) staff       (20)     8755 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1255-hebrew/whatsup.org.il.xml
+drwxr-xr-x   0 danielblanchard   (501) staff       (20)        0 2023-08-01 19:20:08.735360 chardet-5.2.0/tests/windows-1256-arabic/
+-rw-r--r--   0 danielblanchard   (501) staff       (20)      607 2023-08-01 19:07:52.000000 chardet-5.2.0/tests/windows-1256-arabic/_chromium_windows-1256_with_no_encoding_specified.html
```

### Comparing `chardet-5.1.0/LICENSE` & `chardet-5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/NOTES.rst` & `chardet-5.2.0/NOTES.rst`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/PKG-INFO` & `chardet-5.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chardet
-Version: 5.1.0
+Version: 5.2.0
 Summary: Universal encoding detector for Python 3
 Home-page: https://github.com/chardet/chardet
 Author: Mark Pilgrim
 Author-email: mark@diveintomark.org
 Maintainer: Daniel Blanchard
 Maintainer-email: dan.blanchard@gmail.com
 License: LGPL
```

### Comparing `chardet-5.1.0/README.rst` & `chardet-5.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet/__init__.py` & `chardet-5.2.0/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet/big5freq.py` & `chardet-5.2.0/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet/big5prober.py` & `chardet-5.2.0/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet/chardistribution.py` & `chardet-5.2.0/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet/charsetgroupprober.py` & `chardet-5.2.0/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet/charsetprober.py` & `chardet-5.2.0/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet/cli/chardetect.py` & `chardet-5.2.0/chardet/cli/chardetect.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet/codingstatemachine.py` & `chardet-5.2.0/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet/codingstatemachinedict.py` & `chardet-5.2.0/chardet/codingstatemachinedict.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet/cp949prober.py` & `chardet-5.2.0/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet/enums.py` & `chardet-5.2.0/chardet/enums.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet/escprober.py` & `chardet-5.2.0/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet/escsm.py` & `chardet-5.2.0/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet/eucjpprober.py` & `chardet-5.2.0/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet/euckrfreq.py` & `chardet-5.2.0/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet/euckrprober.py` & `chardet-5.2.0/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet/euctwfreq.py` & `chardet-5.2.0/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet/euctwprober.py` & `chardet-5.2.0/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet/gb2312freq.py` & `chardet-5.2.0/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet/gb2312prober.py` & `chardet-5.2.0/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet/hebrewprober.py` & `chardet-5.2.0/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet/jisfreq.py` & `chardet-5.2.0/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet/johabfreq.py` & `chardet-5.2.0/chardet/johabfreq.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet/johabprober.py` & `chardet-5.2.0/chardet/johabprober.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet/jpcntx.py` & `chardet-5.2.0/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet/langbulgarianmodel.py` & `chardet-5.2.0/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet/langgreekmodel.py` & `chardet-5.2.0/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet/langhebrewmodel.py` & `chardet-5.2.0/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet/langhungarianmodel.py` & `chardet-5.2.0/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet/langrussianmodel.py` & `chardet-5.2.0/chardet/langrussianmodel.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet/langthaimodel.py` & `chardet-5.2.0/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet/langturkishmodel.py` & `chardet-5.2.0/chardet/langturkishmodel.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet/latin1prober.py` & `chardet-5.2.0/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet/macromanprober.py` & `chardet-5.2.0/chardet/macromanprober.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet/mbcharsetprober.py` & `chardet-5.2.0/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet/mbcsgroupprober.py` & `chardet-5.2.0/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet/mbcssm.py` & `chardet-5.2.0/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet/metadata/languages.py` & `chardet-5.2.0/chardet/metadata/languages.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet/sbcharsetprober.py` & `chardet-5.2.0/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet/sbcsgroupprober.py` & `chardet-5.2.0/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet/sjisprober.py` & `chardet-5.2.0/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet/universaldetector.py` & `chardet-5.2.0/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet/utf1632prober.py` & `chardet-5.2.0/chardet/utf1632prober.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet/utf8prober.py` & `chardet-5.2.0/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/chardet.egg-info/PKG-INFO` & `chardet-5.2.0/chardet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chardet
-Version: 5.1.0
+Version: 5.2.0
 Summary: Universal encoding detector for Python 3
 Home-page: https://github.com/chardet/chardet
 Author: Mark Pilgrim
 Author-email: mark@diveintomark.org
 Maintainer: Daniel Blanchard
 Maintainer-email: dan.blanchard@gmail.com
 License: LGPL
```

### Comparing `chardet-5.1.0/chardet.egg-info/SOURCES.txt` & `chardet-5.2.0/chardet.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 NOTES.rst
 README.rst
 pyproject.toml
 setup.cfg
 test.py
 chardet/__init__.py
+chardet/__main__.py
 chardet/big5freq.py
 chardet/big5prober.py
 chardet/chardistribution.py
 chardet/charsetgroupprober.py
 chardet/charsetprober.py
 chardet/codingstatemachine.py
 chardet/codingstatemachinedict.py
```

### Comparing `chardet-5.1.0/docs/Makefile` & `chardet-5.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/docs/api/chardet.rst` & `chardet-5.2.0/docs/api/chardet.rst`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/docs/conf.py` & `chardet-5.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/docs/faq.rst` & `chardet-5.2.0/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/docs/how-it-works.rst` & `chardet-5.2.0/docs/how-it-works.rst`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/docs/make.bat` & `chardet-5.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/docs/supported-encodings.rst` & `chardet-5.2.0/docs/supported-encodings.rst`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/docs/usage.rst` & `chardet-5.2.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/setup.cfg` & `chardet-5.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/test.py` & `chardet-5.2.0/test.py`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/Big5/0804.blogspot.com.xml` & `chardet-5.2.0/tests/Big5/0804.blogspot.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/Big5/_chromium_Big5_with_no_encoding_specified.html` & `chardet-5.2.0/tests/Big5/_chromium_Big5_with_no_encoding_specified.html`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/Big5/_ude_1.txt` & `chardet-5.2.0/tests/Big5/_ude_1.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/Big5/blog.worren.net.xml` & `chardet-5.2.0/tests/Big5/blog.worren.net.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/Big5/carbonxiv.blogspot.com.xml` & `chardet-5.2.0/tests/Big5/carbonxiv.blogspot.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/Big5/catshadow.blogspot.com.xml` & `chardet-5.2.0/tests/Big5/catshadow.blogspot.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/Big5/coolloud.org.tw.xml` & `chardet-5.2.0/tests/Big5/coolloud.org.tw.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/Big5/digitalwall.com.xml` & `chardet-5.2.0/tests/Big5/digitalwall.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/Big5/ebao.us.xml` & `chardet-5.2.0/tests/Big5/ebao.us.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/Big5/fudesign.blogspot.com.xml` & `chardet-5.2.0/tests/Big5/fudesign.blogspot.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/Big5/kafkatseng.blogspot.com.xml` & `chardet-5.2.0/tests/Big5/kafkatseng.blogspot.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/Big5/ke207.blogspot.com.xml` & `chardet-5.2.0/tests/Big5/ke207.blogspot.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/Big5/leavesth.blogspot.com.xml` & `chardet-5.2.0/tests/Big5/leavesth.blogspot.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/Big5/letterlego.blogspot.com.xml` & `chardet-5.2.0/tests/Big5/letterlego.blogspot.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/Big5/linyijen.blogspot.com.xml` & `chardet-5.2.0/tests/Big5/linyijen.blogspot.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/Big5/marilynwu.blogspot.com.xml` & `chardet-5.2.0/tests/Big5/marilynwu.blogspot.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/Big5/myblog.pchome.com.tw.xml` & `chardet-5.2.0/tests/Big5/myblog.pchome.com.tw.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/Big5/oui-design.com.xml` & `chardet-5.2.0/tests/Big5/oui-design.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/Big5/sanwenji.blogspot.com.xml` & `chardet-5.2.0/tests/Big5/sanwenji.blogspot.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/Big5/sinica.edu.tw.xml` & `chardet-5.2.0/tests/Big5/sinica.edu.tw.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/Big5/sylvia1976.blogspot.com.xml` & `chardet-5.2.0/tests/Big5/sylvia1976.blogspot.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/Big5/tlkkuo.blogspot.com.xml` & `chardet-5.2.0/tests/Big5/tlkkuo.blogspot.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/Big5/unoriginalblog.com.xml` & `chardet-5.2.0/tests/Big5/unoriginalblog.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/Big5/upsaid.com.xml` & `chardet-5.2.0/tests/Big5/upsaid.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/Big5/willythecop.blogspot.com.xml` & `chardet-5.2.0/tests/Big5/willythecop.blogspot.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/Big5/ytc.blogspot.com.xml` & `chardet-5.2.0/tests/Big5/ytc.blogspot.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/CP932/hardsoft.at.webry.info.xml` & `chardet-5.2.0/tests/CP932/hardsoft.at.webry.info.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/CP932/www2.chuo-u.ac.jp-suishin.xml` & `chardet-5.2.0/tests/CP932/www2.chuo-u.ac.jp-suishin.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/CP932/y-moto.com.xml` & `chardet-5.2.0/tests/CP932/y-moto.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/CP949/ricanet.com.xml` & `chardet-5.2.0/tests/CP949/ricanet.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-JP/_mozilla_bug426271_text-euc-jp.html` & `chardet-5.2.0/tests/EUC-JP/_mozilla_bug426271_text-euc-jp.html`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-JP/_mozilla_bug620106_text.html` & `chardet-5.2.0/tests/EUC-JP/_mozilla_bug620106_text.html`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-JP/_ude_1.txt` & `chardet-5.2.0/tests/EUC-JP/_ude_1.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-JP/aivy.co.jp.xml` & `chardet-5.2.0/tests/EUC-JP/aivy.co.jp.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-JP/akaname.main.jp.xml` & `chardet-5.2.0/tests/EUC-JP/akaname.main.jp.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-JP/arclamp.jp.xml` & `chardet-5.2.0/tests/EUC-JP/arclamp.jp.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-JP/aristrist.s57.xrea.com.xml` & `chardet-5.2.0/tests/EUC-JP/aristrist.s57.xrea.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-JP/artifact-jp.com.xml` & `chardet-5.2.0/tests/EUC-JP/artifact-jp.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-JP/atom.ycf.nanet.co.jp.xml` & `chardet-5.2.0/tests/EUC-JP/atom.ycf.nanet.co.jp.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-JP/azito.under.jp.xml` & `chardet-5.2.0/tests/EUC-JP/azito.under.jp.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-JP/azoz.org.xml` & `chardet-5.2.0/tests/EUC-JP/azoz.org.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-JP/blog.kabu-navi.com.atom.xml` & `chardet-5.2.0/tests/EUC-JP/blog.kabu-navi.com.atom.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-JP/blog.kabu-navi.com.xml` & `chardet-5.2.0/tests/EUC-JP/blog.kabu-navi.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-JP/bphrs.net.xml` & `chardet-5.2.0/tests/EUC-JP/bphrs.net.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-JP/ch.kitaguni.tv.xml` & `chardet-5.2.0/tests/EUC-JP/ch.kitaguni.tv.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-JP/club.h14m.org.xml` & `chardet-5.2.0/tests/EUC-JP/club.h14m.org.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-JP/contents-factory.com.xml` & `chardet-5.2.0/tests/EUC-JP/contents-factory.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-JP/furusatonoeki.cutegirl.jp.xml` & `chardet-5.2.0/tests/EUC-JP/furusatonoeki.cutegirl.jp.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-JP/manana.moo.jp.xml` & `chardet-5.2.0/tests/EUC-JP/manana.moo.jp.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-JP/mimizun.com.xml` & `chardet-5.2.0/tests/EUC-JP/mimizun.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-JP/misuzilla.org.xml` & `chardet-5.2.0/tests/EUC-JP/misuzilla.org.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-JP/overcube.com.atom.xml` & `chardet-5.2.0/tests/EUC-JP/overcube.com.atom.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-JP/overcube.com.xml` & `chardet-5.2.0/tests/EUC-JP/overcube.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-JP/pinkupa.com.xml` & `chardet-5.2.0/tests/EUC-JP/pinkupa.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-JP/rdf.ycf.nanet.co.jp.xml` & `chardet-5.2.0/tests/EUC-JP/rdf.ycf.nanet.co.jp.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-JP/siesta.co.jp.aozora.xml` & `chardet-5.2.0/tests/EUC-JP/siesta.co.jp.aozora.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-JP/tls.org.xml` & `chardet-5.2.0/tests/EUC-JP/tls.org.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-JP/yukiboh.moo.jp.xml` & `chardet-5.2.0/tests/EUC-JP/yukiboh.moo.jp.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-KR/_chromium_windows-949_with_no_encoding_specified.html` & `chardet-5.2.0/tests/EUC-KR/_chromium_windows-949_with_no_encoding_specified.html`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-KR/_ude_euc2.txt` & `chardet-5.2.0/tests/EUC-KR/_ude_euc2.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-KR/acnnewswire.net.xml` & `chardet-5.2.0/tests/EUC-KR/acnnewswire.net.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-KR/alogblog.com.xml` & `chardet-5.2.0/tests/EUC-KR/alogblog.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-KR/arts.egloos.com.xml` & `chardet-5.2.0/tests/EUC-KR/arts.egloos.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-KR/birder.egloos.com.xml` & `chardet-5.2.0/tests/EUC-KR/birder.egloos.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-KR/blog.bd-lab.com.xml` & `chardet-5.2.0/tests/EUC-KR/blog.bd-lab.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-KR/blog.empas.com.xml` & `chardet-5.2.0/tests/EUC-KR/blog.empas.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-KR/blog.rss.naver.com.xml` & `chardet-5.2.0/tests/EUC-KR/blog.rss.naver.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-KR/calmguy.egloos.com.xml` & `chardet-5.2.0/tests/EUC-KR/calmguy.egloos.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-KR/chisato.info.xml` & `chardet-5.2.0/tests/EUC-KR/chisato.info.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-KR/console.linuxstudy.pe.kr.xml` & `chardet-5.2.0/tests/EUC-KR/console.linuxstudy.pe.kr.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-KR/critique.or.kr.xml` & `chardet-5.2.0/tests/EUC-KR/critique.or.kr.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-KR/epitaph.egloos.com.xml` & `chardet-5.2.0/tests/EUC-KR/epitaph.egloos.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-KR/ittrend.egloos.com.xml` & `chardet-5.2.0/tests/EUC-KR/ittrend.egloos.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-KR/jely.egloos.com.xml` & `chardet-5.2.0/tests/EUC-KR/jely.egloos.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-KR/jely.pe.kr.xml` & `chardet-5.2.0/tests/EUC-KR/jely.pe.kr.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-KR/jowchung.oolim.net.xml` & `chardet-5.2.0/tests/EUC-KR/jowchung.oolim.net.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-KR/kina.egloos.com.xml` & `chardet-5.2.0/tests/EUC-KR/kina.egloos.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-KR/lennon81.egloos.com.xml` & `chardet-5.2.0/tests/EUC-KR/lennon81.egloos.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-KR/oroll.egloos.com.xml` & `chardet-5.2.0/tests/EUC-KR/oroll.egloos.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-KR/poliplus.egloos.com.xml` & `chardet-5.2.0/tests/EUC-KR/poliplus.egloos.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-KR/scarletkh2.egloos.com.xml` & `chardet-5.2.0/tests/EUC-KR/scarletkh2.egloos.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-KR/siwoo.org.xml` & `chardet-5.2.0/tests/EUC-KR/siwoo.org.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-KR/sparcs.kaist.ac.kr.xml` & `chardet-5.2.0/tests/EUC-KR/sparcs.kaist.ac.kr.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-KR/tori02.egloos.com.xml` & `chardet-5.2.0/tests/EUC-KR/tori02.egloos.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-KR/willis.egloos.com.xml` & `chardet-5.2.0/tests/EUC-KR/willis.egloos.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-KR/xenix.egloos.com.xml` & `chardet-5.2.0/tests/EUC-KR/xenix.egloos.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-KR/yunho.egloos.com.xml` & `chardet-5.2.0/tests/EUC-KR/yunho.egloos.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-KR/zangsalang.egloos.com.xml` & `chardet-5.2.0/tests/EUC-KR/zangsalang.egloos.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/EUC-TW/_ude_euc-tw1.txt` & `chardet-5.2.0/tests/EUC-TW/_ude_euc-tw1.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/GB2312/14.blog.westca.com.xml` & `chardet-5.2.0/tests/GB2312/14.blog.westca.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/GB2312/2.blog.westca.com.xml` & `chardet-5.2.0/tests/GB2312/2.blog.westca.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/GB2312/_chromium_gb18030_with_no_encoding_specified.html.xml` & `chardet-5.2.0/tests/GB2312/_chromium_gb18030_with_no_encoding_specified.html.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/GB2312/_mozilla_bug171813_text.html` & `chardet-5.2.0/tests/GB2312/_mozilla_bug171813_text.html`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/GB2312/acnnewswire.net.xml` & `chardet-5.2.0/tests/GB2312/acnnewswire.net.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/GB2312/bbs.blogsome.com.xml` & `chardet-5.2.0/tests/GB2312/bbs.blogsome.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/GB2312/cappuccinos.3322.org.xml` & `chardet-5.2.0/tests/GB2312/cappuccinos.3322.org.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/GB2312/chen56.blogcn.com.xml` & `chardet-5.2.0/tests/GB2312/chen56.blogcn.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/GB2312/cindychen.com.xml` & `chardet-5.2.0/tests/GB2312/cindychen.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/GB2312/cnblog.org.xml` & `chardet-5.2.0/tests/GB2312/cnblog.org.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/GB2312/coverer.com.xml` & `chardet-5.2.0/tests/GB2312/coverer.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/GB2312/eighthday.blogspot.com.xml` & `chardet-5.2.0/tests/GB2312/eighthday.blogspot.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/GB2312/godthink.blogsome.com.xml` & `chardet-5.2.0/tests/GB2312/godthink.blogsome.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/GB2312/jjgod.3322.org.xml` & `chardet-5.2.0/tests/GB2312/jjgod.3322.org.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/GB2312/lily.blogsome.com.xml` & `chardet-5.2.0/tests/GB2312/lily.blogsome.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/GB2312/luciferwang.blogcn.com.xml` & `chardet-5.2.0/tests/GB2312/luciferwang.blogcn.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/GB2312/pda.blogsome.com.xml` & `chardet-5.2.0/tests/GB2312/pda.blogsome.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/GB2312/softsea.net.xml` & `chardet-5.2.0/tests/GB2312/softsea.net.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/GB2312/w3cn.org.xml` & `chardet-5.2.0/tests/GB2312/w3cn.org.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/GB2312/xy15400.blogcn.com.xml` & `chardet-5.2.0/tests/GB2312/xy15400.blogcn.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/IBM855/_ude_1.txt` & `chardet-5.2.0/tests/IBM855/_ude_1.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/IBM855/aif.ru.health.xml` & `chardet-5.2.0/tests/IBM855/aif.ru.health.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/IBM855/aug32.hole.ru.xml` & `chardet-5.2.0/tests/IBM855/aug32.hole.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/IBM855/aviaport.ru.xml` & `chardet-5.2.0/tests/IBM855/aviaport.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/IBM855/blog.mlmaster.com.xml` & `chardet-5.2.0/tests/IBM855/blog.mlmaster.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/IBM855/forum.template-toolkit.ru.1.xml` & `chardet-5.2.0/tests/IBM855/forum.template-toolkit.ru.1.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/IBM855/forum.template-toolkit.ru.4.xml` & `chardet-5.2.0/tests/IBM855/forum.template-toolkit.ru.4.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/IBM855/forum.template-toolkit.ru.6.xml` & `chardet-5.2.0/tests/IBM855/forum.template-toolkit.ru.6.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/IBM855/forum.template-toolkit.ru.8.xml` & `chardet-5.2.0/tests/IBM855/forum.template-toolkit.ru.8.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/IBM855/forum.template-toolkit.ru.9.xml` & `chardet-5.2.0/tests/IBM855/forum.template-toolkit.ru.9.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/IBM855/greek.ru.xml` & `chardet-5.2.0/tests/IBM855/greek.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/IBM855/intertat.ru.xml` & `chardet-5.2.0/tests/IBM855/intertat.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/IBM855/janulalife.blogspot.com.xml` & `chardet-5.2.0/tests/IBM855/janulalife.blogspot.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/IBM855/kapranoff.ru.xml` & `chardet-5.2.0/tests/IBM855/kapranoff.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/IBM855/money.rin.ru.xml` & `chardet-5.2.0/tests/IBM855/money.rin.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/IBM855/music.peeps.ru.xml` & `chardet-5.2.0/tests/IBM855/music.peeps.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/IBM855/newsru.com.xml` & `chardet-5.2.0/tests/IBM855/newsru.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/IBM855/susu.ac.ru.xml` & `chardet-5.2.0/tests/IBM855/susu.ac.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/IBM866/_ude_1.txt` & `chardet-5.2.0/tests/IBM866/_ude_1.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/IBM866/aif.ru.health.xml` & `chardet-5.2.0/tests/IBM866/aif.ru.health.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/IBM866/aug32.hole.ru.xml` & `chardet-5.2.0/tests/IBM866/aug32.hole.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/IBM866/aviaport.ru.xml` & `chardet-5.2.0/tests/IBM866/aviaport.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/IBM866/blog.mlmaster.com.xml` & `chardet-5.2.0/tests/IBM866/blog.mlmaster.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/IBM866/forum.template-toolkit.ru.1.xml` & `chardet-5.2.0/tests/IBM866/forum.template-toolkit.ru.1.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/IBM866/forum.template-toolkit.ru.4.xml` & `chardet-5.2.0/tests/IBM866/forum.template-toolkit.ru.4.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/IBM866/forum.template-toolkit.ru.6.xml` & `chardet-5.2.0/tests/IBM866/forum.template-toolkit.ru.6.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/IBM866/forum.template-toolkit.ru.8.xml` & `chardet-5.2.0/tests/IBM866/forum.template-toolkit.ru.8.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/IBM866/forum.template-toolkit.ru.9.xml` & `chardet-5.2.0/tests/IBM866/forum.template-toolkit.ru.9.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/IBM866/greek.ru.xml` & `chardet-5.2.0/tests/IBM866/greek.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/IBM866/intertat.ru.xml` & `chardet-5.2.0/tests/IBM866/intertat.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/IBM866/janulalife.blogspot.com.xml` & `chardet-5.2.0/tests/IBM866/janulalife.blogspot.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/IBM866/kapranoff.ru.xml` & `chardet-5.2.0/tests/IBM866/kapranoff.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/IBM866/money.rin.ru.xml` & `chardet-5.2.0/tests/IBM866/money.rin.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/IBM866/music.peeps.ru.xml` & `chardet-5.2.0/tests/IBM866/music.peeps.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/IBM866/newsru.com.xml` & `chardet-5.2.0/tests/IBM866/newsru.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/IBM866/susu.ac.ru.xml` & `chardet-5.2.0/tests/IBM866/susu.ac.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/Johab/hlpro-readme.txt` & `chardet-5.2.0/tests/Johab/hlpro-readme.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/Johab/iyagi-readme.txt` & `chardet-5.2.0/tests/Johab/iyagi-readme.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/Johab/mdir-doc.txt` & `chardet-5.2.0/tests/Johab/mdir-doc.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/KOI8-R/_chromium_KOI8-R_with_no_encoding_specified.html` & `chardet-5.2.0/tests/KOI8-R/_chromium_KOI8-R_with_no_encoding_specified.html`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/KOI8-R/_ude_1.txt` & `chardet-5.2.0/tests/KOI8-R/_ude_1.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/KOI8-R/aif.ru.health.xml` & `chardet-5.2.0/tests/KOI8-R/aif.ru.health.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/KOI8-R/aug32.hole.ru.xml` & `chardet-5.2.0/tests/KOI8-R/aug32.hole.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/KOI8-R/aviaport.ru.xml` & `chardet-5.2.0/tests/KOI8-R/aviaport.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/KOI8-R/blog.mlmaster.com.xml` & `chardet-5.2.0/tests/KOI8-R/blog.mlmaster.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/KOI8-R/forum.template-toolkit.ru.1.xml` & `chardet-5.2.0/tests/KOI8-R/forum.template-toolkit.ru.1.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/KOI8-R/forum.template-toolkit.ru.4.xml` & `chardet-5.2.0/tests/KOI8-R/forum.template-toolkit.ru.4.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/KOI8-R/forum.template-toolkit.ru.6.xml` & `chardet-5.2.0/tests/KOI8-R/forum.template-toolkit.ru.6.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/KOI8-R/forum.template-toolkit.ru.8.xml` & `chardet-5.2.0/tests/KOI8-R/forum.template-toolkit.ru.8.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/KOI8-R/forum.template-toolkit.ru.9.xml` & `chardet-5.2.0/tests/KOI8-R/forum.template-toolkit.ru.9.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/KOI8-R/greek.ru.xml` & `chardet-5.2.0/tests/KOI8-R/greek.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/KOI8-R/intertat.ru.xml` & `chardet-5.2.0/tests/KOI8-R/intertat.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/KOI8-R/janulalife.blogspot.com.xml` & `chardet-5.2.0/tests/KOI8-R/janulalife.blogspot.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/KOI8-R/kapranoff.ru.xml` & `chardet-5.2.0/tests/KOI8-R/kapranoff.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/KOI8-R/koi.kinder.ru.xml` & `chardet-5.2.0/tests/KOI8-R/koi.kinder.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/KOI8-R/money.rin.ru.xml` & `chardet-5.2.0/tests/KOI8-R/money.rin.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/KOI8-R/music.peeps.ru.xml` & `chardet-5.2.0/tests/KOI8-R/music.peeps.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/KOI8-R/newsru.com.xml` & `chardet-5.2.0/tests/KOI8-R/newsru.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/KOI8-R/susu.ac.ru.xml` & `chardet-5.2.0/tests/KOI8-R/susu.ac.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/MacCyrillic/_ude_1.txt` & `chardet-5.2.0/tests/MacCyrillic/_ude_1.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/MacCyrillic/aif.ru.health.xml` & `chardet-5.2.0/tests/MacCyrillic/aif.ru.health.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/MacCyrillic/aug32.hole.ru.xml` & `chardet-5.2.0/tests/MacCyrillic/aug32.hole.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/MacCyrillic/aviaport.ru.xml` & `chardet-5.2.0/tests/MacCyrillic/aviaport.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/MacCyrillic/blog.mlmaster.com.xml` & `chardet-5.2.0/tests/MacCyrillic/blog.mlmaster.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/MacCyrillic/forum.template-toolkit.ru.4.xml` & `chardet-5.2.0/tests/MacCyrillic/forum.template-toolkit.ru.4.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/MacCyrillic/forum.template-toolkit.ru.6.xml` & `chardet-5.2.0/tests/MacCyrillic/forum.template-toolkit.ru.6.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/MacCyrillic/forum.template-toolkit.ru.8.xml` & `chardet-5.2.0/tests/MacCyrillic/forum.template-toolkit.ru.8.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/MacCyrillic/forum.template-toolkit.ru.9.xml` & `chardet-5.2.0/tests/MacCyrillic/forum.template-toolkit.ru.9.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/MacCyrillic/greek.ru.xml` & `chardet-5.2.0/tests/MacCyrillic/greek.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/MacCyrillic/intertat.ru.xml` & `chardet-5.2.0/tests/MacCyrillic/intertat.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/MacCyrillic/kapranoff.ru.xml` & `chardet-5.2.0/tests/MacCyrillic/kapranoff.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/MacCyrillic/koi.kinder.ru.xml` & `chardet-5.2.0/tests/MacCyrillic/koi.kinder.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/MacCyrillic/money.rin.ru.xml` & `chardet-5.2.0/tests/MacCyrillic/money.rin.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/MacCyrillic/music.peeps.ru.xml` & `chardet-5.2.0/tests/MacCyrillic/music.peeps.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/MacCyrillic/newsru.com.xml` & `chardet-5.2.0/tests/MacCyrillic/newsru.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/MacCyrillic/susu.ac.ru.xml` & `chardet-5.2.0/tests/MacCyrillic/susu.ac.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/MacRoman/ioreg_output.txt` & `chardet-5.2.0/tests/MacRoman/ioreg_output.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/SHIFT_JIS/10e.org.xml` & `chardet-5.2.0/tests/SHIFT_JIS/10e.org.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/SHIFT_JIS/1affliate.com.xml` & `chardet-5.2.0/tests/SHIFT_JIS/1affliate.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/SHIFT_JIS/_chromium_Shift-JIS_with_no_encoding_specified.html` & `chardet-5.2.0/tests/SHIFT_JIS/_chromium_Shift-JIS_with_no_encoding_specified.html`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/SHIFT_JIS/_ude_1.txt` & `chardet-5.2.0/tests/SHIFT_JIS/_ude_1.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/SHIFT_JIS/_ude_2.txt` & `chardet-5.2.0/tests/SHIFT_JIS/_ude_2.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/SHIFT_JIS/_ude_3.txt` & `chardet-5.2.0/tests/SHIFT_JIS/_ude_3.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/SHIFT_JIS/_ude_4.txt` & `chardet-5.2.0/tests/SHIFT_JIS/_ude_4.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/SHIFT_JIS/accessories-brand.com.xml` & `chardet-5.2.0/tests/SHIFT_JIS/accessories-brand.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/SHIFT_JIS/amefoot.net.xml` & `chardet-5.2.0/tests/SHIFT_JIS/amefoot.net.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/SHIFT_JIS/andore.com.inami.xml` & `chardet-5.2.0/tests/SHIFT_JIS/andore.com.inami.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/SHIFT_JIS/andore.com.money.xml` & `chardet-5.2.0/tests/SHIFT_JIS/andore.com.money.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/SHIFT_JIS/andore.com.xml` & `chardet-5.2.0/tests/SHIFT_JIS/andore.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/SHIFT_JIS/blog.inkase.net.xml` & `chardet-5.2.0/tests/SHIFT_JIS/blog.inkase.net.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/SHIFT_JIS/blog.paseri.ne.jp.xml` & `chardet-5.2.0/tests/SHIFT_JIS/blog.paseri.ne.jp.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/SHIFT_JIS/bloglelife.com.xml` & `chardet-5.2.0/tests/SHIFT_JIS/bloglelife.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/SHIFT_JIS/brag.zaka.to.xml` & `chardet-5.2.0/tests/SHIFT_JIS/brag.zaka.to.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/SHIFT_JIS/celeb.lalalu.com.xml` & `chardet-5.2.0/tests/SHIFT_JIS/celeb.lalalu.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/SHIFT_JIS/clickablewords.com.xml` & `chardet-5.2.0/tests/SHIFT_JIS/clickablewords.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/SHIFT_JIS/do.beginnersrack.com.xml` & `chardet-5.2.0/tests/SHIFT_JIS/do.beginnersrack.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/SHIFT_JIS/dogsinn.jp.xml` & `chardet-5.2.0/tests/SHIFT_JIS/dogsinn.jp.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/SHIFT_JIS/grebeweb.net.xml` & `chardet-5.2.0/tests/SHIFT_JIS/grebeweb.net.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/SHIFT_JIS/milliontimes.jp.xml` & `chardet-5.2.0/tests/SHIFT_JIS/milliontimes.jp.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/SHIFT_JIS/moon-light.ne.jp.xml` & `chardet-5.2.0/tests/SHIFT_JIS/moon-light.ne.jp.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/SHIFT_JIS/nextbeaut.com.xml` & `chardet-5.2.0/tests/SHIFT_JIS/nextbeaut.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/SHIFT_JIS/ooganemochi.com.xml` & `chardet-5.2.0/tests/SHIFT_JIS/ooganemochi.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/SHIFT_JIS/perth-on.net.xml` & `chardet-5.2.0/tests/SHIFT_JIS/perth-on.net.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/SHIFT_JIS/sakusaka-silk.net.xml` & `chardet-5.2.0/tests/SHIFT_JIS/sakusaka-silk.net.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/SHIFT_JIS/setsuzei119.jp.xml` & `chardet-5.2.0/tests/SHIFT_JIS/setsuzei119.jp.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/SHIFT_JIS/tamuyou.haun.org.xml` & `chardet-5.2.0/tests/SHIFT_JIS/tamuyou.haun.org.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/SHIFT_JIS/yasuhisa.com.xml` & `chardet-5.2.0/tests/SHIFT_JIS/yasuhisa.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/TIS-620/opentle.org.xml` & `chardet-5.2.0/tests/TIS-620/opentle.org.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/TIS-620/pharmacy.kku.ac.th.analyse1.xml` & `chardet-5.2.0/tests/TIS-620/pharmacy.kku.ac.th.analyse1.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/TIS-620/pharmacy.kku.ac.th.centerlab.xml` & `chardet-5.2.0/tests/TIS-620/pharmacy.kku.ac.th.centerlab.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/TIS-620/pharmacy.kku.ac.th.healthinfo-ne.xml` & `chardet-5.2.0/tests/TIS-620/pharmacy.kku.ac.th.healthinfo-ne.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/TIS-620/trickspot.boxchart.com.xml` & `chardet-5.2.0/tests/TIS-620/trickspot.boxchart.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/UTF-16/bom-utf-16-be.srt` & `chardet-5.2.0/tests/UTF-16/bom-utf-16-be.srt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/UTF-16/bom-utf-16-le.srt` & `chardet-5.2.0/tests/UTF-16/bom-utf-16-le.srt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/UTF-16BE/nobom-utf16be.txt` & `chardet-5.2.0/tests/UTF-16BE/nobom-utf16be.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/UTF-16BE/plane1-utf-16be.html` & `chardet-5.2.0/tests/UTF-16BE/plane1-utf-16be.html`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/UTF-16LE/nobom-utf16le.txt` & `chardet-5.2.0/tests/UTF-16LE/nobom-utf16le.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/UTF-16LE/plane1-utf-16le.html` & `chardet-5.2.0/tests/UTF-16LE/plane1-utf-16le.html`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/UTF-32/bom-utf-32-be.srt` & `chardet-5.2.0/tests/UTF-32/bom-utf-32-be.srt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/UTF-32/bom-utf-32-le.srt` & `chardet-5.2.0/tests/UTF-32/bom-utf-32-le.srt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/UTF-32BE/nobom-utf32be.txt` & `chardet-5.2.0/tests/UTF-32BE/nobom-utf32be.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/UTF-32BE/plane1-utf-32be.html` & `chardet-5.2.0/tests/UTF-32BE/plane1-utf-32be.html`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/UTF-32LE/nobom-utf32le.txt` & `chardet-5.2.0/tests/UTF-32LE/nobom-utf32le.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/UTF-32LE/plane1-utf-32le.html` & `chardet-5.2.0/tests/UTF-32LE/plane1-utf-32le.html`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/ascii/howto.diveintomark.org.xml` & `chardet-5.2.0/tests/ascii/howto.diveintomark.org.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-2022-jp/_ude_1.txt` & `chardet-5.2.0/tests/iso-2022-jp/_ude_1.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-2022-kr/_ude_iso2.txt` & `chardet-5.2.0/tests/iso-2022-kr/_ude_iso2.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-1/_ude_1.txt` & `chardet-5.2.0/tests/iso-8859-1/_ude_1.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-1/_ude_2.txt` & `chardet-5.2.0/tests/iso-8859-1/_ude_2.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-1/_ude_3.txt` & `chardet-5.2.0/tests/iso-8859-1/_ude_3.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-1/_ude_4.txt` & `chardet-5.2.0/tests/iso-8859-1/_ude_4.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-1/_ude_5.txt` & `chardet-5.2.0/tests/iso-8859-1/_ude_5.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-1/_ude_6.txt` & `chardet-5.2.0/tests/iso-8859-1/_ude_6.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-2-croatian/_ude_1.txt` & `chardet-5.2.0/tests/iso-8859-2-croatian/_ude_1.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-2-czech/_ude_1.txt` & `chardet-5.2.0/tests/iso-8859-2-czech/_ude_1.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-2-czech/_ude_2.txt` & `chardet-5.2.0/tests/iso-8859-2-czech/_ude_2.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-2-hungarian/_ude_1.txt` & `chardet-5.2.0/tests/iso-8859-2-hungarian/_ude_1.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-2-hungarian/_ude_2.txt` & `chardet-5.2.0/tests/iso-8859-2-hungarian/_ude_2.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-2-hungarian/_ude_3.txt` & `chardet-5.2.0/tests/iso-8859-2-hungarian/_ude_3.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-2-hungarian/auto-apro.hu.xml` & `chardet-5.2.0/tests/iso-8859-2-hungarian/auto-apro.hu.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-2-hungarian/cigartower.hu.xml` & `chardet-5.2.0/tests/iso-8859-2-hungarian/cigartower.hu.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-2-hungarian/escience.hu.xml` & `chardet-5.2.0/tests/iso-8859-2-hungarian/escience.hu.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-2-hungarian/hirtv.hu.xml` & `chardet-5.2.0/tests/iso-8859-2-hungarian/hirtv.hu.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-2-hungarian/honositomuhely.hu.xml` & `chardet-5.2.0/tests/iso-8859-2-hungarian/honositomuhely.hu.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-2-hungarian/saraspatak.hu.xml` & `chardet-5.2.0/tests/iso-8859-2-hungarian/saraspatak.hu.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-2-hungarian/shamalt.uw.hu.mk.xml` & `chardet-5.2.0/tests/iso-8859-2-hungarian/shamalt.uw.hu.mk.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-2-hungarian/shamalt.uw.hu.mr.xml` & `chardet-5.2.0/tests/iso-8859-2-hungarian/shamalt.uw.hu.mr.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-2-hungarian/shamalt.uw.hu.mv.xml` & `chardet-5.2.0/tests/iso-8859-2-hungarian/shamalt.uw.hu.mv.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-2-hungarian/shamalt.uw.hu.xml` & `chardet-5.2.0/tests/iso-8859-2-hungarian/shamalt.uw.hu.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-2-hungarian/ugyanmar.blogspot.com.xml` & `chardet-5.2.0/tests/iso-8859-2-hungarian/ugyanmar.blogspot.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-2-polish/_ude_1.txt` & `chardet-5.2.0/tests/iso-8859-2-polish/_ude_1.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-2-slovak/_ude_1.txt` & `chardet-5.2.0/tests/iso-8859-2-slovak/_ude_1.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-2-slovak/_ude_2.txt` & `chardet-5.2.0/tests/iso-8859-2-slovak/_ude_2.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-2-slovene/_ude_1.txt` & `chardet-5.2.0/tests/iso-8859-2-slovene/_ude_1.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-5-bulgarian/aero-bg.com.xml` & `chardet-5.2.0/tests/iso-8859-5-bulgarian/aero-bg.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-5-bulgarian/bbc.co.uk.popshow.xml` & `chardet-5.2.0/tests/iso-8859-5-bulgarian/bbc.co.uk.popshow.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-5-bulgarian/bpm.cult.bg.2.xml` & `chardet-5.2.0/tests/iso-8859-5-bulgarian/bpm.cult.bg.2.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-5-bulgarian/bpm.cult.bg.4.xml` & `chardet-5.2.0/tests/iso-8859-5-bulgarian/bpm.cult.bg.4.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-5-bulgarian/bpm.cult.bg.9.xml` & `chardet-5.2.0/tests/iso-8859-5-bulgarian/bpm.cult.bg.9.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-5-bulgarian/bpm.cult.bg.medusa.4.xml` & `chardet-5.2.0/tests/iso-8859-5-bulgarian/bpm.cult.bg.medusa.4.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-5-bulgarian/bpm.cult.bg.xml` & `chardet-5.2.0/tests/iso-8859-5-bulgarian/bpm.cult.bg.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-5-bulgarian/debian.gabrovo.com.news.xml` & `chardet-5.2.0/tests/iso-8859-5-bulgarian/debian.gabrovo.com.news.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-5-bulgarian/debian.gabrovo.com.xml` & `chardet-5.2.0/tests/iso-8859-5-bulgarian/debian.gabrovo.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-5-bulgarian/doncho.net.comments.xml` & `chardet-5.2.0/tests/iso-8859-5-bulgarian/doncho.net.comments.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-5-bulgarian/ecloga.cult.bg.xml` & `chardet-5.2.0/tests/iso-8859-5-bulgarian/ecloga.cult.bg.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-5-bulgarian/ide.li.xml` & `chardet-5.2.0/tests/iso-8859-5-bulgarian/ide.li.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-5-bulgarian/linux-bg.org.xml` & `chardet-5.2.0/tests/iso-8859-5-bulgarian/linux-bg.org.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-5-russian/_chromium_ISO-8859-5_with_no_encoding_specified.html` & `chardet-5.2.0/tests/iso-8859-5-russian/_chromium_ISO-8859-5_with_no_encoding_specified.html`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-5-russian/aif.ru.health.xml` & `chardet-5.2.0/tests/iso-8859-5-russian/aif.ru.health.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-5-russian/aug32.hole.ru.xml` & `chardet-5.2.0/tests/iso-8859-5-russian/aug32.hole.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-5-russian/aviaport.ru.xml` & `chardet-5.2.0/tests/iso-8859-5-russian/aviaport.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-5-russian/blog.mlmaster.com.xml` & `chardet-5.2.0/tests/iso-8859-5-russian/blog.mlmaster.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-5-russian/forum.template-toolkit.ru.1.xml` & `chardet-5.2.0/tests/iso-8859-5-russian/forum.template-toolkit.ru.1.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-5-russian/forum.template-toolkit.ru.4.xml` & `chardet-5.2.0/tests/iso-8859-5-russian/forum.template-toolkit.ru.4.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-5-russian/forum.template-toolkit.ru.6.xml` & `chardet-5.2.0/tests/iso-8859-5-russian/forum.template-toolkit.ru.6.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-5-russian/forum.template-toolkit.ru.8.xml` & `chardet-5.2.0/tests/iso-8859-5-russian/forum.template-toolkit.ru.8.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-5-russian/forum.template-toolkit.ru.9.xml` & `chardet-5.2.0/tests/iso-8859-5-russian/forum.template-toolkit.ru.9.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-5-russian/greek.ru.xml` & `chardet-5.2.0/tests/iso-8859-5-russian/greek.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-5-russian/intertat.ru.xml` & `chardet-5.2.0/tests/iso-8859-5-russian/intertat.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-5-russian/janulalife.blogspot.com.xml` & `chardet-5.2.0/tests/iso-8859-5-russian/janulalife.blogspot.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-5-russian/kapranoff.ru.xml` & `chardet-5.2.0/tests/iso-8859-5-russian/kapranoff.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-5-russian/money.rin.ru.xml` & `chardet-5.2.0/tests/iso-8859-5-russian/money.rin.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-5-russian/music.peeps.ru.xml` & `chardet-5.2.0/tests/iso-8859-5-russian/music.peeps.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-5-russian/newsru.com.xml` & `chardet-5.2.0/tests/iso-8859-5-russian/newsru.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-5-russian/susu.ac.ru.xml` & `chardet-5.2.0/tests/iso-8859-5-russian/susu.ac.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-6-arabic/_chromium_ISO-8859-6_with_no_encoding_specified.html` & `chardet-5.2.0/tests/iso-8859-6-arabic/_chromium_ISO-8859-6_with_no_encoding_specified.html`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-7-greek/_ude_1.txt` & `chardet-5.2.0/tests/iso-8859-7-greek/_ude_1.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-7-greek/_ude_2.txt` & `chardet-5.2.0/tests/iso-8859-7-greek/_ude_2.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-7-greek/_ude_3.txt` & `chardet-5.2.0/tests/iso-8859-7-greek/_ude_3.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-7-greek/_ude_greek.txt` & `chardet-5.2.0/tests/iso-8859-7-greek/_ude_greek.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-7-greek/disabled.gr.xml` & `chardet-5.2.0/tests/iso-8859-7-greek/disabled.gr.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-7-greek/hotstation.gr.xml` & `chardet-5.2.0/tests/iso-8859-7-greek/hotstation.gr.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-7-greek/naftemporiki.gr.bus.xml` & `chardet-5.2.0/tests/iso-8859-7-greek/naftemporiki.gr.bus.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-7-greek/naftemporiki.gr.cmm.xml` & `chardet-5.2.0/tests/iso-8859-7-greek/naftemporiki.gr.cmm.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-7-greek/naftemporiki.gr.fin.xml` & `chardet-5.2.0/tests/iso-8859-7-greek/naftemporiki.gr.fin.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-7-greek/naftemporiki.gr.mrk.xml` & `chardet-5.2.0/tests/iso-8859-7-greek/naftemporiki.gr.mrk.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-7-greek/naftemporiki.gr.mrt.xml` & `chardet-5.2.0/tests/iso-8859-7-greek/naftemporiki.gr.mrt.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-7-greek/naftemporiki.gr.spo.xml` & `chardet-5.2.0/tests/iso-8859-7-greek/naftemporiki.gr.spo.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-7-greek/naftemporiki.gr.wld.xml` & `chardet-5.2.0/tests/iso-8859-7-greek/naftemporiki.gr.wld.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-9-turkish/_ude_1.txt` & `chardet-5.2.0/tests/iso-8859-9-turkish/_ude_1.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-9-turkish/_ude_2.txt` & `chardet-5.2.0/tests/iso-8859-9-turkish/_ude_2.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-9-turkish/divxplanet.com.xml` & `chardet-5.2.0/tests/iso-8859-9-turkish/divxplanet.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-9-turkish/subtitle.srt` & `chardet-5.2.0/tests/iso-8859-9-turkish/subtitle.srt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/iso-8859-9-turkish/wikitop_tr_ISO-8859-9.txt` & `chardet-5.2.0/tests/iso-8859-9-turkish/wikitop_tr_ISO-8859-9.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/utf-8/_chromium_UTF-8_with_no_encoding_specified.html` & `chardet-5.2.0/tests/utf-8/_chromium_UTF-8_with_no_encoding_specified.html`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/utf-8/_mozilla_bug426271_text-utf-8.html` & `chardet-5.2.0/tests/utf-8/_mozilla_bug426271_text-utf-8.html`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/utf-8/_ude_1.txt` & `chardet-5.2.0/tests/utf-8/_ude_1.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/utf-8/_ude_2.txt` & `chardet-5.2.0/tests/utf-8/_ude_2.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/utf-8/_ude_greek.txt` & `chardet-5.2.0/tests/utf-8/_ude_greek.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/utf-8/_ude_he1.txt` & `chardet-5.2.0/tests/utf-8/_ude_he1.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/utf-8/_ude_he2.txt` & `chardet-5.2.0/tests/utf-8/_ude_he2.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/utf-8/_ude_he3.txt` & `chardet-5.2.0/tests/utf-8/_ude_he3.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/utf-8/_ude_russian.txt` & `chardet-5.2.0/tests/utf-8/_ude_russian.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/utf-8/anitabee.blogspot.com.xml` & `chardet-5.2.0/tests/utf-8/anitabee.blogspot.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/utf-8/balatonblog.typepad.com.xml` & `chardet-5.2.0/tests/utf-8/balatonblog.typepad.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/utf-8/boobooo.blogspot.com.xml` & `chardet-5.2.0/tests/utf-8/boobooo.blogspot.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/utf-8/linuxbox.hu.xml` & `chardet-5.2.0/tests/utf-8/linuxbox.hu.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/utf-8/pihgy.hu.xml` & `chardet-5.2.0/tests/utf-8/pihgy.hu.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/utf-8/weblabor.hu.2.xml` & `chardet-5.2.0/tests/utf-8/weblabor.hu.2.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/utf-8/weblabor.hu.xml` & `chardet-5.2.0/tests/utf-8/weblabor.hu.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/utf-8-sig/_ude_4.txt` & `chardet-5.2.0/tests/utf-8-sig/_ude_4.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/utf-8-sig/bom-utf-8.srt` & `chardet-5.2.0/tests/utf-8-sig/bom-utf-8.srt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1250-croatian/_ude_1.txt` & `chardet-5.2.0/tests/windows-1250-croatian/_ude_1.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1250-czech/_ude_1.txt` & `chardet-5.2.0/tests/windows-1250-czech/_ude_1.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1250-czech/_ude_2.txt` & `chardet-5.2.0/tests/windows-1250-czech/_ude_2.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1250-hungarian/_ude_1.txt` & `chardet-5.2.0/tests/windows-1250-hungarian/_ude_1.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1250-hungarian/_ude_2.txt` & `chardet-5.2.0/tests/windows-1250-hungarian/_ude_2.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1250-hungarian/_ude_3.txt` & `chardet-5.2.0/tests/windows-1250-hungarian/_ude_3.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1250-hungarian/bbc.co.uk.hu.forum.xml` & `chardet-5.2.0/tests/windows-1250-hungarian/bbc.co.uk.hu.forum.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1250-hungarian/bbc.co.uk.hu.learningenglish.xml` & `chardet-5.2.0/tests/windows-1250-hungarian/bbc.co.uk.hu.learningenglish.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1250-hungarian/bbc.co.uk.hu.pressreview.xml` & `chardet-5.2.0/tests/windows-1250-hungarian/bbc.co.uk.hu.pressreview.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1250-hungarian/bbc.co.uk.hu.xml` & `chardet-5.2.0/tests/windows-1250-hungarian/bbc.co.uk.hu.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1250-hungarian/objektivhir.hu.xml` & `chardet-5.2.0/tests/windows-1250-hungarian/objektivhir.hu.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1250-hungarian/torokorszag.blogspot.com.xml` & `chardet-5.2.0/tests/windows-1250-hungarian/torokorszag.blogspot.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1250-polish/_ude_1.txt` & `chardet-5.2.0/tests/windows-1250-polish/_ude_1.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1250-romanian/_ude_1.txt` & `chardet-5.2.0/tests/windows-1250-romanian/_ude_1.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1250-slovak/_ude_1.txt` & `chardet-5.2.0/tests/windows-1250-slovak/_ude_1.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1250-slovak/_ude_2.txt` & `chardet-5.2.0/tests/windows-1250-slovak/_ude_2.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1250-slovak/_ude_3.txt` & `chardet-5.2.0/tests/windows-1250-slovak/_ude_3.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1250-slovene/_ude_1.txt` & `chardet-5.2.0/tests/windows-1250-slovene/_ude_1.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1251-bulgarian/bbc.co.uk.popshow.xml` & `chardet-5.2.0/tests/windows-1251-bulgarian/bbc.co.uk.popshow.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1251-bulgarian/bpm.cult.bg.2.xml` & `chardet-5.2.0/tests/windows-1251-bulgarian/bpm.cult.bg.2.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1251-bulgarian/bpm.cult.bg.3.xml` & `chardet-5.2.0/tests/windows-1251-bulgarian/bpm.cult.bg.3.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1251-bulgarian/bpm.cult.bg.4.xml` & `chardet-5.2.0/tests/windows-1251-bulgarian/bpm.cult.bg.4.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1251-bulgarian/bpm.cult.bg.9.xml` & `chardet-5.2.0/tests/windows-1251-bulgarian/bpm.cult.bg.9.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1251-bulgarian/bpm.cult.bg.medusa.4.xml` & `chardet-5.2.0/tests/windows-1251-bulgarian/bpm.cult.bg.medusa.4.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1251-bulgarian/bpm.cult.bg.xml` & `chardet-5.2.0/tests/windows-1251-bulgarian/bpm.cult.bg.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1251-bulgarian/debian.gabrovo.com.news.xml` & `chardet-5.2.0/tests/windows-1251-bulgarian/debian.gabrovo.com.news.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1251-bulgarian/debian.gabrovo.com.xml` & `chardet-5.2.0/tests/windows-1251-bulgarian/debian.gabrovo.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1251-bulgarian/doncho.net.comments.xml` & `chardet-5.2.0/tests/windows-1251-bulgarian/doncho.net.comments.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1251-bulgarian/doncho.net.xml` & `chardet-5.2.0/tests/windows-1251-bulgarian/doncho.net.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1251-bulgarian/ecloga.cult.bg.xml` & `chardet-5.2.0/tests/windows-1251-bulgarian/ecloga.cult.bg.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1251-bulgarian/ide.li.xml` & `chardet-5.2.0/tests/windows-1251-bulgarian/ide.li.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1251-bulgarian/informator.org.xml` & `chardet-5.2.0/tests/windows-1251-bulgarian/informator.org.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1251-bulgarian/linux-bg.org.xml` & `chardet-5.2.0/tests/windows-1251-bulgarian/linux-bg.org.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1251-bulgarian/rinennor.org.xml` & `chardet-5.2.0/tests/windows-1251-bulgarian/rinennor.org.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1251-russian/_chromium_windows-1251_with_no_encoding_specified.html` & `chardet-5.2.0/tests/windows-1251-russian/_chromium_windows-1251_with_no_encoding_specified.html`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1251-russian/_ude_1.txt` & `chardet-5.2.0/tests/windows-1251-russian/_ude_1.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1251-russian/aif.ru.health.xml` & `chardet-5.2.0/tests/windows-1251-russian/aif.ru.health.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1251-russian/anthropology.ru.xml` & `chardet-5.2.0/tests/windows-1251-russian/anthropology.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1251-russian/aug32.hole.ru.xml` & `chardet-5.2.0/tests/windows-1251-russian/aug32.hole.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1251-russian/aviaport.ru.xml` & `chardet-5.2.0/tests/windows-1251-russian/aviaport.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1251-russian/blog.mlmaster.com.xml` & `chardet-5.2.0/tests/windows-1251-russian/blog.mlmaster.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1251-russian/forum.template-toolkit.ru.1.xml` & `chardet-5.2.0/tests/windows-1251-russian/forum.template-toolkit.ru.1.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1251-russian/forum.template-toolkit.ru.4.xml` & `chardet-5.2.0/tests/windows-1251-russian/forum.template-toolkit.ru.4.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1251-russian/forum.template-toolkit.ru.6.xml` & `chardet-5.2.0/tests/windows-1251-russian/forum.template-toolkit.ru.6.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1251-russian/forum.template-toolkit.ru.8.xml` & `chardet-5.2.0/tests/windows-1251-russian/forum.template-toolkit.ru.8.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1251-russian/forum.template-toolkit.ru.9.xml` & `chardet-5.2.0/tests/windows-1251-russian/forum.template-toolkit.ru.9.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1251-russian/greek.ru.xml` & `chardet-5.2.0/tests/windows-1251-russian/greek.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1251-russian/intertat.ru.xml` & `chardet-5.2.0/tests/windows-1251-russian/intertat.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1251-russian/janulalife.blogspot.com.xml` & `chardet-5.2.0/tests/windows-1251-russian/janulalife.blogspot.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1251-russian/kapranoff.ru.xml` & `chardet-5.2.0/tests/windows-1251-russian/kapranoff.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1251-russian/money.rin.ru.xml` & `chardet-5.2.0/tests/windows-1251-russian/money.rin.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1251-russian/music.peeps.ru.xml` & `chardet-5.2.0/tests/windows-1251-russian/music.peeps.ru.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1251-russian/newsru.com.xml` & `chardet-5.2.0/tests/windows-1251-russian/newsru.com.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1252/_mozilla_bug421271_text.html` & `chardet-5.2.0/tests/windows-1252/_mozilla_bug421271_text.html`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1252/_ude_1.txt` & `chardet-5.2.0/tests/windows-1252/_ude_1.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1252/_ude_2.txt` & `chardet-5.2.0/tests/windows-1252/_ude_2.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1254-turkish/_ude_1.txt` & `chardet-5.2.0/tests/windows-1254-turkish/_ude_1.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1255-hebrew/_chromium_ISO-8859-8_with_no_encoding_specified.html` & `chardet-5.2.0/tests/windows-1255-hebrew/_chromium_ISO-8859-8_with_no_encoding_specified.html`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1255-hebrew/_chromium_windows-1255_with_no_encoding_specified.html` & `chardet-5.2.0/tests/windows-1255-hebrew/_chromium_windows-1255_with_no_encoding_specified.html`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1255-hebrew/_ude_he1.txt` & `chardet-5.2.0/tests/windows-1255-hebrew/_ude_he1.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1255-hebrew/_ude_he2.txt` & `chardet-5.2.0/tests/windows-1255-hebrew/_ude_he2.txt`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1255-hebrew/carshops.co.il.xml` & `chardet-5.2.0/tests/windows-1255-hebrew/carshops.co.il.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1255-hebrew/exego.net.2.xml` & `chardet-5.2.0/tests/windows-1255-hebrew/exego.net.2.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1255-hebrew/hagada.org.il.xml` & `chardet-5.2.0/tests/windows-1255-hebrew/hagada.org.il.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1255-hebrew/halemo.net.edoar.xml` & `chardet-5.2.0/tests/windows-1255-hebrew/halemo.net.edoar.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1255-hebrew/hevra.org.il.xml` & `chardet-5.2.0/tests/windows-1255-hebrew/hevra.org.il.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1255-hebrew/hydepark.hevre.co.il.7957.xml` & `chardet-5.2.0/tests/windows-1255-hebrew/hydepark.hevre.co.il.7957.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1255-hebrew/info.org.il.xml` & `chardet-5.2.0/tests/windows-1255-hebrew/info.org.il.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1255-hebrew/infomed.co.il.xml` & `chardet-5.2.0/tests/windows-1255-hebrew/infomed.co.il.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1255-hebrew/law.co.il.xml` & `chardet-5.2.0/tests/windows-1255-hebrew/law.co.il.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1255-hebrew/maakav.org.xml` & `chardet-5.2.0/tests/windows-1255-hebrew/maakav.org.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1255-hebrew/neviim.net.xml` & `chardet-5.2.0/tests/windows-1255-hebrew/neviim.net.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1255-hebrew/notes.co.il.50.xml` & `chardet-5.2.0/tests/windows-1255-hebrew/notes.co.il.50.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1255-hebrew/notes.co.il.6.xml` & `chardet-5.2.0/tests/windows-1255-hebrew/notes.co.il.6.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1255-hebrew/notes.co.il.7.xml` & `chardet-5.2.0/tests/windows-1255-hebrew/notes.co.il.7.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1255-hebrew/notes.co.il.8.xml` & `chardet-5.2.0/tests/windows-1255-hebrew/notes.co.il.8.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1255-hebrew/pcplus.co.il.xml` & `chardet-5.2.0/tests/windows-1255-hebrew/pcplus.co.il.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1255-hebrew/sharks.co.il.xml` & `chardet-5.2.0/tests/windows-1255-hebrew/sharks.co.il.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1255-hebrew/whatsup.org.il.xml` & `chardet-5.2.0/tests/windows-1255-hebrew/whatsup.org.il.xml`

 * *Files identical despite different names*

### Comparing `chardet-5.1.0/tests/windows-1256-arabic/_chromium_windows-1256_with_no_encoding_specified.html` & `chardet-5.2.0/tests/windows-1256-arabic/_chromium_windows-1256_with_no_encoding_specified.html`

 * *Files identical despite different names*

