# Comparing `tmp/pytoniq-0.0.7.tar.gz` & `tmp/pytoniq-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytoniq-0.0.7.tar", last modified: Sun Jul 30 15:05:36 2023, max compression
+gzip compressed data, was "dist/pytoniq-0.0.8.tar", last modified: Tue Aug  1 12:37:09 2023, max compression
```

## Comparing `pytoniq-0.0.7.tar` & `pytoniq-0.0.8.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-30 15:05:36.647804 pytoniq-0.0.7/
--rw-r--r--   0 maxankurb   (501) staff       (20)       29 2023-07-27 17:44:46.000000 pytoniq-0.0.7/MANIFEST.in
--rw-r--r--   0 maxankurb   (501) staff       (20)    13684 2023-07-30 15:05:36.647040 pytoniq-0.0.7/PKG-INFO
--rw-r--r--   0 maxankurb   (501) staff       (20)    13278 2023-07-27 17:32:45.000000 pytoniq-0.0.7/README.md
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-30 15:05:36.598394 pytoniq-0.0.7/pytoniq/
--rw-r--r--   0 maxankurb   (501) staff       (20)      149 2023-07-23 15:42:41.000000 pytoniq-0.0.7/pytoniq/__init__.py
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-30 15:05:36.607803 pytoniq-0.0.7/pytoniq/boc/
--rw-r--r--   0 maxankurb   (501) staff       (20)      222 2023-07-23 15:42:41.000000 pytoniq-0.0.7/pytoniq/boc/__init__.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     3700 2023-07-27 16:08:51.000000 pytoniq-0.0.7/pytoniq/boc/address.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     4204 2023-07-21 09:13:36.000000 pytoniq-0.0.7/pytoniq/boc/builder.py
--rw-r--r--   0 maxankurb   (501) staff       (20)    11007 2023-07-23 16:49:28.000000 pytoniq-0.0.7/pytoniq/boc/cell.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     9079 2023-07-28 16:29:36.000000 pytoniq-0.0.7/pytoniq/boc/deserialize.py
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-30 15:05:36.610860 pytoniq-0.0.7/pytoniq/boc/dict/
--rw-r--r--   0 maxankurb   (501) staff       (20)       41 2023-07-23 15:42:41.000000 pytoniq-0.0.7/pytoniq/boc/dict/__init__.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     5060 2023-07-23 15:16:15.000000 pytoniq-0.0.7/pytoniq/boc/dict/dict.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     3919 2023-07-23 17:27:59.000000 pytoniq-0.0.7/pytoniq/boc/dict/parse.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     4989 2023-06-19 11:55:15.000000 pytoniq-0.0.7/pytoniq/boc/dict/utils.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     1026 2023-07-23 13:47:12.000000 pytoniq-0.0.7/pytoniq/boc/exotic.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     7521 2023-07-11 20:09:21.000000 pytoniq-0.0.7/pytoniq/boc/slice.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     1866 2023-07-05 13:08:40.000000 pytoniq-0.0.7/pytoniq/boc/tvm_bitarray.py
--rw-r--r--   0 maxankurb   (501) staff       (20)      298 2023-07-13 12:16:46.000000 pytoniq-0.0.7/pytoniq/boc/utils.py
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-30 15:05:36.613290 pytoniq-0.0.7/pytoniq/contract/
--rw-r--r--   0 maxankurb   (501) staff       (20)       69 2023-07-23 15:42:41.000000 pytoniq-0.0.7/pytoniq/contract/__init__.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     6750 2023-07-28 19:24:43.000000 pytoniq-0.0.7/pytoniq/contract/contract.py
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-30 15:05:36.614773 pytoniq-0.0.7/pytoniq/contract/nft/
--rw-r--r--   0 maxankurb   (501) staff       (20)       25 2023-07-27 17:13:15.000000 pytoniq-0.0.7/pytoniq/contract/nft/__init__.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     3643 2023-07-27 17:10:31.000000 pytoniq-0.0.7/pytoniq/contract/nft/nft.py
--rw-r--r--   0 maxankurb   (501) staff       (20)      102 2023-07-22 17:41:04.000000 pytoniq-0.0.7/pytoniq/contract/utils.py
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-30 15:05:36.617205 pytoniq-0.0.7/pytoniq/contract/wallets/
--rw-r--r--   0 maxankurb   (501) staff       (20)      151 2023-07-23 15:42:41.000000 pytoniq-0.0.7/pytoniq/contract/wallets/__init__.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     7615 2023-07-23 07:51:49.000000 pytoniq-0.0.7/pytoniq/contract/wallets/highload.py
--rw-r--r--   0 maxankurb   (501) staff       (20)    18779 2023-07-23 07:41:58.000000 pytoniq-0.0.7/pytoniq/contract/wallets/wallet.py
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-30 15:05:36.620548 pytoniq-0.0.7/pytoniq/crypto/
--rw-r--r--   0 maxankurb   (501) staff       (20)        0 2023-06-17 12:05:39.000000 pytoniq-0.0.7/pytoniq/crypto/__init__.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     2087 2023-05-27 14:21:05.000000 pytoniq-0.0.7/pytoniq/crypto/ciphers.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     6558 2023-06-17 13:10:44.000000 pytoniq-0.0.7/pytoniq/crypto/crc.py
--rw-r--r--   0 maxankurb   (501) staff       (20)    22014 2023-07-22 13:35:04.000000 pytoniq-0.0.7/pytoniq/crypto/keys.py
--rw-r--r--   0 maxankurb   (501) staff       (20)      820 2023-07-27 14:32:52.000000 pytoniq-0.0.7/pytoniq/crypto/signature.py
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-30 15:05:36.624807 pytoniq-0.0.7/pytoniq/liteclient/
--rw-r--r--   0 maxankurb   (501) staff       (20)       88 2023-07-23 15:42:41.000000 pytoniq-0.0.7/pytoniq/liteclient/__init__.py
--rw-r--r--   0 maxankurb   (501) staff       (20)    39226 2023-07-30 15:02:06.000000 pytoniq-0.0.7/pytoniq/liteclient/client.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     5409 2023-07-30 14:31:13.000000 pytoniq-0.0.7/pytoniq/liteclient/sync.py
--rw-r--r--   0 maxankurb   (501) staff       (20)      625 2023-07-24 15:34:43.000000 pytoniq-0.0.7/pytoniq/liteclient/utils.py
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-30 15:05:36.626302 pytoniq-0.0.7/pytoniq/proof/
--rw-r--r--   0 maxankurb   (501) staff       (20)      186 2023-07-23 15:42:41.000000 pytoniq-0.0.7/pytoniq/proof/__init__.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     6193 2023-07-21 11:26:13.000000 pytoniq-0.0.7/pytoniq/proof/check_proof.py
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-30 15:05:36.629267 pytoniq-0.0.7/pytoniq/tl/
--rw-r--r--   0 maxankurb   (501) staff       (20)      118 2023-07-23 15:42:41.000000 pytoniq-0.0.7/pytoniq/tl/__init__.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     2990 2023-07-23 08:44:15.000000 pytoniq-0.0.7/pytoniq/tl/block.py
--rw-r--r--   0 maxankurb   (501) staff       (20)    14400 2023-07-30 15:03:21.000000 pytoniq-0.0.7/pytoniq/tl/generator.py
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-30 15:05:36.631790 pytoniq-0.0.7/pytoniq/tl/schemas/
--rw-r--r--   0 maxankurb   (501) staff       (20)     7204 2023-07-30 12:46:41.000000 pytoniq-0.0.7/pytoniq/tl/schemas/lite_api.tl
--rw-r--r--   0 maxankurb   (501) staff       (20)    45439 2023-06-17 21:53:59.000000 pytoniq-0.0.7/pytoniq/tl/schemas/ton_api.tl
--rw-r--r--   0 maxankurb   (501) staff       (20)    18697 2023-05-29 07:39:43.000000 pytoniq-0.0.7/pytoniq/tl/schemas/tonlib_api.tl
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-30 15:05:36.643910 pytoniq-0.0.7/pytoniq/tlb/
--rw-r--r--   0 maxankurb   (501) staff       (20)      924 2023-07-24 08:29:16.000000 pytoniq-0.0.7/pytoniq/tlb/__init__.py
--rw-r--r--   0 maxankurb   (501) staff       (20)    11853 2023-07-23 13:10:19.000000 pytoniq-0.0.7/pytoniq/tlb/account.py
--rw-r--r--   0 maxankurb   (501) staff       (20)    34959 2023-07-24 08:25:46.000000 pytoniq-0.0.7/pytoniq/tlb/block.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     5137 2023-06-30 16:07:22.000000 pytoniq-0.0.7/pytoniq/tlb/code_generator.py
--rw-r--r--   0 maxankurb   (501) staff       (20)    56951 2023-07-13 14:13:51.000000 pytoniq-0.0.7/pytoniq/tlb/config.py
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-30 15:05:36.645893 pytoniq-0.0.7/pytoniq/tlb/custom/
--rw-r--r--   0 maxankurb   (501) staff       (20)       91 2023-07-27 17:13:15.000000 pytoniq-0.0.7/pytoniq/tlb/custom/__init__.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     1436 2023-07-27 17:07:58.000000 pytoniq-0.0.7/pytoniq/tlb/custom/nft.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     4584 2023-07-23 14:27:13.000000 pytoniq-0.0.7/pytoniq/tlb/custom/wallet.py
--rw-r--r--   0 maxankurb   (501) staff       (20)    12530 2023-07-27 17:28:35.000000 pytoniq-0.0.7/pytoniq/tlb/generator.py
--rw-r--r--   0 maxankurb   (501) staff       (20)      382 2023-07-23 14:10:34.000000 pytoniq-0.0.7/pytoniq/tlb/tlb.py
--rw-r--r--   0 maxankurb   (501) staff       (20)    44289 2023-07-28 18:49:05.000000 pytoniq-0.0.7/pytoniq/tlb/transaction.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     2292 2023-07-12 11:03:41.000000 pytoniq-0.0.7/pytoniq/tlb/utils.py
--rw-r--r--   0 maxankurb   (501) staff       (20)    15591 2023-07-21 07:26:25.000000 pytoniq-0.0.7/pytoniq/tlb/vm_stack.py
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-30 15:05:36.600487 pytoniq-0.0.7/pytoniq.egg-info/
--rw-r--r--   0 maxankurb   (501) staff       (20)    13684 2023-07-30 15:05:36.000000 pytoniq-0.0.7/pytoniq.egg-info/PKG-INFO
--rw-r--r--   0 maxankurb   (501) staff       (20)     1552 2023-07-30 15:05:36.000000 pytoniq-0.0.7/pytoniq.egg-info/SOURCES.txt
--rw-r--r--   0 maxankurb   (501) staff       (20)        1 2023-07-30 15:05:36.000000 pytoniq-0.0.7/pytoniq.egg-info/dependency_links.txt
--rw-r--r--   0 maxankurb   (501) staff       (20)      101 2023-07-30 15:05:36.000000 pytoniq-0.0.7/pytoniq.egg-info/requires.txt
--rw-r--r--   0 maxankurb   (501) staff       (20)        8 2023-07-30 15:05:36.000000 pytoniq-0.0.7/pytoniq.egg-info/top_level.txt
--rw-r--r--   0 maxankurb   (501) staff       (20)       38 2023-07-30 15:05:36.647899 pytoniq-0.0.7/setup.cfg
--rw-r--r--   0 maxankurb   (501) staff       (20)      948 2023-07-30 15:05:20.000000 pytoniq-0.0.7/setup.py
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-08-01 12:37:09.688151 pytoniq-0.0.8/
+-rw-r--r--   0 maxankurb   (501) staff       (20)       29 2023-07-27 17:44:46.000000 pytoniq-0.0.8/MANIFEST.in
+-rw-r--r--   0 maxankurb   (501) staff       (20)    13983 2023-08-01 12:37:09.687630 pytoniq-0.0.8/PKG-INFO
+-rw-r--r--   0 maxankurb   (501) staff       (20)    13577 2023-07-30 15:08:36.000000 pytoniq-0.0.8/README.md
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-08-01 12:37:09.646350 pytoniq-0.0.8/pytoniq/
+-rw-r--r--   0 maxankurb   (501) staff       (20)      149 2023-07-23 15:42:41.000000 pytoniq-0.0.8/pytoniq/__init__.py
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-08-01 12:37:09.655274 pytoniq-0.0.8/pytoniq/boc/
+-rw-r--r--   0 maxankurb   (501) staff       (20)      222 2023-07-23 15:42:41.000000 pytoniq-0.0.8/pytoniq/boc/__init__.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     3700 2023-07-27 16:08:51.000000 pytoniq-0.0.8/pytoniq/boc/address.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     4204 2023-07-21 09:13:36.000000 pytoniq-0.0.8/pytoniq/boc/builder.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)    11007 2023-07-23 16:49:28.000000 pytoniq-0.0.8/pytoniq/boc/cell.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     9079 2023-07-28 16:29:36.000000 pytoniq-0.0.8/pytoniq/boc/deserialize.py
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-08-01 12:37:09.657991 pytoniq-0.0.8/pytoniq/boc/dict/
+-rw-r--r--   0 maxankurb   (501) staff       (20)       41 2023-07-23 15:42:41.000000 pytoniq-0.0.8/pytoniq/boc/dict/__init__.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     5060 2023-07-23 15:16:15.000000 pytoniq-0.0.8/pytoniq/boc/dict/dict.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     3919 2023-07-23 17:27:59.000000 pytoniq-0.0.8/pytoniq/boc/dict/parse.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     4989 2023-06-19 11:55:15.000000 pytoniq-0.0.8/pytoniq/boc/dict/utils.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     1026 2023-07-23 13:47:12.000000 pytoniq-0.0.8/pytoniq/boc/exotic.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     7521 2023-07-11 20:09:21.000000 pytoniq-0.0.8/pytoniq/boc/slice.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     1866 2023-07-05 13:08:40.000000 pytoniq-0.0.8/pytoniq/boc/tvm_bitarray.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)      298 2023-07-13 12:16:46.000000 pytoniq-0.0.8/pytoniq/boc/utils.py
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-08-01 12:37:09.660008 pytoniq-0.0.8/pytoniq/contract/
+-rw-r--r--   0 maxankurb   (501) staff       (20)       69 2023-07-23 15:42:41.000000 pytoniq-0.0.8/pytoniq/contract/__init__.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     6750 2023-07-28 19:24:43.000000 pytoniq-0.0.8/pytoniq/contract/contract.py
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-08-01 12:37:09.661358 pytoniq-0.0.8/pytoniq/contract/nft/
+-rw-r--r--   0 maxankurb   (501) staff       (20)       25 2023-07-27 17:13:15.000000 pytoniq-0.0.8/pytoniq/contract/nft/__init__.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     3643 2023-07-27 17:10:31.000000 pytoniq-0.0.8/pytoniq/contract/nft/nft.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)      102 2023-07-22 17:41:04.000000 pytoniq-0.0.8/pytoniq/contract/utils.py
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-08-01 12:37:09.663351 pytoniq-0.0.8/pytoniq/contract/wallets/
+-rw-r--r--   0 maxankurb   (501) staff       (20)      151 2023-07-23 15:42:41.000000 pytoniq-0.0.8/pytoniq/contract/wallets/__init__.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     7615 2023-07-23 07:51:49.000000 pytoniq-0.0.8/pytoniq/contract/wallets/highload.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)    18779 2023-07-23 07:41:58.000000 pytoniq-0.0.8/pytoniq/contract/wallets/wallet.py
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-08-01 12:37:09.667157 pytoniq-0.0.8/pytoniq/crypto/
+-rw-r--r--   0 maxankurb   (501) staff       (20)        0 2023-06-17 12:05:39.000000 pytoniq-0.0.8/pytoniq/crypto/__init__.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     2087 2023-05-27 14:21:05.000000 pytoniq-0.0.8/pytoniq/crypto/ciphers.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     6558 2023-06-17 13:10:44.000000 pytoniq-0.0.8/pytoniq/crypto/crc.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)    22014 2023-07-22 13:35:04.000000 pytoniq-0.0.8/pytoniq/crypto/keys.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)      820 2023-07-27 14:32:52.000000 pytoniq-0.0.8/pytoniq/crypto/signature.py
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-08-01 12:37:09.670123 pytoniq-0.0.8/pytoniq/liteclient/
+-rw-r--r--   0 maxankurb   (501) staff       (20)       88 2023-07-23 15:42:41.000000 pytoniq-0.0.8/pytoniq/liteclient/__init__.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)    39251 2023-08-01 12:37:03.000000 pytoniq-0.0.8/pytoniq/liteclient/client.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     5409 2023-07-30 14:31:13.000000 pytoniq-0.0.8/pytoniq/liteclient/sync.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)      625 2023-07-24 15:34:43.000000 pytoniq-0.0.8/pytoniq/liteclient/utils.py
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-08-01 12:37:09.671431 pytoniq-0.0.8/pytoniq/proof/
+-rw-r--r--   0 maxankurb   (501) staff       (20)      186 2023-07-23 15:42:41.000000 pytoniq-0.0.8/pytoniq/proof/__init__.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     6193 2023-07-21 11:26:13.000000 pytoniq-0.0.8/pytoniq/proof/check_proof.py
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-08-01 12:37:09.673465 pytoniq-0.0.8/pytoniq/tl/
+-rw-r--r--   0 maxankurb   (501) staff       (20)      118 2023-07-23 15:42:41.000000 pytoniq-0.0.8/pytoniq/tl/__init__.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     2990 2023-07-23 08:44:15.000000 pytoniq-0.0.8/pytoniq/tl/block.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)    14400 2023-07-30 15:03:21.000000 pytoniq-0.0.8/pytoniq/tl/generator.py
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-08-01 12:37:09.675851 pytoniq-0.0.8/pytoniq/tl/schemas/
+-rw-r--r--   0 maxankurb   (501) staff       (20)     7204 2023-07-30 12:46:41.000000 pytoniq-0.0.8/pytoniq/tl/schemas/lite_api.tl
+-rw-r--r--   0 maxankurb   (501) staff       (20)    45439 2023-06-17 21:53:59.000000 pytoniq-0.0.8/pytoniq/tl/schemas/ton_api.tl
+-rw-r--r--   0 maxankurb   (501) staff       (20)    18697 2023-05-29 07:39:43.000000 pytoniq-0.0.8/pytoniq/tl/schemas/tonlib_api.tl
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-08-01 12:37:09.684347 pytoniq-0.0.8/pytoniq/tlb/
+-rw-r--r--   0 maxankurb   (501) staff       (20)      924 2023-07-24 08:29:16.000000 pytoniq-0.0.8/pytoniq/tlb/__init__.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)    11853 2023-07-23 13:10:19.000000 pytoniq-0.0.8/pytoniq/tlb/account.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)    34959 2023-07-24 08:25:46.000000 pytoniq-0.0.8/pytoniq/tlb/block.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     5137 2023-06-30 16:07:22.000000 pytoniq-0.0.8/pytoniq/tlb/code_generator.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)    56951 2023-07-13 14:13:51.000000 pytoniq-0.0.8/pytoniq/tlb/config.py
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-08-01 12:37:09.686843 pytoniq-0.0.8/pytoniq/tlb/custom/
+-rw-r--r--   0 maxankurb   (501) staff       (20)       91 2023-07-27 17:13:15.000000 pytoniq-0.0.8/pytoniq/tlb/custom/__init__.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     1436 2023-07-27 17:07:58.000000 pytoniq-0.0.8/pytoniq/tlb/custom/nft.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     4584 2023-07-23 14:27:13.000000 pytoniq-0.0.8/pytoniq/tlb/custom/wallet.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)    12530 2023-07-27 17:28:35.000000 pytoniq-0.0.8/pytoniq/tlb/generator.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)      382 2023-07-23 14:10:34.000000 pytoniq-0.0.8/pytoniq/tlb/tlb.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)    44289 2023-07-28 18:49:05.000000 pytoniq-0.0.8/pytoniq/tlb/transaction.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     2292 2023-07-12 11:03:41.000000 pytoniq-0.0.8/pytoniq/tlb/utils.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)    15591 2023-08-01 07:42:26.000000 pytoniq-0.0.8/pytoniq/tlb/vm_stack.py
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-08-01 12:37:09.648697 pytoniq-0.0.8/pytoniq.egg-info/
+-rw-r--r--   0 maxankurb   (501) staff       (20)    13983 2023-08-01 12:37:09.000000 pytoniq-0.0.8/pytoniq.egg-info/PKG-INFO
+-rw-r--r--   0 maxankurb   (501) staff       (20)     1552 2023-08-01 12:37:09.000000 pytoniq-0.0.8/pytoniq.egg-info/SOURCES.txt
+-rw-r--r--   0 maxankurb   (501) staff       (20)        1 2023-08-01 12:37:09.000000 pytoniq-0.0.8/pytoniq.egg-info/dependency_links.txt
+-rw-r--r--   0 maxankurb   (501) staff       (20)      101 2023-08-01 12:37:09.000000 pytoniq-0.0.8/pytoniq.egg-info/requires.txt
+-rw-r--r--   0 maxankurb   (501) staff       (20)        8 2023-08-01 12:37:09.000000 pytoniq-0.0.8/pytoniq.egg-info/top_level.txt
+-rw-r--r--   0 maxankurb   (501) staff       (20)       38 2023-08-01 12:37:09.688316 pytoniq-0.0.8/setup.cfg
+-rw-r--r--   0 maxankurb   (501) staff       (20)      948 2023-08-01 12:36:17.000000 pytoniq-0.0.8/setup.py
```

### Comparing `pytoniq-0.0.7/PKG-INFO` & `pytoniq-0.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,11 @@
-Metadata-Version: 2.1
-Name: pytoniq
-Version: 0.0.7
-Summary: TON Blockchain SDK
-Home-page: https://github.com/yungwine/pytoniq
-Author: Maksim Kurbatov
-Author-email: cyrbatoff@gmail.com
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-
 # pytoniq
 
+[![PyPI version](https://badge.fury.io/py/pytoniq.svg)](https://badge.fury.io/py/pytoniq) ![](https://pepy.tech/badge/pytoniq) [![Downloads](https://static.pepy.tech/badge/pytoniq/month)](https://pepy.tech/project/pytoniq) [![](https://img.shields.io/badge/%F0%9F%92%8E-TON-grey)](https://ton.org)
+
 Pytoniq is a Python SDK for the TON Blockchain. 
 Currently, it has native ADNL over TCP connection to Liteservers,
 boc types implementation, wrappers for almost all TLB schemes from block.tlb,
 automaic TL schemes serialization/deserialization,
 some popular contracts wrappers.
 
 * Work in progress
```

### Comparing `pytoniq-0.0.7/README.md` & `pytoniq-0.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,24 @@
+Metadata-Version: 2.1
+Name: pytoniq
+Version: 0.0.8
+Summary: TON Blockchain SDK
+Home-page: https://github.com/yungwine/pytoniq
+Author: Maksim Kurbatov
+Author-email: cyrbatoff@gmail.com
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+
 # pytoniq
 
+[![PyPI version](https://badge.fury.io/py/pytoniq.svg)](https://badge.fury.io/py/pytoniq) ![](https://pepy.tech/badge/pytoniq) [![Downloads](https://static.pepy.tech/badge/pytoniq/month)](https://pepy.tech/project/pytoniq) [![](https://img.shields.io/badge/%F0%9F%92%8E-TON-grey)](https://ton.org)
+
 Pytoniq is a Python SDK for the TON Blockchain. 
 Currently, it has native ADNL over TCP connection to Liteservers,
 boc types implementation, wrappers for almost all TLB schemes from block.tlb,
 automaic TL schemes serialization/deserialization,
 some popular contracts wrappers.
 
 * Work in progress
```

### Comparing `pytoniq-0.0.7/pytoniq/boc/address.py` & `pytoniq-0.0.8/pytoniq/boc/address.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.7/pytoniq/boc/builder.py` & `pytoniq-0.0.8/pytoniq/boc/builder.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.7/pytoniq/boc/cell.py` & `pytoniq-0.0.8/pytoniq/boc/cell.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.7/pytoniq/boc/deserialize.py` & `pytoniq-0.0.8/pytoniq/boc/deserialize.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.7/pytoniq/boc/dict/dict.py` & `pytoniq-0.0.8/pytoniq/boc/dict/dict.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.7/pytoniq/boc/dict/parse.py` & `pytoniq-0.0.8/pytoniq/boc/dict/parse.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.7/pytoniq/boc/dict/utils.py` & `pytoniq-0.0.8/pytoniq/boc/dict/utils.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.7/pytoniq/boc/exotic.py` & `pytoniq-0.0.8/pytoniq/boc/exotic.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.7/pytoniq/boc/slice.py` & `pytoniq-0.0.8/pytoniq/boc/slice.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.7/pytoniq/boc/tvm_bitarray.py` & `pytoniq-0.0.8/pytoniq/boc/tvm_bitarray.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.7/pytoniq/contract/contract.py` & `pytoniq-0.0.8/pytoniq/contract/contract.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.7/pytoniq/contract/nft/nft.py` & `pytoniq-0.0.8/pytoniq/contract/nft/nft.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.7/pytoniq/contract/wallets/highload.py` & `pytoniq-0.0.8/pytoniq/contract/wallets/highload.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.7/pytoniq/contract/wallets/wallet.py` & `pytoniq-0.0.8/pytoniq/contract/wallets/wallet.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.7/pytoniq/crypto/ciphers.py` & `pytoniq-0.0.8/pytoniq/crypto/ciphers.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.7/pytoniq/crypto/crc.py` & `pytoniq-0.0.8/pytoniq/crypto/crc.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.7/pytoniq/crypto/keys.py` & `pytoniq-0.0.8/pytoniq/crypto/keys.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.7/pytoniq/crypto/signature.py` & `pytoniq-0.0.8/pytoniq/crypto/signature.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.7/pytoniq/liteclient/client.py` & `pytoniq-0.0.8/pytoniq/liteclient/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
         """########### connection ###########"""
         self.reader: asyncio.StreamReader = None
         self.writer: asyncio.StreamWriter = None
         self.listener: asyncio.Task = None
         self.pinger: asyncio.Task = None
         self.updater: asyncio.Task = None
-        self.loop = asyncio.get_event_loop()
+        self.loop: asyncio.AbstractEventLoop = None
         self.delta = 0.02  # listen delay
 
         """########### TL ###########"""
         if tl_schemas_path is None:
             tl_schemas_path = os.path.join(os.path.dirname(__file__), os.pardir, 'tl/schemas')
         self.schemas = TlGenerator(tl_schemas_path).generate()
         # for better performance:
@@ -142,26 +142,29 @@
 
             request = self.tasks.pop(qid)
 
             result = result.get('answer', {})
             request.set_result(result)
 
     async def connect(self) -> None:
+        self.loop = asyncio.get_running_loop()
         handshake = self.handshake()
         self.reader, self.writer = await asyncio.open_connection(self.server.host, self.server.port)
         future = await self.send(handshake, None)
-        # async with asyncio.TaskGroup() as tg:
-        #     self.listener = tg.create_task(self.listen(), name='listener')
         self.listener = asyncio.create_task(self.listen(), name='listener')
         await self.update_last_blocks()
         self.pinger = asyncio.create_task(self.ping(), name='pinger')
         self.updater = asyncio.create_task(self.block_updater(), name='updater')
         await future
         self.inited = True
 
+    async def reconnect(self) -> None:
+        await self.close()
+        await self.connect()
+
     async def close(self) -> None:
         for i in asyncio.all_tasks(self.loop):
             if i.get_name() in ('pinger', 'listener', 'updater'):
                 i.cancel()
         self.logger.info(msg='client has been closed')
 
     def handshake(self) -> bytes:
```

### Comparing `pytoniq-0.0.7/pytoniq/liteclient/sync.py` & `pytoniq-0.0.8/pytoniq/liteclient/sync.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.7/pytoniq/liteclient/utils.py` & `pytoniq-0.0.8/pytoniq/liteclient/utils.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.7/pytoniq/proof/check_proof.py` & `pytoniq-0.0.8/pytoniq/proof/check_proof.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.7/pytoniq/tl/block.py` & `pytoniq-0.0.8/pytoniq/tl/block.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.7/pytoniq/tl/generator.py` & `pytoniq-0.0.8/pytoniq/tl/generator.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.7/pytoniq/tl/schemas/lite_api.tl` & `pytoniq-0.0.8/pytoniq/tl/schemas/lite_api.tl`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.7/pytoniq/tl/schemas/ton_api.tl` & `pytoniq-0.0.8/pytoniq/tl/schemas/ton_api.tl`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.7/pytoniq/tl/schemas/tonlib_api.tl` & `pytoniq-0.0.8/pytoniq/tl/schemas/tonlib_api.tl`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.7/pytoniq/tlb/__init__.py` & `pytoniq-0.0.8/pytoniq/tlb/__init__.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.7/pytoniq/tlb/account.py` & `pytoniq-0.0.8/pytoniq/tlb/account.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.7/pytoniq/tlb/block.py` & `pytoniq-0.0.8/pytoniq/tlb/block.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.7/pytoniq/tlb/code_generator.py` & `pytoniq-0.0.8/pytoniq/tlb/code_generator.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.7/pytoniq/tlb/config.py` & `pytoniq-0.0.8/pytoniq/tlb/config.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.7/pytoniq/tlb/custom/nft.py` & `pytoniq-0.0.8/pytoniq/tlb/custom/nft.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.7/pytoniq/tlb/custom/wallet.py` & `pytoniq-0.0.8/pytoniq/tlb/custom/wallet.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.7/pytoniq/tlb/generator.py` & `pytoniq-0.0.8/pytoniq/tlb/generator.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.7/pytoniq/tlb/transaction.py` & `pytoniq-0.0.8/pytoniq/tlb/transaction.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.7/pytoniq/tlb/utils.py` & `pytoniq-0.0.8/pytoniq/tlb/utils.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.7/pytoniq/tlb/vm_stack.py` & `pytoniq-0.0.8/pytoniq/tlb/vm_stack.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.7/pytoniq.egg-info/PKG-INFO` & `pytoniq-0.0.8/pytoniq.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: pytoniq
-Version: 0.0.7
+Version: 0.0.8
 Summary: TON Blockchain SDK
 Home-page: https://github.com/yungwine/pytoniq
 Author: Maksim Kurbatov
 Author-email: cyrbatoff@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # pytoniq
 
+[![PyPI version](https://badge.fury.io/py/pytoniq.svg)](https://badge.fury.io/py/pytoniq) ![](https://pepy.tech/badge/pytoniq) [![Downloads](https://static.pepy.tech/badge/pytoniq/month)](https://pepy.tech/project/pytoniq) [![](https://img.shields.io/badge/%F0%9F%92%8E-TON-grey)](https://ton.org)
+
 Pytoniq is a Python SDK for the TON Blockchain. 
 Currently, it has native ADNL over TCP connection to Liteservers,
 boc types implementation, wrappers for almost all TLB schemes from block.tlb,
 automaic TL schemes serialization/deserialization,
 some popular contracts wrappers.
 
 * Work in progress
```

### Comparing `pytoniq-0.0.7/pytoniq.egg-info/SOURCES.txt` & `pytoniq-0.0.8/pytoniq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytoniq-0.0.7/setup.py` & `pytoniq-0.0.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pytoniq",
-    version="0.0.7",
+    version="0.0.8",
     author="Maksim Kurbatov",
     author_email="cyrbatoff@gmail.com",
     description="TON Blockchain SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages('.', exclude=['tests', 'examples', 'pytoniq/adnl']),
     include_package_data=True,
```

