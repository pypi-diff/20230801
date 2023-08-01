# Comparing `tmp/heroprotocol-2.55.3.89754.tar.gz` & `tmp/heroprotocol-2.55.3.90670.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\heroprotocol-2.55.3.89754.tar", last modified: Tue Feb  7 22:23:54 2023, max compression
+gzip compressed data, was "dist\heroprotocol-2.55.3.90670.tar", last modified: Mon Jul 31 23:49:53 2023, max compression
```

## Comparing `heroprotocol-2.55.3.89754.tar` & `heroprotocol-2.55.3.90670.tar`

### file list

```diff
@@ -1,340 +1,342 @@
-drwxrwxrwx   0        0        0        0 2023-02-07 22:23:54.789165 heroprotocol-2.55.3.89754/
--rw-rw-rw-   0        0        0     7574 2023-02-07 22:23:54.787158 heroprotocol-2.55.3.89754/PKG-INFO
--rw-rw-rw-   0        0        0     5545 2021-06-19 16:13:55.000000 heroprotocol-2.55.3.89754/README.md
-drwxrwxrwx   0        0        0        0 2023-02-07 22:23:53.299790 heroprotocol-2.55.3.89754/heroprotocol/
--rw-rw-rw-   0        0        0      316 2023-02-07 22:23:46.000000 heroprotocol-2.55.3.89754/heroprotocol/__init__.py
--rw-rw-rw-   0        0        0      206 2021-06-19 16:13:55.000000 heroprotocol-2.55.3.89754/heroprotocol/__main__.py
--rw-rw-rw-   0        0        0     1081 2023-02-07 22:23:46.000000 heroprotocol-2.55.3.89754/heroprotocol/build.py
--rw-rw-rw-   0        0        0      352 2021-06-19 16:13:55.000000 heroprotocol-2.55.3.89754/heroprotocol/compat.py
--rw-rw-rw-   0        0        0     9512 2021-06-19 16:13:55.000000 heroprotocol-2.55.3.89754/heroprotocol/decoders.py
--rw-rw-rw-   0        0        0     4570 2021-06-19 16:13:55.000000 heroprotocol-2.55.3.89754/heroprotocol/hero_cli.py
-drwxrwxrwx   0        0        0        0 2023-02-07 22:23:54.784159 heroprotocol-2.55.3.89754/heroprotocol/versions/
--rw-rw-rw-   0        0        0     2153 2021-06-19 16:13:55.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/__init__.py
--rw-rw-rw-   0        0        0    28330 2021-06-19 16:13:55.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol29406.py
--rw-rw-rw-   0        0        0    28582 2021-06-19 16:24:24.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol30414.py
--rw-rw-rw-   0        0        0    28582 2021-06-19 16:24:26.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol30509.py
--rw-rw-rw-   0        0        0    28582 2021-06-19 16:24:27.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol30829.py
--rw-rw-rw-   0        0        0    28582 2021-06-19 16:24:29.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol30948.py
--rw-rw-rw-   0        0        0    28582 2021-06-19 16:24:30.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol31090.py
--rw-rw-rw-   0        0        0    28698 2021-06-19 16:24:32.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol31360.py
--rw-rw-rw-   0        0        0    28698 2021-06-19 16:24:34.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol31566.py
--rw-rw-rw-   0        0        0    28698 2021-06-19 16:24:35.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol31726.py
--rw-rw-rw-   0        0        0    28698 2021-06-19 16:24:37.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol31948.py
--rw-rw-rw-   0        0        0    28690 2021-06-19 16:24:38.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol32120.py
--rw-rw-rw-   0        0        0    28690 2021-06-19 16:24:39.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol32253.py
--rw-rw-rw-   0        0        0    28838 2021-06-19 16:24:41.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol32455.py
--rw-rw-rw-   0        0        0    28838 2021-06-19 16:24:42.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol32524.py
--rw-rw-rw-   0        0        0    29057 2021-06-19 16:24:44.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol33182.py
--rw-rw-rw-   0        0        0    29057 2021-06-19 16:24:45.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol33353.py
--rw-rw-rw-   0        0        0    29196 2021-06-19 16:24:47.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol33684.py
--rw-rw-rw-   0        0        0    29261 2021-06-19 16:24:48.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol34053.py
--rw-rw-rw-   0        0        0    29261 2021-06-19 16:24:50.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol34190.py
--rw-rw-rw-   0        0        0    29261 2021-06-19 16:24:51.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol34659.py
--rw-rw-rw-   0        0        0    29261 2021-06-19 16:24:52.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol34846.py
--rw-rw-rw-   0        0        0    29314 2021-06-19 16:24:54.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol35360.py
--rw-rw-rw-   0        0        0    29314 2021-06-19 16:24:55.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol35529.py
--rw-rw-rw-   0        0        0    29314 2021-06-19 16:13:55.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol35634.py
--rw-rw-rw-   0        0        0    29314 2021-06-19 16:24:57.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol35702.py
--rw-rw-rw-   0        0        0    29314 2021-06-19 16:24:58.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol36144.py
--rw-rw-rw-   0        0        0    29314 2021-06-19 16:25:00.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol36280.py
--rw-rw-rw-   0        0        0    29314 2021-06-19 16:25:01.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol36359.py
--rw-rw-rw-   0        0        0    29314 2021-06-19 16:25:03.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol36536.py
--rw-rw-rw-   0        0        0    29314 2021-06-19 16:25:04.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol36693.py
--rw-rw-rw-   0        0        0    29646 2021-06-19 16:25:06.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol37069.py
--rw-rw-rw-   0        0        0    29646 2021-06-19 16:25:07.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol37117.py
--rw-rw-rw-   0        0        0    29646 2021-06-19 16:13:55.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol37274.py
--rw-rw-rw-   0        0        0    29646 2021-06-19 16:25:08.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol37351.py
--rw-rw-rw-   0        0        0    29646 2021-06-19 16:25:10.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol37569.py
--rw-rw-rw-   0        0        0    29646 2021-06-19 16:13:55.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol37795.py
--rw-rw-rw-   0        0        0    29691 2021-06-19 16:25:11.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol38236.py
--rw-rw-rw-   0        0        0    29691 2021-06-19 16:25:13.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol38500.py
--rw-rw-rw-   0        0        0    29691 2021-06-19 16:25:14.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol38593.py
--rw-rw-rw-   0        0        0    29691 2021-06-19 16:25:16.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol38793.py
--rw-rw-rw-   0        0        0    29691 2021-06-19 16:25:17.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol39015.py
--rw-rw-rw-   0        0        0    29691 2021-06-19 16:25:19.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol39153.py
--rw-rw-rw-   0        0        0    29691 2021-06-19 16:25:20.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol39271.py
--rw-rw-rw-   0        0        0    29691 2021-06-19 16:25:22.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol39445.py
--rw-rw-rw-   0        0        0    29691 2021-06-19 16:25:23.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol39595.py
--rw-rw-rw-   0        0        0    29691 2021-06-19 16:25:24.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol39709.py
--rw-rw-rw-   0        0        0    29691 2021-06-19 16:25:26.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol39951.py
--rw-rw-rw-   0        0        0    29691 2021-06-19 16:25:27.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol40087.py
--rw-rw-rw-   0        0        0    29691 2021-06-19 16:25:29.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol40322.py
--rw-rw-rw-   0        0        0    30706 2021-06-19 16:13:55.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol40336.py
--rw-rw-rw-   0        0        0    30706 2021-06-19 16:25:30.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol40431.py
--rw-rw-rw-   0        0        0    30706 2021-06-19 16:25:32.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol40697.py
--rw-rw-rw-   0        0        0    30706 2021-06-19 16:25:33.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol40798.py
--rw-rw-rw-   0        0        0    31128 2021-06-19 16:25:35.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol41150.py
--rw-rw-rw-   0        0        0    31128 2021-06-19 16:25:36.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol41393.py
--rw-rw-rw-   0        0        0    31128 2021-06-19 16:25:38.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol41504.py
--rw-rw-rw-   0        0        0    26364 2021-06-19 16:25:39.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol41609.py
--rw-rw-rw-   0        0        0    26364 2021-06-19 16:25:40.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol41707.py
--rw-rw-rw-   0        0        0    26364 2021-06-19 16:25:42.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol41764.py
--rw-rw-rw-   0        0        0    26364 2021-06-19 16:25:43.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol41810.py
--rw-rw-rw-   0        0        0    26364 2021-06-19 16:25:44.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol42178.py
--rw-rw-rw-   0        0        0    26364 2021-06-19 16:25:46.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol42273.py
--rw-rw-rw-   0        0        0    26364 2021-06-19 16:25:47.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol42406.py
--rw-rw-rw-   0        0        0    26364 2021-06-19 16:25:49.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol42506.py
--rw-rw-rw-   0        0        0    26364 2021-06-19 16:25:50.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol42590.py
--rw-rw-rw-   0        0        0    26364 2021-06-19 16:25:51.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol42742.py
--rw-rw-rw-   0        0        0    26364 2021-06-19 16:25:53.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol42958.py
--rw-rw-rw-   0        0        0    26364 2021-06-19 16:25:54.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol43051.py
--rw-rw-rw-   0        0        0    26364 2021-06-19 16:25:56.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol43170.py
--rw-rw-rw-   0        0        0    26364 2021-06-19 16:25:57.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol43259.py
--rw-rw-rw-   0        0        0    26364 2021-06-19 16:25:58.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol43481.py
--rw-rw-rw-   0        0        0    26364 2021-06-19 16:26:00.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol43527.py
--rw-rw-rw-   0        0        0    26364 2021-06-19 16:26:01.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol43571.py
--rw-rw-rw-   0        0        0    26383 2021-06-19 16:26:02.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol43905.py
--rw-rw-rw-   0        0        0    26383 2021-06-19 16:26:04.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol44124.py
--rw-rw-rw-   0        0        0    26434 2021-06-19 16:26:05.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol44256.py
--rw-rw-rw-   0        0        0    26434 2021-06-19 16:26:07.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol44468.py
--rw-rw-rw-   0        0        0    26434 2021-06-19 16:26:08.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol44737.py
--rw-rw-rw-   0        0        0    26434 2021-06-19 16:26:09.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol44797.py
--rw-rw-rw-   0        0        0    26434 2021-06-19 16:26:11.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol44941.py
--rw-rw-rw-   0        0        0    26434 2021-06-19 16:26:12.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol45024.py
--rw-rw-rw-   0        0        0    26434 2021-06-19 16:26:13.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol45228.py
--rw-rw-rw-   0        0        0    26434 2021-06-19 16:26:15.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol45635.py
--rw-rw-rw-   0        0        0    26459 2021-06-19 16:26:16.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol45815.py
--rw-rw-rw-   0        0        0    26459 2021-06-19 16:26:18.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol45889.py
--rw-rw-rw-   0        0        0    26459 2021-06-19 16:26:19.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol45949.py
--rw-rw-rw-   0        0        0    26459 2021-06-19 16:26:20.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol46158.py
--rw-rw-rw-   0        0        0    26459 2021-06-19 16:26:22.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol46416.py
--rw-rw-rw-   0        0        0    26459 2021-06-19 16:26:23.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol46446.py
--rw-rw-rw-   0        0        0    26459 2021-06-19 16:26:24.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol46690.py
--rw-rw-rw-   0        0        0    26459 2021-06-19 16:26:26.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol46787.py
--rw-rw-rw-   0        0        0    26459 2021-06-19 16:26:27.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol46869.py
--rw-rw-rw-   0        0        0    26459 2021-06-19 16:26:29.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol46889.py
--rw-rw-rw-   0        0        0    26459 2021-06-19 16:26:30.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol47024.py
--rw-rw-rw-   0        0        0    26459 2021-06-19 16:26:31.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol47133.py
--rw-rw-rw-   0        0        0    26459 2021-06-19 16:26:33.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol47219.py
--rw-rw-rw-   0        0        0    26459 2021-06-19 16:26:34.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol47479.py
--rw-rw-rw-   0        0        0    26459 2021-06-19 16:26:35.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol47801.py
--rw-rw-rw-   0        0        0    26459 2021-06-19 16:26:37.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol47903.py
--rw-rw-rw-   0        0        0    26459 2021-06-19 16:26:38.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol47944.py
--rw-rw-rw-   0        0        0    26459 2021-06-19 16:26:40.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol48027.py
--rw-rw-rw-   0        0        0    26459 2021-06-19 16:26:41.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol48297.py
--rw-rw-rw-   0        0        0    26459 2021-06-19 16:26:42.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol48548.py
--rw-rw-rw-   0        0        0    26459 2021-06-19 16:26:44.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol48583.py
--rw-rw-rw-   0        0        0    26459 2021-06-19 16:26:45.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol48760.py
--rw-rw-rw-   0        0        0    26459 2021-06-19 16:26:46.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol49008.py
--rw-rw-rw-   0        0        0    26459 2021-06-19 16:26:48.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol49076.py
--rw-rw-rw-   0        0        0    26459 2021-06-19 16:26:49.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol49278.py
--rw-rw-rw-   0        0        0    26459 2021-06-19 16:26:51.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol49495.py
--rw-rw-rw-   0        0        0    26447 2021-06-19 16:26:52.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol49582.py
--rw-rw-rw-   0        0        0    26447 2021-06-19 16:26:53.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol49747.py
--rw-rw-rw-   0        0        0    26459 2021-06-19 16:26:55.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol49838.py
--rw-rw-rw-   0        0        0    26447 2021-06-19 16:26:56.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol49907.py
--rw-rw-rw-   0        0        0    26447 2021-06-19 16:26:58.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol50286.py
--rw-rw-rw-   0        0        0    26447 2021-06-19 16:26:59.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol50424.py
--rw-rw-rw-   0        0        0    26447 2021-06-19 16:27:01.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol50441.py
--rw-rw-rw-   0        0        0    26447 2021-06-19 16:27:02.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol50673.py
--rw-rw-rw-   0        0        0    26447 2021-06-19 16:27:04.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol50950.py
--rw-rw-rw-   0        0        0    26447 2021-06-19 16:27:05.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol51150.py
--rw-rw-rw-   0        0        0    26447 2021-06-19 16:27:07.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol51375.py
--rw-rw-rw-   0        0        0    26447 2021-06-19 16:27:08.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol51609.py
--rw-rw-rw-   0        0        0    26447 2021-06-19 16:27:10.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol51779.py
--rw-rw-rw-   0        0        0    26447 2021-06-19 16:27:11.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol51923.py
--rw-rw-rw-   0        0        0    26888 2021-06-19 16:27:12.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol51978.py
--rw-rw-rw-   0        0        0    26447 2021-06-19 16:27:14.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol52008.py
--rw-rw-rw-   0        0        0    26447 2021-06-19 16:27:15.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol52124.py
--rw-rw-rw-   0        0        0    26888 2021-06-19 16:27:17.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol52214.py
--rw-rw-rw-   0        0        0    26447 2021-06-19 16:27:18.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol52351.py
--rw-rw-rw-   0        0        0    26888 2021-06-19 16:27:19.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol52381.py
--rw-rw-rw-   0        0        0    27019 2021-06-19 16:27:21.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol52561.py
--rw-rw-rw-   0        0        0    26447 2021-06-19 16:27:22.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol52647.py
--rw-rw-rw-   0        0        0    27019 2021-06-19 16:27:24.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol52860.py
--rw-rw-rw-   0        0        0    27019 2021-06-19 16:27:25.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol52986.py
--rw-rw-rw-   0        0        0    27019 2021-06-19 16:27:26.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol53174.py
--rw-rw-rw-   0        0        0    27019 2021-06-19 16:27:28.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol53270.py
--rw-rw-rw-   0        0        0    27019 2021-06-19 16:27:29.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol53275.py
--rw-rw-rw-   0        0        0    27019 2021-06-19 16:27:31.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol53548.py
--rw-rw-rw-   0        0        0    27019 2021-06-19 16:27:32.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol53965.py
--rw-rw-rw-   0        0        0    27019 2021-06-19 16:27:33.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol54098.py
--rw-rw-rw-   0        0        0    27019 2021-06-19 16:27:35.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol54339.py
--rw-rw-rw-   0        0        0    27019 2021-06-19 16:27:36.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol54968.py
--rw-rw-rw-   0        0        0    27019 2021-06-19 16:27:37.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol55010.py
--rw-rw-rw-   0        0        0    27019 2021-06-19 16:27:39.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol55058.py
--rw-rw-rw-   0        0        0    27019 2021-06-19 16:27:40.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol55288.py
--rw-rw-rw-   0        0        0    27019 2021-06-19 16:27:42.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol55844.py
--rw-rw-rw-   0        0        0    27019 2021-06-19 16:27:43.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol55929.py
--rw-rw-rw-   0        0        0    27019 2021-06-19 16:27:44.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol56175.py
--rw-rw-rw-   0        0        0    27019 2021-06-19 16:27:46.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol56361.py
--rw-rw-rw-   0        0        0    27019 2021-06-19 16:27:47.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol56705.py
--rw-rw-rw-   0        0        0    27019 2021-06-19 16:27:49.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol56784.py
--rw-rw-rw-   0        0        0    27019 2021-06-19 16:27:50.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol56859.py
--rw-rw-rw-   0        0        0    27019 2021-06-19 16:27:51.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol57062.py
--rw-rw-rw-   0        0        0    27019 2021-06-19 16:27:53.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol57286.py
--rw-rw-rw-   0        0        0    27092 2021-06-19 16:27:54.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol57547.py
--rw-rw-rw-   0        0        0    27019 2021-06-19 16:27:56.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol57589.py
--rw-rw-rw-   0        0        0    27092 2021-06-19 16:27:57.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol57797.py
--rw-rw-rw-   0        0        0    27092 2021-06-19 16:27:58.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol58209.py
--rw-rw-rw-   0        0        0    27092 2021-06-19 16:28:00.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol58344.py
--rw-rw-rw-   0        0        0    27092 2021-06-19 16:28:01.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol58482.py
--rw-rw-rw-   0        0        0    27092 2021-06-19 16:28:03.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol58623.py
--rw-rw-rw-   0        0        0    27092 2021-06-19 16:28:04.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol58795.py
--rw-rw-rw-   0        0        0    27092 2021-06-19 16:28:05.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol59239.py
--rw-rw-rw-   0        0        0    27126 2021-06-19 16:28:07.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol59279.py
--rw-rw-rw-   0        0        0    27126 2021-06-19 16:28:08.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol59657.py
--rw-rw-rw-   0        0        0    27126 2021-06-19 16:28:10.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol59799.py
--rw-rw-rw-   0        0        0    27126 2021-06-19 16:28:11.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol59837.py
--rw-rw-rw-   0        0        0    27126 2021-06-19 16:28:12.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol59944.py
--rw-rw-rw-   0        0        0    27126 2021-06-19 16:28:14.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol59988.py
--rw-rw-rw-   0        0        0    27126 2021-06-19 16:28:15.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol60228.py
--rw-rw-rw-   0        0        0    27126 2021-06-19 16:28:17.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol60265.py
--rw-rw-rw-   0        0        0    27126 2021-06-19 16:28:18.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol60399.py
--rw-rw-rw-   0        0        0    27126 2021-06-19 16:28:19.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol60522.py
--rw-rw-rw-   0        0        0    27126 2021-06-19 16:28:21.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol60567.py
--rw-rw-rw-   0        0        0    27126 2021-06-19 16:28:22.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol60632.py
--rw-rw-rw-   0        0        0    27126 2021-06-19 16:28:24.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol60821.py
--rw-rw-rw-   0        0        0    27126 2021-06-19 16:28:26.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol61129.py
--rw-rw-rw-   0        0        0    27126 2021-06-19 16:28:27.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol61361.py
--rw-rw-rw-   0        0        0    27126 2021-06-19 16:28:29.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol61552.py
--rw-rw-rw-   0        0        0    27162 2021-06-19 16:28:30.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol61718.py
--rw-rw-rw-   0        0        0    27162 2021-06-19 16:28:31.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol61872.py
--rw-rw-rw-   0        0        0    27162 2021-06-19 16:28:33.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol61952.py
--rw-rw-rw-   0        0        0    27162 2021-06-19 16:28:35.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol62119.py
--rw-rw-rw-   0        0        0    27162 2021-06-19 16:28:36.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol62212.py
--rw-rw-rw-   0        0        0    27162 2021-06-19 16:28:37.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol62424.py
--rw-rw-rw-   0        0        0    27162 2021-06-19 16:28:39.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol62548.py
--rw-rw-rw-   0        0        0    27162 2021-06-19 16:28:40.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol62833.py
--rw-rw-rw-   0        0        0    27162 2021-06-19 16:28:42.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol63070.py
--rw-rw-rw-   0        0        0    27162 2021-06-19 16:28:43.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol63203.py
--rw-rw-rw-   0        0        0    27162 2021-06-19 16:28:44.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol63402.py
--rw-rw-rw-   0        0        0    27162 2021-06-19 16:28:46.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol63507.py
--rw-rw-rw-   0        0        0    27162 2021-06-19 16:28:47.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol63635.py
--rw-rw-rw-   0        0        0    27162 2021-06-19 16:28:48.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol64100.py
--rw-rw-rw-   0        0        0    27162 2021-06-19 16:28:50.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol64129.py
--rw-rw-rw-   0        0        0    27162 2021-06-19 16:28:51.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol64255.py
--rw-rw-rw-   0        0        0    27162 2021-06-19 16:28:53.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol64331.py
--rw-rw-rw-   0        0        0    27162 2021-06-19 16:28:54.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol64455.py
--rw-rw-rw-   0        0        0    27162 2021-06-19 16:28:55.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol64657.py
--rw-rw-rw-   0        0        0    27162 2021-06-19 16:28:57.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol64863.py
--rw-rw-rw-   0        0        0    27162 2021-06-19 16:28:58.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol65006.py
--rw-rw-rw-   0        0        0    27162 2021-06-19 16:29:00.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol65054.py
--rw-rw-rw-   0        0        0    27162 2021-06-19 16:29:01.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol65285.py
--rw-rw-rw-   0        0        0    27104 2021-06-19 16:29:02.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol65579.py
--rw-rw-rw-   0        0        0    27162 2021-06-19 16:29:04.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol65617.py
--rw-rw-rw-   0        0        0    27162 2021-06-19 16:29:05.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol65654.py
--rw-rw-rw-   0        0        0    27104 2021-06-19 16:29:07.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol65655.py
--rw-rw-rw-   0        0        0    27104 2021-06-19 16:29:08.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol65751.py
--rw-rw-rw-   0        0        0    27104 2021-06-19 16:29:09.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol65846.py
--rw-rw-rw-   0        0        0    27104 2021-06-19 16:29:11.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol65943.py
--rw-rw-rw-   0        0        0    27104 2021-06-19 16:29:12.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol66182.py
--rw-rw-rw-   0        0        0    27104 2021-06-19 16:29:14.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol66292.py
--rw-rw-rw-   0        0        0    27104 2021-06-19 16:29:15.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol66488.py
--rw-rw-rw-   0        0        0    27104 2021-06-19 16:29:16.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol66810.py
--rw-rw-rw-   0        0        0    27104 2021-06-19 16:29:18.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol66946.py
--rw-rw-rw-   0        0        0    27133 2021-06-19 16:29:19.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol66977.py
--rw-rw-rw-   0        0        0    27133 2021-06-19 16:29:20.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol67143.py
--rw-rw-rw-   0        0        0    27133 2021-06-19 16:29:22.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol67462.py
--rw-rw-rw-   0        0        0    27133 2021-06-19 16:29:23.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol67621.py
--rw-rw-rw-   0        0        0    27133 2021-06-19 16:29:25.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol67679.py
--rw-rw-rw-   0        0        0    27133 2021-06-19 16:29:26.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol67985.py
--rw-rw-rw-   0        0        0    27213 2021-06-19 16:13:56.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol68406.py
--rw-rw-rw-   0        0        0    27133 2021-06-19 16:29:27.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol68509.py
--rw-rw-rw-   0        0        0    27281 2021-06-19 16:29:29.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol68669.py
--rw-rw-rw-   0        0        0    27281 2021-06-19 16:29:30.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol68740.py
--rw-rw-rw-   0        0        0    27281 2021-06-19 16:29:32.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol68778.py
--rw-rw-rw-   0        0        0    27281 2021-06-19 16:29:33.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol69099.py
--rw-rw-rw-   0        0        0    27281 2021-06-19 16:29:34.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol69185.py
--rw-rw-rw-   0        0        0    27281 2021-06-19 16:29:36.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol69228.py
--rw-rw-rw-   0        0        0    27281 2021-06-19 16:29:37.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol69264.py
--rw-rw-rw-   0        0        0    27281 2021-06-19 16:29:39.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol69350.py
--rw-rw-rw-   0        0        0    27281 2021-06-19 16:29:40.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol69790.py
--rw-rw-rw-   0        0        0    27281 2021-06-19 16:29:41.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol69823.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:29:43.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol69947.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:29:44.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol70133.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:29:46.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol70200.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:29:47.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol70616.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:29:48.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol70682.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:29:50.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol70920.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:29:51.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol71040.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:29:53.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol71134.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:29:54.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol71138.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:29:55.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol71449.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:29:57.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol71652.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:29:58.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol71931.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:30:00.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol72053.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:30:01.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol72191.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:30:02.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol72307.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:30:04.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol72481.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:30:05.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol72649.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:30:07.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol72880.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:30:08.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol73016.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:30:09.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol73493.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:30:11.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol73576.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:30:12.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol73662.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:30:14.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol74238.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:30:15.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol74592.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:30:16.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol74665.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:30:18.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol74739.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:30:19.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol75132.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:30:21.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol75410.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:30:22.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol75484.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:30:23.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol75589.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:30:25.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol75792.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:30:26.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol76003.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:30:28.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol76124.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:30:29.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol76268.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:30:30.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol76389.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:30:32.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol76437.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:30:33.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol76517.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:30:35.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol76753.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:30:36.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol76781.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:30:37.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol76893.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:30:39.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol77205.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:30:40.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol77406.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:30:42.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol77435.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:30:43.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol77525.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:30:44.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol77548.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:30:46.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol77662.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:30:47.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol77692.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:30:49.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol77981.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:30:50.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol78256.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:30:51.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol78679.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:30:53.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol78725.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:30:54.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol79033.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:30:56.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol79155.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:30:57.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol79515.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:30:58.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol79999.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:31:00.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol80046.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:31:01.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol80205.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:31:03.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol80293.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:31:04.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol80333.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:31:06.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol80702.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:31:07.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol81376.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:31:08.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol81571.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:31:10.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol81700.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:31:11.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol82169.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:31:13.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol82624.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:31:14.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol83004.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:31:15.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol83077.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:31:17.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol83086.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:31:18.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol83632.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:31:20.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol83716.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:31:21.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol84200.py
--rw-rw-rw-   0        0        0    27309 2021-06-19 16:31:22.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol84249.py
--rw-rw-rw-   0        0        0    27406 2021-06-19 16:31:24.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol85027.py
--rw-rw-rw-   0        0        0    27406 2021-06-19 16:31:25.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol85267.py
--rw-rw-rw-   0        0        0    27406 2021-06-21 19:24:27.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol85311.py
--rw-rw-rw-   0        0        0    27406 2021-07-20 19:23:49.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol85551.py
--rw-rw-rw-   0        0        0    27406 2021-07-22 19:23:42.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol85576.py
--rw-rw-rw-   0        0        0    27406 2021-08-20 19:23:50.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol85894.py
--rw-rw-rw-   0        0        0    27406 2021-09-27 19:23:56.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol86223.py
--rw-rw-rw-   0        0        0    27406 2021-12-07 20:24:02.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol86938.py
--rw-rw-rw-   0        0        0    27406 2022-02-01 20:23:58.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol87306.py
--rw-rw-rw-   0        0        0    27406 2022-04-20 19:24:00.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol87774.py
--rw-rw-rw-   0        0        0    27406 2022-04-28 07:23:58.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol87990.py
--rw-rw-rw-   0        0        0    27406 2022-05-11 22:23:58.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol88122.py
--rw-rw-rw-   0        0        0    27406 2022-09-21 01:24:07.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol88481.py
--rw-rw-rw-   0        0        0    27406 2022-10-11 19:24:11.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol88936.py
--rw-rw-rw-   0        0        0    27406 2023-01-10 22:23:36.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol89566.py
--rw-rw-rw-   0        0        0    27406 2023-02-07 22:23:45.000000 heroprotocol-2.55.3.89754/heroprotocol/versions/protocol89754.py
-drwxrwxrwx   0        0        0        0 2023-02-07 22:23:53.316054 heroprotocol-2.55.3.89754/heroprotocol.egg-info/
--rw-rw-rw-   0        0        0     7574 2023-02-07 22:23:52.000000 heroprotocol-2.55.3.89754/heroprotocol.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    12856 2023-02-07 22:23:52.000000 heroprotocol-2.55.3.89754/heroprotocol.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-07 22:23:52.000000 heroprotocol-2.55.3.89754/heroprotocol.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-02-07 22:23:52.000000 heroprotocol-2.55.3.89754/heroprotocol.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       24 2023-02-07 22:23:52.000000 heroprotocol-2.55.3.89754/heroprotocol.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-02-07 22:23:52.000000 heroprotocol-2.55.3.89754/heroprotocol.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-07 22:23:54.789165 heroprotocol-2.55.3.89754/setup.cfg
--rw-rw-rw-   0        0        0     1547 2021-06-19 16:13:56.000000 heroprotocol-2.55.3.89754/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 23:49:53.448286 heroprotocol-2.55.3.90670/
+-rw-rw-rw-   0        0        0     1085 2023-01-10 18:41:55.000000 heroprotocol-2.55.3.90670/LICENSE
+-rw-rw-rw-   0        0        0     6475 2023-07-31 23:49:53.446287 heroprotocol-2.55.3.90670/PKG-INFO
+-rw-rw-rw-   0        0        0     5545 2023-01-10 18:41:55.000000 heroprotocol-2.55.3.90670/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 23:49:52.046161 heroprotocol-2.55.3.90670/heroprotocol/
+-rw-rw-rw-   0        0        0      316 2023-07-31 23:49:49.000000 heroprotocol-2.55.3.90670/heroprotocol/__init__.py
+-rw-rw-rw-   0        0        0      206 2023-01-10 18:41:55.000000 heroprotocol-2.55.3.90670/heroprotocol/__main__.py
+-rw-rw-rw-   0        0        0     1081 2023-07-31 23:49:49.000000 heroprotocol-2.55.3.90670/heroprotocol/build.py
+-rw-rw-rw-   0        0        0      352 2023-01-10 18:41:55.000000 heroprotocol-2.55.3.90670/heroprotocol/compat.py
+-rw-rw-rw-   0        0        0     9512 2023-01-10 18:41:55.000000 heroprotocol-2.55.3.90670/heroprotocol/decoders.py
+-rw-rw-rw-   0        0        0     4570 2023-01-10 18:41:55.000000 heroprotocol-2.55.3.90670/heroprotocol/hero_cli.py
+drwxrwxrwx   0        0        0        0 2023-07-31 23:49:53.442289 heroprotocol-2.55.3.90670/heroprotocol/versions/
+-rw-rw-rw-   0        0        0     2153 2023-01-10 18:41:55.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/__init__.py
+-rw-rw-rw-   0        0        0    28330 2023-01-10 18:41:55.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol29406.py
+-rw-rw-rw-   0        0        0    28582 2023-01-10 18:43:35.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol30414.py
+-rw-rw-rw-   0        0        0    28582 2023-01-10 18:43:37.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol30509.py
+-rw-rw-rw-   0        0        0    28582 2023-01-10 18:43:38.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol30829.py
+-rw-rw-rw-   0        0        0    28582 2023-01-10 18:43:39.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol30948.py
+-rw-rw-rw-   0        0        0    28582 2023-01-10 18:43:41.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol31090.py
+-rw-rw-rw-   0        0        0    28698 2023-01-10 18:43:42.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol31360.py
+-rw-rw-rw-   0        0        0    28698 2023-01-10 18:43:43.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol31566.py
+-rw-rw-rw-   0        0        0    28698 2023-01-10 18:43:45.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol31726.py
+-rw-rw-rw-   0        0        0    28698 2023-01-10 18:43:46.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol31948.py
+-rw-rw-rw-   0        0        0    28690 2023-01-10 18:43:47.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol32120.py
+-rw-rw-rw-   0        0        0    28690 2023-01-10 18:43:49.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol32253.py
+-rw-rw-rw-   0        0        0    28838 2023-01-10 18:43:50.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol32455.py
+-rw-rw-rw-   0        0        0    28838 2023-01-10 18:43:51.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol32524.py
+-rw-rw-rw-   0        0        0    29057 2023-01-10 18:43:53.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol33182.py
+-rw-rw-rw-   0        0        0    29057 2023-01-10 18:43:54.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol33353.py
+-rw-rw-rw-   0        0        0    29196 2023-01-10 18:43:55.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol33684.py
+-rw-rw-rw-   0        0        0    29261 2023-01-10 18:43:57.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol34053.py
+-rw-rw-rw-   0        0        0    29261 2023-01-10 18:43:58.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol34190.py
+-rw-rw-rw-   0        0        0    29261 2023-01-10 18:43:59.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol34659.py
+-rw-rw-rw-   0        0        0    29261 2023-01-10 18:44:01.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol34846.py
+-rw-rw-rw-   0        0        0    29314 2023-01-10 18:44:02.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol35360.py
+-rw-rw-rw-   0        0        0    29314 2023-01-10 18:44:03.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol35529.py
+-rw-rw-rw-   0        0        0    29314 2023-01-10 18:41:55.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol35634.py
+-rw-rw-rw-   0        0        0    29314 2023-01-10 18:44:05.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol35702.py
+-rw-rw-rw-   0        0        0    29314 2023-01-10 18:44:06.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol36144.py
+-rw-rw-rw-   0        0        0    29314 2023-01-10 18:44:07.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol36280.py
+-rw-rw-rw-   0        0        0    29314 2023-01-10 18:44:09.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol36359.py
+-rw-rw-rw-   0        0        0    29314 2023-01-10 18:44:10.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol36536.py
+-rw-rw-rw-   0        0        0    29314 2023-01-10 18:44:11.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol36693.py
+-rw-rw-rw-   0        0        0    29646 2023-01-10 18:44:13.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol37069.py
+-rw-rw-rw-   0        0        0    29646 2023-01-10 18:44:14.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol37117.py
+-rw-rw-rw-   0        0        0    29646 2023-01-10 18:41:56.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol37274.py
+-rw-rw-rw-   0        0        0    29646 2023-01-10 18:44:15.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol37351.py
+-rw-rw-rw-   0        0        0    29646 2023-01-10 18:44:17.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol37569.py
+-rw-rw-rw-   0        0        0    29646 2023-01-10 18:41:56.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol37795.py
+-rw-rw-rw-   0        0        0    29691 2023-01-10 18:44:18.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol38236.py
+-rw-rw-rw-   0        0        0    29691 2023-01-10 18:44:19.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol38500.py
+-rw-rw-rw-   0        0        0    29691 2023-01-10 18:44:21.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol38593.py
+-rw-rw-rw-   0        0        0    29691 2023-01-10 18:44:22.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol38793.py
+-rw-rw-rw-   0        0        0    29691 2023-01-10 18:44:23.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol39015.py
+-rw-rw-rw-   0        0        0    29691 2023-01-10 18:44:25.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol39153.py
+-rw-rw-rw-   0        0        0    29691 2023-01-10 18:44:26.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol39271.py
+-rw-rw-rw-   0        0        0    29691 2023-01-10 18:44:27.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol39445.py
+-rw-rw-rw-   0        0        0    29691 2023-01-10 18:44:29.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol39595.py
+-rw-rw-rw-   0        0        0    29691 2023-01-10 18:44:30.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol39709.py
+-rw-rw-rw-   0        0        0    29691 2023-01-10 18:44:31.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol39951.py
+-rw-rw-rw-   0        0        0    29691 2023-01-10 18:44:33.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol40087.py
+-rw-rw-rw-   0        0        0    29691 2023-01-10 18:44:34.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol40322.py
+-rw-rw-rw-   0        0        0    30706 2023-01-10 18:41:56.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol40336.py
+-rw-rw-rw-   0        0        0    30706 2023-01-10 18:44:35.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol40431.py
+-rw-rw-rw-   0        0        0    30706 2023-01-10 18:44:37.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol40697.py
+-rw-rw-rw-   0        0        0    30706 2023-01-10 18:44:38.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol40798.py
+-rw-rw-rw-   0        0        0    31128 2023-01-10 18:44:39.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol41150.py
+-rw-rw-rw-   0        0        0    31128 2023-01-10 18:44:41.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol41393.py
+-rw-rw-rw-   0        0        0    31128 2023-01-10 18:44:42.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol41504.py
+-rw-rw-rw-   0        0        0    26364 2023-01-10 18:44:43.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol41609.py
+-rw-rw-rw-   0        0        0    26364 2023-01-10 18:44:45.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol41707.py
+-rw-rw-rw-   0        0        0    26364 2023-01-10 18:44:46.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol41764.py
+-rw-rw-rw-   0        0        0    26364 2023-01-10 18:44:47.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol41810.py
+-rw-rw-rw-   0        0        0    26364 2023-01-10 18:44:49.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol42178.py
+-rw-rw-rw-   0        0        0    26364 2023-01-10 18:44:50.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol42273.py
+-rw-rw-rw-   0        0        0    26364 2023-01-10 18:44:51.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol42406.py
+-rw-rw-rw-   0        0        0    26364 2023-01-10 18:44:52.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol42506.py
+-rw-rw-rw-   0        0        0    26364 2023-01-10 18:44:54.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol42590.py
+-rw-rw-rw-   0        0        0    26364 2023-01-10 18:44:55.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol42742.py
+-rw-rw-rw-   0        0        0    26364 2023-01-10 18:44:56.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol42958.py
+-rw-rw-rw-   0        0        0    26364 2023-01-10 18:44:58.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol43051.py
+-rw-rw-rw-   0        0        0    26364 2023-01-10 18:44:59.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol43170.py
+-rw-rw-rw-   0        0        0    26364 2023-01-10 18:45:00.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol43259.py
+-rw-rw-rw-   0        0        0    26364 2023-01-10 18:45:01.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol43481.py
+-rw-rw-rw-   0        0        0    26364 2023-01-10 18:45:03.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol43527.py
+-rw-rw-rw-   0        0        0    26364 2023-01-10 18:45:04.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol43571.py
+-rw-rw-rw-   0        0        0    26383 2023-01-10 18:45:05.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol43905.py
+-rw-rw-rw-   0        0        0    26383 2023-01-10 18:45:07.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol44124.py
+-rw-rw-rw-   0        0        0    26434 2023-01-10 18:45:08.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol44256.py
+-rw-rw-rw-   0        0        0    26434 2023-01-10 18:45:09.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol44468.py
+-rw-rw-rw-   0        0        0    26434 2023-01-10 18:45:10.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol44737.py
+-rw-rw-rw-   0        0        0    26434 2023-01-10 18:45:12.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol44797.py
+-rw-rw-rw-   0        0        0    26434 2023-01-10 18:45:13.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol44941.py
+-rw-rw-rw-   0        0        0    26434 2023-01-10 18:45:14.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol45024.py
+-rw-rw-rw-   0        0        0    26434 2023-01-10 18:45:15.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol45228.py
+-rw-rw-rw-   0        0        0    26434 2023-01-10 18:45:17.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol45635.py
+-rw-rw-rw-   0        0        0    26459 2023-01-10 18:45:18.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol45815.py
+-rw-rw-rw-   0        0        0    26459 2023-01-10 18:45:19.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol45889.py
+-rw-rw-rw-   0        0        0    26459 2023-01-10 18:45:21.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol45949.py
+-rw-rw-rw-   0        0        0    26459 2023-01-10 18:45:22.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol46158.py
+-rw-rw-rw-   0        0        0    26459 2023-01-10 18:45:23.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol46416.py
+-rw-rw-rw-   0        0        0    26459 2023-01-10 18:45:25.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol46446.py
+-rw-rw-rw-   0        0        0    26459 2023-01-10 18:45:26.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol46690.py
+-rw-rw-rw-   0        0        0    26459 2023-01-10 18:45:27.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol46787.py
+-rw-rw-rw-   0        0        0    26459 2023-01-10 18:45:28.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol46869.py
+-rw-rw-rw-   0        0        0    26459 2023-01-10 18:45:30.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol46889.py
+-rw-rw-rw-   0        0        0    26459 2023-01-10 18:45:31.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol47024.py
+-rw-rw-rw-   0        0        0    26459 2023-01-10 18:45:32.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol47133.py
+-rw-rw-rw-   0        0        0    26459 2023-01-10 18:45:34.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol47219.py
+-rw-rw-rw-   0        0        0    26459 2023-01-10 18:45:35.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol47479.py
+-rw-rw-rw-   0        0        0    26459 2023-01-10 18:45:36.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol47801.py
+-rw-rw-rw-   0        0        0    26459 2023-01-10 18:45:38.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol47903.py
+-rw-rw-rw-   0        0        0    26459 2023-01-10 18:45:39.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol47944.py
+-rw-rw-rw-   0        0        0    26459 2023-01-10 18:45:40.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol48027.py
+-rw-rw-rw-   0        0        0    26459 2023-01-10 18:45:41.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol48297.py
+-rw-rw-rw-   0        0        0    26459 2023-01-10 18:45:43.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol48548.py
+-rw-rw-rw-   0        0        0    26459 2023-01-10 18:45:44.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol48583.py
+-rw-rw-rw-   0        0        0    26459 2023-01-10 18:45:45.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol48760.py
+-rw-rw-rw-   0        0        0    26459 2023-01-10 18:45:47.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol49008.py
+-rw-rw-rw-   0        0        0    26459 2023-01-10 18:45:48.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol49076.py
+-rw-rw-rw-   0        0        0    26459 2023-01-10 18:45:49.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol49278.py
+-rw-rw-rw-   0        0        0    26459 2023-01-10 18:45:51.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol49495.py
+-rw-rw-rw-   0        0        0    26447 2023-01-10 18:45:52.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol49582.py
+-rw-rw-rw-   0        0        0    26447 2023-01-10 18:45:54.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol49747.py
+-rw-rw-rw-   0        0        0    26459 2023-01-10 18:45:55.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol49838.py
+-rw-rw-rw-   0        0        0    26447 2023-01-10 18:45:56.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol49907.py
+-rw-rw-rw-   0        0        0    26447 2023-01-10 18:45:57.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol50286.py
+-rw-rw-rw-   0        0        0    26447 2023-01-10 18:45:59.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol50424.py
+-rw-rw-rw-   0        0        0    26447 2023-01-10 18:46:00.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol50441.py
+-rw-rw-rw-   0        0        0    26447 2023-01-10 18:46:02.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol50673.py
+-rw-rw-rw-   0        0        0    26447 2023-01-10 18:46:03.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol50950.py
+-rw-rw-rw-   0        0        0    26447 2023-01-10 18:46:05.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol51150.py
+-rw-rw-rw-   0        0        0    26447 2023-01-10 18:46:06.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol51375.py
+-rw-rw-rw-   0        0        0    26447 2023-01-10 18:46:08.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol51609.py
+-rw-rw-rw-   0        0        0    26447 2023-01-10 18:46:09.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol51779.py
+-rw-rw-rw-   0        0        0    26447 2023-01-10 18:46:10.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol51923.py
+-rw-rw-rw-   0        0        0    26888 2023-01-10 18:46:12.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol51978.py
+-rw-rw-rw-   0        0        0    26447 2023-01-10 18:46:13.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol52008.py
+-rw-rw-rw-   0        0        0    26447 2023-01-10 18:46:14.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol52124.py
+-rw-rw-rw-   0        0        0    26888 2023-01-10 18:46:15.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol52214.py
+-rw-rw-rw-   0        0        0    26447 2023-01-10 18:46:17.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol52351.py
+-rw-rw-rw-   0        0        0    26888 2023-01-10 18:46:18.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol52381.py
+-rw-rw-rw-   0        0        0    27019 2023-01-10 18:46:19.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol52561.py
+-rw-rw-rw-   0        0        0    26447 2023-01-10 18:46:20.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol52647.py
+-rw-rw-rw-   0        0        0    27019 2023-01-10 18:46:22.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol52860.py
+-rw-rw-rw-   0        0        0    27019 2023-01-10 18:46:23.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol52986.py
+-rw-rw-rw-   0        0        0    27019 2023-01-10 18:46:24.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol53174.py
+-rw-rw-rw-   0        0        0    27019 2023-01-10 18:46:26.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol53270.py
+-rw-rw-rw-   0        0        0    27019 2023-01-10 18:46:27.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol53275.py
+-rw-rw-rw-   0        0        0    27019 2023-01-10 18:46:28.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol53548.py
+-rw-rw-rw-   0        0        0    27019 2023-01-10 18:46:29.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol53965.py
+-rw-rw-rw-   0        0        0    27019 2023-01-10 18:46:31.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol54098.py
+-rw-rw-rw-   0        0        0    27019 2023-01-10 18:46:32.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol54339.py
+-rw-rw-rw-   0        0        0    27019 2023-01-10 18:46:33.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol54968.py
+-rw-rw-rw-   0        0        0    27019 2023-01-10 18:46:35.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol55010.py
+-rw-rw-rw-   0        0        0    27019 2023-01-10 18:46:36.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol55058.py
+-rw-rw-rw-   0        0        0    27019 2023-01-10 18:46:38.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol55288.py
+-rw-rw-rw-   0        0        0    27019 2023-01-10 18:46:39.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol55844.py
+-rw-rw-rw-   0        0        0    27019 2023-01-10 18:46:40.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol55929.py
+-rw-rw-rw-   0        0        0    27019 2023-01-10 18:46:42.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol56175.py
+-rw-rw-rw-   0        0        0    27019 2023-01-10 18:46:43.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol56361.py
+-rw-rw-rw-   0        0        0    27019 2023-01-10 18:46:44.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol56705.py
+-rw-rw-rw-   0        0        0    27019 2023-01-10 18:46:46.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol56784.py
+-rw-rw-rw-   0        0        0    27019 2023-01-10 18:46:47.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol56859.py
+-rw-rw-rw-   0        0        0    27019 2023-01-10 18:46:48.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol57062.py
+-rw-rw-rw-   0        0        0    27019 2023-01-10 18:46:50.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol57286.py
+-rw-rw-rw-   0        0        0    27092 2023-01-10 18:46:51.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol57547.py
+-rw-rw-rw-   0        0        0    27019 2023-01-10 18:46:52.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol57589.py
+-rw-rw-rw-   0        0        0    27092 2023-01-10 18:46:53.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol57797.py
+-rw-rw-rw-   0        0        0    27092 2023-01-10 18:46:55.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol58209.py
+-rw-rw-rw-   0        0        0    27092 2023-01-10 18:46:56.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol58344.py
+-rw-rw-rw-   0        0        0    27092 2023-01-10 18:46:57.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol58482.py
+-rw-rw-rw-   0        0        0    27092 2023-01-10 18:46:58.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol58623.py
+-rw-rw-rw-   0        0        0    27092 2023-01-10 18:47:00.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol58795.py
+-rw-rw-rw-   0        0        0    27092 2023-01-10 18:47:01.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol59239.py
+-rw-rw-rw-   0        0        0    27126 2023-01-10 18:47:02.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol59279.py
+-rw-rw-rw-   0        0        0    27126 2023-01-10 18:47:04.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol59657.py
+-rw-rw-rw-   0        0        0    27126 2023-01-10 18:47:05.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol59799.py
+-rw-rw-rw-   0        0        0    27126 2023-01-10 18:47:07.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol59837.py
+-rw-rw-rw-   0        0        0    27126 2023-01-10 18:47:08.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol59944.py
+-rw-rw-rw-   0        0        0    27126 2023-01-10 18:47:09.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol59988.py
+-rw-rw-rw-   0        0        0    27126 2023-01-10 18:47:11.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol60228.py
+-rw-rw-rw-   0        0        0    27126 2023-01-10 18:47:12.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol60265.py
+-rw-rw-rw-   0        0        0    27126 2023-01-10 18:47:13.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol60399.py
+-rw-rw-rw-   0        0        0    27126 2023-01-10 18:47:15.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol60522.py
+-rw-rw-rw-   0        0        0    27126 2023-01-10 18:47:16.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol60567.py
+-rw-rw-rw-   0        0        0    27126 2023-01-10 18:47:17.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol60632.py
+-rw-rw-rw-   0        0        0    27126 2023-01-10 18:47:18.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol60821.py
+-rw-rw-rw-   0        0        0    27126 2023-01-10 18:47:20.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol61129.py
+-rw-rw-rw-   0        0        0    27126 2023-01-10 18:47:21.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol61361.py
+-rw-rw-rw-   0        0        0    27126 2023-01-10 18:47:22.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol61552.py
+-rw-rw-rw-   0        0        0    27162 2023-01-10 18:47:23.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol61718.py
+-rw-rw-rw-   0        0        0    27162 2023-01-10 18:47:25.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol61872.py
+-rw-rw-rw-   0        0        0    27162 2023-01-10 18:47:26.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol61952.py
+-rw-rw-rw-   0        0        0    27162 2023-01-10 18:47:27.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol62119.py
+-rw-rw-rw-   0        0        0    27162 2023-01-10 18:47:29.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol62212.py
+-rw-rw-rw-   0        0        0    27162 2023-01-10 18:47:30.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol62424.py
+-rw-rw-rw-   0        0        0    27162 2023-01-10 18:47:31.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol62548.py
+-rw-rw-rw-   0        0        0    27162 2023-01-10 18:47:32.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol62833.py
+-rw-rw-rw-   0        0        0    27162 2023-01-10 18:47:34.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol63070.py
+-rw-rw-rw-   0        0        0    27162 2023-01-10 18:47:35.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol63203.py
+-rw-rw-rw-   0        0        0    27162 2023-01-10 18:47:36.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol63402.py
+-rw-rw-rw-   0        0        0    27162 2023-01-10 18:47:37.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol63507.py
+-rw-rw-rw-   0        0        0    27162 2023-01-10 18:47:39.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol63635.py
+-rw-rw-rw-   0        0        0    27162 2023-01-10 18:47:40.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol64100.py
+-rw-rw-rw-   0        0        0    27162 2023-01-10 18:47:41.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol64129.py
+-rw-rw-rw-   0        0        0    27162 2023-01-10 18:47:42.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol64255.py
+-rw-rw-rw-   0        0        0    27162 2023-01-10 18:47:44.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol64331.py
+-rw-rw-rw-   0        0        0    27162 2023-01-10 18:47:45.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol64455.py
+-rw-rw-rw-   0        0        0    27162 2023-01-10 18:47:46.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol64657.py
+-rw-rw-rw-   0        0        0    27162 2023-01-10 18:47:47.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol64863.py
+-rw-rw-rw-   0        0        0    27162 2023-01-10 18:47:49.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol65006.py
+-rw-rw-rw-   0        0        0    27162 2023-01-10 18:47:50.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol65054.py
+-rw-rw-rw-   0        0        0    27162 2023-01-10 18:47:51.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol65285.py
+-rw-rw-rw-   0        0        0    27104 2023-01-10 18:47:52.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol65579.py
+-rw-rw-rw-   0        0        0    27162 2023-01-10 18:47:54.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol65617.py
+-rw-rw-rw-   0        0        0    27162 2023-01-10 18:47:55.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol65654.py
+-rw-rw-rw-   0        0        0    27104 2023-01-10 18:47:56.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol65655.py
+-rw-rw-rw-   0        0        0    27104 2023-01-10 18:47:57.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol65751.py
+-rw-rw-rw-   0        0        0    27104 2023-01-10 18:47:59.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol65846.py
+-rw-rw-rw-   0        0        0    27104 2023-01-10 18:48:00.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol65943.py
+-rw-rw-rw-   0        0        0    27104 2023-01-10 18:48:01.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol66182.py
+-rw-rw-rw-   0        0        0    27104 2023-01-10 18:48:03.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol66292.py
+-rw-rw-rw-   0        0        0    27104 2023-01-10 18:48:04.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol66488.py
+-rw-rw-rw-   0        0        0    27104 2023-01-10 18:48:05.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol66810.py
+-rw-rw-rw-   0        0        0    27104 2023-01-10 18:48:06.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol66946.py
+-rw-rw-rw-   0        0        0    27133 2023-01-10 18:48:08.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol66977.py
+-rw-rw-rw-   0        0        0    27133 2023-01-10 18:48:09.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol67143.py
+-rw-rw-rw-   0        0        0    27133 2023-01-10 18:48:10.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol67462.py
+-rw-rw-rw-   0        0        0    27133 2023-01-10 18:48:12.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol67621.py
+-rw-rw-rw-   0        0        0    27133 2023-01-10 18:48:13.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol67679.py
+-rw-rw-rw-   0        0        0    27133 2023-01-10 18:48:14.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol67985.py
+-rw-rw-rw-   0        0        0    27213 2023-01-10 18:41:56.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol68406.py
+-rw-rw-rw-   0        0        0    27133 2023-01-10 18:48:15.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol68509.py
+-rw-rw-rw-   0        0        0    27281 2023-01-10 18:48:17.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol68669.py
+-rw-rw-rw-   0        0        0    27281 2023-01-10 18:48:18.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol68740.py
+-rw-rw-rw-   0        0        0    27281 2023-01-10 18:48:19.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol68778.py
+-rw-rw-rw-   0        0        0    27281 2023-01-10 18:48:20.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol69099.py
+-rw-rw-rw-   0        0        0    27281 2023-01-10 18:48:22.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol69185.py
+-rw-rw-rw-   0        0        0    27281 2023-01-10 18:48:23.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol69228.py
+-rw-rw-rw-   0        0        0    27281 2023-01-10 18:48:24.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol69264.py
+-rw-rw-rw-   0        0        0    27281 2023-01-10 18:48:26.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol69350.py
+-rw-rw-rw-   0        0        0    27281 2023-01-10 18:48:27.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol69790.py
+-rw-rw-rw-   0        0        0    27281 2023-01-10 18:48:28.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol69823.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:48:30.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol69947.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:48:31.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol70133.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:48:32.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol70200.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:48:33.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol70616.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:48:35.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol70682.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:48:36.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol70920.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:48:37.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol71040.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:48:39.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol71134.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:48:40.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol71138.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:48:41.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol71449.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:48:43.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol71652.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:48:44.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol71931.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:48:45.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol72053.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:48:47.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol72191.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:48:48.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol72307.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:48:49.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol72481.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:48:50.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol72649.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:48:52.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol72880.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:48:53.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol73016.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:48:54.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol73493.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:48:55.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol73576.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:48:57.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol73662.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:48:58.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol74238.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:48:59.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol74592.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:00.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol74665.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:02.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol74739.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:03.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol75132.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:04.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol75410.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:05.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol75484.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:07.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol75589.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:08.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol75792.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:09.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol76003.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:10.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol76124.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:12.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol76268.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:13.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol76389.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:14.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol76437.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:15.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol76517.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:17.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol76753.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:18.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol76781.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:19.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol76893.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:20.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol77205.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:22.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol77406.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:23.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol77435.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:24.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol77525.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:25.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol77548.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:27.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol77662.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:28.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol77692.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:29.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol77981.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:30.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol78256.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:32.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol78679.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:33.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol78725.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:34.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol79033.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:35.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol79155.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:37.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol79515.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:38.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol79999.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:39.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol80046.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:40.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol80205.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:42.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol80293.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:43.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol80333.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:44.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol80702.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:45.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol81376.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:47.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol81571.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:48.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol81700.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:49.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol82169.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:51.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol82624.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:52.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol83004.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:53.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol83077.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:54.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol83086.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:56.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol83632.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:57.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol83716.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:58.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol84200.py
+-rw-rw-rw-   0        0        0    27309 2023-01-10 18:49:59.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol84249.py
+-rw-rw-rw-   0        0        0    27406 2023-01-10 18:50:00.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol85027.py
+-rw-rw-rw-   0        0        0    27406 2023-01-10 18:50:02.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol85267.py
+-rw-rw-rw-   0        0        0    27406 2023-01-10 18:50:03.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol85311.py
+-rw-rw-rw-   0        0        0    27406 2023-01-10 18:50:04.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol85551.py
+-rw-rw-rw-   0        0        0    27406 2023-01-10 18:50:05.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol85576.py
+-rw-rw-rw-   0        0        0    27406 2023-01-10 18:50:07.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol85894.py
+-rw-rw-rw-   0        0        0    27406 2023-01-10 18:50:08.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol86223.py
+-rw-rw-rw-   0        0        0    27406 2023-01-10 18:50:09.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol86938.py
+-rw-rw-rw-   0        0        0    27406 2023-01-10 18:50:10.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol87306.py
+-rw-rw-rw-   0        0        0    27406 2023-01-10 18:50:12.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol87774.py
+-rw-rw-rw-   0        0        0    27406 2023-01-10 18:50:13.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol87990.py
+-rw-rw-rw-   0        0        0    27406 2023-01-10 18:50:14.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol88122.py
+-rw-rw-rw-   0        0        0    27406 2023-01-10 18:50:15.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol88481.py
+-rw-rw-rw-   0        0        0    27406 2023-01-10 18:50:17.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol88936.py
+-rw-rw-rw-   0        0        0    27406 2023-02-14 02:44:40.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol89566.py
+-rw-rw-rw-   0        0        0    27406 2023-02-14 02:44:40.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol89754.py
+-rw-rw-rw-   0        0        0    27406 2023-07-31 23:49:49.000000 heroprotocol-2.55.3.90670/heroprotocol/versions/protocol90670.py
+drwxrwxrwx   0        0        0        0 2023-07-31 23:49:52.061163 heroprotocol-2.55.3.90670/heroprotocol.egg-info/
+-rw-rw-rw-   0        0        0     6475 2023-07-31 23:49:51.000000 heroprotocol-2.55.3.90670/heroprotocol.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    12903 2023-07-31 23:49:51.000000 heroprotocol-2.55.3.90670/heroprotocol.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 23:49:51.000000 heroprotocol-2.55.3.90670/heroprotocol.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-07-31 23:49:51.000000 heroprotocol-2.55.3.90670/heroprotocol.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       24 2023-07-31 23:49:51.000000 heroprotocol-2.55.3.90670/heroprotocol.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-31 23:49:51.000000 heroprotocol-2.55.3.90670/heroprotocol.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 23:49:53.448286 heroprotocol-2.55.3.90670/setup.cfg
+-rw-rw-rw-   0        0        0     1547 2023-01-10 18:41:56.000000 heroprotocol-2.55.3.90670/setup.py
```

### Comparing `heroprotocol-2.55.3.89754/PKG-INFO` & `heroprotocol-2.55.3.90670/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,158 +1,157 @@
 Metadata-Version: 2.1
 Name: heroprotocol
-Version: 2.55.3.89754
+Version: 2.55.3.90670
 Summary: Python library to decode Heroes of the Storm replays
 Home-page: https://github.com/Blizzard/heroprotocol
 Author: Blizzard Entertainment
 Author-email: HeroesReplays@blizzard.com
-License: UNKNOWN
-Description: # heroprotocol
-        
-        heroprotocol is a [Python](https://www.python.org/downloads/) library and command-line tool to decode Heroes of the Storm replay files into Python data structures.
-        
-        The tool is available as a [PyPI Package](https://pypi.org/project/heroprotocol/) or as source code.
-        
-        Currently heroprotocol can decode these structures and events:
-        
-        * Replay header
-        * Game details
-        * Replay init data
-        * Game events
-        * Message events
-        * Tracker events
-        
-        heroprotocol can be used as a base-build-specific library to decode binary blobs, or it can be run as a standalone tool
-        to pretty print information from supported replay files.
-        
-        Note that heroprotocol does not expose game balance information or provide any kind of high level analysis of replays;
-        it's meant to be just the first tool in the chain for your data mining application.
-        
-        ## Supported Versions
-        
-        heroprotocol supports all Hereos of the Storm replay files that were played with retail and PTR versions of the game.
-        
-        ## Requirements
-        
-        * Python 2.7 or 3.x
-          * Note: A future release may remove support for Python 2.7
-        * Python Packages:
-          * mpyq 0.2.5+
-          * six 1.14.0+
-        
-        ## Installation
-        
-        Either install/update using pip:
-        
-        ```bash
-        python -m pip install --upgrade heroprotocol
-        ```
-        
-        Or clone the repository and run from source:
-        
-        ```bash
-        git clone https://github.com/Blizzard/heroprotocol.git
-        python -m pip install -r ./heroprotocol/heroprotocol/requirements.txt
-        ```
-        
-        ## Command Line Arguments
-        
-        ```plain
-        -h, --help          Show the options that are available.
-        
-        Tracker Events:
-        --gameevents        Print all game events including coordinates
-        --messageevents     Print message events such as ping events
-        --trackerevents     Print tracker events such as units killed, game stat events,
-                            score result event
-        --attributeevents   Print attribute events, a table of attrid, namespace, and attribute values
-        --header            Print protocol header including build id and elapsedGameLoops
-        --details           Print protocol details, e.g. teamId, player names and chosen heroes,
-                            player region, game result, observer status
-        --initdata          Print protocol initdata, e.g. interface settings for every player
-        
-        Output Options:
-        --stats             Output stats about the active tracker event to the STDERR stream
-        --json              Use JSON syntax for output
-        ```
-        
-        ## Example Usage
-        
-        If you want the output shown directly in the terminal, leave out the `> output.txt`.
-        
-        ```bash
-        python -m heroprotocol --details "Blackheart's Bay.StormReplay" > output.txt
-        ```
-        
-        By default, data is output as a Python dictionary object. To output a JSON file, add `--json`.
-        
-        **Note**, however, that the JSON file is formatted as a sequence/stream of JSON objects and
-        will likely not parse as regular JSON.
-        
-        ## Tracker Events
-        
-        Some notes on tracker events:
-        
-        * Convert unit tag index, recycle pairs into unit tags (as seen in game events) with protocol.unit_tag (index, recycle)
-        * Interpret the NNet.Replay.Tracker.SUnitPositionsEvent events like this:
-        
-        ```python
-        unitIndex = event['m_firstUnitIndex']
-        for i in range(0, len(event['m_items']), 3):
-            unitIndex += event['m_items'][i + 0]
-            x = event['m_items'][i + 1] * 4
-            y = event['m_items'][i + 2] * 4
-            # unit identified by unitIndex at the current event['_gameloop'] time
-            # is at approximate position (x, y)
-        ```
-        
-        * Only units that have inflicted or taken damage are mentioned in unit position events, and they occur periodically with a limit of 256 units mentioned per event.
-        * NNet.Replay.Tracker.SUnitInitEvent events appear for units under construction. When complete you'll see a NNet.Replay.Tracker.SUnitDoneEvent with the same unit tag.
-        * NNet.Replay.Tracker.SUnitBornEvent events appear for units that are created fully constructed.
-        * You may receive a NNet.Replay.Tracker.SUnitDiedEvent after either a UnitInit or UnitBorn event for the corresponding unit tag.
-        * In NNet.Replay.Tracker.SPlayerStatsEvent, m_scoreValueFoodUsed and m_scoreValueFoodMade are in fixed point (divide by 4096 for integer values). All other values are in integers.
-        * There's a known issue where revived units are not tracked, and placeholder units track death but not birth.
-        
-        ## Reporting Bugs
-        
-        Please report bugs at the [Heroes of the Storm Bug Report Forum](https://us.forums.blizzard.com/en/heroes/c/bug-report).
-        
-        ## Acknowledgements
-        
-        The standalone tool uses [mpyq](https://github.com/eagleflo/mpyq) by
-        [Aku Kotkavuo](https://github.com/eagleflo) to read mopaq files.
-        
-        Thank you to [healingbrew](https://github.com/healingbrew), [MGatner](https://github.com/mgatner),
-        [koliva8245](https://github.com/koliva8245), [casualMLG](https://github.com/casualmlg), and others for submitting issues
-        and feedback.
-        
-        Thank you to [Christian Clauss](https://github.com/cclauss), [Jingbei Li](https://github.com/petronny), and
-        [Regner Blok-Andersen](https://github.com/regner) for contributions to the Python 3 update.
-        
-        Thank you to David Joerg and Graylin Kim of [GGTracker](http://www.ggtracker.com) for design feedback and beta-testing of
-        the s2protocol library that heroprotocol is based upon.
-        
-        Thanks to Ben Barrett of [HOTSLogs](http://www.hotslogs.com) for early feedback on and beta-testing of the heroprotocol
-        library.
-        
-        ## License
-        
-        Copyright 2021 Blizzard Entertainment
-        
-        Source code for this project is released to the public under the MIT license.
-        See the included [LICENSE](LICENSE) file for more information.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Games/Entertainment :: Real Time Strategy
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Archiving
 Classifier: Topic :: Utilities
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# heroprotocol
+
+heroprotocol is a [Python](https://www.python.org/downloads/) library and command-line tool to decode Heroes of the Storm replay files into Python data structures.
+
+The tool is available as a [PyPI Package](https://pypi.org/project/heroprotocol/) or as source code.
+
+Currently heroprotocol can decode these structures and events:
+
+* Replay header
+* Game details
+* Replay init data
+* Game events
+* Message events
+* Tracker events
+
+heroprotocol can be used as a base-build-specific library to decode binary blobs, or it can be run as a standalone tool
+to pretty print information from supported replay files.
+
+Note that heroprotocol does not expose game balance information or provide any kind of high level analysis of replays;
+it's meant to be just the first tool in the chain for your data mining application.
+
+## Supported Versions
+
+heroprotocol supports all Hereos of the Storm replay files that were played with retail and PTR versions of the game.
+
+## Requirements
+
+* Python 2.7 or 3.x
+  * Note: A future release may remove support for Python 2.7
+* Python Packages:
+  * mpyq 0.2.5+
+  * six 1.14.0+
+
+## Installation
+
+Either install/update using pip:
+
+```bash
+python -m pip install --upgrade heroprotocol
+```
+
+Or clone the repository and run from source:
+
+```bash
+git clone https://github.com/Blizzard/heroprotocol.git
+python -m pip install -r ./heroprotocol/heroprotocol/requirements.txt
+```
+
+## Command Line Arguments
+
+```plain
+-h, --help          Show the options that are available.
+
+Tracker Events:
+--gameevents        Print all game events including coordinates
+--messageevents     Print message events such as ping events
+--trackerevents     Print tracker events such as units killed, game stat events,
+                    score result event
+--attributeevents   Print attribute events, a table of attrid, namespace, and attribute values
+--header            Print protocol header including build id and elapsedGameLoops
+--details           Print protocol details, e.g. teamId, player names and chosen heroes,
+                    player region, game result, observer status
+--initdata          Print protocol initdata, e.g. interface settings for every player
+
+Output Options:
+--stats             Output stats about the active tracker event to the STDERR stream
+--json              Use JSON syntax for output
+```
+
+## Example Usage
+
+If you want the output shown directly in the terminal, leave out the `> output.txt`.
+
+```bash
+python -m heroprotocol --details "Blackheart's Bay.StormReplay" > output.txt
+```
+
+By default, data is output as a Python dictionary object. To output a JSON file, add `--json`.
+
+**Note**, however, that the JSON file is formatted as a sequence/stream of JSON objects and
+will likely not parse as regular JSON.
+
+## Tracker Events
+
+Some notes on tracker events:
+
+* Convert unit tag index, recycle pairs into unit tags (as seen in game events) with protocol.unit_tag (index, recycle)
+* Interpret the NNet.Replay.Tracker.SUnitPositionsEvent events like this:
+
+```python
+unitIndex = event['m_firstUnitIndex']
+for i in range(0, len(event['m_items']), 3):
+    unitIndex += event['m_items'][i + 0]
+    x = event['m_items'][i + 1] * 4
+    y = event['m_items'][i + 2] * 4
+    # unit identified by unitIndex at the current event['_gameloop'] time
+    # is at approximate position (x, y)
+```
+
+* Only units that have inflicted or taken damage are mentioned in unit position events, and they occur periodically with a limit of 256 units mentioned per event.
+* NNet.Replay.Tracker.SUnitInitEvent events appear for units under construction. When complete you'll see a NNet.Replay.Tracker.SUnitDoneEvent with the same unit tag.
+* NNet.Replay.Tracker.SUnitBornEvent events appear for units that are created fully constructed.
+* You may receive a NNet.Replay.Tracker.SUnitDiedEvent after either a UnitInit or UnitBorn event for the corresponding unit tag.
+* In NNet.Replay.Tracker.SPlayerStatsEvent, m_scoreValueFoodUsed and m_scoreValueFoodMade are in fixed point (divide by 4096 for integer values). All other values are in integers.
+* There's a known issue where revived units are not tracked, and placeholder units track death but not birth.
+
+## Reporting Bugs
+
+Please report bugs at the [Heroes of the Storm Bug Report Forum](https://us.forums.blizzard.com/en/heroes/c/bug-report).
+
+## Acknowledgements
+
+The standalone tool uses [mpyq](https://github.com/eagleflo/mpyq) by
+[Aku Kotkavuo](https://github.com/eagleflo) to read mopaq files.
+
+Thank you to [healingbrew](https://github.com/healingbrew), [MGatner](https://github.com/mgatner),
+[koliva8245](https://github.com/koliva8245), [casualMLG](https://github.com/casualmlg), and others for submitting issues
+and feedback.
+
+Thank you to [Christian Clauss](https://github.com/cclauss), [Jingbei Li](https://github.com/petronny), and
+[Regner Blok-Andersen](https://github.com/regner) for contributions to the Python 3 update.
+
+Thank you to David Joerg and Graylin Kim of [GGTracker](http://www.ggtracker.com) for design feedback and beta-testing of
+the s2protocol library that heroprotocol is based upon.
+
+Thanks to Ben Barrett of [HOTSLogs](http://www.hotslogs.com) for early feedback on and beta-testing of the heroprotocol
+library.
+
+## License
+
+Copyright 2021 Blizzard Entertainment
+
+Source code for this project is released to the public under the MIT license.
+See the included [LICENSE](LICENSE) file for more information.
```

### Comparing `heroprotocol-2.55.3.89754/README.md` & `heroprotocol-2.55.3.90670/README.md`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/build.py` & `heroprotocol-2.55.3.90670/heroprotocol/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # See the included LICENSE file for more information.
 #
 
 import subprocess
 
 
 def game_version():
-    return '2.55.3.89754'
+    return '2.55.3.90670'
 
 
 def read_command_output(cmd):
     lines = []
     handle = subprocess.Popen(cmd, stdout=subprocess.PIPE)
     while True:
         line = handle.stdout.readline()
```

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/decoders.py` & `heroprotocol-2.55.3.90670/heroprotocol/decoders.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/hero_cli.py` & `heroprotocol-2.55.3.90670/heroprotocol/hero_cli.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/__init__.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol29406.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol29406.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol30414.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol30414.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol30509.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol30509.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol30829.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol30829.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol30948.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol30948.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol31090.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol31090.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol31360.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol31360.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol31566.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol31566.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol31726.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol31726.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol31948.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol31948.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol32120.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol32120.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol32253.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol32253.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol32455.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol32455.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol32524.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol32524.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol33182.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol33182.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol33353.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol33353.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol33684.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol33684.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol34053.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol34053.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol34190.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol34190.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol34659.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol34659.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol34846.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol34846.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol35360.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol35360.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol35529.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol35529.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol35634.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol35634.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol35702.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol35702.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol36144.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol36144.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol36280.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol36280.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol36359.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol36359.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol36536.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol36536.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol36693.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol36693.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol37069.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol37069.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol37117.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol37117.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol37274.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol37274.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol37351.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol37351.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol37569.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol37569.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol37795.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol37795.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol38236.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol38236.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol38500.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol38500.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol38593.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol38593.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol38793.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol38793.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol39015.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol39015.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol39153.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol39153.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol39271.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol39271.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol39445.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol39445.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol39595.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol39595.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol39709.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol39709.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol39951.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol39951.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol40087.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol40087.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol40322.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol40322.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol40336.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol40336.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol40431.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol40431.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol40697.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol40697.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol40798.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol40798.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol41150.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol41150.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol41393.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol41393.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol41504.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol41504.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol41609.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol41609.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol41707.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol41707.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol41764.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol41764.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol41810.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol41810.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol42178.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol42178.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol42273.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol42273.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol42406.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol42406.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol42506.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol42506.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol42590.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol42590.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol42742.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol42742.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol42958.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol42958.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol43051.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol43051.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol43170.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol43170.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol43259.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol43259.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol43481.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol43481.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol43527.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol43527.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol43571.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol43571.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol43905.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol43905.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol44124.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol44124.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol44256.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol44256.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol44468.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol44468.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol44737.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol44737.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol44797.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol44797.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol44941.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol44941.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol45024.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol45024.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol45228.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol45228.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol45635.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol45635.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol45815.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol45815.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol45889.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol45889.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol45949.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol45949.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol46158.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol46158.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol46416.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol46416.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol46446.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol46446.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol46690.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol46690.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol46787.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol46787.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol46869.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol46869.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol46889.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol46889.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol47024.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol47024.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol47133.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol47133.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol47219.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol47219.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol47479.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol47479.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol47801.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol47801.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol47903.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol47903.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol47944.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol47944.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol48027.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol48027.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol48297.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol48297.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol48548.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol48548.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol48583.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol48583.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol48760.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol48760.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol49008.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol49008.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol49076.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol49076.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol49278.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol49278.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol49495.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol49495.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol49582.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol49582.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol49747.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol49747.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol49838.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol49838.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol49907.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol49907.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol50286.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol50286.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol50424.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol50424.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol50441.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol50441.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol50673.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol50673.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol50950.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol50950.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol51150.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol51150.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol51375.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol51375.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol51609.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol51609.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol51779.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol51779.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol51923.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol51923.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol51978.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol51978.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol52008.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol52008.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol52124.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol52124.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol52214.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol52214.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol52351.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol52351.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol52381.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol52381.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol52561.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol52561.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol52647.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol52647.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol52860.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol52860.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol52986.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol52986.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol53174.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol53174.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol53270.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol53270.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol53275.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol53275.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol53548.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol53548.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol53965.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol53965.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol54098.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol54098.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol54339.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol54339.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol54968.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol54968.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol55010.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol55010.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol55058.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol55058.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol55288.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol55288.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol55844.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol55844.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol55929.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol55929.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol56175.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol56175.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol56361.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol56361.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol56705.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol56705.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol56784.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol56784.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol56859.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol56859.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol57062.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol57062.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol57286.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol57286.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol57547.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol57547.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol57589.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol57589.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol57797.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol57797.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol58209.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol58209.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol58344.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol58344.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol58482.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol58482.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol58623.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol58623.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol58795.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol58795.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol59239.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol59239.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol59279.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol59279.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol59657.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol59657.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol59799.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol59799.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol59837.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol59837.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol59944.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol59944.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol59988.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol59988.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol60228.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol60228.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol60265.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol60265.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol60399.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol60399.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol60522.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol60522.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol60567.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol60567.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol60632.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol60632.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol60821.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol60821.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol61129.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol61129.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol61361.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol61361.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol61552.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol61552.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol61718.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol61718.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol61872.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol61872.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol61952.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol61952.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol62119.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol62119.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol62212.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol62212.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol62424.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol62424.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol62548.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol62548.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol62833.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol62833.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol63070.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol63070.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol63203.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol63203.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol63402.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol63402.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol63507.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol63507.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol63635.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol63635.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol64100.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol64100.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol64129.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol64129.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol64255.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol64255.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol64331.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol64331.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol64455.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol64455.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol64657.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol64657.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol64863.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol64863.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol65006.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol65006.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol65054.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol65054.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol65285.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol65285.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol65579.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol65579.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol65617.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol65617.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol65654.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol65654.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol65655.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol65655.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol65751.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol65751.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol65846.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol65846.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol65943.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol65943.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol66182.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol66182.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol66292.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol66292.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol66488.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol66488.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol66810.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol66810.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol66946.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol66946.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol66977.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol66977.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol67143.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol67143.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol67462.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol67462.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol67621.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol67621.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol67679.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol67679.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol67985.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol67985.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol68406.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol68406.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol68509.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol68509.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol68669.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol68669.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol68740.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol68740.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol68778.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol68778.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol69099.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol69099.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol69185.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol69185.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol69228.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol69228.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol69264.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol69264.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol69350.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol69350.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol69790.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol69790.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol69823.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol69823.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol69947.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol69947.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol70133.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol70133.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol70200.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol70200.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol70616.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol70616.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol70682.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol70682.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol70920.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol70920.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol71040.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol71040.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol71134.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol71134.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol71138.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol71138.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol71449.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol71449.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol71652.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol71652.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol71931.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol71931.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol72053.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol72053.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol72191.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol72191.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol72307.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol72307.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol72481.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol72481.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol72649.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol72649.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol72880.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol72880.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol73016.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol73016.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol73493.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol73493.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol73576.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol73576.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol73662.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol73662.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol74238.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol74238.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol74592.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol74592.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol74665.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol74665.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol74739.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol74739.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol75132.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol75132.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol75410.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol75410.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol75484.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol75484.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol75589.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol75589.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol75792.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol75792.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol76003.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol76003.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol76124.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol76124.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol76268.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol76268.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol76389.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol76389.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol76437.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol76437.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol76517.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol76517.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol76753.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol76753.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol76781.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol76781.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol76893.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol76893.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol77205.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol77205.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol77406.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol77406.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol77435.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol77435.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol77525.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol77525.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol77548.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol77548.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol77662.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol77662.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol77692.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol77692.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol77981.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol77981.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol78256.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol78256.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol78679.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol78679.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol78725.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol78725.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol79033.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol79033.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol79155.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol79155.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol79515.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol79515.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol79999.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol79999.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol80046.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol80046.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol80205.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol80205.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol80293.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol80293.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol80333.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol80333.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol80702.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol80702.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol81376.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol81376.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol81571.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol81571.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol81700.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol81700.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol82169.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol82169.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol82624.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol82624.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol83004.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol83004.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol83077.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol83077.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol83086.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol83086.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol83632.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol83632.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol83716.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol83716.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol84200.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol84200.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol84249.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol84249.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol85027.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol85027.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol85267.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol85267.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol85311.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol85311.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol85551.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol85551.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol85576.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol85576.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol85894.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol85894.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol86223.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol86223.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol86938.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol86938.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol87306.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol87306.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol87774.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol87774.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol87990.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol87990.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol88122.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol88122.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol88481.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol88481.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol88936.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol88936.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol89566.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol89566.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol/versions/protocol89754.py` & `heroprotocol-2.55.3.90670/heroprotocol/versions/protocol89754.py`

 * *Files identical despite different names*

### Comparing `heroprotocol-2.55.3.89754/heroprotocol.egg-info/PKG-INFO` & `heroprotocol-2.55.3.90670/heroprotocol.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,158 +1,157 @@
 Metadata-Version: 2.1
 Name: heroprotocol
-Version: 2.55.3.89754
+Version: 2.55.3.90670
 Summary: Python library to decode Heroes of the Storm replays
 Home-page: https://github.com/Blizzard/heroprotocol
 Author: Blizzard Entertainment
 Author-email: HeroesReplays@blizzard.com
-License: UNKNOWN
-Description: # heroprotocol
-        
-        heroprotocol is a [Python](https://www.python.org/downloads/) library and command-line tool to decode Heroes of the Storm replay files into Python data structures.
-        
-        The tool is available as a [PyPI Package](https://pypi.org/project/heroprotocol/) or as source code.
-        
-        Currently heroprotocol can decode these structures and events:
-        
-        * Replay header
-        * Game details
-        * Replay init data
-        * Game events
-        * Message events
-        * Tracker events
-        
-        heroprotocol can be used as a base-build-specific library to decode binary blobs, or it can be run as a standalone tool
-        to pretty print information from supported replay files.
-        
-        Note that heroprotocol does not expose game balance information or provide any kind of high level analysis of replays;
-        it's meant to be just the first tool in the chain for your data mining application.
-        
-        ## Supported Versions
-        
-        heroprotocol supports all Hereos of the Storm replay files that were played with retail and PTR versions of the game.
-        
-        ## Requirements
-        
-        * Python 2.7 or 3.x
-          * Note: A future release may remove support for Python 2.7
-        * Python Packages:
-          * mpyq 0.2.5+
-          * six 1.14.0+
-        
-        ## Installation
-        
-        Either install/update using pip:
-        
-        ```bash
-        python -m pip install --upgrade heroprotocol
-        ```
-        
-        Or clone the repository and run from source:
-        
-        ```bash
-        git clone https://github.com/Blizzard/heroprotocol.git
-        python -m pip install -r ./heroprotocol/heroprotocol/requirements.txt
-        ```
-        
-        ## Command Line Arguments
-        
-        ```plain
-        -h, --help          Show the options that are available.
-        
-        Tracker Events:
-        --gameevents        Print all game events including coordinates
-        --messageevents     Print message events such as ping events
-        --trackerevents     Print tracker events such as units killed, game stat events,
-                            score result event
-        --attributeevents   Print attribute events, a table of attrid, namespace, and attribute values
-        --header            Print protocol header including build id and elapsedGameLoops
-        --details           Print protocol details, e.g. teamId, player names and chosen heroes,
-                            player region, game result, observer status
-        --initdata          Print protocol initdata, e.g. interface settings for every player
-        
-        Output Options:
-        --stats             Output stats about the active tracker event to the STDERR stream
-        --json              Use JSON syntax for output
-        ```
-        
-        ## Example Usage
-        
-        If you want the output shown directly in the terminal, leave out the `> output.txt`.
-        
-        ```bash
-        python -m heroprotocol --details "Blackheart's Bay.StormReplay" > output.txt
-        ```
-        
-        By default, data is output as a Python dictionary object. To output a JSON file, add `--json`.
-        
-        **Note**, however, that the JSON file is formatted as a sequence/stream of JSON objects and
-        will likely not parse as regular JSON.
-        
-        ## Tracker Events
-        
-        Some notes on tracker events:
-        
-        * Convert unit tag index, recycle pairs into unit tags (as seen in game events) with protocol.unit_tag (index, recycle)
-        * Interpret the NNet.Replay.Tracker.SUnitPositionsEvent events like this:
-        
-        ```python
-        unitIndex = event['m_firstUnitIndex']
-        for i in range(0, len(event['m_items']), 3):
-            unitIndex += event['m_items'][i + 0]
-            x = event['m_items'][i + 1] * 4
-            y = event['m_items'][i + 2] * 4
-            # unit identified by unitIndex at the current event['_gameloop'] time
-            # is at approximate position (x, y)
-        ```
-        
-        * Only units that have inflicted or taken damage are mentioned in unit position events, and they occur periodically with a limit of 256 units mentioned per event.
-        * NNet.Replay.Tracker.SUnitInitEvent events appear for units under construction. When complete you'll see a NNet.Replay.Tracker.SUnitDoneEvent with the same unit tag.
-        * NNet.Replay.Tracker.SUnitBornEvent events appear for units that are created fully constructed.
-        * You may receive a NNet.Replay.Tracker.SUnitDiedEvent after either a UnitInit or UnitBorn event for the corresponding unit tag.
-        * In NNet.Replay.Tracker.SPlayerStatsEvent, m_scoreValueFoodUsed and m_scoreValueFoodMade are in fixed point (divide by 4096 for integer values). All other values are in integers.
-        * There's a known issue where revived units are not tracked, and placeholder units track death but not birth.
-        
-        ## Reporting Bugs
-        
-        Please report bugs at the [Heroes of the Storm Bug Report Forum](https://us.forums.blizzard.com/en/heroes/c/bug-report).
-        
-        ## Acknowledgements
-        
-        The standalone tool uses [mpyq](https://github.com/eagleflo/mpyq) by
-        [Aku Kotkavuo](https://github.com/eagleflo) to read mopaq files.
-        
-        Thank you to [healingbrew](https://github.com/healingbrew), [MGatner](https://github.com/mgatner),
-        [koliva8245](https://github.com/koliva8245), [casualMLG](https://github.com/casualmlg), and others for submitting issues
-        and feedback.
-        
-        Thank you to [Christian Clauss](https://github.com/cclauss), [Jingbei Li](https://github.com/petronny), and
-        [Regner Blok-Andersen](https://github.com/regner) for contributions to the Python 3 update.
-        
-        Thank you to David Joerg and Graylin Kim of [GGTracker](http://www.ggtracker.com) for design feedback and beta-testing of
-        the s2protocol library that heroprotocol is based upon.
-        
-        Thanks to Ben Barrett of [HOTSLogs](http://www.hotslogs.com) for early feedback on and beta-testing of the heroprotocol
-        library.
-        
-        ## License
-        
-        Copyright 2021 Blizzard Entertainment
-        
-        Source code for this project is released to the public under the MIT license.
-        See the included [LICENSE](LICENSE) file for more information.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Games/Entertainment :: Real Time Strategy
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Archiving
 Classifier: Topic :: Utilities
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# heroprotocol
+
+heroprotocol is a [Python](https://www.python.org/downloads/) library and command-line tool to decode Heroes of the Storm replay files into Python data structures.
+
+The tool is available as a [PyPI Package](https://pypi.org/project/heroprotocol/) or as source code.
+
+Currently heroprotocol can decode these structures and events:
+
+* Replay header
+* Game details
+* Replay init data
+* Game events
+* Message events
+* Tracker events
+
+heroprotocol can be used as a base-build-specific library to decode binary blobs, or it can be run as a standalone tool
+to pretty print information from supported replay files.
+
+Note that heroprotocol does not expose game balance information or provide any kind of high level analysis of replays;
+it's meant to be just the first tool in the chain for your data mining application.
+
+## Supported Versions
+
+heroprotocol supports all Hereos of the Storm replay files that were played with retail and PTR versions of the game.
+
+## Requirements
+
+* Python 2.7 or 3.x
+  * Note: A future release may remove support for Python 2.7
+* Python Packages:
+  * mpyq 0.2.5+
+  * six 1.14.0+
+
+## Installation
+
+Either install/update using pip:
+
+```bash
+python -m pip install --upgrade heroprotocol
+```
+
+Or clone the repository and run from source:
+
+```bash
+git clone https://github.com/Blizzard/heroprotocol.git
+python -m pip install -r ./heroprotocol/heroprotocol/requirements.txt
+```
+
+## Command Line Arguments
+
+```plain
+-h, --help          Show the options that are available.
+
+Tracker Events:
+--gameevents        Print all game events including coordinates
+--messageevents     Print message events such as ping events
+--trackerevents     Print tracker events such as units killed, game stat events,
+                    score result event
+--attributeevents   Print attribute events, a table of attrid, namespace, and attribute values
+--header            Print protocol header including build id and elapsedGameLoops
+--details           Print protocol details, e.g. teamId, player names and chosen heroes,
+                    player region, game result, observer status
+--initdata          Print protocol initdata, e.g. interface settings for every player
+
+Output Options:
+--stats             Output stats about the active tracker event to the STDERR stream
+--json              Use JSON syntax for output
+```
+
+## Example Usage
+
+If you want the output shown directly in the terminal, leave out the `> output.txt`.
+
+```bash
+python -m heroprotocol --details "Blackheart's Bay.StormReplay" > output.txt
+```
+
+By default, data is output as a Python dictionary object. To output a JSON file, add `--json`.
+
+**Note**, however, that the JSON file is formatted as a sequence/stream of JSON objects and
+will likely not parse as regular JSON.
+
+## Tracker Events
+
+Some notes on tracker events:
+
+* Convert unit tag index, recycle pairs into unit tags (as seen in game events) with protocol.unit_tag (index, recycle)
+* Interpret the NNet.Replay.Tracker.SUnitPositionsEvent events like this:
+
+```python
+unitIndex = event['m_firstUnitIndex']
+for i in range(0, len(event['m_items']), 3):
+    unitIndex += event['m_items'][i + 0]
+    x = event['m_items'][i + 1] * 4
+    y = event['m_items'][i + 2] * 4
+    # unit identified by unitIndex at the current event['_gameloop'] time
+    # is at approximate position (x, y)
+```
+
+* Only units that have inflicted or taken damage are mentioned in unit position events, and they occur periodically with a limit of 256 units mentioned per event.
+* NNet.Replay.Tracker.SUnitInitEvent events appear for units under construction. When complete you'll see a NNet.Replay.Tracker.SUnitDoneEvent with the same unit tag.
+* NNet.Replay.Tracker.SUnitBornEvent events appear for units that are created fully constructed.
+* You may receive a NNet.Replay.Tracker.SUnitDiedEvent after either a UnitInit or UnitBorn event for the corresponding unit tag.
+* In NNet.Replay.Tracker.SPlayerStatsEvent, m_scoreValueFoodUsed and m_scoreValueFoodMade are in fixed point (divide by 4096 for integer values). All other values are in integers.
+* There's a known issue where revived units are not tracked, and placeholder units track death but not birth.
+
+## Reporting Bugs
+
+Please report bugs at the [Heroes of the Storm Bug Report Forum](https://us.forums.blizzard.com/en/heroes/c/bug-report).
+
+## Acknowledgements
+
+The standalone tool uses [mpyq](https://github.com/eagleflo/mpyq) by
+[Aku Kotkavuo](https://github.com/eagleflo) to read mopaq files.
+
+Thank you to [healingbrew](https://github.com/healingbrew), [MGatner](https://github.com/mgatner),
+[koliva8245](https://github.com/koliva8245), [casualMLG](https://github.com/casualmlg), and others for submitting issues
+and feedback.
+
+Thank you to [Christian Clauss](https://github.com/cclauss), [Jingbei Li](https://github.com/petronny), and
+[Regner Blok-Andersen](https://github.com/regner) for contributions to the Python 3 update.
+
+Thank you to David Joerg and Graylin Kim of [GGTracker](http://www.ggtracker.com) for design feedback and beta-testing of
+the s2protocol library that heroprotocol is based upon.
+
+Thanks to Ben Barrett of [HOTSLogs](http://www.hotslogs.com) for early feedback on and beta-testing of the heroprotocol
+library.
+
+## License
+
+Copyright 2021 Blizzard Entertainment
+
+Source code for this project is released to the public under the MIT license.
+See the included [LICENSE](LICENSE) file for more information.
```

### Comparing `heroprotocol-2.55.3.89754/heroprotocol.egg-info/SOURCES.txt` & `heroprotocol-2.55.3.90670/heroprotocol.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 heroprotocol/__init__.py
 heroprotocol/__main__.py
 heroprotocol/build.py
 heroprotocol/compat.py
 heroprotocol/decoders.py
@@ -327,8 +328,9 @@
 heroprotocol/versions/protocol87306.py
 heroprotocol/versions/protocol87774.py
 heroprotocol/versions/protocol87990.py
 heroprotocol/versions/protocol88122.py
 heroprotocol/versions/protocol88481.py
 heroprotocol/versions/protocol88936.py
 heroprotocol/versions/protocol89566.py
-heroprotocol/versions/protocol89754.py
+heroprotocol/versions/protocol89754.py
+heroprotocol/versions/protocol90670.py
```

### Comparing `heroprotocol-2.55.3.89754/setup.py` & `heroprotocol-2.55.3.90670/setup.py`

 * *Files identical despite different names*

