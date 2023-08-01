# Comparing `tmp/rclip-1.4.2.tar.gz` & `tmp/rclip-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rclip-1.4.2.tar", max compression
+gzip compressed data, was "rclip-1.4.3.tar", max compression
```

## Comparing `rclip-1.4.2.tar` & `rclip-1.4.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1074 2021-12-18 09:44:28.707592 rclip-1.4.2/LICENSE
--rw-r--r--   0        0        0     4197 2023-08-01 04:51:20.720004 rclip-1.4.2/README.md
--rw-r--r--   0        0        0     1564 2023-08-01 04:51:46.762368 rclip-1.4.2/pyproject.toml
--rw-r--r--   0        0        0     2940 2023-07-31 14:28:36.693991 rclip-1.4.2/rclip/db.py
--rw-r--r--   0        0        0     5586 2023-07-24 08:17:08.004229 rclip-1.4.2/rclip/main.py
--rw-r--r--   0        0        0     5161 2023-08-01 04:46:19.501263 rclip-1.4.2/rclip/model.py
--rw-r--r--   0        0        0     4551 2023-07-23 16:44:40.439264 rclip-1.4.2/rclip/utils.py
--rw-r--r--   0        0        0     5593 1970-01-01 00:00:00.000000 rclip-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2021-12-18 09:44:28.707592 rclip-1.4.3/LICENSE
+-rw-r--r--   0        0        0     4791 2023-08-01 05:05:25.103033 rclip-1.4.3/README.md
+-rw-r--r--   0        0        0     1556 2023-08-01 05:16:40.977956 rclip-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0     2940 2023-07-31 14:28:36.693991 rclip-1.4.3/rclip/db.py
+-rw-r--r--   0        0        0     5586 2023-07-24 08:17:08.004229 rclip-1.4.3/rclip/main.py
+-rw-r--r--   0        0        0     5161 2023-08-01 04:46:19.501263 rclip-1.4.3/rclip/model.py
+-rw-r--r--   0        0        0     4551 2023-07-23 16:44:40.439264 rclip-1.4.3/rclip/utils.py
+-rw-r--r--   0        0        0     6296 1970-01-01 00:00:00.000000 rclip-1.4.3/PKG-INFO
```

### Comparing `rclip-1.4.2/LICENSE` & `rclip-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rclip-1.4.2/README.md` & `rclip-1.4.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -106,158 +106,195 @@
 00000690: 656c c2a0 4365 6c65 726f 6ec2 a04a 3334  el..Celeron..J34
 000006a0: 3535 2e0a 0a46 6f72 2061 2064 6574 6169  55...For a detai
 000006b0: 6c65 6420 6465 6d6f 6e73 7472 6174 696f  led demonstratio
 000006c0: 6e2c 2077 6174 6368 2074 6865 2076 6964  n, watch the vid
 000006d0: 656f 3a20 6874 7470 733a 2f2f 7777 772e  eo: https://www.
 000006e0: 796f 7574 7562 652e 636f 6d2f 7761 7463  youtube.com/watc
 000006f0: 683f 763d 7441 4a48 584f 6b48 6964 772e  h?v=tAJHXOkHidw.
-00000700: 0a0a 596f 7520 6361 6e20 616c 736f 2075  ..You can also u
-00000710: 7365 2061 6e6f 7468 6572 2069 6d61 6765  se another image
-00000720: 2061 7320 6120 7175 6572 7920 6279 2070   as a query by p
-00000730: 6173 7369 6e67 2061 2066 696c 6520 7061  assing a file pa
-00000740: 7468 206f 7220 6576 656e 2061 6e20 5552  th or even an UR
-00000750: 4c20 746f 2074 6865 2069 6d61 6765 2066  L to the image f
-00000760: 696c 652c 2061 6e64 202a 2a72 636c 6970  ile, and **rclip
-00000770: 2a2a 2077 696c 6c20 6669 6e64 2074 6865  ** will find the
-00000780: 2069 6d61 6765 7320 6d6f 7374 2073 696d   images most sim
-00000790: 696c 6172 2074 6f20 7468 6520 6f6e 6520  ilar to the one 
-000007a0: 796f 7520 7573 6564 2061 7320 6120 7175  you used as a qu
-000007b0: 6572 792e 2049 6620 796f 7520 6172 6520  ery. If you are 
-000007c0: 7265 6665 7265 6e63 696e 6720 6120 6c6f  referencing a lo
-000007d0: 6361 6c20 696d 6167 6520 7669 6120 6120  cal image via a 
-000007e0: 7265 6c61 7469 7665 2070 6174 682c 2079  relative path, y
-000007f0: 6f75 202a 2a6d 7573 742a 2a20 7072 6566  ou **must** pref
-00000800: 6978 2069 7420 7769 7468 2060 2e2f 602e  ix it with `./`.
-00000810: 2046 6f72 2065 7861 6d70 6c65 3a0a 0a60   For example:..`
-00000820: 6060 6261 7368 0a63 6420 7068 6f74 6f73  ``bash.cd photos
-00000830: 2026 2620 7263 6c69 7020 2e2f 6361 742e   && rclip ./cat.
-00000840: 6a70 670a 0a23 206f 7220 7573 6520 5552  jpg..# or use UR
-00000850: 4c0a 6364 2070 686f 746f 7320 2626 2072  L.cd photos && r
-00000860: 636c 6970 2068 7474 7073 3a2f 2f72 6177  clip https://raw
-00000870: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
-00000880: 6e74 2e63 6f6d 2f79 7572 696a 6d69 6b68  nt.com/yurijmikh
-00000890: 616c 6576 6963 682f 7263 6c69 702f 6d61  alevich/rclip/ma
-000008a0: 696e 2f74 6573 7473 2f65 3265 2f69 6d61  in/tests/e2e/ima
-000008b0: 6765 732f 6361 742e 6a70 670a 6060 600a  ges/cat.jpg.```.
-000008c0: 0a43 6865 636b 2074 6869 7320 7669 6465  .Check this vide
-000008d0: 6f20 6f75 7420 666f 7220 7468 6520 696d  o out for the im
-000008e0: 6167 652d 746f 2d69 6d61 6765 2073 6561  age-to-image sea
-000008f0: 7263 6820 6465 6d6f 3a20 6874 7470 733a  rch demo: https:
-00000900: 2f2f 7777 772e 796f 7574 7562 652e 636f  //www.youtube.co
-00000910: 6d2f 7761 7463 683f 763d 3159 515a 4b65  m/watch?v=1YQZKe
-00000920: 4342 7857 4d2e 0a0a 2323 2320 486f 7720  CBxWM...### How 
-00000930: 646f 2049 2070 7265 7669 6577 2074 6865  do I preview the
-00000940: 2072 6573 756c 7473 3f0a 0a54 6865 2063   results?..The c
-00000950: 6f6d 6d61 6e64 2066 726f 6d20 6265 6c6f  ommand from belo
-00000960: 7720 7769 6c6c 206f 7065 6e20 746f 702d  w will open top-
-00000970: 3520 7265 7375 6c74 7320 666f 7220 226b  5 results for "k
-00000980: 6974 7479 2220 696e 2079 6f75 7220 6465  itty" in your de
-00000990: 6661 756c 7420 696d 6167 6520 7669 6577  fault image view
-000009a0: 6572 3a0a 0a60 6060 6261 7368 0a72 636c  er:..```bash.rcl
-000009b0: 6970 202d 6620 2d74 2035 206b 6974 7479  ip -f -t 5 kitty
-000009c0: 207c 2078 6172 6773 202d 6420 275c 6e27   | xargs -d '\n'
-000009d0: 202d 6e20 3120 7864 672d 6f70 656e 0a60   -n 1 xdg-open.`
-000009e0: 6060 0a0a 4920 7072 6566 6572 2074 6f20  ``..I prefer to 
-000009f0: 7573 6520 6066 6568 6027 7320 7468 756d  use `feh`'s thum
-00000a00: 626e 6169 6c20 6d6f 6465 2074 6f20 7072  bnail mode to pr
-00000a10: 6576 6965 7720 6d75 6c74 6970 6c65 2072  eview multiple r
-00000a20: 6573 756c 7473 3a0a 0a60 6060 6261 7368  esults:..```bash
-00000a30: 0a72 636c 6970 202d 6620 2d74 2035 206b  .rclip -f -t 5 k
-00000a40: 6974 7479 207c 2066 6568 202d 6620 2d20  itty | feh -f - 
-00000a50: 2d74 0a60 6060 0a0a 2323 2048 656c 700a  -t.```..## Help.
-00000a60: 0a60 6060 6261 7368 0a72 636c 6970 202d  .```bash.rclip -
-00000a70: 2d68 656c 700a 6060 600a 0a23 2320 436f  -help.```..## Co
-00000a80: 6e74 7269 6275 7469 6e67 0a0a 5468 6973  ntributing..This
-00000a90: 2072 6570 6f73 6974 6f72 7920 666f 6c6c   repository foll
-00000aa0: 6f77 7320 7468 6520 5b43 6f6e 7665 6e74  ows the [Convent
-00000ab0: 696f 6e61 6c20 436f 6d6d 6974 735d 2868  ional Commits](h
-00000ac0: 7474 7073 3a2f 2f77 7777 2e63 6f6e 7665  ttps://www.conve
-00000ad0: 6e74 696f 6e61 6c63 6f6d 6d69 7473 2e6f  ntionalcommits.o
-00000ae0: 7267 2f65 6e2f 7631 2e30 2e30 2f29 2073  rg/en/v1.0.0/) s
-00000af0: 7461 6e64 6172 642e 0a0a 2323 2320 5275  tandard...### Ru
-00000b00: 6e6e 696e 6720 6c6f 6361 6c6c 7920 6672  nning locally fr
-00000b10: 6f6d 2074 6865 2073 6f75 7263 6520 636f  om the source co
-00000b20: 6465 0a0a 546f 2072 756e 202a 2a72 636c  de..To run **rcl
-00000b30: 6970 2a2a 206c 6f63 616c 6c79 2066 726f  ip** locally fro
-00000b40: 6d20 7468 6520 736f 7572 6365 2063 6f64  m the source cod
-00000b50: 652c 2079 6f75 206d 7573 7420 6861 7665  e, you must have
-00000b60: 205b 5079 7468 6f6e 5d28 6874 7470 733a   [Python](https:
-00000b70: 2f2f 7777 772e 7079 7468 6f6e 2e6f 7267  //www.python.org
-00000b80: 2f64 6f77 6e6c 6f61 6473 2f29 2061 6e64  /downloads/) and
-00000b90: 205b 506f 6574 7279 5d28 6874 7470 733a   [Poetry](https:
-00000ba0: 2f2f 7079 7468 6f6e 2d70 6f65 7472 792e  //python-poetry.
-00000bb0: 6f72 672f 2920 696e 7374 616c 6c65 642e  org/) installed.
-00000bc0: 0a0a 5468 656e 2064 6f3a 0a60 6060 6261  ..Then do:.```ba
-00000bd0: 7368 0a23 2063 6c6f 6e65 2074 6865 2073  sh.# clone the s
-00000be0: 6f75 7263 6520 636f 6465 2072 6570 6f73  ource code repos
-00000bf0: 6974 6f72 790a 6769 7420 636c 6f6e 6520  itory.git clone 
-00000c00: 6769 7440 6769 7468 7562 2e63 6f6d 3a79  git@github.com:y
-00000c10: 7572 696a 6d69 6b68 616c 6576 6963 682f  urijmikhalevich/
-00000c20: 7263 6c69 702e 6769 740a 0a23 2069 6e73  rclip.git..# ins
-00000c30: 7461 6c6c 2064 6570 656e 6465 6e63 6965  tall dependencie
-00000c40: 7320 616e 6420 7263 6c69 700a 6364 2072  s and rclip.cd r
-00000c50: 636c 6970 0a70 6f65 7472 7920 696e 7374  clip.poetry inst
-00000c60: 616c 6c0a 0a23 2061 6374 6976 6174 6520  all..# activate 
-00000c70: 7468 6520 6e65 7720 706f 6574 7279 2065  the new poetry e
-00000c80: 6e76 6972 6f6e 6d65 6e74 0a70 6f65 7472  nvironment.poetr
-00000c90: 7920 7368 656c 6c0a 6060 600a 0a49 6620  y shell.```..If 
-00000ca0: 7468 6520 706f 6574 7279 2065 6e76 6972  the poetry envir
-00000cb0: 6f6e 6d65 6e74 2069 7320 6163 7469 7665  onment is active
-00000cc0: 2c20 796f 7520 6361 6e20 7573 6520 2a2a  , you can use **
-00000cd0: 7263 6c69 702a 2a20 6c6f 6361 6c6c 792c  rclip** locally,
-00000ce0: 2061 7320 6465 7363 7269 6265 6420 696e   as described in
-00000cf0: 2074 6865 205b 5573 6167 655d 2823 7573   the [Usage](#us
-00000d00: 6167 6529 2073 6563 7469 6f6e 2061 626f  age) section abo
-00000d10: 7665 2e0a 0a23 2320 436f 6e74 7269 6275  ve...## Contribu
-00000d20: 746f 7273 20e2 9ca8 0a0a 5468 616e 6b73  tors .....Thanks
-00000d30: 2067 6f20 746f 2074 6865 7365 2077 6f6e   go to these won
-00000d40: 6465 7266 756c 2070 656f 706c 6520 285b  derful people ([
-00000d50: 656d 6f6a 6920 6b65 795d 2868 7474 7073  emoji key](https
-00000d60: 3a2f 2f61 6c6c 636f 6e74 7269 6275 746f  ://allcontributo
-00000d70: 7273 2e6f 7267 2f64 6f63 732f 656e 2f65  rs.org/docs/en/e
-00000d80: 6d6f 6a69 2d6b 6579 2929 3a0a 0a3c 212d  moji-key)):..<!-
-00000d90: 2d20 414c 4c2d 434f 4e54 5249 4255 544f  - ALL-CONTRIBUTO
-00000da0: 5253 2d4c 4953 543a 5354 4152 5420 2d20  RS-LIST:START - 
-00000db0: 446f 206e 6f74 2072 656d 6f76 6520 6f72  Do not remove or
-00000dc0: 206d 6f64 6966 7920 7468 6973 2073 6563   modify this sec
-00000dd0: 7469 6f6e 202d 2d3e 0a3c 212d 2d20 7072  tion -->.<!-- pr
-00000de0: 6574 7469 6572 2d69 676e 6f72 652d 7374  ettier-ignore-st
-00000df0: 6172 7420 2d2d 3e0a 3c21 2d2d 206d 6172  art -->.<!-- mar
-00000e00: 6b64 6f77 6e6c 696e 742d 6469 7361 626c  kdownlint-disabl
-00000e10: 6520 2d2d 3e0a 3c74 6162 6c65 3e0a 2020  e -->.<table>.  
-00000e20: 3c74 723e 0a20 2020 203c 7464 2061 6c69  <tr>.    <td ali
-00000e30: 676e 3d22 6365 6e74 6572 223e 3c61 2068  gn="center"><a h
-00000e40: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
-00000e50: 6875 622e 636f 6d2f 7261 6d61 7965 7222  hub.com/ramayer"
-00000e60: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
-00000e70: 3a2f 2f61 7661 7461 7273 2e67 6974 6875  ://avatars.githu
-00000e80: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-00000e90: 2f75 2f37 3233 3230 3f76 3d34 3f73 3d31  /u/72320?v=4?s=1
-00000ea0: 3030 2220 7769 6474 683d 2231 3030 7078  00" width="100px
-00000eb0: 3b22 2061 6c74 3d22 222f 3e3c 6272 202f  ;" alt=""/><br /
-00000ec0: 3e3c 7375 623e 3c62 3e72 616d 6179 6572  ><sub><b>ramayer
-00000ed0: 3c2f 623e 3c2f 7375 623e 3c2f 613e 3c62  </b></sub></a><b
-00000ee0: 7220 2f3e 3c61 2068 7265 663d 2268 7474  r /><a href="htt
-00000ef0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000f00: 7975 7269 6a6d 696b 6861 6c65 7669 6368  yurijmikhalevich
-00000f10: 2f72 636c 6970 2f63 6f6d 6d69 7473 3f61  /rclip/commits?a
-00000f20: 7574 686f 723d 7261 6d61 7965 7222 2074  uthor=ramayer" t
-00000f30: 6974 6c65 3d22 436f 6465 223e f09f 92bb  itle="Code">....
-00000f40: 3c2f 613e 3c2f 7464 3e0a 2020 3c2f 7472  </a></td>.  </tr
-00000f50: 3e0a 3c2f 7461 626c 653e 0a0a 3c21 2d2d  >.</table>..<!--
-00000f60: 206d 6172 6b64 6f77 6e6c 696e 742d 7265   markdownlint-re
-00000f70: 7374 6f72 6520 2d2d 3e0a 3c21 2d2d 2070  store -->.<!-- p
-00000f80: 7265 7474 6965 722d 6967 6e6f 7265 2d65  rettier-ignore-e
-00000f90: 6e64 202d 2d3e 0a0a 3c21 2d2d 2041 4c4c  nd -->..<!-- ALL
-00000fa0: 2d43 4f4e 5452 4942 5554 4f52 532d 4c49  -CONTRIBUTORS-LI
-00000fb0: 5354 3a45 4e44 202d 2d3e 0a0a 5468 6973  ST:END -->..This
-00000fc0: 2070 726f 6a65 6374 2066 6f6c 6c6f 7773   project follows
-00000fd0: 2074 6865 205b 616c 6c2d 636f 6e74 7269   the [all-contri
-00000fe0: 6275 746f 7273 5d28 6874 7470 733a 2f2f  butors](https://
-00000ff0: 6769 7468 7562 2e63 6f6d 2f61 6c6c 2d63  github.com/all-c
-00001000: 6f6e 7472 6962 7574 6f72 732f 616c 6c2d  ontributors/all-
-00001010: 636f 6e74 7269 6275 746f 7273 2920 7370  contributors) sp
-00001020: 6563 6966 6963 6174 696f 6e2e 2043 6f6e  ecification. Con
-00001030: 7472 6962 7574 696f 6e73 206f 6620 616e  tributions of an
-00001040: 7920 6b69 6e64 2061 7265 2077 656c 636f  y kind are welco
-00001050: 6d65 210a 0a23 2320 4c69 6365 6e73 650a  me!..## License.
-00001060: 0a4d 4954 0a                             .MIT.
+00000700: 0a0a 2323 2320 5369 6d69 6c61 7220 696d  ..### Similar im
+00000710: 6167 6520 7365 6172 6368 0a0a 596f 7520  age search..You 
+00000720: 6361 6e20 7573 6520 616e 6f74 6865 7220  can use another 
+00000730: 696d 6167 6520 6173 2061 2071 7565 7279  image as a query
+00000740: 2062 7920 7061 7373 696e 6720 6120 6669   by passing a fi
+00000750: 6c65 2070 6174 6820 6f72 2065 7665 6e20  le path or even 
+00000760: 616e 2055 524c 2074 6f20 7468 6520 696d  an URL to the im
+00000770: 6167 6520 6669 6c65 2c20 616e 6420 2a2a  age file, and **
+00000780: 7263 6c69 702a 2a20 7769 6c6c 2066 696e  rclip** will fin
+00000790: 6420 7468 6520 696d 6167 6573 206d 6f73  d the images mos
+000007a0: 7420 7369 6d69 6c61 7220 746f 2074 6865  t similar to the
+000007b0: 206f 6e65 2079 6f75 2075 7365 6420 6173   one you used as
+000007c0: 2061 2071 7565 7279 2e20 4966 2079 6f75   a query. If you
+000007d0: 2061 7265 2072 6566 6572 656e 6369 6e67   are referencing
+000007e0: 2061 206c 6f63 616c 2069 6d61 6765 2076   a local image v
+000007f0: 6961 2061 2072 656c 6174 6976 6520 7061  ia a relative pa
+00000800: 7468 2c20 796f 7520 2a2a 6d75 7374 2a2a  th, you **must**
+00000810: 2070 7265 6669 7820 6974 2077 6974 6820   prefix it with 
+00000820: 602e 2f60 2e20 466f 7220 6578 616d 706c  `./`. For exampl
+00000830: 653a 0a0a 6060 6062 6173 680a 6364 2070  e:..```bash.cd p
+00000840: 686f 746f 7320 2626 2072 636c 6970 202e  hotos && rclip .
+00000850: 2f63 6174 2e6a 7067 0a0a 2320 6f72 2075  /cat.jpg..# or u
+00000860: 7365 2055 524c 0a63 6420 7068 6f74 6f73  se URL.cd photos
+00000870: 2026 2620 7263 6c69 7020 6874 7470 733a   && rclip https:
+00000880: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
+00000890: 636f 6e74 656e 742e 636f 6d2f 7975 7269  content.com/yuri
+000008a0: 6a6d 696b 6861 6c65 7669 6368 2f72 636c  jmikhalevich/rcl
+000008b0: 6970 2f6d 6169 6e2f 7465 7374 732f 6532  ip/main/tests/e2
+000008c0: 652f 696d 6167 6573 2f63 6174 2e6a 7067  e/images/cat.jpg
+000008d0: 0a60 6060 0a0a 4368 6563 6b20 7468 6973  .```..Check this
+000008e0: 2076 6964 656f 206f 7574 2066 6f72 2074   video out for t
+000008f0: 6865 2069 6d61 6765 2d74 6f2d 696d 6167  he image-to-imag
+00000900: 6520 7365 6172 6368 2064 656d 6f3a 2068  e search demo: h
+00000910: 7474 7073 3a2f 2f77 7777 2e79 6f75 7475  ttps://www.youtu
+00000920: 6265 2e63 6f6d 2f77 6174 6368 3f76 3d31  be.com/watch?v=1
+00000930: 5951 5a4b 6543 4278 574d 2e0a 0a23 2323  YQZKeCBxWM...###
+00000940: 2043 6f6d 6269 6e69 6e67 206d 756c 7469   Combining multi
+00000950: 706c 6520 7175 6572 6965 730a 0a59 6f75  ple queries..You
+00000960: 2063 616e 2061 6464 2061 6e64 2073 7562   can add and sub
+00000970: 7472 6163 7420 696d 6167 6520 616e 6420  tract image and 
+00000980: 7465 7874 2071 7565 7269 6573 2066 726f  text queries fro
+00000990: 6d20 6561 6368 206f 7468 6572 3b20 6865  m each other; he
+000009a0: 7265 2061 7265 2061 2066 6577 2075 7361  re are a few usa
+000009b0: 6765 2065 7861 6d70 6c65 733a 0a0a 6060  ge examples:..``
+000009c0: 6062 6173 680a 6364 2070 686f 746f 7320  `bash.cd photos 
+000009d0: 2626 2072 636c 6970 2068 6f72 7365 202b  && rclip horse +
+000009e0: 2073 7472 6970 6573 0a63 6420 7068 6f74   stripes.cd phot
+000009f0: 6f73 2026 2620 7263 6c69 7020 6170 706c  os && rclip appl
+00000a00: 6520 2d20 6672 7569 740a 6364 2070 686f  e - fruit.cd pho
+00000a10: 746f 7320 2626 2072 636c 6970 2022 2e2f  tos && rclip "./
+00000a20: 6e65 7720 796f 726b 2063 6974 792e 6a70  new york city.jp
+00000a30: 6722 202b 206e 6967 6874 0a63 6420 7068  g" + night.cd ph
+00000a40: 6f74 6f73 2026 2620 7263 6c69 7020 2232  otos && rclip "2
+00000a50: 3a67 6f6c 6465 6e20 7265 7472 6965 7665  :golden retrieve
+00000a60: 7222 202b 2022 2e2f 7377 696d 6d69 6e67  r" + "./swimming
+00000a70: 2070 6f6f 6c2e 6a70 6722 0a63 6420 7068   pool.jpg".cd ph
+00000a80: 6f74 6f73 2026 2620 7263 6c69 7020 222e  otos && rclip ".
+00000a90: 2f72 6163 696e 6720 6361 722e 6a70 6722  /racing car.jpg"
+00000aa0: 202d 2022 323a 7370 6f72 7473 2063 6172   - "2:sports car
+00000ab0: 2220 2b20 2232 3a73 6e6f 7722 0a60 6060  " + "2:snow".```
+00000ac0: 0a0a 4966 2079 6f75 2077 616e 7420 746f  ..If you want to
+00000ad0: 2073 6565 2068 6f77 2074 6865 7365 2071   see how these q
+00000ae0: 7565 7269 6573 2070 6572 666f 726d 2077  ueries perform w
+00000af0: 6865 6e20 6578 6563 7574 6564 206f 6e20  hen executed on 
+00000b00: 7468 6520 312e 3238 206d 696c 6c69 6f6e  the 1.28 million
+00000b10: 2069 6d61 6765 7320 496d 6167 654e 6574   images ImageNet
+00000b20: 2d31 6b20 6461 7461 7365 742c 2063 6865  -1k dataset, che
+00000b30: 636b 206f 7574 2074 6865 2064 656d 6f20  ck out the demo 
+00000b40: 6f6e 2059 6f75 5475 6265 3a20 6874 7470  on YouTube: http
+00000b50: 733a 2f2f 7777 772e 796f 7574 7562 652e  s://www.youtube.
+00000b60: 636f 6d2f 7761 7463 683f 763d 4d73 5467  com/watch?v=MsTg
+00000b70: 5964 4f70 6763 512e 0a0a 2323 2320 486f  YdOpgcQ...### Ho
+00000b80: 7720 646f 2049 2070 7265 7669 6577 2074  w do I preview t
+00000b90: 6865 2072 6573 756c 7473 3f0a 0a54 6865  he results?..The
+00000ba0: 2063 6f6d 6d61 6e64 2066 726f 6d20 6265   command from be
+00000bb0: 6c6f 7720 7769 6c6c 206f 7065 6e20 746f  low will open to
+00000bc0: 702d 3520 7265 7375 6c74 7320 666f 7220  p-5 results for 
+00000bd0: 226b 6974 7479 2220 696e 2079 6f75 7220  "kitty" in your 
+00000be0: 6465 6661 756c 7420 696d 6167 6520 7669  default image vi
+00000bf0: 6577 6572 3a0a 0a60 6060 6261 7368 0a72  ewer:..```bash.r
+00000c00: 636c 6970 202d 6620 2d74 2035 206b 6974  clip -f -t 5 kit
+00000c10: 7479 207c 2078 6172 6773 202d 6420 275c  ty | xargs -d '\
+00000c20: 6e27 202d 6e20 3120 7864 672d 6f70 656e  n' -n 1 xdg-open
+00000c30: 0a60 6060 0a0a 4920 7072 6566 6572 2074  .```..I prefer t
+00000c40: 6f20 7573 6520 6066 6568 6027 7320 7468  o use `feh`'s th
+00000c50: 756d 626e 6169 6c20 6d6f 6465 2074 6f20  umbnail mode to 
+00000c60: 7072 6576 6965 7720 6d75 6c74 6970 6c65  preview multiple
+00000c70: 2072 6573 756c 7473 3a0a 0a60 6060 6261   results:..```ba
+00000c80: 7368 0a72 636c 6970 202d 6620 2d74 2035  sh.rclip -f -t 5
+00000c90: 206b 6974 7479 207c 2066 6568 202d 6620   kitty | feh -f 
+00000ca0: 2d20 2d74 0a60 6060 0a0a 2323 2048 656c  - -t.```..## Hel
+00000cb0: 700a 0a60 6060 6261 7368 0a72 636c 6970  p..```bash.rclip
+00000cc0: 202d 2d68 656c 700a 6060 600a 0a23 2320   --help.```..## 
+00000cd0: 436f 6e74 7269 6275 7469 6e67 0a0a 5468  Contributing..Th
+00000ce0: 6973 2072 6570 6f73 6974 6f72 7920 666f  is repository fo
+00000cf0: 6c6c 6f77 7320 7468 6520 5b43 6f6e 7665  llows the [Conve
+00000d00: 6e74 696f 6e61 6c20 436f 6d6d 6974 735d  ntional Commits]
+00000d10: 2868 7474 7073 3a2f 2f77 7777 2e63 6f6e  (https://www.con
+00000d20: 7665 6e74 696f 6e61 6c63 6f6d 6d69 7473  ventionalcommits
+00000d30: 2e6f 7267 2f65 6e2f 7631 2e30 2e30 2f29  .org/en/v1.0.0/)
+00000d40: 2073 7461 6e64 6172 642e 0a0a 2323 2320   standard...### 
+00000d50: 5275 6e6e 696e 6720 6c6f 6361 6c6c 7920  Running locally 
+00000d60: 6672 6f6d 2074 6865 2073 6f75 7263 6520  from the source 
+00000d70: 636f 6465 0a0a 546f 2072 756e 202a 2a72  code..To run **r
+00000d80: 636c 6970 2a2a 206c 6f63 616c 6c79 2066  clip** locally f
+00000d90: 726f 6d20 7468 6520 736f 7572 6365 2063  rom the source c
+00000da0: 6f64 652c 2079 6f75 206d 7573 7420 6861  ode, you must ha
+00000db0: 7665 205b 5079 7468 6f6e 5d28 6874 7470  ve [Python](http
+00000dc0: 733a 2f2f 7777 772e 7079 7468 6f6e 2e6f  s://www.python.o
+00000dd0: 7267 2f64 6f77 6e6c 6f61 6473 2f29 2061  rg/downloads/) a
+00000de0: 6e64 205b 506f 6574 7279 5d28 6874 7470  nd [Poetry](http
+00000df0: 733a 2f2f 7079 7468 6f6e 2d70 6f65 7472  s://python-poetr
+00000e00: 792e 6f72 672f 2920 696e 7374 616c 6c65  y.org/) installe
+00000e10: 642e 0a0a 5468 656e 2064 6f3a 0a60 6060  d...Then do:.```
+00000e20: 6261 7368 0a23 2063 6c6f 6e65 2074 6865  bash.# clone the
+00000e30: 2073 6f75 7263 6520 636f 6465 2072 6570   source code rep
+00000e40: 6f73 6974 6f72 790a 6769 7420 636c 6f6e  ository.git clon
+00000e50: 6520 6769 7440 6769 7468 7562 2e63 6f6d  e git@github.com
+00000e60: 3a79 7572 696a 6d69 6b68 616c 6576 6963  :yurijmikhalevic
+00000e70: 682f 7263 6c69 702e 6769 740a 0a23 2069  h/rclip.git..# i
+00000e80: 6e73 7461 6c6c 2064 6570 656e 6465 6e63  nstall dependenc
+00000e90: 6965 7320 616e 6420 7263 6c69 700a 6364  ies and rclip.cd
+00000ea0: 2072 636c 6970 0a70 6f65 7472 7920 696e   rclip.poetry in
+00000eb0: 7374 616c 6c0a 0a23 2061 6374 6976 6174  stall..# activat
+00000ec0: 6520 7468 6520 6e65 7720 706f 6574 7279  e the new poetry
+00000ed0: 2065 6e76 6972 6f6e 6d65 6e74 0a70 6f65   environment.poe
+00000ee0: 7472 7920 7368 656c 6c0a 6060 600a 0a49  try shell.```..I
+00000ef0: 6620 7468 6520 706f 6574 7279 2065 6e76  f the poetry env
+00000f00: 6972 6f6e 6d65 6e74 2069 7320 6163 7469  ironment is acti
+00000f10: 7665 2c20 796f 7520 6361 6e20 7573 6520  ve, you can use 
+00000f20: 2a2a 7263 6c69 702a 2a20 6c6f 6361 6c6c  **rclip** locall
+00000f30: 792c 2061 7320 6465 7363 7269 6265 6420  y, as described 
+00000f40: 696e 2074 6865 205b 5573 6167 655d 2823  in the [Usage](#
+00000f50: 7573 6167 6529 2073 6563 7469 6f6e 2061  usage) section a
+00000f60: 626f 7665 2e0a 0a23 2320 436f 6e74 7269  bove...## Contri
+00000f70: 6275 746f 7273 20e2 9ca8 0a0a 5468 616e  butors .....Than
+00000f80: 6b73 2067 6f20 746f 2074 6865 7365 2077  ks go to these w
+00000f90: 6f6e 6465 7266 756c 2070 656f 706c 6520  onderful people 
+00000fa0: 285b 656d 6f6a 6920 6b65 795d 2868 7474  ([emoji key](htt
+00000fb0: 7073 3a2f 2f61 6c6c 636f 6e74 7269 6275  ps://allcontribu
+00000fc0: 746f 7273 2e6f 7267 2f64 6f63 732f 656e  tors.org/docs/en
+00000fd0: 2f65 6d6f 6a69 2d6b 6579 2929 3a0a 0a3c  /emoji-key)):..<
+00000fe0: 212d 2d20 414c 4c2d 434f 4e54 5249 4255  !-- ALL-CONTRIBU
+00000ff0: 544f 5253 2d4c 4953 543a 5354 4152 5420  TORS-LIST:START 
+00001000: 2d20 446f 206e 6f74 2072 656d 6f76 6520  - Do not remove 
+00001010: 6f72 206d 6f64 6966 7920 7468 6973 2073  or modify this s
+00001020: 6563 7469 6f6e 202d 2d3e 0a3c 212d 2d20  ection -->.<!-- 
+00001030: 7072 6574 7469 6572 2d69 676e 6f72 652d  prettier-ignore-
+00001040: 7374 6172 7420 2d2d 3e0a 3c21 2d2d 206d  start -->.<!-- m
+00001050: 6172 6b64 6f77 6e6c 696e 742d 6469 7361  arkdownlint-disa
+00001060: 626c 6520 2d2d 3e0a 3c74 6162 6c65 3e0a  ble -->.<table>.
+00001070: 2020 3c74 723e 0a20 2020 203c 7464 2061    <tr>.    <td a
+00001080: 6c69 676e 3d22 6365 6e74 6572 223e 3c61  lign="center"><a
+00001090: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+000010a0: 6974 6875 622e 636f 6d2f 7261 6d61 7965  ithub.com/ramaye
+000010b0: 7222 3e3c 696d 6720 7372 633d 2268 7474  r"><img src="htt
+000010c0: 7073 3a2f 2f61 7661 7461 7273 2e67 6974  ps://avatars.git
+000010d0: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+000010e0: 6f6d 2f75 2f37 3233 3230 3f76 3d34 3f73  om/u/72320?v=4?s
+000010f0: 3d31 3030 2220 7769 6474 683d 2231 3030  =100" width="100
+00001100: 7078 3b22 2061 6c74 3d22 222f 3e3c 6272  px;" alt=""/><br
+00001110: 202f 3e3c 7375 623e 3c62 3e72 616d 6179   /><sub><b>ramay
+00001120: 6572 3c2f 623e 3c2f 7375 623e 3c2f 613e  er</b></sub></a>
+00001130: 3c62 7220 2f3e 3c61 2068 7265 663d 2268  <br /><a href="h
+00001140: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001150: 6d2f 7975 7269 6a6d 696b 6861 6c65 7669  m/yurijmikhalevi
+00001160: 6368 2f72 636c 6970 2f63 6f6d 6d69 7473  ch/rclip/commits
+00001170: 3f61 7574 686f 723d 7261 6d61 7965 7222  ?author=ramayer"
+00001180: 2074 6974 6c65 3d22 436f 6465 223e f09f   title="Code">..
+00001190: 92bb 3c2f 613e 3c2f 7464 3e0a 2020 3c2f  ..</a></td>.  </
+000011a0: 7472 3e0a 3c2f 7461 626c 653e 0a0a 3c21  tr>.</table>..<!
+000011b0: 2d2d 206d 6172 6b64 6f77 6e6c 696e 742d  -- markdownlint-
+000011c0: 7265 7374 6f72 6520 2d2d 3e0a 3c21 2d2d  restore -->.<!--
+000011d0: 2070 7265 7474 6965 722d 6967 6e6f 7265   prettier-ignore
+000011e0: 2d65 6e64 202d 2d3e 0a0a 3c21 2d2d 2041  -end -->..<!-- A
+000011f0: 4c4c 2d43 4f4e 5452 4942 5554 4f52 532d  LL-CONTRIBUTORS-
+00001200: 4c49 5354 3a45 4e44 202d 2d3e 0a0a 5468  LIST:END -->..Th
+00001210: 6973 2070 726f 6a65 6374 2066 6f6c 6c6f  is project follo
+00001220: 7773 2074 6865 205b 616c 6c2d 636f 6e74  ws the [all-cont
+00001230: 7269 6275 746f 7273 5d28 6874 7470 733a  ributors](https:
+00001240: 2f2f 6769 7468 7562 2e63 6f6d 2f61 6c6c  //github.com/all
+00001250: 2d63 6f6e 7472 6962 7574 6f72 732f 616c  -contributors/al
+00001260: 6c2d 636f 6e74 7269 6275 746f 7273 2920  l-contributors) 
+00001270: 7370 6563 6966 6963 6174 696f 6e2e 2043  specification. C
+00001280: 6f6e 7472 6962 7574 696f 6e73 206f 6620  ontributions of 
+00001290: 616e 7920 6b69 6e64 2061 7265 2077 656c  any kind are wel
+000012a0: 636f 6d65 210a 0a23 2320 4c69 6365 6e73  come!..## Licens
+000012b0: 650a 0a4d 4954 0a                        e..MIT.
```

### Comparing `rclip-1.4.2/pyproject.toml` & `rclip-1.4.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rclip"
-version = "1.4.2"
+version = "1.4.3"
 description = "AI-Powered Command-Line Photo Search Tool"
 authors = ["Yurij Mikhalevich <yurij@mikhalevi.ch>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/yurijmikhalevich/rclip"
 keywords = ["image search", "computer vision", "photography"]
 classifiers = [
@@ -14,17 +14,17 @@
   "Topic :: Scientific/Engineering :: Artificial Intelligence",
   "Topic :: Scientific/Engineering :: Image Processing",
   "Topic :: Scientific/Engineering :: Image Recognition",
   "Topic :: Utilities",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.10"
+python = "^3.8"
 open_clip_torch = "^2.20.0"
-pillow = ">=9.0.1"
+pillow = "^9.0.1"
 requests = "~=2.26"
 torch = [
   { version = "==2.0.1", source = "pypi", markers = "sys_platform != 'linux'" },
   { version = "==2.0.1+cpu", source = "pytorch-cpu", markers = "sys_platform == 'linux'" }
 ]
 torchvision = [
   { version = "==0.15.2", source = "pypi", markers = "sys_platform != 'linux'" },
```

### Comparing `rclip-1.4.2/rclip/db.py` & `rclip-1.4.3/rclip/db.py`

 * *Files identical despite different names*

### Comparing `rclip-1.4.2/rclip/main.py` & `rclip-1.4.3/rclip/main.py`

 * *Files identical despite different names*

### Comparing `rclip-1.4.2/rclip/model.py` & `rclip-1.4.3/rclip/model.py`

 * *Files identical despite different names*

### Comparing `rclip-1.4.2/rclip/utils.py` & `rclip-1.4.3/rclip/utils.py`

 * *Files identical despite different names*

### Comparing `rclip-1.4.2/PKG-INFO` & `rclip-1.4.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: rclip
-Version: 1.4.2
+Version: 1.4.3
 Summary: AI-Powered Command-Line Photo Search Tool
 Home-page: https://github.com/yurijmikhalevich/rclip
 License: MIT
 Keywords: image search,computer vision,photography
 Author: Yurij Mikhalevich
 Author-email: yurij@mikhalevi.ch
-Requires-Python: >=3.8,<3.10
+Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Topic :: Utilities
 Requires-Dist: open_clip_torch (>=2.20.0,<3.0.0)
-Requires-Dist: pillow (>=9.0.1)
+Requires-Dist: pillow (>=9.0.1,<10.0.0)
 Requires-Dist: requests (>=2.26,<3.0)
 Requires-Dist: torch (==2.0.1) ; sys_platform != "linux"
 Requires-Dist: torch (==2.0.1+cpu) ; sys_platform == "linux"
 Requires-Dist: torchvision (==0.15.2) ; sys_platform != "linux"
 Requires-Dist: torchvision (==0.15.2+cpu) ; sys_platform == "linux"
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Project-URL: Repository, https://github.com/yurijmikhalevich/rclip
@@ -64,25 +66,41 @@
 
 <img alt="rclip usage demo" src="https://raw.githubusercontent.com/yurijmikhalevich/rclip/main/resources/rclip-usage.gif" width="640px" />
 
 When you run **rclip** for the first time in a particular directory, it's going to extract features from the photos, and this takes time. How long it takes depends on your CPU and the number of pictures you will search through. It took about a day to process 73 thousand photos on my NAS, which runs an old-ish Intel Celeron J3455.
 
 For a detailed demonstration, watch the video: https://www.youtube.com/watch?v=tAJHXOkHidw.
 
-You can also use another image as a query by passing a file path or even an URL to the image file, and **rclip** will find the images most similar to the one you used as a query. If you are referencing a local image via a relative path, you **must** prefix it with `./`. For example:
+### Similar image search
+
+You can use another image as a query by passing a file path or even an URL to the image file, and **rclip** will find the images most similar to the one you used as a query. If you are referencing a local image via a relative path, you **must** prefix it with `./`. For example:
 
 ```bash
 cd photos && rclip ./cat.jpg
 
 # or use URL
 cd photos && rclip https://raw.githubusercontent.com/yurijmikhalevich/rclip/main/tests/e2e/images/cat.jpg
 ```
 
 Check this video out for the image-to-image search demo: https://www.youtube.com/watch?v=1YQZKeCBxWM.
 
+### Combining multiple queries
+
+You can add and subtract image and text queries from each other; here are a few usage examples:
+
+```bash
+cd photos && rclip horse + stripes
+cd photos && rclip apple - fruit
+cd photos && rclip "./new york city.jpg" + night
+cd photos && rclip "2:golden retriever" + "./swimming pool.jpg"
+cd photos && rclip "./racing car.jpg" - "2:sports car" + "2:snow"
+```
+
+If you want to see how these queries perform when executed on the 1.28 million images ImageNet-1k dataset, check out the demo on YouTube: https://www.youtube.com/watch?v=MsTgYdOpgcQ.
+
 ### How do I preview the results?
 
 The command from below will open top-5 results for "kitty" in your default image viewer:
 
 ```bash
 rclip -f -t 5 kitty | xargs -d '\n' -n 1 xdg-open
 ```
```

