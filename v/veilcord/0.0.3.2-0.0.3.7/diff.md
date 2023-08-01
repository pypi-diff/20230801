# Comparing `tmp/veilcord-0.0.3.2.tar.gz` & `tmp/veilcord-0.0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veilcord-0.0.3.2.tar", last modified: Fri Jul 28 22:22:41 2023, max compression
+gzip compressed data, was "veilcord-0.0.3.7.tar", last modified: Tue Aug  1 16:02:44 2023, max compression
```

## Comparing `veilcord-0.0.3.2.tar` & `veilcord-0.0.3.7.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 22:22:41.517614 veilcord-0.0.3.2/
--rw-rw-rw-   0        0        0     1085 2023-05-20 20:15:11.000000 veilcord-0.0.3.2/LICENSE
--rw-rw-rw-   0        0        0     3462 2023-07-28 22:22:41.516615 veilcord-0.0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     2242 2023-07-28 22:11:38.000000 veilcord-0.0.3.2/README.md
--rw-rw-rw-   0        0        0       86 2023-05-08 02:01:12.000000 veilcord-0.0.3.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-28 22:22:41.517614 veilcord-0.0.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1667 2023-07-28 20:52:56.000000 veilcord-0.0.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-28 22:22:41.501150 veilcord-0.0.3.2/veilcord/
--rw-rw-rw-   0        0        0     9215 2023-07-28 22:12:14.000000 veilcord-0.0.3.2/veilcord/__init__.py
--rw-rw-rw-   0        0        0    11729 2023-07-28 22:20:51.000000 veilcord-0.0.3.2/veilcord/__main__.py
--rw-rw-rw-   0        0        0     5313 2023-07-28 22:15:32.000000 veilcord-0.0.3.2/veilcord/__session__.py
-drwxrwxrwx   0        0        0        0 2023-07-28 22:22:41.516615 veilcord-0.0.3.2/veilcord.egg-info/
--rw-rw-rw-   0        0        0     3462 2023-07-28 22:22:41.000000 veilcord-0.0.3.2/veilcord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-07-28 22:22:41.000000 veilcord-0.0.3.2/veilcord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 22:22:41.000000 veilcord-0.0.3.2/veilcord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-07-28 22:22:41.000000 veilcord-0.0.3.2/veilcord.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-28 22:22:41.000000 veilcord-0.0.3.2/veilcord.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 16:02:44.742056 veilcord-0.0.3.7/
+-rw-rw-rw-   0        0        0     1085 2023-05-20 20:15:11.000000 veilcord-0.0.3.7/LICENSE
+-rw-rw-rw-   0        0        0     4131 2023-08-01 16:02:44.742056 veilcord-0.0.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2864 2023-08-01 05:18:56.000000 veilcord-0.0.3.7/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-08 02:01:12.000000 veilcord-0.0.3.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-01 16:02:44.742056 veilcord-0.0.3.7/setup.cfg
+-rw-rw-rw-   0        0        0     1713 2023-08-01 05:09:15.000000 veilcord-0.0.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 16:02:44.725204 veilcord-0.0.3.7/veilcord/
+-rw-rw-rw-   0        0        0     3952 2023-08-01 03:34:58.000000 veilcord-0.0.3.7/veilcord/__extra__.py
+-rw-rw-rw-   0        0        0     9243 2023-08-01 05:09:12.000000 veilcord-0.0.3.7/veilcord/__init__.py
+-rw-rw-rw-   0        0        0    12694 2023-08-01 03:49:27.000000 veilcord-0.0.3.7/veilcord/__main__.py
+-rw-rw-rw-   0        0        0     5504 2023-08-01 03:13:28.000000 veilcord-0.0.3.7/veilcord/__session__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 16:02:44.741060 veilcord-0.0.3.7/veilcord.egg-info/
+-rw-rw-rw-   0        0        0     4131 2023-08-01 16:02:44.000000 veilcord-0.0.3.7/veilcord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2023-08-01 16:02:44.000000 veilcord-0.0.3.7/veilcord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 16:02:44.000000 veilcord-0.0.3.7/veilcord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-08-01 16:02:44.000000 veilcord-0.0.3.7/veilcord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-01 16:02:44.000000 veilcord-0.0.3.7/veilcord.egg-info/top_level.txt
```

### Comparing `veilcord-0.0.3.2/LICENSE` & `veilcord-0.0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `veilcord-0.0.3.2/PKG-INFO` & `veilcord-0.0.3.7/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,217 +1,179 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310d 0a4e 616d 653a 2076 6569  : 2.1..Name: vei
-00000020: 6c63 6f72 640d 0a56 6572 7369 6f6e 3a20  lcord..Version: 
-00000030: 302e 302e 332e 320d 0a53 756d 6d61 7279  0.0.3.2..Summary
-00000040: 3a20 5665 696c 436f 7264 202f 2f20 4069  : VeilCord // @i
-00000050: 6d76 6173 740d 0a48 6f6d 652d 7061 6765  mvast..Home-page
-00000060: 3a20 6874 7470 3a2f 2f70 7970 692e 7079  : http://pypi.py
-00000070: 7468 6f6e 2e6f 7267 2f70 7970 692f 7665  thon.org/pypi/ve
-00000080: 696c 636f 7264 0d0a 4175 7468 6f72 3a20  ilcord..Author: 
-00000090: 4069 6d76 6173 740d 0a41 7574 686f 722d  @imvast..Author-
-000000a0: 656d 6169 6c3a 2064 6576 4076 6173 742e  email: dev@vast.
-000000b0: 7368 0d0a 4c69 6365 6e73 653a 204d 4954  sh..License: MIT
-000000c0: 0d0a 5072 6f6a 6563 742d 5552 4c3a 2048  ..Project-URL: H
-000000d0: 6f6d 6570 6167 652c 2068 7474 7073 3a2f  omepage, https:/
-000000e0: 2f67 6974 6875 622e 636f 6d2f 696d 7661  /github.com/imva
-000000f0: 7374 2f76 6569 6c63 6f72 640d 0a50 726f  st/veilcord..Pro
-00000100: 6a65 6374 2d55 524c 3a20 5375 6767 6573  ject-URL: Sugges
-00000110: 7469 6f6e 732c 2068 7474 7073 3a2f 2f67  tions, https://g
-00000120: 6974 6875 622e 636f 6d2f 696d 7661 7374  ithub.com/imvast
-00000130: 2f76 6569 6c63 6f72 642f 6973 7375 6573  /veilcord/issues
-00000140: 0d0a 436c 6173 7369 6669 6572 3a20 4465  ..Classifier: De
-00000150: 7665 6c6f 706d 656e 7420 5374 6174 7573  velopment Status
-00000160: 203a 3a20 3320 2d20 416c 7068 610d 0a43   :: 3 - Alpha..C
-00000170: 6c61 7373 6966 6965 723a 2049 6e74 656e  lassifier: Inten
-00000180: 6465 6420 4175 6469 656e 6365 203a 3a20  ded Audience :: 
-00000190: 4465 7665 6c6f 7065 7273 0d0a 436c 6173  Developers..Clas
-000001a0: 7369 6669 6572 3a20 4c69 6365 6e73 6520  sifier: License 
-000001b0: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
-000001c0: 3a3a 204d 4954 204c 6963 656e 7365 0d0a  :: MIT License..
-000001d0: 436c 6173 7369 6669 6572 3a20 4e61 7475  Classifier: Natu
-000001e0: 7261 6c20 4c61 6e67 7561 6765 203a 3a20  ral Language :: 
-000001f0: 456e 676c 6973 680d 0a43 6c61 7373 6966  English..Classif
-00000200: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-00000210: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000220: 686f 6e0d 0a43 6c61 7373 6966 6965 723a  hon..Classifier:
-00000230: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-00000240: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000250: 3a3a 2033 0d0a 436c 6173 7369 6669 6572  :: 3..Classifier
-00000260: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-00000270: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000280: 203a 3a20 332e 380d 0a43 6c61 7373 6966   :: 3.8..Classif
-00000290: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-000002a0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-000002b0: 686f 6e20 3a3a 2033 2e39 0d0a 436c 6173  hon :: 3.9..Clas
-000002c0: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-000002d0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-000002e0: 5079 7468 6f6e 203a 3a20 332e 3130 0d0a  Python :: 3.10..
-000002f0: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
-00000300: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000310: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000320: 3131 0d0a 436c 6173 7369 6669 6572 3a20  11..Classifier: 
-00000330: 546f 7069 6320 3a3a 2053 6369 656e 7469  Topic :: Scienti
-00000340: 6669 632f 456e 6769 6e65 6572 696e 670d  fic/Engineering.
-00000350: 0a43 6c61 7373 6966 6965 723a 2054 6f70  .Classifier: Top
-00000360: 6963 203a 3a20 5363 6965 6e74 6966 6963  ic :: Scientific
-00000370: 2f45 6e67 696e 6565 7269 6e67 203a 3a20  /Engineering :: 
-00000380: 496e 666f 726d 6174 696f 6e20 416e 616c  Information Anal
-00000390: 7973 6973 0d0a 436c 6173 7369 6669 6572  ysis..Classifier
-000003a0: 3a20 546f 7069 6320 3a3a 2053 6369 656e  : Topic :: Scien
-000003b0: 7469 6669 632f 456e 6769 6e65 6572 696e  tific/Engineerin
-000003c0: 6720 3a3a 204d 6174 6865 6d61 7469 6373  g :: Mathematics
-000003d0: 0d0a 436c 6173 7369 6669 6572 3a20 546f  ..Classifier: To
-000003e0: 7069 6320 3a3a 2053 6369 656e 7469 6669  pic :: Scientifi
-000003f0: 632f 456e 6769 6e65 6572 696e 6720 3a3a  c/Engineering ::
-00000400: 2056 6973 7561 6c69 7a61 7469 6f6e 0d0a   Visualization..
-00000410: 436c 6173 7369 6669 6572 3a20 546f 7069  Classifier: Topi
-00000420: 6320 3a3a 2053 6f66 7477 6172 6520 4465  c :: Software De
-00000430: 7665 6c6f 706d 656e 7420 3a3a 204c 6962  velopment :: Lib
-00000440: 7261 7269 6573 0d0a 436c 6173 7369 6669  raries..Classifi
-00000450: 6572 3a20 546f 7069 6320 3a3a 2055 7469  er: Topic :: Uti
-00000460: 6c69 7469 6573 0d0a 5265 7175 6972 6573  lities..Requires
-00000470: 2d50 7974 686f 6e3a 207e 3d33 2e38 0d0a  -Python: ~=3.8..
-00000480: 4465 7363 7269 7074 696f 6e2d 436f 6e74  Description-Cont
-00000490: 656e 742d 5479 7065 3a20 7465 7874 2f6d  ent-Type: text/m
-000004a0: 6172 6b64 6f77 6e0d 0a4c 6963 656e 7365  arkdown..License
-000004b0: 2d46 696c 653a 204c 4943 454e 5345 0d0a  -File: LICENSE..
-000004c0: 0d0a 2320 5665 696c 436f 7264 2e0d 0a3c  ..# VeilCord...<
-000004d0: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-000004e0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-000004f0: 7079 7069 2f76 2f76 6569 6c63 6f72 643f  pypi/v/veilcord?
-00000500: 7374 796c 653d 666f 722d 7468 652d 6261  style=for-the-ba
-00000510: 6467 6526 6c6f 676f 3d70 7974 686f 6e22  dge&logo=python"
-00000520: 3e0d 0a3c 696d 6720 616c 743d 2266 6f6c  >..<img alt="fol
-00000530: 6c6f 7765 7273 2220 7372 633d 2268 7474  lowers" src="htt
-00000540: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000550: 2e69 6f2f 6769 7468 7562 2f66 6f6c 6c6f  .io/github/follo
-00000560: 7765 7273 2f69 6d76 6173 743f 636f 6c6f  wers/imvast?colo
-00000570: 723d 6634 3239 6666 2673 7479 6c65 3d66  r=f429ff&style=f
-00000580: 6f72 2d74 6865 2d62 6164 6765 266c 6f67  or-the-badge&log
-00000590: 6f3d 6769 7468 7562 266c 6162 656c 3d46  o=github&label=F
-000005a0: 6f6c 6c6f 7722 2f3e 0d0a 0d0a 6060 606c  ollow"/>....```l
-000005b0: 6573 730d 0a20 2020 2020 2020 2020 2020  ess..           
-000005c0: 2020 203e 2043 7573 746f 6d20 4469 7363     > Custom Disc
-000005d0: 6f72 6420 546f 6f6c 7320 476f 696e 6720  ord Tools Going 
-000005e0: 546f 2042 6520 5573 6564 2046 6f72 204d  To Be Used For M
-000005f0: 7920 5072 6f6a 6563 7473 0d0a 2020 2020  y Projects..    
-00000600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000610: 416e 6420 4176 6169 6c61 626c 6520 546f  And Available To
-00000620: 2041 6e79 6f6e 6520 456c 7365 2057 686f   Anyone Else Who
-00000630: 2057 616e 7473 2054 6f20 5573 6520 3c0d   Wants To Use <.
-00000640: 0a60 6060 0d0a 0d0a 2d2d 2d0d 0a0d 0a23  .```....---....#
-00000650: 2323 2049 6e73 7461 6c6c 6174 696f 6e0d  ## Installation.
-00000660: 0a60 6060 7961 6d6c 0d0a 2120 7061 636b  .```yaml..! pack
-00000670: 6167 6520 4e4f 5420 4655 4c4c 5920 6176  age NOT FULLY av
-00000680: 6169 6c61 626c 6520 666f 7220 6e6f 6e2d  ailable for non-
-00000690: 7065 7273 6f6e 616c 2075 7365 2021 0d0a  personal use !..
-000006a0: 6060 600d 0a0d 0a23 2323 2045 7861 6d70  ```....### Examp
-000006b0: 6c65 2055 7361 6765 0d0a 6060 6070 790d  le Usage..```py.
-000006c0: 0a66 726f 6d20 7665 696c 636f 7264 2069  .from veilcord i
-000006d0: 6d70 6f72 7420 5665 696c 436f 7264 0d0a  mport VeilCord..
-000006e0: 0d0a 7665 696c 636f 7264 203d 2056 6569  ..veilcord = Vei
-000006f0: 6c43 6f72 6428 0d0a 2020 2020 7365 7373  lCord(..    sess
-00000700: 696f 6e20 3d20 4e6f 6e65 2c20 2320 666f  ion = None, # fo
-00000710: 7220 6375 7374 6f6d 2074 6c73 5f63 6c69  r custom tls_cli
-00000720: 656e 7420 7365 7373 696f 6e73 0d0a 2020  ent sessions..  
-00000730: 2020 6465 7669 6365 5f74 7970 6520 3d20    device_type = 
-00000740: 2262 726f 7773 6572 222c 2023 2074 7970  "browser", # typ
-00000750: 6573 203a 2062 726f 7773 6572 2c20 6d6f  es : browser, mo
-00000760: 6269 6c65 2c20 6170 700d 0a20 2020 2075  bile, app..    u
-00000770: 7365 725f 6167 656e 7420 3d20 4e6f 6e65  ser_agent = None
-00000780: 2023 2066 6f72 2063 7573 746f 6d20 7573   # for custom us
-00000790: 6572 2061 6765 6e74 0d0a 290d 0a0d 0a23  er agent..)....#
-000007a0: 2047 4554 5449 4e47 2058 2d53 7570 6572   GETTING X-Super
-000007b0: 2d50 726f 7065 7274 6965 730d 0a78 7375  -Properties..xsu
-000007c0: 7020 3d20 7665 696c 636f 7264 2e67 656e  p = veilcord.gen
-000007d0: 6572 6174 6558 5072 6f70 2829 0d0a 7072  erateXProp()..pr
-000007e0: 696e 7428 6622 282b 2920 5265 7472 6965  int(f"(+) Retrie
-000007f0: 7665 6420 5853 7570 3a20 7b78 7375 707d  ved XSup: {xsup}
-00000800: 2229 0d0a 0d0a 0d0a 2320 4745 5454 494e  ")......# GETTIN
-00000810: 4720 414c 4c20 5448 4520 434f 4f4b 4945  G ALL THE COOKIE
-00000820: 5320 414e 4420 4649 4e47 4552 5052 494e  S AND FINGERPRIN
-00000830: 540d 0a66 702c 2063 6f6f 6b69 6573 203d  T..fp, cookies =
-00000840: 2076 6569 6c63 6f72 642e 6765 7446 696e   veilcord.getFin
-00000850: 6765 7270 7269 6e74 2878 7375 702c 2063  gerprint(xsup, c
-00000860: 6f6f 6b69 6554 7970 653d 226a 736f 6e22  ookieType="json"
-00000870: 290d 0a70 7269 6e74 2866 2228 2b29 2052  )..print(f"(+) R
-00000880: 6574 7269 6576 6564 2046 696e 6765 7270  etrieved Fingerp
-00000890: 7269 6e74 3a20 7b66 707d 2229 0d0a 7072  rint: {fp}")..pr
-000008a0: 696e 7428 6622 282b 2920 5265 7472 6965  int(f"(+) Retrie
-000008b0: 7665 6420 436f 6f6b 6965 733a 207b 636f  ved Cookies: {co
-000008c0: 6f6b 6965 737d 2229 0d0a 2320 7265 7475  okies}")..# retu
-000008d0: 726e 7320 6120 7365 742e 2020 5b30 5d20  rns a set.  [0] 
-000008e0: 2d20 4669 6e67 6572 7072 696e 7420 207c  - Fingerprint  |
-000008f0: 2020 5b31 5d20 2d20 434f 4f4b 4945 534a    [1] - COOKIESJ
-00000900: 4152 206f 7220 4a53 4f4e 0d0a 0d0a 0d0a  AR or JSON......
-00000910: 2320 4745 5420 5448 4520 4e45 5720 5345  # GET THE NEW SE
-00000920: 5353 494f 4e20 4944 2042 5320 207c 7c20  SSION ID BS  || 
-00000930: 7468 6973 2063 616e 2061 6c73 6f20 6265  this can also be
-00000940: 2075 7365 6420 666f 7220 7765 6273 6f63   used for websoc
-00000950: 6b65 7420 636f 6e6e 6563 7469 6f6e 2062  ket connection b
-00000960: 7574 206e 6f74 2072 6563 6f6d 6d65 6e64  ut not recommend
-00000970: 6564 2061 7320 6f66 2072 6e0d 0a73 6573  ed as of rn..ses
-00000980: 7369 6f6e 203d 2076 6569 6c63 6f72 642e  sion = veilcord.
-00000990: 6f70 656e 5365 7373 696f 6e28 290d 0a0d  openSession()...
-000009a0: 0a74 6f6b 656e 203d 2022 220d 0a73 6573  .token = ""..ses
-000009b0: 7369 6f6e 4944 203d 2076 6569 6c63 6f72  sionID = veilcor
-000009c0: 642e 6765 7453 6573 7369 6f6e 280d 0a20  d.getSession(.. 
-000009d0: 2020 2073 6573 7369 6f6e 203d 2073 6573     session = ses
-000009e0: 7369 6f6e 2c20 2320 7468 6520 7365 7373  sion, # the sess
-000009f0: 696f 6e20 7265 7475 726e 6564 2066 726f  ion returned fro
-00000a00: 6d20 7665 696c 636f 7264 2e6f 7065 6e53  m veilcord.openS
-00000a10: 6573 7369 6f6e 2829 0d0a 2020 2020 746f  ession()..    to
-00000a20: 6b65 6e20 3d20 746f 6b65 6e2c 2023 206f  ken = token, # o
-00000a30: 6276 2074 6865 2074 6f6b 656e 0d0a 2020  bv the token..  
-00000a40: 2020 6b65 6570 5f61 6c69 7665 203d 2046    keep_alive = F
-00000a50: 616c 7365 2c20 2023 206b 6565 7020 7468  alse,  # keep th
-00000a60: 6520 7365 7373 696f 6e20 616c 6976 6520  e session alive 
-00000a70: 7c20 6f6e 6c79 206e 6565 6465 6420 6966  | only needed if
-00000a80: 2075 7220 636f 6465 2069 7320 736c 6f77   ur code is slow
-00000a90: 2028 6176 672e 2073 6573 7369 6f6e 2069   (avg. session i
-00000aa0: 7320 6c69 7665 2066 6f72 207e 3430 2073  s live for ~40 s
-00000ab0: 6563 6f6e 6473 2e29 0d0a 2020 2020 7368  econds.)..    sh
-00000ac0: 6f77 5f68 6220 3d20 4661 6c73 6520 2320  ow_hb = False # 
-00000ad0: 7072 696e 7473 2077 6865 6e20 6974 2073  prints when it s
-00000ae0: 656e 6473 2074 6865 2068 6561 7274 6265  ends the heartbe
-00000af0: 6174 2061 6e64 2077 6865 6e20 7468 6520  at and when the 
-00000b00: 6e65 7874 206f 6e65 2069 730d 0a29 0d0a  next one is..)..
-00000b10: 7072 696e 7428 6622 282b 2920 476f 7420  print(f"(+) Got 
-00000b20: 5365 7373 696f 6e20 4944 3a20 7b73 6573  Session ID: {ses
-00000b30: 7369 6f6e 4944 7d22 290d 0a0d 0a23 2063  sionID}")....# c
-00000b40: 6c6f 7365 2074 6865 2073 6573 7369 6f6e  lose the session
-00000b50: 2c20 6966 206b 6565 7041 6c69 7665 2069  , if keepAlive i
-00000b60: 7320 656e 6162 6c65 642e 0d0a 2320 7665  s enabled...# ve
-00000b70: 696c 636f 7264 2e63 6c6f 7365 5365 7373  ilcord.closeSess
-00000b80: 696f 6e28 7365 7373 696f 6e29 0d0a 0d0a  ion(session)....
-00000b90: 0d0a 2323 2045 7874 7261 2043 6f6f 6c20  ..## Extra Cool 
-00000ba0: 5374 7566 660d 0a0d 0a23 2067 6574 2064  Stuff....# get d
-00000bb0: 6973 636f 7264 2062 7569 6c64 206e 756d  iscord build num
-00000bc0: 6265 720d 0a62 7569 6c64 4e75 6d20 3d20  ber..buildNum = 
-00000bd0: 5665 696c 436f 7264 2e67 6574 4275 696c  VeilCord.getBuil
-00000be0: 644e 756d 2829 0d0a 7072 696e 7428 6275  dNum()..print(bu
-00000bf0: 696c 644e 756d 290d 0a0d 0a23 202d 2d20  ildNum)....# -- 
-00000c00: 6f72 2077 6974 6820 616c 6c20 7468 6520  or with all the 
-00000c10: 6578 7472 6120 7374 6174 730d 0a0d 0a62  extra stats....b
-00000c20: 7569 6c64 4e75 6d2c 2062 7569 6c64 5453  uildNum, buildTS
-00000c30: 2c20 7572 6c2c 2074 696d 655f 7461 6b65  , url, time_take
-00000c40: 6e20 3d20 5665 696c 436f 7264 2e67 6574  n = VeilCord.get
-00000c50: 4275 696c 644e 756d 2877 6974 6853 7461  BuildNum(withSta
-00000c60: 743d 5472 7565 290d 0a70 7269 6e74 2822  t=True)..print("
-00000c70: 5552 4c3a 222c 2075 726c 290d 0a70 7269  URL:", url)..pri
-00000c80: 6e74 2822 4275 696c 6420 4e75 6d62 6572  nt("Build Number
-00000c90: 3a22 2c20 6275 696c 644e 756d 290d 0a70  :", buildNum)..p
-00000ca0: 7269 6e74 2822 4275 696c 6420 5469 6d65  rint("Build Time
-00000cb0: 7374 616d 703a 222c 2062 7569 6c64 5453  stamp:", buildTS
-00000cc0: 290d 0a70 7269 6e74 2822 456c 6170 7365  )..print("Elapse
-00000cd0: 643a 222c 2074 696d 655f 7461 6b65 6e29  d:", time_taken)
-00000ce0: 0d0a 0d0a 0d0a 6060 600d 0a0d 0a2d 2d2d  ......```....---
-00000cf0: 0d0a 0d0a 2323 202a 205b 696d 7661 7374  ....## * [imvast
-00000d00: 4064 6973 636f 7264 5d28 6874 7470 733a  @discord](https:
-00000d10: 2f2f 6469 7363 6f72 642e 636f 6d2f 7573  //discord.com/us
-00000d20: 6572 732f 3131 3138 3635 3436 3735 3839  ers/111865467589
-00000d30: 3836 3137 3839 3129 207c 205b 696d 7661  8617891) | [imva
-00000d40: 7374 4067 6974 6875 625d 2868 7474 7073  st@github](https
-00000d50: 3a2f 2f67 6974 6875 622e 636f 6d2f 696d  ://github.com/im
-00000d60: 7661 7374 2920 7c20 5b76 6173 742e 7368  vast) | [vast.sh
-00000d70: 5d28 6874 7470 733a 2f2f 7661 7374 2e73  ](https://vast.s
-00000d80: 6829 202a 0d0a                           h) *..
+00000000: 2320 5665 696c 436f 7264 2e0d 0a3c 696d  # VeilCord...<im
+00000010: 6720 7372 633d 2268 7474 7073 3a2f 2f69  g src="https://i
+00000020: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
+00000030: 7069 2f76 2f76 6569 6c63 6f72 643f 7374  pi/v/veilcord?st
+00000040: 796c 653d 666f 722d 7468 652d 6261 6467  yle=for-the-badg
+00000050: 6526 6c6f 676f 3d70 7974 686f 6e22 3e0d  e&logo=python">.
+00000060: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
+00000070: 2f2f 6769 7468 7562 2e63 6f6d 2f69 6d76  //github.com/imv
+00000080: 6173 7422 2074 6172 6765 743d 225f 626c  ast" target="_bl
+00000090: 616e 6b22 3e0d 0a20 2020 203c 696d 6720  ank">..    <img 
+000000a0: 616c 743d 2266 6f6c 6c6f 7765 7273 2220  alt="followers" 
+000000b0: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
+000000c0: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
+000000d0: 7562 2f66 6f6c 6c6f 7765 7273 2f69 6d76  ub/followers/imv
+000000e0: 6173 743f 636f 6c6f 723d 6634 3239 6666  ast?color=f429ff
+000000f0: 2673 7479 6c65 3d66 6f72 2d74 6865 2d62  &style=for-the-b
+00000100: 6164 6765 266c 6f67 6f3d 6769 7468 7562  adge&logo=github
+00000110: 266c 6162 656c 3d46 6f6c 6c6f 7722 2f3e  &label=Follow"/>
+00000120: 0d0a 3c2f 613e 0d0a 0d0a 6060 606c 6573  ..</a>....```les
+00000130: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
+00000140: 2020 203e 2043 7573 746f 6d20 4469 7363     > Custom Disc
+00000150: 6f72 6420 546f 6f6c 7320 476f 696e 6720  ord Tools Going 
+00000160: 546f 2042 6520 5573 6564 2046 6f72 204d  To Be Used For M
+00000170: 7920 5072 6f6a 6563 7473 0d0a 2020 2020  y Projects..    
+00000180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000190: 2020 416e 6420 4176 6169 6c61 626c 6520    And Available 
+000001a0: 546f 2041 6e79 6f6e 6520 456c 7365 2057  To Anyone Else W
+000001b0: 686f 2057 616e 7473 2054 6f20 5573 6520  ho Wants To Use 
+000001c0: 3c0d 0a60 6060 0d0a 0d0a 0d0a 2d2d 2d0d  <..```......---.
+000001d0: 0a0d 0a23 2323 2049 6e73 7461 6c6c 6174  ...### Installat
+000001e0: 696f 6e0d 0a60 6060 7961 6d6c 0d0a 2120  ion..```yaml..! 
+000001f0: 7061 636b 6167 6520 4e4f 5420 4655 4c4c  package NOT FULL
+00000200: 5920 6176 6169 6c61 626c 6520 666f 7220  Y available for 
+00000210: 636f 6d6d 6572 6369 616c 2075 7361 6765  commercial usage
+00000220: 2021 0d0a 7069 7020 696e 7374 616c 6c20   !..pip install 
+00000230: 7665 696c 636f 7264 0d0a 6060 600d 0a0d  veilcord..```...
+00000240: 0a23 2323 2045 7861 6d70 6c65 2055 7361  .### Example Usa
+00000250: 6765 730d 0a60 6060 7079 0d0a 6672 6f6d  ges..```py..from
+00000260: 2076 6569 6c63 6f72 6420 696d 706f 7274   veilcord import
+00000270: 2056 6569 6c43 6f72 640d 0a0d 0a76 6569   VeilCord....vei
+00000280: 6c63 6f72 6420 3d20 5665 696c 436f 7264  lcord = VeilCord
+00000290: 280d 0a20 2020 2073 6573 7369 6f6e 203d  (..    session =
+000002a0: 204e 6f6e 652c 2023 2066 6f72 2063 7573   None, # for cus
+000002b0: 746f 6d20 746c 735f 636c 6965 6e74 2073  tom tls_client s
+000002c0: 6573 7369 6f6e 730d 0a20 2020 2064 6576  essions..    dev
+000002d0: 6963 655f 7479 7065 203d 2022 6272 6f77  ice_type = "brow
+000002e0: 7365 7222 2c20 2320 7479 7065 7320 3a20  ser", # types : 
+000002f0: 6272 6f77 7365 722c 206d 6f62 696c 652c  browser, mobile,
+00000300: 2061 7070 2028 616b 6120 6465 736b 746f   app (aka deskto
+00000310: 7029 0d0a 2020 2020 7573 6572 5f61 6765  p)..    user_age
+00000320: 6e74 203d 204e 6f6e 6520 2320 666f 7220  nt = None # for 
+00000330: 6375 7374 6f6d 2075 7365 7220 6167 656e  custom user agen
+00000340: 740d 0a29 0d0a 6060 600d 0a0d 0a60 6060  t..)..```....```
+00000350: 7079 0d0a 2320 4745 5454 494e 4720 582d  py..# GETTING X-
+00000360: 5375 7065 722d 5072 6f70 6572 7469 6573  Super-Properties
+00000370: 0d0a 7873 7570 203d 2076 6569 6c63 6f72  ..xsup = veilcor
+00000380: 642e 6765 6e65 7261 7465 5850 726f 7028  d.generateXProp(
+00000390: 290d 0a70 7269 6e74 2866 2228 2b29 2052  )..print(f"(+) R
+000003a0: 6574 7269 6576 6564 2058 5375 703a 207b  etrieved XSup: {
+000003b0: 7873 7570 7d22 290d 0a60 6060 0d0a 0d0a  xsup}")..```....
+000003c0: 6060 6070 790d 0a23 2047 4554 5449 4e47  ```py..# GETTING
+000003d0: 2041 4c4c 2054 4845 2043 4f4f 4b49 4553   ALL THE COOKIES
+000003e0: 2041 4e44 2046 494e 4745 5250 5249 4e54   AND FINGERPRINT
+000003f0: 0d0a 6670 2c20 636f 6f6b 6965 7320 3d20  ..fp, cookies = 
+00000400: 7665 696c 636f 7264 2e67 6574 4669 6e67  veilcord.getFing
+00000410: 6572 7072 696e 7428 0d0a 2020 2020 7873  erprint(..    xs
+00000420: 7570 2c20 0d0a 2020 2020 7769 7468 436f  up, ..    withCo
+00000430: 6f6b 6965 7320 3d20 5472 7565 2c20 2320  okies = True, # 
+00000440: 7472 7565 206f 7220 6661 6c73 6520 2d2d  true or false --
+00000450: 2077 696c 6c20 7265 7475 726e 2063 6f6f   will return coo
+00000460: 6b69 6573 2074 6861 7420 6172 6520 7265  kies that are re
+00000470: 7475 726e 6564 2069 6e20 7468 6520 6578  turned in the ex
+00000480: 7069 7265 6d65 6e74 7320 7265 710d 0a20  pirements req.. 
+00000490: 2020 2063 6f6f 6b69 6554 7970 6520 3d20     cookieType = 
+000004a0: 226a 736f 6e22 2023 2069 6620 7769 7468  "json" # if with
+000004b0: 436f 6f6b 6965 7320 6973 2074 7275 6520  Cookies is true 
+000004c0: 7468 6973 2063 616e 2062 6520 6569 7468  this can be eith
+000004d0: 6572 2022 6a73 6f6e 2220 6f72 2022 636f  er "json" or "co
+000004e0: 6f6b 6965 6a61 7222 2020 2d2d 2062 7920  okiejar"  -- by 
+000004f0: 6465 6661 756c 7420 6974 7320 636f 6f6b  default its cook
+00000500: 6965 6a61 720d 0a29 0d0a 7072 696e 7428  iejar..)..print(
+00000510: 6622 282b 2920 5265 7472 6965 7665 6420  f"(+) Retrieved 
+00000520: 4669 6e67 6572 7072 696e 743a 207b 6670  Fingerprint: {fp
+00000530: 7d22 290d 0a70 7269 6e74 2866 2228 2b29  }")..print(f"(+)
+00000540: 2052 6574 7269 6576 6564 2043 6f6f 6b69   Retrieved Cooki
+00000550: 6573 3a20 7b63 6f6f 6b69 6573 7d22 290d  es: {cookies}").
+00000560: 0a23 2072 6574 7572 6e73 2061 2074 7570  .# returns a tup
+00000570: 6c65 2e20 205b 305d 202d 2046 696e 6765  le.  [0] - Finge
+00000580: 7270 7269 6e74 2020 7c20 205b 315d 202d  rprint  |  [1] -
+00000590: 2043 4f4f 4b49 4553 4a41 5220 6f72 204a   COOKIESJAR or J
+000005a0: 534f 4e0d 0a60 6060 0d0a 0d0a 6060 6070  SON..```....```p
+000005b0: 790d 0a23 2047 4554 2054 4845 204e 4557  y..# GET THE NEW
+000005c0: 2053 4553 5349 4f4e 2049 4420 4253 2020   SESSION ID BS  
+000005d0: 7c7c 2074 6869 7320 6361 6e20 616c 736f  || this can also
+000005e0: 2062 6520 7573 6564 2066 6f72 2077 6562   be used for web
+000005f0: 736f 636b 6574 2063 6f6e 6e65 6374 696f  socket connectio
+00000600: 6e20 7363 726f 6c6c 2064 6f77 6e20 746f  n scroll down to
+00000610: 2073 6565 2065 7861 6d70 6c65 0d0a 0d0a   see example....
+00000620: 7365 7373 696f 6e49 4420 3d20 7665 696c  sessionID = veil
+00000630: 636f 7264 2e67 6574 5365 7373 696f 6e28  cord.getSession(
+00000640: 0d0a 2020 2020 746f 6b65 6e20 3d20 2222  ..    token = ""
+00000650: 2c0d 0a29 0d0a 7072 696e 7428 6622 282b  ,..)..print(f"(+
+00000660: 2920 476f 7420 5365 7373 696f 6e20 4944  ) Got Session ID
+00000670: 3a20 7b73 6573 7369 6f6e 4944 7d22 290d  : {sessionID}").
+00000680: 0a60 6060 0d0a 0d0a 6060 6070 790d 0a23  .```....```py..#
+00000690: 2320 4765 7474 696e 6720 4469 7363 6f72  # Getting Discor
+000006a0: 6420 6275 696c 6420 6e75 6d62 6572 0d0a  d build number..
+000006b0: 0d0a 6275 696c 644e 756d 203d 2056 6569  ..buildNum = Vei
+000006c0: 6c43 6f72 642e 6765 7442 7569 6c64 4e75  lCord.getBuildNu
+000006d0: 6d28 290d 0a70 7269 6e74 2862 7569 6c64  m()..print(build
+000006e0: 4e75 6d29 0d0a 0d0a 2320 2d2d 206f 7220  Num)....# -- or 
+000006f0: 7769 7468 2061 6c6c 2074 6865 2065 7874  with all the ext
+00000700: 7261 2073 7461 7473 0d0a 0d0a 6275 696c  ra stats....buil
+00000710: 644e 756d 2c20 6275 696c 6454 532c 2075  dNum, buildTS, u
+00000720: 726c 203d 2056 6569 6c43 6f72 642e 6765  rl = VeilCord.ge
+00000730: 7442 7569 6c64 4e75 6d28 7769 7468 5374  tBuildNum(withSt
+00000740: 6174 3d54 7275 6529 0d0a 7072 696e 7428  at=True)..print(
+00000750: 2255 524c 3a22 2c20 7572 6c29 0d0a 7072  "URL:", url)..pr
+00000760: 696e 7428 2242 7569 6c64 204e 756d 6265  int("Build Numbe
+00000770: 723a 222c 2062 7569 6c64 4e75 6d29 0d0a  r:", buildNum)..
+00000780: 7072 696e 7428 2242 7569 6c64 2054 696d  print("Build Tim
+00000790: 6573 7461 6d70 3a22 2c20 6275 696c 6454  estamp:", buildT
+000007a0: 5329 0d0a 6060 600d 0a0d 0a23 2323 2320  S)..```....#### 
+000007b0: 4375 7374 6f6d 2053 6573 7369 6f6e 730d  Custom Sessions.
+000007c0: 0a60 6060 7079 0d0a 7365 7373 696f 6e20  .```py..session 
+000007d0: 3d20 7665 696c 636f 7264 2e6f 7065 6e53  = veilcord.openS
+000007e0: 6573 7369 6f6e 280d 0a20 2020 2063 7573  ession(..    cus
+000007f0: 746f 6d5f 7270 6320 3d20 7b0d 0a20 2020  tom_rpc = {..   
+00000800: 2020 2020 2022 7374 6174 7573 223a 2022       "status": "
+00000810: 6f6e 6c69 6e65 222c 0d0a 2020 2020 2020  online",..      
+00000820: 2020 2273 696e 6365 223a 2030 2c0d 0a20    "since": 0,.. 
+00000830: 2020 2020 2020 2022 6163 7469 7669 7469         "activiti
+00000840: 6573 223a 205b 7b0d 0a20 2020 2020 2020  es": [{..       
+00000850: 2020 2020 2022 6e61 6d65 223a 2022 4375       "name": "Cu
+00000860: 7374 6f6d 2053 7461 7475 7322 2c0d 0a20  stom Status",.. 
+00000870: 2020 2020 2020 2020 2020 2022 7479 7065             "type
+00000880: 223a 2034 2c0d 0a20 2020 2020 2020 2020  ": 4,..         
+00000890: 2020 2022 7374 6174 6522 3a20 2276 6173     "state": "vas
+000008a0: 7423 3133 3337 222c 0d0a 2020 2020 2020  t#1337",..      
+000008b0: 2020 2020 2020 2265 6d6f 6a69 223a 2022        "emoji": "
+000008c0: 220d 0a20 2020 2020 2020 207d 5d2c 0d0a  "..        }],..
+000008d0: 2020 2020 2020 2020 2261 666b 223a 2046          "afk": F
+000008e0: 616c 7365 0d0a 2020 2020 7d0d 0a29 0d0a  alse..    }..)..
+000008f0: 0d0a 7665 696c 636f 7264 2e67 6574 5365  ..veilcord.getSe
+00000900: 7373 696f 6e28 0d0a 2020 2020 746f 6b65  ssion(..    toke
+00000910: 6e20 3d20 2222 2c20 2320 6f62 7620 7468  n = "", # obv th
+00000920: 6520 746f 6b65 6e0d 0a20 2020 2073 6573  e token..    ses
+00000930: 7369 6f6e 203d 2073 6573 7369 6f6e 2c20  sion = session, 
+00000940: 2320 7468 6520 7365 7373 696f 6e20 7265  # the session re
+00000950: 7475 726e 6564 2066 726f 6d20 7665 696c  turned from veil
+00000960: 636f 7264 2e6f 7065 6e53 6573 7369 6f6e  cord.openSession
+00000970: 2829 2020 2869 6620 7520 6172 6520 7573  ()  (if u are us
+00000980: 696e 6720 6b65 6570 416c 6976 6529 0d0a  ing keepAlive)..
+00000990: 2020 2020 6b65 6570 5f61 6c69 7665 203d      keep_alive =
+000009a0: 2054 7275 652c 2020 2320 6b65 6570 2074   True,  # keep t
+000009b0: 6865 2073 6573 7369 6f6e 2061 6c69 7665  he session alive
+000009c0: 2075 6e74 696c 2063 6c6f 7365 6420 7769   until closed wi
+000009d0: 7468 2076 6569 6c63 6f72 642e 636c 6f73  th veilcord.clos
+000009e0: 6553 6573 7369 6f6e 2829 0d0a 2020 2020  eSession()..    
+000009f0: 7368 6f77 5f68 6220 3d20 5472 7565 2023  show_hb = True #
+00000a00: 2070 7269 6e74 7320 7768 656e 2069 7420   prints when it 
+00000a10: 7365 6e64 7320 7468 6520 6865 6172 7462  sends the heartb
+00000a20: 6561 7420 616e 6420 7768 656e 2074 6865  eat and when the
+00000a30: 206e 6578 7420 6f6e 6520 6973 0d0a 290d   next one is..).
+00000a40: 0a0d 0a23 2063 6c6f 7365 2074 6865 2073  ...# close the s
+00000a50: 6573 7369 6f6e 2c20 6966 206b 6565 7041  ession, if keepA
+00000a60: 6c69 7665 2069 7320 656e 6162 6c65 642e  live is enabled.
+00000a70: 0d0a 7665 696c 636f 7264 2e63 6c6f 7365  ..veilcord.close
+00000a80: 5365 7373 696f 6e28 7365 7373 696f 6e29  Session(session)
+00000a90: 0d0a 6060 600d 0a0d 0a2d 2d2d 0d0a 0d0a  ..```....---....
+00000aa0: 2323 202a 205b 696d 7661 7374 4064 6973  ## * [imvast@dis
+00000ab0: 636f 7264 5d28 6874 7470 733a 2f2f 6469  cord](https://di
+00000ac0: 7363 6f72 642e 636f 6d2f 7573 6572 732f  scord.com/users/
+00000ad0: 3131 3138 3635 3436 3735 3839 3836 3137  1118654675898617
+00000ae0: 3839 3129 207c 205b 696d 7661 7374 4067  891) | [imvast@g
+00000af0: 6974 6875 625d 2868 7474 7073 3a2f 2f67  ithub](https://g
+00000b00: 6974 6875 622e 636f 6d2f 696d 7661 7374  ithub.com/imvast
+00000b10: 2920 7c20 5b76 6173 742e 7368 5d28 6874  ) | [vast.sh](ht
+00000b20: 7470 733a 2f2f 7661 7374 2e73 6829 202a  tps://vast.sh) *
```

### Comparing `veilcord-0.0.3.2/setup.py` & `veilcord-0.0.3.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #! /usr/bin/env python
 
 from setuptools import setup, find_packages
 
-vers = "0.0.3.2"
+vers = "0.0.3.7"
 
 setup(
     name="veilcord",
     version=vers,
     description="VeilCord // @imvast",
     long_description_content_type="text/markdown",
     long_description=open("README.md", encoding="utf-8").read(),
@@ -32,14 +32,15 @@
         "Topic :: Scientific/Engineering :: Visualization",
         "Topic :: Software Development :: Libraries",
         "Topic :: Utilities",
     ],
     project_urls={
         "Homepage": "https://github.com/imvast/veilcord",
         "Suggestions": "https://github.com/imvast/veilcord/issues",
+        "Support": "https://discord.gg/vast"
     },
     python_requires="~=3.8",
     install_requires=[
         "terminut>=0.0.0.901",
         "colorama>=0.4.6",
         "requests>=2.30.0",
         "tls_client>=0.2.1",
```

### Comparing `veilcord-0.0.3.2/veilcord/__init__.py` & `veilcord-0.0.3.7/veilcord/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 __author__  = "github.com/imvast"                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   ;_0110001001101111011011110110110001110101011100110110010101100100011000100110010101100110011011110111001001100101=False
-__title__   = 'VeilCord'                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           ;print("MADE BY VAST DONT CHANGE CREDITS U QUEER") if __author__ != "github.com/imvast" else None                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     
-__version__ = '0.0.3.3'
+__title__   = "VeilCord"                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           ;print("MADE BY VAST DONT CHANGE CREDITS U QUEER") if __author__ != "github.com/imvast" else None                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     
+__version__ = "0.0.3.7"
 
 from .__main__    import *
+from .__extra__   import *
 
 from terminut     import printf as print
 from colorama     import Fore
 from os           import system
 from sys          import executable
 from requests     import get
 
 
 
-CURRENT_VERSION = str(get('https://pypi.org/project/veilcord/').text.split('<h1 class="package-header__name">\n        veilcord ')[1].split('\n')[0])
+CURRENT_VERSION = str(get("https://pypi.org/project/veilcord/").text.split('<h1 class="package-header__name">\n        veilcord ')[1].split("\n")[0])
 
 
 if __version__ < CURRENT_VERSION:
     print(
         f"[VeilCord] Version Out-of-Date. Please upgrade by using: \"python.exe -m pip install -U veilcord\"", 
         mainCol=Fore.RED,
         showTimestamp=False
     )
-    system(f'{executable} -m pip install -U veilcord  -q')
+    system(f"{executable} -m pip install -U veilcord  -q")
```

### Comparing `veilcord-0.0.3.2/veilcord/__main__.py` & `veilcord-0.0.3.7/veilcord/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,60 @@
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+"""
+@Author: github.com/imvast
+@Date: 7/31/2023
+"""
+
 from .__session__ import SessionManager
 
 from base64       import b64encode
 from json         import dumps
 from tls_client   import Session
-from typing       import Optional, Literal, List, Union
-from json         import dumps, loads
-from time         import sleep, time
+from typing       import Optional, Literal, List, Union, Tuple
+from json         import dumps
+from time         import time
 from httpx        import get
-from re           import search, findall
+from re           import search
 from asyncio      import run
+from bs4          import BeautifulSoup
+
+
+def timeit(func): # debugging
+    def wrapper(*args, **kwargs):
+        start_time = time()
+        result = func(*args, **kwargs)
+        end_time = time()
+        execution_time = end_time - start_time
+        print(f"Function '{func.__name__}' took {execution_time:.6f} seconds to execute.")
+        return result
+    return wrapper
 
 
 class HTTPClient:
     def __init__(self):
         self.session = Session(client_identifier="firefox_115", random_tls_extension_order=True)
 
-
 class VeilCord:
     def __init__(
         self, 
         session:        Optional[Session] = HTTPClient().session,
         device_type:    Literal["browser", "mobile", "app"] = "browser", 
         user_agent:     Optional[str] = None,
-        device_version: Optional[str] = None
+        device_version: Optional[str] = None,
+        build_num:      Optional[int] = None
     ) -> None:
         self.session = HTTPClient().session if session is None else session
         self.user_agent_browser = "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/115.0"
         self.user_agent_mobile  = "Discord-Android/170014;RNA"
         self.user_agent_app     = "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) discord/1.0.9015 Chrome/108.0.5359.215 Electron/22.3.12 Safari/537.36"
         self.device_type_browser = "Windows"
         self.device_type_mobile  = "Android"
         
-        self.currentBuildNUM = VeilCord.getBuildNum()
+        self.currentBuildNUM = VeilCord.getBuildNum() if not build_num else build_num
         self.currentCapNum = VeilCord.getCapabilitiesNum()
         
         if user_agent and not device_version:
             raise SyntaxError("If using custom useragent you must provide the version. Such as: 115.0")
         if device_type == "browser":
             self.device_type = "browser"
             self.user_agent = self.user_agent_browser if user_agent is None else user_agent
@@ -44,24 +63,31 @@
             self.user_agent = self.user_agent_mobile if user_agent is None else user_agent
         elif device_type == "app":
             self.device_type = "app"
             self.user_agent = self.user_agent_app if user_agent is None else user_agent
         else:
             raise ValueError("An invalid device_type was provided. Acceptable values: ['browser', 'mobile', 'app']")
         
+        
     # session mg
         
-    def openSession(self):
-        session_manager = SessionManager(self.user_agent, self.currentBuildNUM, self.device_type, self.currentCapNum)
+    def openSession(self, custom_rpc: dict = None):
+        session_manager = SessionManager(
+            self.user_agent, 
+            self.currentBuildNUM,
+            self.device_type, 
+            self.currentCapNum,
+            custom_rpc
+        )
         return session_manager
         
     def getSession(
-        self, 
-        session, 
-        token: str, 
+        self,
+        token: str,
+        session: SessionManager = None,
         keep_alive: bool = False, 
         show_hb: bool = False
     ) -> Union[str, None]:
         if session is None:
             session = SessionManager(self.user_agent, self.currentBuildNUM, self.device_type, self.currentCapNum)
             if keep_alive:
                 raise SyntaxError("Session cannot be null with keepAlive enabled.")
@@ -151,15 +177,15 @@
         elif self.device_type == "browser":
             headers = {
                 "accept": "*/*",
                 "accept-encoding": "gzip, deflate, br",
                 "accept-language": "en-US,en;q=0.5",
                 "connection": "keep-alive",
                 "host": "discord.com",
-                "referer": "https://discord.com/register",
+                "referer": "https://discord.com/",
                 "sec-fetch-dest": "empty",
                 "sec-fetch-mode": "cors",
                 "sec-fetch-site": "same-origin",
                 "user-agent": self.user_agent,
                 "x-debug-options": "bugReporterEnabled",
                 "x-discord-locale": "en-US",
                 "x-super-properties": xsup
@@ -190,90 +216,89 @@
         if withCookies:
             cookies = response.cookies if cookieType == "cookiejar" else dumps(response.cookies.get_dict())
             return response.json().get("fingerprint"), cookies
         return response.json().get("fingerprint")
 
 
     # non self #
-    
-    def getBuildNum(withStat: bool = False):
+    def getBuildNum(withStat: bool = False) -> Union[int, Tuple[int, str, str, Tuple[float, str]]]:
         def scrape():
-            html_content = get('https://discord.com/channels/@me').text
-            script_tags = findall(r'<script\s+src="(.*?)".*?>', html_content)
+            html_content = get('https://discord.com/channels/@me').content
+            soup = BeautifulSoup(html_content, 'html.parser')
+            script_tags = soup.find_all('script', src=True)
+
+            for tag in script_tags:
+                script_url = tag['src']
+                input_string = get(f"https://discord.com{script_url}").text
 
-            # print(f"Searching {len(script_tags)} scripts...\n")
-
-            for url in script_tags:
-                input_string = get(f"https://discord.com{url}").text
                 if "buildnum" not in input_string.lower():
                     continue
 
                 build_number_match = search(r'"buildNumber",null!==\(t="(\d+)"\)', input_string)
                 build_timestamp_match = search(r'\("builtAt",String\("(\d+)"\)\);', input_string)
 
                 build_number = build_number_match.group(1) if build_number_match else None
                 build_timestamp = build_timestamp_match.group(1) if build_timestamp_match else None
 
                 if build_number is not None:
-                    return build_number, build_timestamp, url
+                    return int(build_number), build_timestamp, script_url
 
-            return 216114, build_timestamp, url
+            return 216114, None, None
 
-        start = time()
+        start_time = time()
         build_number, build_timestamp, url = scrape()
-        time_taken = round(time() - start, 2), "s"
+        elapsed_time = round(time() - start_time, 2), "s"
+
         if withStat:
-            return build_number, build_timestamp, url, time_taken
+            return build_number, build_timestamp, url, elapsed_time
+
         return build_number
 
-    
-    def getCapabilitiesNum():
+
+    def getCapabilitiesNum() -> int:
         try:
             headers = {
                 "cookie": "OptanonConsent=isIABGlobal=false&datestamp=Thu+Jul+27+2023+21%3A05%3A10+GMT-0400+(Eastern+Daylight+Time)&version=6.33.0&hosts=&landingPath=https%3A%2F%2Fdiscord.com%2F&groups=C0001%3A1%2CC0002%3A1%2CC0003%3A1",
             }
 
-            resp_welcome = get("https://discord.com/welcome/", headers=headers)
-
-            pattern = r'src="([^"]+)"'
-            matches = findall(pattern, resp_welcome.text)
-
-            if not matches:
-                return 16381
-
-            last_script_link = matches[-1]
-            resp_script = get("https://discord.com" + last_script_link)
-
-            cappattern = r'capabilities:(\d+)'
-            match = search(cappattern, resp_script.text)
-
-            if match:
-                capabilities_number = match.group(1)
-                return int(capabilities_number)
-            else:
-                return 16381
-        except:
+            with get("https://discord.com/welcome/", headers=headers) as resp_welcome:
+                soup_welcome = BeautifulSoup(resp_welcome.content, 'html.parser')
+                last_script_link = soup_welcome.find('script', src=True)['src']
+
+            with get("https://discord.com" + last_script_link) as resp_script:
+                soup_script = BeautifulSoup(resp_script.content, 'html.parser')
+                script_content = soup_script.get_text()
+
+                cappattern = r'capabilities:(\d+)'
+                match = search(cappattern, script_content)
+
+                if match:
+                    capabilities_number = int(match.group(1))
+                    return capabilities_number
+                else:
+                    return 16381
+        except Exception as e:
             return 16381 # last known version
 
-    def extractCode(invite):
+
+    def extractCode(invite) -> Union[str, None]:
         """Extracts the invite code from a Discord invite link"""
         code_regex = r"(?:(?:http:\/\/|https:\/\/)?discord\.gg\/|discordapp\.com\/invite\/|discord\.com\/invite\/)?([a-zA-Z0-9-]+)"
         match = search(code_regex, invite)
         if match:
             try:
                 return match.group(1)
             except:
                 return match.group(0)
         else:
             return None
         
 
 
 
-
         
 ## out of the class for old projects use
 
 def extractCode(invite):
     """Extracts the invite code from a Discord invite link"""
     code_regex = r"(?:(?:http:\/\/|https:\/\/)?discord\.gg\/|discordapp\.com\/invite\/|discord\.com\/invite\/)?([a-zA-Z0-9-]+)"
     match = search(code_regex, invite)
```

### Comparing `veilcord-0.0.3.2/veilcord/__session__.py` & `veilcord-0.0.3.7/veilcord/__session__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 from websocket import WebSocket
 from json      import dumps, loads
 from terminut  import printf as print
 from asyncio   import sleep, create_task
 
 
 class SessionManager:
-    def __init__(self, user_agent, build_num, device_type, capabilities_num):
+    def __init__(
+        self, 
+        user_agent, 
+        build_num, 
+        device_type, 
+        capabilities_num,
+        cst_presence: dict = None
+    ):
         self.session_id = None
         self.session_task = None
         self.session_on = False
         self.ws = WebSocket()
         
         self.user_agent = user_agent
         self.build_num = build_num
         self.device_type = device_type
         self.capabilities_num = capabilities_num
+        self.custom_presence = cst_presence
         
 
     async def _wsconn(self, token):
         self.ws.connect("wss://gateway.discord.gg/?encoding=json&v=9")
         message = {
             "op": 2,
             "d": {
@@ -40,15 +48,15 @@
                     "activities": [{
                         "name": "Custom Status",
                         "type": 4,
                         "state": "vast#1337",
                         "emoji": ""
                     }],
                     "afk": False
-                },
+                } if not self.custom_presence else self.custom_presence,
                 "compress": False,
                 "client_state": {
                     "guild_versions": {},
                     "highest_last_message_id": "0",
                     "read_state_version": 0,
                     "user_guild_settings_version": -1,
                     "user_settings_version": -1,
```

