# Comparing `tmp/bhv-0.6.5.tar.gz` & `tmp/bhv-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bhv-0.6.5.tar", last modified: Mon Jun 26 21:03:12 2023, max compression
+gzip compressed data, was "bhv-0.8.0.tar", last modified: Tue Aug  1 14:31:08 2023, max compression
```

## Comparing `bhv-0.6.5.tar` & `bhv-0.8.0.tar`

### file list

```diff
@@ -1,50 +1,128 @@
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-06-26 21:03:12.783940 bhv-0.6.5/
--rw-r--r--   0 adamv     (1000) adamv     (1000)    35149 2023-04-23 16:58:42.000000 bhv-0.6.5/LICENSE
--rw-r--r--   0 adamv     (1000) adamv     (1000)       50 2023-06-25 20:42:11.000000 bhv-0.6.5/MANIFEST.in
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1054 2023-06-26 21:03:12.783940 bhv-0.6.5/PKG-INFO
--rw-r--r--   0 adamv     (1000) adamv     (1000)     6887 2023-06-26 21:02:34.000000 bhv-0.6.5/README.md
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-06-26 21:03:12.780606 bhv-0.6.5/bhv/
--rw-r--r--   0 adamv     (1000) adamv     (1000)       64 2023-04-24 11:50:09.000000 bhv-0.6.5/bhv/__init__.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    17289 2023-06-26 20:49:31.000000 bhv-0.6.5/bhv/abstract.py
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-06-26 21:03:12.780606 bhv-0.6.5/bhv/cnative/
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-06-26 21:03:12.783940 bhv-0.6.5/bhv/cnative/TurboSHAKEopt/
--rw-r--r--   0 adamv     (1000) adamv     (1000)    22154 2023-06-25 20:42:11.000000 bhv-0.6.5/bhv/cnative/TurboSHAKEopt/KeccakP-1600-64.macros
--rw-r--r--   0 adamv     (1000) adamv     (1000)     2383 2023-06-25 20:42:11.000000 bhv-0.6.5/bhv/cnative/TurboSHAKEopt/KeccakP-1600-SnP.h
--rw-r--r--   0 adamv     (1000) adamv     (1000)      186 2023-06-25 20:42:11.000000 bhv-0.6.5/bhv/cnative/TurboSHAKEopt/KeccakP-1600-opt64-config.h
--rw-r--r--   0 adamv     (1000) adamv     (1000)    18997 2023-06-25 20:42:11.000000 bhv-0.6.5/bhv/cnative/TurboSHAKEopt/KeccakP-1600-opt64.cpp
--rw-r--r--   0 adamv     (1000) adamv     (1000)     9730 2023-06-25 20:42:11.000000 bhv-0.6.5/bhv/cnative/TurboSHAKEopt/KeccakP-1600-unrolling.macros
--rw-r--r--   0 adamv     (1000) adamv     (1000)     2537 2023-06-25 20:42:11.000000 bhv-0.6.5/bhv/cnative/TurboSHAKEopt/KeccakSponge.cpp
--rw-r--r--   0 adamv     (1000) adamv     (1000)     2811 2023-06-25 20:42:11.000000 bhv-0.6.5/bhv/cnative/TurboSHAKEopt/KeccakSponge.h
--rw-r--r--   0 adamv     (1000) adamv     (1000)    11249 2023-06-25 20:42:11.000000 bhv-0.6.5/bhv/cnative/TurboSHAKEopt/KeccakSponge.inc
--rw-r--r--   0 adamv     (1000) adamv     (1000)     6272 2023-06-25 20:42:11.000000 bhv-0.6.5/bhv/cnative/TurboSHAKEopt/SnP-Relaned.h
--rw-r--r--   0 adamv     (1000) adamv     (1000)     2381 2023-06-25 20:42:11.000000 bhv-0.6.5/bhv/cnative/TurboSHAKEopt/TurboSHAKE.cpp
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1673 2023-06-25 20:42:11.000000 bhv-0.6.5/bhv/cnative/TurboSHAKEopt/TurboSHAKE.h
--rw-r--r--   0 adamv     (1000) adamv     (1000)      873 2023-06-25 20:42:11.000000 bhv-0.6.5/bhv/cnative/TurboSHAKEopt/align.h
--rw-r--r--   0 adamv     (1000) adamv     (1000)     5638 2023-06-25 20:42:11.000000 bhv-0.6.5/bhv/cnative/TurboSHAKEopt/brg_endian.h
--rw-r--r--   0 adamv     (1000) adamv     (1000)      136 2023-06-25 20:42:11.000000 bhv-0.6.5/bhv/cnative/TurboSHAKEopt/config.h
--rw-r--r--   0 adamv     (1000) adamv     (1000)    11558 2023-06-25 20:42:11.000000 bhv-0.6.5/bhv/cnative/bindings.cpp
--rw-r--r--   0 adamv     (1000) adamv     (1000)     8239 2023-06-25 20:42:11.000000 bhv-0.6.5/bhv/cnative/packed.h
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1566 2023-06-12 22:49:54.000000 bhv-0.6.5/bhv/cnative/plain_test.cpp
--rw-r--r--   0 adamv     (1000) adamv     (1000)       68 2023-06-12 22:49:54.000000 bhv-0.6.5/bhv/cnative/run.sh
--rw-r--r--   0 adamv     (1000) adamv     (1000)      392 2023-06-12 22:49:54.000000 bhv-0.6.5/bhv/cnative/shared.h
--rw-r--r--   0 adamv     (1000) adamv     (1000)     2120 2023-05-09 10:08:10.000000 bhv-0.6.5/bhv/embedding.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     4208 2023-06-25 20:42:11.000000 bhv-0.6.5/bhv/lookup.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1897 2023-06-25 20:42:11.000000 bhv-0.6.5/bhv/native.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    12746 2023-06-26 20:55:33.000000 bhv-0.6.5/bhv/np.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    11425 2023-05-27 17:35:51.000000 bhv-0.6.5/bhv/poibin.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1683 2023-04-28 18:20:39.000000 bhv-0.6.5/bhv/positions.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     8293 2023-05-23 15:35:44.000000 bhv-0.6.5/bhv/pytorch.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     3360 2023-05-15 19:33:58.000000 bhv-0.6.5/bhv/shared.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1195 2023-05-23 15:35:44.000000 bhv-0.6.5/bhv/slice.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    26226 2023-05-25 00:18:10.000000 bhv-0.6.5/bhv/symbolic.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1747 2023-05-23 17:48:54.000000 bhv-0.6.5/bhv/unification.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     3762 2023-06-26 20:54:32.000000 bhv-0.6.5/bhv/vanilla.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     2059 2023-06-26 20:45:33.000000 bhv-0.6.5/bhv/visualization.py
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-06-26 21:03:12.780606 bhv-0.6.5/bhv.egg-info/
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1054 2023-06-26 21:03:12.000000 bhv-0.6.5/bhv.egg-info/PKG-INFO
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1124 2023-06-26 21:03:12.000000 bhv-0.6.5/bhv.egg-info/SOURCES.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)        1 2023-06-26 21:03:12.000000 bhv-0.6.5/bhv.egg-info/dependency_links.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)       44 2023-06-26 21:03:12.000000 bhv-0.6.5/bhv.egg-info/requires.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)        4 2023-06-26 21:03:12.000000 bhv-0.6.5/bhv.egg-info/top_level.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)       38 2023-06-26 21:03:12.783940 bhv-0.6.5/setup.cfg
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1961 2023-06-26 21:01:15.000000 bhv-0.6.5/setup.py
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-08-01 14:31:08.800197 bhv-0.8.0/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       47 2023-05-13 14:44:39.000000 bhv-0.8.0/.gitignore
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    35149 2023-04-23 16:58:42.000000 bhv-0.8.0/LICENSE
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       50 2023-06-25 20:42:11.000000 bhv-0.8.0/MANIFEST.in
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1054 2023-08-01 14:31:08.800197 bhv-0.8.0/PKG-INFO
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     6987 2023-07-27 10:41:19.000000 bhv-0.8.0/README.md
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-08-01 14:31:08.783529 bhv-0.8.0/benchmarks/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2158 2023-06-25 20:42:11.000000 bhv-0.8.0/benchmarks/exact_synthesis.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1879 2023-06-25 20:42:11.000000 bhv-0.8.0/benchmarks/layerwise_random_execution.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1829 2023-06-25 20:42:11.000000 bhv-0.8.0/benchmarks/lookup.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1307 2023-07-27 10:41:19.000000 bhv-0.8.0/benchmarks/majority.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2635 2023-06-25 20:42:11.000000 bhv-0.8.0/benchmarks/random_network.py
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-08-01 14:31:08.786863 bhv-0.8.0/bhv/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       64 2023-04-24 11:50:09.000000 bhv-0.8.0/bhv/__init__.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    17267 2023-07-27 10:41:19.000000 bhv-0.8.0/bhv/abstract.py
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-08-01 14:31:08.790196 bhv-0.8.0/bhv/cnative/
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-08-01 14:31:08.790196 bhv-0.8.0/bhv/cnative/TurboSHAKE_AVX512/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      186 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_AVX512/KeccakP-1600-AVX512-config.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    18986 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_AVX512/KeccakP-1600-AVX512.cpp
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2183 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_AVX512/KeccakP-1600-SnP.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2537 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_AVX512/KeccakSponge.cpp
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2811 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_AVX512/KeccakSponge.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    11249 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_AVX512/KeccakSponge.inc
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2406 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_AVX512/TurboSHAKE.cpp
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1673 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_AVX512/TurboSHAKE.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      873 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_AVX512/align.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     5638 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_AVX512/brg_endian.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      136 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_AVX512/config.h
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-08-01 14:31:08.793530 bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    22154 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/KeccakP-1600-64.macros
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2383 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/KeccakP-1600-SnP.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      186 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/KeccakP-1600-opt64-config.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    19024 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/KeccakP-1600-opt64.cpp
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     9730 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/KeccakP-1600-unrolling.macros
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2537 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/KeccakSponge.cpp
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2811 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/KeccakSponge.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    11249 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/KeccakSponge.inc
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     6272 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/SnP-Relaned.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2408 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/TurboSHAKE.cpp
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1673 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/TurboSHAKE.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      873 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/align.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     5638 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/brg_endian.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      136 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/config.h
+-rwxr-xr-x   0 adamv     (1000) adamv     (1000)  1202008 2023-08-01 13:51:25.000000 bhv-0.8.0/bhv/cnative/a.out
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    35552 2023-08-01 14:05:51.000000 bhv-0.8.0/bhv/cnative/benchmark.cpp
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    14176 2023-08-01 14:12:36.000000 bhv-0.8.0/bhv/cnative/bindings.cpp
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2708 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/core.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    10024 2023-07-31 19:36:17.000000 bhv-0.8.0/bhv/cnative/distance.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      124 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/hash.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     7813 2023-08-01 11:07:04.000000 bhv-0.8.0/bhv/cnative/majority.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     6296 2023-07-27 10:41:19.000000 bhv-0.8.0/bhv/cnative/permutation.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2267 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/plain_test.cpp
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     9955 2023-07-31 19:36:17.000000 bhv-0.8.0/bhv/cnative/random.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)   107227 2023-07-28 00:14:59.000000 bhv-0.8.0/bhv/cnative/random_experiments.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1428 2023-07-27 10:41:19.000000 bhv-0.8.0/bhv/cnative/representative.h
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-08-01 14:31:08.793530 bhv-0.8.0/bhv/cnative/results/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    15710 2023-07-27 15:32:26.000000 bhv-0.8.0/bhv/cnative/results/2-4Mop-128Wavefront-DualScalar.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    16196 2023-07-27 12:26:54.000000 bhv-0.8.0/bhv/cnative/results/2-8Mop-DualScalar.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    15728 2023-07-27 15:07:54.000000 bhv-0.8.0/bhv/cnative/results/4-Bit-Unified-Wavefront-AVX-512.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    15735 2023-07-27 15:26:42.000000 bhv-0.8.0/bhv/cnative/results/4Mop-256Wavefront-AVX.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    15721 2023-07-27 15:22:28.000000 bhv-0.8.0/bhv/cnative/results/4Mop-512-Wavefront.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    15726 2023-07-27 15:13:50.000000 bhv-0.8.0/bhv/cnative/results/4Mop.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    16198 2023-07-27 12:19:02.000000 bhv-0.8.0/bhv/cnative/results/8-Bit-Unified-Wavefront-AVX-512.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    15311 2023-07-27 15:37:51.000000 bhv-0.8.0/bhv/cnative/results/Single-Bit-Parsimonious-Scalar.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    15712 2023-07-27 19:46:41.000000 bhv-0.8.0/bhv/cnative/results/Single-Bit-Single-Buffer-AVX-512.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    15695 2023-07-27 15:44:08.000000 bhv-0.8.0/bhv/cnative/results/Single-Bit-Single-Buffer-AVX2.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    15339 2023-07-27 15:39:40.000000 bhv-0.8.0/bhv/cnative/results/Single-Bit-Single-Buffer-Scalar.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    31555 2023-08-01 14:04:19.000000 bhv-0.8.0/bhv/cnative/results/all_avx2.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    15799 2023-07-27 15:07:32.000000 bhv-0.8.0/bhv/cnative/results/negative_tree_avx512.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    16189 2023-07-27 13:48:36.000000 bhv-0.8.0/bhv/cnative/results/sparse_tree.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    15775 2023-07-28 00:02:07.000000 bhv-0.8.0/bhv/cnative/results/ternary_tree.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    39644 2023-07-27 15:49:27.000000 bhv-0.8.0/bhv/cnative/results.zip
+-rwxr-xr-x   0 adamv     (1000) adamv     (1000)      255 2023-08-01 14:05:16.000000 bhv-0.8.0/bhv/cnative/run.sh
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      396 2023-07-27 10:41:19.000000 bhv-0.8.0/bhv/cnative/shared.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     8457 2023-07-27 10:41:19.000000 bhv-0.8.0/bhv/cnative/simdpcg.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    46933 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/ternary.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     5189 2023-07-28 01:18:44.000000 bhv-0.8.0/bhv/cnative/testing.cpp
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    38396 2023-08-01 14:05:51.000000 bhv-0.8.0/bhv/cnative/threshold.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2120 2023-05-09 10:08:10.000000 bhv-0.8.0/bhv/embedding.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     4208 2023-06-25 20:42:11.000000 bhv-0.8.0/bhv/lookup.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2608 2023-07-27 10:41:19.000000 bhv-0.8.0/bhv/native.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    13110 2023-07-27 10:41:19.000000 bhv-0.8.0/bhv/np.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    11425 2023-05-27 17:35:51.000000 bhv-0.8.0/bhv/poibin.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1683 2023-04-28 18:20:39.000000 bhv-0.8.0/bhv/positions.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     8455 2023-07-27 10:41:19.000000 bhv-0.8.0/bhv/pytorch.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     3588 2023-07-27 10:41:19.000000 bhv-0.8.0/bhv/shared.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1195 2023-05-23 15:35:44.000000 bhv-0.8.0/bhv/slice.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    27835 2023-07-28 01:18:57.000000 bhv-0.8.0/bhv/symbolic.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1747 2023-05-23 17:48:54.000000 bhv-0.8.0/bhv/unification.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     3839 2023-07-27 10:41:19.000000 bhv-0.8.0/bhv/vanilla.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     6602 2023-07-27 10:41:19.000000 bhv-0.8.0/bhv/variants.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2069 2023-07-27 10:41:19.000000 bhv-0.8.0/bhv/visualization.py
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-08-01 14:31:08.786863 bhv-0.8.0/bhv.egg-info/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1054 2023-08-01 14:31:08.000000 bhv-0.8.0/bhv.egg-info/PKG-INFO
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     3478 2023-08-01 14:31:08.000000 bhv-0.8.0/bhv.egg-info/SOURCES.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)        1 2023-08-01 14:31:08.000000 bhv-0.8.0/bhv.egg-info/dependency_links.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       44 2023-08-01 14:31:08.000000 bhv-0.8.0/bhv.egg-info/requires.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)        4 2023-08-01 14:31:08.000000 bhv-0.8.0/bhv.egg-info/top_level.txt
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-08-01 14:31:08.796863 bhv-0.8.0/examples/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    23765 2023-05-14 01:00:15.000000 bhv-0.8.0/examples/Kanerva09.ipynb
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    11380 2023-05-14 01:00:15.000000 bhv-0.8.0/examples/Metric_Picker.ipynb
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      903 2023-07-11 12:00:53.000000 bhv-0.8.0/examples/ca_rules.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1843 2023-05-13 14:46:42.000000 bhv-0.8.0/examples/grandmother_example.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    13478 2023-05-13 15:07:15.000000 bhv-0.8.0/examples/kanerva09.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      389 2023-07-27 10:41:19.000000 bhv-0.8.0/examples/majority_classification.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2414 2023-07-27 10:41:19.000000 bhv-0.8.0/examples/reasoning_by_analogy_adiabatic.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2726 2023-07-27 10:41:19.000000 bhv-0.8.0/examples/reasoning_by_analogy_linear.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1169 2023-05-13 15:04:14.000000 bhv-0.8.0/examples/state_machine.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      294 2023-05-13 15:04:14.000000 bhv-0.8.0/examples/viz_distances.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      686 2023-05-13 15:07:15.000000 bhv-0.8.0/examples/winnow_classification.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       38 2023-08-01 14:31:08.800197 bhv-0.8.0/setup.cfg
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2050 2023-08-01 14:27:17.000000 bhv-0.8.0/setup.py
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-08-01 14:31:08.796863 bhv-0.8.0/tests/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     3196 2023-05-15 19:48:48.000000 bhv-0.8.0/tests/blocklsynth.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     3981 2023-06-25 20:42:11.000000 bhv-0.8.0/tests/composites.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      837 2023-04-11 14:49:00.000000 bhv-0.8.0/tests/embedding.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     3037 2023-06-12 22:49:54.000000 bhv-0.8.0/tests/fiestal.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1193 2023-07-27 10:41:19.000000 bhv-0.8.0/tests/inspect_random.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    13700 2023-07-27 10:41:19.000000 bhv-0.8.0/tests/laws.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1253 2023-06-28 14:28:44.000000 bhv-0.8.0/tests/lsynthesis.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1437 2023-06-26 20:59:59.000000 bhv-0.8.0/tests/marshalling.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      332 2023-06-12 22:49:54.000000 bhv-0.8.0/tests/metrics.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      913 2023-08-01 11:05:34.000000 bhv-0.8.0/tests/native_test.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      835 2023-05-23 15:42:03.000000 bhv-0.8.0/tests/reconstruct_program.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      998 2023-07-28 01:19:06.000000 bhv-0.8.0/tests/sym.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     7032 2023-05-23 17:58:09.000000 bhv-0.8.0/tests/sym_laws.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      715 2023-06-25 20:42:11.000000 bhv-0.8.0/tests/symbolic.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      927 2023-03-28 11:00:31.000000 bhv-0.8.0/tests/test_pytorch.py
```

### Comparing `bhv-0.6.5/LICENSE` & `bhv-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bhv-0.6.5/PKG-INFO` & `bhv-0.8.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.6.5
+Version: 0.8.0
 Summary: Boolean Hypervectors
 Home-page: https://github.com/Adam-Vandervorst/PyBHV
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
 Keywords: ai binary hypervector hdc bsc
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bhv-0.6.5/README.md` & `bhv-0.8.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 - A (performant) [plain Python implementation](bhv/vanilla.py)
 - A minimal abstraction for permutations with caching and composition
 - Very [basic embeddings](bhv/embedding.py) for other datatypes (more to come)
 - Graph visualization of distances in hyperdimensional space ([see example](examples/viz_distances.py)).
 - Boolean expression and network synthesis (e.g. [Cellular Automata](examples/ca_rules) and [perfectly random functions](benchmarks/exact_synthesis.py))
 - Visualization and storage via [pbm](bhv/visualization.py) (e.g. [Cellular Automata](examples/ca_rules))
 - A normal form and conversions between different implementations and storage methods
+- [Linear and adiabatic variants](bhv/variants.py) and [example](examples/reasoning_by_analogy_linear.py)
 
 ## Installation
 Make sure you have a recent Python version, 3.10 is recommended.
 
 `pip install bhv`
 
 If you only want to work with plain Python, you're good to go with `from bhv.vanilla VanillaBHV as BHV`.
@@ -53,15 +54,15 @@
 ### New to Hyperdimensional Computing
 Basic uses (in the context of [neo-GOFAI](https://www.cs.cmu.edu/~cga/gofai/)) are given in [my presentation with a installation-free notebook](https://colab.research.google.com/drive/10XSpooxDAeYVMivF3W2-N0W5yEIUfdZl?usp=sharing). 
 
 The fundamental angle is to start is with [Kanerva's initial paper](http://ww.robertdick.org/iesr/papers/kanerva09jan.pdf) together with the library.
 For that, multiple resources are provided:
 - [A notebook going over the very basics](examples/Kanerva09.ipynb)
 - [The grandmother example](examples/grandmother_example.py)
-- [A Google Colab hosted reasoning by analogy example notebook](https://colab.research.google.com/drive/10gOc39TsM5CE-6u3kj2oe1t-8KZHr_bB?usp=sharing)
+- [A Google Colab "reasoning by analogy" hosted notebook](https://colab.research.google.com/drive/10gOc39TsM5CE-6u3kj2oe1t-8KZHr_bB?usp=sharing)
 - [A guide to picking metrics](examples/Metric_Picker.ipynb)
 
 As for a Machine Learning angle, you may enjoy:
 - [A minimal implementation](examples/winnow_classification.py) of the [winnow algorithm](https://en.wikipedia.org/wiki/Winnow_(algorithm)) on a minimal problem
 - [A minimal implementation of classification based on the majority operator](examples/majority_classification.py) on a minimal problem
 - [A Google Colab hosted digit classification via plain majority notebook](https://colab.research.google.com/drive/1xYQAXxcdFw89RV5CsflcvFhx3zpmEUxk?usp=sharing)
 - [Graph classification notebook](https://colab.research.google.com/drive/1NrmCc99GrkmHm_VLs5nv9Q7BCbCLs0ar?usp=sharing) re-implementing [GraphHD](https://arxiv.org/abs/2205.07826)
```

### Comparing `bhv-0.6.5/bhv/abstract.py` & `bhv-0.8.0/bhv/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 from math import comb, log2
 from typing import Iterator
 
 from .shared import *
 
 
 class StoreBHV:
+    def __deepcopy__(self, memodict={}):
+        return self.from_bytes(self.to_bytes())
+
     def to_bytes(self):
         raise NotImplementedError()
 
     @classmethod
     def from_bytes(cls, bs: bytes):
         raise NotImplementedError()
 
@@ -153,18 +156,14 @@
 
     def __or__(self, other: Self) -> Self:
         raise NotImplementedError()
 
     def __invert__(self) -> Self:
         return self ^ self.ONE
 
-    # recall
-    # information_entropy(p) = -p*log2(p) - (1 - p)*log2(1 - p)
-    # so for some active fractions, it should be a lot cheaper than for others
-    # hence a specialized method for 2^-n
     @classmethod
     def rand2(cls, power: int) -> Self:
         assert power >= 0
         r = cls.rand()
         return r if power == 0 else r & cls.rand2(power - 1)
 
     @classmethod
@@ -515,21 +514,25 @@
         for _ in range(power - 1):
             permutation = permutation*permutation
         return permutation
 
     def __call__(self, hv: 'AbstractBHV') -> 'AbstractBHV':
         raise NotImplementedError()
 
+    IDENTITY: Self
+
 
 class MemoizedPermutation(Permutation):
     _permutations: 'dict[int | tuple[int, ...], Self]'
 
     @classmethod
     def _get_singular(cls, permutation_id: int) -> Self:
-        if permutation_id in cls._permutations:
+        if permutation_id == 0:
+            return cls.IDENTITY
+        elif permutation_id in cls._permutations:
             return cls._permutations[permutation_id]
         elif -permutation_id in cls._permutations:
             inv_permutation = cls._permutations[-permutation_id]
             permutation = ~inv_permutation
             cls._permutations[permutation_id] = permutation
             return permutation
         else:
```

### Comparing `bhv-0.6.5/bhv/cnative/TurboSHAKEopt/KeccakP-1600-64.macros` & `bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/KeccakP-1600-64.macros`

 * *Files identical despite different names*

### Comparing `bhv-0.6.5/bhv/cnative/TurboSHAKEopt/KeccakP-1600-SnP.h` & `bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/KeccakP-1600-SnP.h`

 * *Files identical despite different names*

### Comparing `bhv-0.6.5/bhv/cnative/TurboSHAKEopt/KeccakP-1600-opt64.cpp` & `bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/KeccakP-1600-opt64.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 This file implements Keccak-p[1600] in a SnP-compatible way.
 Please refer to SnP-documentation.h for more details.
 
 This implementation comes with KeccakP-1600-SnP.h in the same folder.
 Please refer to LowLevel.build for the exact list of other files it must be combined with.
 */
-
+#ifndef __AVX512BW__
 #include <stdint.h>
 #include <string.h>
 #include <stdlib.h>
 #include "brg_endian.h"
 #include "KeccakP-1600-opt64-config.h"
 
 #if defined(KeccakP1600_useLaneComplementing)
@@ -559,7 +559,8 @@
         rounds12
         inDataAsLanes += laneCount;
         dataByteLen -= laneCount*8;
     }
     copyToState(stateAsLanes, A)
     return originalDataByteLen - dataByteLen;
 }
+#endif
```

### Comparing `bhv-0.6.5/bhv/cnative/TurboSHAKEopt/KeccakP-1600-unrolling.macros` & `bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/KeccakP-1600-unrolling.macros`

 * *Files identical despite different names*

### Comparing `bhv-0.6.5/bhv/cnative/TurboSHAKEopt/KeccakSponge.cpp` & `bhv-0.8.0/bhv/cnative/TurboSHAKE_AVX512/KeccakSponge.cpp`

 * *Files identical despite different names*

### Comparing `bhv-0.6.5/bhv/cnative/TurboSHAKEopt/KeccakSponge.h` & `bhv-0.8.0/bhv/cnative/TurboSHAKE_AVX512/KeccakSponge.h`

 * *Files identical despite different names*

### Comparing `bhv-0.6.5/bhv/cnative/TurboSHAKEopt/KeccakSponge.inc` & `bhv-0.8.0/bhv/cnative/TurboSHAKE_AVX512/KeccakSponge.inc`

 * *Files identical despite different names*

### Comparing `bhv-0.6.5/bhv/cnative/TurboSHAKEopt/SnP-Relaned.h` & `bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/SnP-Relaned.h`

 * *Files identical despite different names*

### Comparing `bhv-0.6.5/bhv/cnative/TurboSHAKEopt/TurboSHAKE.cpp` & `bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/TurboSHAKE.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 For more information, feedback or questions, please refer to the Keccak Team website:
 https://keccak.team/
 
 To the extent possible under law, the implementer has waived all copyright
 and related or neighboring rights to the source code in this file.
 http://creativecommons.org/publicdomain/zero/1.0/
 */
-
+#ifndef __AVX512BW__
 #include "TurboSHAKE.h"
 
 #ifdef XKCP_has_KeccakP1600
     #include "KeccakP-1600-SnP.h"
 
     #define prefix TurboSHAKE
     #define SnP KeccakP1600
@@ -65,7 +65,8 @@
     return TurboSHAKE_SpongeAbsorbLastFewBits(instance, domain);
 }
 
 int TurboSHAKE_Squeeze(TurboSHAKE_Instance *instance, unsigned char *data, size_t dataByteLen)
 {
     return TurboSHAKE_SpongeSqueeze(instance, data, dataByteLen);
 }
+#endif
```

### Comparing `bhv-0.6.5/bhv/cnative/TurboSHAKEopt/TurboSHAKE.h` & `bhv-0.8.0/bhv/cnative/TurboSHAKE_AVX512/TurboSHAKE.h`

 * *Files identical despite different names*

### Comparing `bhv-0.6.5/bhv/cnative/TurboSHAKEopt/align.h` & `bhv-0.8.0/bhv/cnative/TurboSHAKE_AVX512/align.h`

 * *Files identical despite different names*

### Comparing `bhv-0.6.5/bhv/cnative/TurboSHAKEopt/brg_endian.h` & `bhv-0.8.0/bhv/cnative/TurboSHAKE_AVX512/brg_endian.h`

 * *Files identical despite different names*

### Comparing `bhv-0.6.5/bhv/cnative/plain_test.cpp` & `bhv-0.8.0/bhv/cnative/plain_test.cpp`

 * *Files 25% similar despite different names*

```diff
@@ -1,58 +1,77 @@
 #include <iostream>
 #include <chrono>
 
-#include "packed.h"
+#include "core.h"
 
 using namespace std;
 
 int main() {
-    unsigned long N = 201;
+    constexpr unsigned long N = 201;
 
+    // burn some cycles to get the OS's attention
+    volatile uint64_t x = 0x7834d688d8827099ULL;
+    for (size_t i = 0; i < 50000000; ++i)
+        x = x + (x % 7);
 
     auto t0 = chrono::high_resolution_clock::now();
 
-    word_t * rs[N];
+    word_t *rs[N];
     for (size_t i = 0; i < N; ++i)
         rs[i] = bhv::rand();
 
     auto t1 = chrono::high_resolution_clock::now();
     cout << "rand " << chrono::duration_cast<chrono::nanoseconds>(t1 - t0).count() << endl;
 
-    word_t * m = bhv::true_majority(rs, N);
+
+    word_t *ps[N];
+    for (size_t i = 0; i < N; ++i) {
+        ps[i] = bhv::empty();
+        bhv::roll_word_bits_into(rs[i], 42, ps[i]);
+    }
 
     auto t2 = chrono::high_resolution_clock::now();
-    cout << "majority " << chrono::duration_cast<chrono::nanoseconds>(t2 - t1).count() << endl;
+    cout << "new permute " << chrono::duration_cast<chrono::nanoseconds>(t2 - t1).count() << endl;
+
+    for (size_t i = 0; i < N; ++i) {
+        word_t tmp [WORDS];
+        bhv::roll_word_bits_into(ps[i], -42, tmp);
+        assert(bhv::eq(rs[i], tmp));
+    }
+
+    auto t3 = chrono::high_resolution_clock::now();
+    cout << "rpermute eq " << chrono::duration_cast<chrono::nanoseconds>(t3 - t2).count() << endl;
+
+    word_t *m = bhv::true_majority(rs, N);
+
+    auto t4 = chrono::high_resolution_clock::now();
+    cout << "majority " << chrono::duration_cast<chrono::nanoseconds>(t4 - t3).count() << endl;
 
 #if false
     word_t * ds[N];
     for (size_t i = 0; i < N; ++i) {
         word_t * d = bhv::empty();
         bhv::xor_into(rs[i], m, d);
         ds[i] = d;
     }
 
-    auto t3 = chrono::high_resolution_clock::now();
-    cout << "xor " << chrono::duration_cast<chrono::nanoseconds>(t3 - t2).count() << endl;
+    auto t5 = chrono::high_resolution_clock::now();
+    cout << "xor " << chrono::duration_cast<chrono::nanoseconds>(t5 - t4).count() << endl;
 
     unsigned long qs[N];
     for (size_t i = 0; i < N; ++i)
         qs[i] = bhv::active(ds[i]);
 
-    auto t4 = chrono::high_resolution_clock::now();
-    cout << "active " << chrono::duration_cast<chrono::nanoseconds>(t4 - t3).count() << endl;
+    auto t6 = chrono::high_resolution_clock::now();
+    cout << "active " << chrono::duration_cast<chrono::nanoseconds>(t6 - t5).count() << endl;
 #else
-    unsigned long qs[N];
+    unsigned long total = 0;
     for (size_t i = 0; i < N; ++i)
-        qs[i] = bhv::hamming(rs[i], m);
+        total += bhv::hamming(rs[i], m);
 
-    auto t3 = chrono::high_resolution_clock::now();
-    cout << "hamming " << chrono::duration_cast<chrono::nanoseconds>(t3 - t2).count() << endl;
+    auto t5 = chrono::high_resolution_clock::now();
+    cout << "hamming " << chrono::duration_cast<chrono::nanoseconds>(t5 - t4).count() << endl;
 #endif
 
-    unsigned long total = 0;
-    for (size_t i = 0; i < N; ++i)
-        total += qs[i];
-
-    cout << ((double)total/(double )N) << endl;
+    cout << ((double) total / (double) N) << endl;
     return 0;
 }
```

### Comparing `bhv-0.6.5/bhv/embedding.py` & `bhv-0.8.0/bhv/embedding.py`

 * *Files identical despite different names*

### Comparing `bhv-0.6.5/bhv/lookup.py` & `bhv-0.8.0/bhv/lookup.py`

 * *Files identical despite different names*

### Comparing `bhv-0.6.5/bhv/native.py` & `bhv-0.8.0/bhv/native.py`

 * *Files 26% similar despite different names*

```diff
@@ -37,15 +37,35 @@
 
     def active(self):
         return self.ins.active()
 
     def hamming(self, other):
         return self.ins.hamming(other.ins)
 
-    def permute(self, permutation_id: int):
+    def permute_words(self, permutation_id: int):
+        return NativePackedBHV(self.ins.permute_words(permutation_id))
+
+    def permute_byte_bits(self, permutation_id: int):
+        return NativePackedBHV(self.ins.permute_byte_bits(permutation_id))
+
+    def roll_words(self, d: int):
+        return NativePackedBHV(self.ins.roll_words(d))
+
+    def roll_word_bits(self, d: int):
+        return NativePackedBHV(self.ins.roll_word_bits(d))
+
+    def _permute_composite(self, permutation_id: 'tuple'):
+        v = self
+        for e in permutation_id:
+            v = v.permute(e)
+        return v
+
+    def permute(self, permutation_id: 'int | tuple'):
+        if isinstance(permutation_id, tuple):
+            return self._permute_composite(permutation_id)
         return NativePackedBHV(self.ins.permute(permutation_id))
 
     def rehash(self):
         return NativePackedBHV(self.ins.rehash())
 
     def swap_halves(self):
         return NativePackedBHV(self.ins.swap_halves())
```

### Comparing `bhv-0.6.5/bhv/np.py` & `bhv-0.8.0/bhv/np.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,16 @@
         inv_permutation = np.empty_like(self.data)
         inv_permutation[self.data] = np.arange(DIMENSION)
         return NumPyBoolPermutation(inv_permutation)
 
     def __call__(self, hv: 'NumPyBoolBHV') -> 'NumPyBoolBHV':
         return hv.permute_bits(self)
 
+NumPyBoolPermutation.IDENTITY = NumPyBoolPermutation(np.arange(DIMENSION))
+
 
 class NumPyBoolBHV(AbstractBHV):
     def __init__(self, array: np.ndarray):
         self.data: np.ndarray = array
 
     @classmethod
     def rand(cls) -> 'NumPyBoolBHV':
@@ -138,14 +140,16 @@
         inv_permutation = np.empty_like(self.data)
         inv_permutation[self.data] = np.arange(DIMENSION//8)
         return NumPyBytePermutation(inv_permutation)
 
     def __call__(self, hv: 'NumPyPacked8BHV') -> 'NumPyPacked8BHV':
         return hv.permute_bytes(self)
 
+NumPyBytePermutation.IDENTITY = NumPyBytePermutation(np.arange(DIMENSION//8))
+
 
 class NumPyPacked8BHV(AbstractBHV):
     def __init__(self, array: np.ndarray):
         self.data: np.ndarray = array
 
     @classmethod
     def rand(cls) -> 'NumPyPacked8BHV':
@@ -238,14 +242,16 @@
         inv_permutation = np.empty_like(self.data)
         inv_permutation[self.data] = np.arange(DIMENSION//64)
         return NumPyWordPermutation(inv_permutation)
 
     def __call__(self, hv: 'NumPyPacked64BHV') -> 'NumPyPacked64BHV':
         return hv.permute_words(self)
 
+NumPyWordPermutation.IDENTITY = NumPyWordPermutation(np.arange(DIMENSION//64))
+
 
 class NumPyPacked64BHV(AbstractBHV):
     rng = np.random.SFC64()
 
     def __init__(self, array: np.ndarray):
         self.data: np.ndarray = array
 
@@ -277,20 +283,21 @@
 
     def roll_words(self, n: int) -> 'NumPyPacked64BHV':
         assert abs(n) < DIMENSION//64, "only supports DIMENSION/64 rolls"
         return NumPyPacked64BHV(np.roll(self.data, n))
 
     def roll_word_bits(self, n: int) -> 'NumPyPacked64BHV':
         assert abs(n) < 64, "only supports 64 rolls"
+        # https://github.com/numba/numba/issues/6381
         if n == 0:
             return NumPyPacked64BHV(self.data)
         elif n > 0:
-            return np.bitwise_or(np.right_shift(self.data, n), np.left_shift(self.data, (64 - n)))
+            return NumPyPacked64BHV(np.bitwise_or(np.right_shift(self.data, np.uint64(n)), np.left_shift(self.data, np.uint64(64 - n))))
         else:
-            return np.bitwise_or(np.left_shift(self.data, n), np.right_shift(self.data, (64 - n)))
+            return NumPyPacked64BHV(np.bitwise_or(np.left_shift(self.data, np.uint64(n)), np.right_shift(self.data, np.uint64(64 - n))))
 
     # roll_words and roll_word_bits could be combined for more options allowing positive and negative combinations
     # ((1 2 3 4) (a b c d) (α β γ δ))
     # rolled by 1, -2 for example results in
     # ((γ δ α β) (3 4 1 2) (c d a b))
 
     def permute_words(self, permutation: 'NumPyWordPermutation') -> 'NumPyPacked64BHV':
```

### Comparing `bhv-0.6.5/bhv/poibin.py` & `bhv-0.8.0/bhv/poibin.py`

 * *Files identical despite different names*

### Comparing `bhv-0.6.5/bhv/positions.py` & `bhv-0.8.0/bhv/positions.py`

 * *Files identical despite different names*

### Comparing `bhv-0.6.5/bhv/pytorch.py` & `bhv-0.8.0/bhv/pytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,16 @@
         inv_permutation = torch.empty_like(self.data)
         inv_permutation[self.data] = torch.arange(DIMENSION)
         return TorchBoolPermutation(inv_permutation)
 
     def __call__(self, hv: 'TorchBoolBHV') -> 'TorchBoolBHV':
         return hv.permute_bits(self)
 
+TorchBoolPermutation.IDENTITY = TorchBoolPermutation(torch.arange(DIMENSION))
+
 
 class TorchBoolBHV(AbstractBHV):
     def __init__(self, tensor: torch.BoolTensor):
         self.data: torch.BoolTensor = tensor
 
     @classmethod
     def rand(cls) -> 'TorchBoolBHV':
@@ -146,14 +148,16 @@
         inv_permutation = torch.empty_like(self.data)
         inv_permutation[self.data] = torch.arange(DIMENSION//64)
         return TorchWordPermutation(inv_permutation)
 
     def __call__(self, hv: 'TorchPackedBHV') -> 'TorchPackedBHV':
         return hv.permute_words(self)
 
+TorchWordPermutation.IDENTITY = TorchWordPermutation(torch.arange(DIMENSION//64))
+
 
 class TorchPackedBHV(AbstractBHV):
     def __init__(self, tensor: torch.LongTensor):
         assert DIMENSION % 64 == 0
         self.data: torch.LongTensor = tensor
 
     @classmethod
```

### Comparing `bhv-0.6.5/bhv/shared.py` & `bhv-0.8.0/bhv/shared.py`

 * *Files 6% similar despite different names*

```diff
@@ -107,7 +107,18 @@
         return start + sep.rstrip(" ").join("\n" + aindent + indent + s for s in ss) + "\n" + aindent + end
     else:
         return start + sep.join(s for s in ss) + end
 
 
 def format_list(xs, **kwargs):
     return format_multiple(xs, start="[", sep=", ", end="]", **kwargs)
+
+
+class IdSet:
+    def __init__(self, iterable=()):
+        self.data = {id(x) for x in iterable}
+
+    def __contains__(self, item):
+        return id(item) in self.data
+
+    def add(self, item):
+        self.data.add(id(item))
```

### Comparing `bhv-0.6.5/bhv/slice.py` & `bhv-0.8.0/bhv/slice.py`

 * *Files identical despite different names*

### Comparing `bhv-0.6.5/bhv/symbolic.py` & `bhv-0.8.0/bhv/symbolic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from dataclasses import dataclass, field, fields
+from string import ascii_uppercase
 from .abstract import *
 from .shared import stable_hashcode, bitconfigs, unique_by_id, format_multiple, format_list
 from .slice import Slice
 
 
 class Symbolic:
     name = None
@@ -303,14 +304,60 @@
             return vs[0].select(
                     cls.synth(vs[1:], t[:len(t)//2]),
                     cls.synth(vs[1:], t[len(t)//2:]))
         else:
             return cls.ONE if t[0] else cls.ZERO
 
     @classmethod
+    def synth_af(cls, af: float, depth=1, v_gen=lambda x: Rand(x), threshold=1e-6):
+        assert 0. < af < 1.
+        d = af - (1 / 2) ** depth
+        v = v_gen(depth)
+        if abs(d) > threshold:
+            if d > 0:
+                return v | cls.synth_af(d, depth + 1, v_gen, threshold)
+            else:
+                return v & cls.synth_af(af, depth + 1, v_gen, threshold)
+        else:
+            return v
+
+    @classmethod
+    def synth_af_ternary(cls, af: float, depth=1, v_gen=lambda x: Rand(x), threshold=1e-6):
+        assert 0. < af < 1.
+        da = af - (1 / 2) ** depth
+        va = v_gen(depth)
+
+        if abs(da) < threshold:
+            return va
+
+        if da > 0:
+            af = da
+
+        depth += 1
+        db = af - (1 / 2) ** depth
+        vb = v_gen(depth)
+
+        if db > 0:
+            af = db
+
+        if abs(db) > threshold:
+            ternary_instr = {(True, True): [0,1,1,1,1,1,1,1],
+                             (True, False): [0,0,0,1,1,1,1,1],
+                             (False, True): [0,0,0,0,0,1,1,1],
+                             (False, False): [0,0,0,0,0,0,0,1]}[(da > 0, db > 0)]
+            # TODO implement Ternary op
+            vr = cls.synth_af_ternary(af, depth + 1, v_gen, threshold)
+            return cls.synth([va, vb, vr], ternary_instr)
+
+        if da > 0:
+            return va | vb
+        else:
+            return va & vb
+
+    @classmethod
     def rand(cls) -> Self:
         return Rand()
 
     @classmethod
     def rand2(cls, power: int) -> Self:
         assert power >= 0
         return Rand2(power)
@@ -376,14 +423,19 @@
         return self.p.execute(**kwargs)(self.v.execute(**kwargs))
 
     def expected_active_fraction(self, **kwargs):
         return self.v.expected_active(**kwargs)
 @dataclass
 class Var(SymbolicBHV):
     name: str
+    @classmethod
+    def shortname(cls, i: int, letters=ascii_uppercase):
+        n = len(letters)
+        return cls(letters[i % n] + str(i // n) * (i > n))
+
     def nodename(self, **kwards):
         return self.name
 
     def show(self, **kwargs):
         symbolic_var = kwargs.get("symbolic_var", False)
         return f"Var(\"{self.name}\")" if symbolic_var else self.name
```

### Comparing `bhv-0.6.5/bhv/unification.py` & `bhv-0.8.0/bhv/unification.py`

 * *Files identical despite different names*

### Comparing `bhv-0.6.5/bhv/vanilla.py` & `bhv-0.8.0/bhv/vanilla.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,16 @@
         for i, j in enumerate(self.data):
             p[j] = i
         return VanillaPermutation(p)
 
     def __call__(self, hv: 'VanillaBHV') -> 'VanillaBHV':
         return hv.permute_bytes(self)
 
+VanillaPermutation.IDENTITY = VanillaPermutation(list(range(DIMENSION//8)))
+
 
 class VanillaBHV(AbstractBHV):
     def __init__(self, data: bytes):
         self.data: bytes = data
 
     @classmethod
     def rand(cls) -> 'VanillaBHV':
```

### Comparing `bhv-0.6.5/bhv/visualization.py` & `bhv-0.8.0/bhv/visualization.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,23 +5,23 @@
     @classmethod
     def from_scope(cls, local_dict):
         return cls(*zip(*[(v, k) for k, v in local_dict.items() if isinstance(v, AbstractBHV)]))
 
     def __init__(self, hvs: 'list[AbstractBHV]', labels: 'list[str]'):
         self.hvs = hvs
         self.labels = labels
-        self.adj = [[round(min(v.std_apart(w, invert=True), v.std_apart(w))) if not v.unrelated(w) else 0
+        self.adj = [[round(min(v.std_apart(w, invert=True), v.std_apart(w))) if not v.unrelated(w) else None
                      for v in self.hvs]
                     for w in self.hvs]
 
     def graphviz(self):
         for i, (r, l) in enumerate(zip(self.adj, self.labels)):
             print(f"{i} [label=\"{l}\"];")
             for j, d in enumerate(r):
-                if d != 0 and i < j:
+                if i < j and d is not None:
                     print(f"{i} -- {j} [label=\"{d}\"];")
 
 
 class Image:
     @classmethod
     def load_pbm(cls, file: 'IO[Any]', bhv: 'AbstractBHV', binary=False):
         if binary:
```

### Comparing `bhv-0.6.5/bhv.egg-info/PKG-INFO` & `bhv-0.8.0/bhv.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.6.5
+Version: 0.8.0
 Summary: Boolean Hypervectors
 Home-page: https://github.com/Adam-Vandervorst/PyBHV
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
 Keywords: ai binary hypervector hdc bsc
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bhv-0.6.5/setup.py` & `bhv-0.8.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from setuptools import setup, find_packages, Extension
 
-VERSION = '0.6.5'
+VERSION = '0.8.0'
 DESCRIPTION = 'Boolean Hypervectors'
 LONG_DESCRIPTION = 'Boolean Hypervectors with various operators for experiments in hyperdimensional computing (HDC).'
 
 native = Extension("bhv.cnative",
                    sources=['bhv/cnative/bindings.cpp',
-                            'bhv/cnative/TurboSHAKEopt/TurboSHAKE.cpp',
-                            'bhv/cnative/TurboSHAKEopt/KeccakSponge.cpp',
-                            'bhv/cnative/TurboSHAKEopt/KeccakP-1600-opt64.cpp',
+                            'bhv/cnative/TurboSHAKE_opt/TurboSHAKE.cpp',
+                            'bhv/cnative/TurboSHAKE_opt/KeccakP-1600-opt64.cpp',
+                            'bhv/cnative/TurboSHAKE_AVX512/TurboSHAKE.cpp',
+                            'bhv/cnative/TurboSHAKE_AVX512/KeccakP-1600-AVX512.cpp',
                             ],
                    include_dirs=['bhv/cnative', 'bhv/cnative/TurboSHAKEopt'],
                    extra_compile_args=['-std=c++2a', '-O3', '-march=native', '-Wall'],
                    language='c++',
                    optional=True)
 
 setup(
```

