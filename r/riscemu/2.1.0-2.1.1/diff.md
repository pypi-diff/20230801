# Comparing `tmp/riscemu-2.1.0.tar.gz` & `tmp/riscemu-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "riscemu-2.1.0.tar", last modified: Tue Jun  6 15:00:25 2023, max compression
+gzip compressed data, was "riscemu-2.1.1.tar", last modified: Tue Aug  1 10:30:39 2023, max compression
```

## Comparing `riscemu-2.1.0.tar` & `riscemu-2.1.1.tar`

### file list

```diff
@@ -1,90 +1,91 @@
-drwxr-xr-x   0 anton     (1000) users      (100)        0 2023-06-06 15:00:25.655292 riscemu-2.1.0/
--rw-r--r--   0 anton     (1000) users      (100)     1074 2023-05-01 15:55:17.000000 riscemu-2.1.0/LICENSE
--rw-r--r--   0 anton     (1000) users      (100)     5579 2023-06-06 15:00:25.655292 riscemu-2.1.0/PKG-INFO
--rw-r--r--   0 anton     (1000) users      (100)     5049 2023-05-02 15:45:37.000000 riscemu-2.1.0/README.md
-drwxr-xr-x   0 anton     (1000) users      (100)        0 2023-06-06 15:00:25.653293 riscemu-2.1.0/libc/
--rw-r--r--   0 anton     (1000) users      (100)      345 2023-06-05 20:16:21.000000 riscemu-2.1.0/libc/crt0.s
--rw-r--r--   0 anton     (1000) users      (100)     4518 2023-06-05 20:16:21.000000 riscemu-2.1.0/libc/stdlib.s
--rw-r--r--   0 anton     (1000) users      (100)     4749 2023-06-05 20:16:21.000000 riscemu-2.1.0/libc/string.s
-drwxr-xr-x   0 anton     (1000) users      (100)        0 2023-06-06 15:00:25.649293 riscemu-2.1.0/riscemu/
--rw-r--r--   0 anton     (1000) users      (100)     4403 2023-06-05 20:16:21.000000 riscemu-2.1.0/riscemu/CPU.py
-drwxr-xr-x   0 anton     (1000) users      (100)        0 2023-06-06 15:00:25.649293 riscemu-2.1.0/riscemu/IO/
--rw-r--r--   0 anton     (1000) users      (100)      830 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/IO/IOModule.py
--rw-r--r--   0 anton     (1000) users      (100)     1567 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/IO/TextIO.py
--rw-r--r--   0 anton     (1000) users      (100)        0 2021-10-26 20:05:33.000000 riscemu-2.1.0/riscemu/IO/__init__.py
--rw-r--r--   0 anton     (1000) users      (100)    11795 2023-06-06 14:08:29.000000 riscemu-2.1.0/riscemu/MMU.py
--rw-r--r--   0 anton     (1000) users      (100)      942 2023-06-06 14:20:37.000000 riscemu-2.1.0/riscemu/__init__.py
--rw-r--r--   0 anton     (1000) users      (100)      493 2023-06-05 20:16:21.000000 riscemu-2.1.0/riscemu/__main__.py
--rw-r--r--   0 anton     (1000) users      (100)     8330 2023-06-05 20:16:21.000000 riscemu-2.1.0/riscemu/assembler.py
--rw-r--r--   0 anton     (1000) users      (100)      559 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/colors.py
--rw-r--r--   0 anton     (1000) users      (100)      621 2023-06-05 20:16:21.000000 riscemu-2.1.0/riscemu/config.py
--rw-r--r--   0 anton     (1000) users      (100)     2259 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/debug.py
-drwxr-xr-x   0 anton     (1000) users      (100)        0 2023-06-06 15:00:25.650293 riscemu-2.1.0/riscemu/decoder/
--rw-r--r--   0 anton     (1000) users      (100)       74 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/decoder/__init__.py
--rw-r--r--   0 anton     (1000) users      (100)      589 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/decoder/__main__.py
--rw-r--r--   0 anton     (1000) users      (100)     2648 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/decoder/decoder.py
--rw-r--r--   0 anton     (1000) users      (100)     2283 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/decoder/formats.py
--rw-r--r--   0 anton     (1000) users      (100)     1349 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/decoder/formatter.py
--rw-r--r--   0 anton     (1000) users      (100)     1842 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/decoder/instruction_table.py
--rw-r--r--   0 anton     (1000) users      (100)      341 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/decoder/regs.py
--rw-r--r--   0 anton     (1000) users      (100)     3340 2023-06-05 21:45:49.000000 riscemu-2.1.0/riscemu/helpers.py
-drwxr-xr-x   0 anton     (1000) users      (100)        0 2023-06-06 15:00:25.651293 riscemu-2.1.0/riscemu/instructions/
--rw-r--r--   0 anton     (1000) users      (100)     2908 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/instructions/RV32A.py
--rw-r--r--   0 anton     (1000) users      (100)    20423 2023-06-06 14:08:29.000000 riscemu-2.1.0/riscemu/instructions/RV32F.py
--rw-r--r--   0 anton     (1000) users      (100)     9416 2023-06-05 20:16:21.000000 riscemu-2.1.0/riscemu/instructions/RV32I.py
--rw-r--r--   0 anton     (1000) users      (100)     1325 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/instructions/RV32M.py
--rw-r--r--   0 anton     (1000) users      (100)      888 2023-06-06 14:08:20.000000 riscemu-2.1.0/riscemu/instructions/RV_Debug.py
--rw-r--r--   0 anton     (1000) users      (100)      412 2023-06-06 14:08:29.000000 riscemu-2.1.0/riscemu/instructions/__init__.py
--rw-r--r--   0 anton     (1000) users      (100)     4901 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/instructions/instruction_set.py
--rw-r--r--   0 anton     (1000) users      (100)     1027 2023-06-05 20:16:21.000000 riscemu-2.1.0/riscemu/interactive.py
--rw-r--r--   0 anton     (1000) users      (100)     5042 2023-06-06 14:08:29.000000 riscemu-2.1.0/riscemu/parser.py
-drwxr-xr-x   0 anton     (1000) users      (100)        0 2023-06-06 15:00:25.652293 riscemu-2.1.0/riscemu/priv/
--rw-r--r--   0 anton     (1000) users      (100)     4604 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/priv/CSR.py
--rw-r--r--   0 anton     (1000) users      (100)     1981 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/priv/CSRConsts.py
--rw-r--r--   0 anton     (1000) users      (100)     4414 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/priv/ElfLoader.py
--rw-r--r--   0 anton     (1000) users      (100)     3159 2023-05-01 15:55:17.000000 riscemu-2.1.0/riscemu/priv/Exceptions.py
--rw-r--r--   0 anton     (1000) users      (100)     2843 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/priv/ImageLoader.py
--rw-r--r--   0 anton     (1000) users      (100)     8747 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/priv/PrivCPU.py
--rw-r--r--   0 anton     (1000) users      (100)     1737 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/priv/PrivMMU.py
--rw-r--r--   0 anton     (1000) users      (100)     5946 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/priv/PrivRV32I.py
--rw-r--r--   0 anton     (1000) users      (100)      455 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/priv/__init__.py
--rw-r--r--   0 anton     (1000) users      (100)     1706 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/priv/__main__.py
--rw-r--r--   0 anton     (1000) users      (100)       96 2021-10-26 20:05:33.000000 riscemu-2.1.0/riscemu/priv/privmodes.py
--rw-r--r--   0 anton     (1000) users      (100)     5271 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/priv/types.py
--rw-r--r--   0 anton     (1000) users      (100)        0 2023-06-05 20:16:21.000000 riscemu-2.1.0/riscemu/py.typed
--rw-r--r--   0 anton     (1000) users      (100)     6444 2023-06-06 14:08:29.000000 riscemu-2.1.0/riscemu/registers.py
--rw-r--r--   0 anton     (1000) users      (100)     9491 2023-06-05 20:16:21.000000 riscemu-2.1.0/riscemu/riscemu_main.py
--rw-r--r--   0 anton     (1000) users      (100)     8444 2023-06-05 20:16:21.000000 riscemu-2.1.0/riscemu/syscall.py
--rw-r--r--   0 anton     (1000) users      (100)     3366 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/tokenizer.py
-drwxr-xr-x   0 anton     (1000) users      (100)        0 2023-06-06 15:00:25.654292 riscemu-2.1.0/riscemu/tools/
--rwxr-xr-x   0 anton     (1000) users      (100)       44 2023-06-05 20:16:21.000000 riscemu-2.1.0/riscemu/tools/riscemu
-drwxr-xr-x   0 anton     (1000) users      (100)        0 2023-06-06 15:00:25.653293 riscemu-2.1.0/riscemu/types/
--rw-r--r--   0 anton     (1000) users      (100)     1193 2023-06-06 14:08:29.000000 riscemu-2.1.0/riscemu/types/__init__.py
--rw-r--r--   0 anton     (1000) users      (100)     1718 2023-06-05 20:16:21.000000 riscemu-2.1.0/riscemu/types/binary_data_memory_section.py
--rw-r--r--   0 anton     (1000) users      (100)     3334 2023-06-05 20:16:21.000000 riscemu-2.1.0/riscemu/types/cpu.py
--rw-r--r--   0 anton     (1000) users      (100)     4807 2023-06-05 20:16:21.000000 riscemu-2.1.0/riscemu/types/exceptions.py
--rw-r--r--   0 anton     (1000) users      (100)      262 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/types/flags.py
--rw-r--r--   0 anton     (1000) users      (100)     5836 2023-06-06 14:08:29.000000 riscemu-2.1.0/riscemu/types/float32.py
--rw-r--r--   0 anton     (1000) users      (100)      642 2022-03-31 20:48:16.000000 riscemu-2.1.0/riscemu/types/instruction.py
--rw-r--r--   0 anton     (1000) users      (100)     2195 2023-05-01 15:55:17.000000 riscemu-2.1.0/riscemu/types/instruction_context.py
--rw-r--r--   0 anton     (1000) users      (100)     1496 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/types/instruction_memory_section.py
--rw-r--r--   0 anton     (1000) users      (100)     8612 2023-06-06 14:08:29.000000 riscemu-2.1.0/riscemu/types/int32.py
--rw-r--r--   0 anton     (1000) users      (100)     5271 2023-06-05 20:16:21.000000 riscemu-2.1.0/riscemu/types/memory_section.py
--rw-r--r--   0 anton     (1000) users      (100)     4143 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/types/program.py
--rw-r--r--   0 anton     (1000) users      (100)     1865 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/types/program_loader.py
--rw-r--r--   0 anton     (1000) users      (100)      927 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/types/simple_instruction.py
-drwxr-xr-x   0 anton     (1000) users      (100)        0 2023-06-06 15:00:25.654292 riscemu-2.1.0/riscemu.egg-info/
--rw-r--r--   0 anton     (1000) users      (100)     5579 2023-06-06 15:00:25.000000 riscemu-2.1.0/riscemu.egg-info/PKG-INFO
--rw-r--r--   0 anton     (1000) users      (100)     2005 2023-06-06 15:00:25.000000 riscemu-2.1.0/riscemu.egg-info/SOURCES.txt
--rw-r--r--   0 anton     (1000) users      (100)        1 2023-06-06 15:00:25.000000 riscemu-2.1.0/riscemu.egg-info/dependency_links.txt
--rw-r--r--   0 anton     (1000) users      (100)       17 2023-06-06 15:00:25.000000 riscemu-2.1.0/riscemu.egg-info/requires.txt
--rw-r--r--   0 anton     (1000) users      (100)        8 2023-06-06 15:00:25.000000 riscemu-2.1.0/riscemu.egg-info/top_level.txt
--rw-r--r--   0 anton     (1000) users      (100)       38 2023-06-06 15:00:25.655292 riscemu-2.1.0/setup.cfg
--rw-r--r--   0 anton     (1000) users      (100)     1195 2023-06-06 14:52:50.000000 riscemu-2.1.0/setup.py
-drwxr-xr-x   0 anton     (1000) users      (100)        0 2023-06-06 15:00:25.654292 riscemu-2.1.0/test/
--rw-r--r--   0 anton     (1000) users      (100)      466 2023-06-06 14:08:29.000000 riscemu-2.1.0/test/test_float32.py
--rw-r--r--   0 anton     (1000) users      (100)      395 2023-06-05 21:52:17.000000 riscemu-2.1.0/test/test_helpers.py
--rw-r--r--   0 anton     (1000) users      (100)      468 2023-05-01 15:29:41.000000 riscemu-2.1.0/test/test_integers.py
--rw-r--r--   0 anton     (1000) users      (100)     2326 2023-05-01 15:37:55.000000 riscemu-2.1.0/test/test_isa.py
--rw-r--r--   0 anton     (1000) users      (100)      578 2023-06-06 14:08:29.000000 riscemu-2.1.0/test/test_regs.py
--rw-r--r--   0 anton     (1000) users      (100)     4548 2023-05-01 15:37:55.000000 riscemu-2.1.0/test/test_tokenizer.py
+drwxr-xr-x   0 anton     (1000) users      (100)        0 2023-08-01 10:30:39.879780 riscemu-2.1.1/
+-rw-r--r--   0 anton     (1000) users      (100)     1074 2023-05-29 10:25:04.000000 riscemu-2.1.1/LICENSE
+-rw-r--r--   0 anton     (1000) users      (100)     5579 2023-08-01 10:30:39.879780 riscemu-2.1.1/PKG-INFO
+-rw-r--r--   0 anton     (1000) users      (100)     5049 2023-05-29 10:25:04.000000 riscemu-2.1.1/README.md
+drwxr-xr-x   0 anton     (1000) users      (100)        0 2023-08-01 10:30:39.877780 riscemu-2.1.1/libc/
+-rw-r--r--   0 anton     (1000) users      (100)      345 2023-05-29 10:29:06.000000 riscemu-2.1.1/libc/crt0.s
+-rw-r--r--   0 anton     (1000) users      (100)      377 2023-06-20 16:34:10.000000 riscemu-2.1.1/libc/stdio.s
+-rw-r--r--   0 anton     (1000) users      (100)     4518 2023-05-29 15:04:09.000000 riscemu-2.1.1/libc/stdlib.s
+-rw-r--r--   0 anton     (1000) users      (100)     4749 2023-05-29 13:10:40.000000 riscemu-2.1.1/libc/string.s
+drwxr-xr-x   0 anton     (1000) users      (100)        0 2023-08-01 10:30:39.869780 riscemu-2.1.1/riscemu/
+-rw-r--r--   0 anton     (1000) users      (100)     4403 2023-05-29 10:25:04.000000 riscemu-2.1.1/riscemu/CPU.py
+drwxr-xr-x   0 anton     (1000) users      (100)        0 2023-08-01 10:30:39.869780 riscemu-2.1.1/riscemu/IO/
+-rw-r--r--   0 anton     (1000) users      (100)      830 2023-05-29 10:25:04.000000 riscemu-2.1.1/riscemu/IO/IOModule.py
+-rw-r--r--   0 anton     (1000) users      (100)     1567 2023-05-29 10:25:04.000000 riscemu-2.1.1/riscemu/IO/TextIO.py
+-rw-r--r--   0 anton     (1000) users      (100)        0 2021-10-26 20:05:33.000000 riscemu-2.1.1/riscemu/IO/__init__.py
+-rw-r--r--   0 anton     (1000) users      (100)    11795 2023-08-01 10:18:56.000000 riscemu-2.1.1/riscemu/MMU.py
+-rw-r--r--   0 anton     (1000) users      (100)      942 2023-08-01 10:21:11.000000 riscemu-2.1.1/riscemu/__init__.py
+-rw-r--r--   0 anton     (1000) users      (100)      493 2023-05-30 08:10:55.000000 riscemu-2.1.1/riscemu/__main__.py
+-rw-r--r--   0 anton     (1000) users      (100)     8330 2023-05-29 13:14:37.000000 riscemu-2.1.1/riscemu/assembler.py
+-rw-r--r--   0 anton     (1000) users      (100)      559 2023-05-29 10:25:04.000000 riscemu-2.1.1/riscemu/colors.py
+-rw-r--r--   0 anton     (1000) users      (100)      621 2023-05-29 15:02:25.000000 riscemu-2.1.1/riscemu/config.py
+-rw-r--r--   0 anton     (1000) users      (100)     2259 2023-05-29 10:25:04.000000 riscemu-2.1.1/riscemu/debug.py
+drwxr-xr-x   0 anton     (1000) users      (100)        0 2023-08-01 10:30:39.870780 riscemu-2.1.1/riscemu/decoder/
+-rw-r--r--   0 anton     (1000) users      (100)       74 2023-05-29 10:25:04.000000 riscemu-2.1.1/riscemu/decoder/__init__.py
+-rw-r--r--   0 anton     (1000) users      (100)      589 2023-05-29 10:25:04.000000 riscemu-2.1.1/riscemu/decoder/__main__.py
+-rw-r--r--   0 anton     (1000) users      (100)     2648 2023-05-29 10:25:04.000000 riscemu-2.1.1/riscemu/decoder/decoder.py
+-rw-r--r--   0 anton     (1000) users      (100)     2283 2023-05-29 10:25:04.000000 riscemu-2.1.1/riscemu/decoder/formats.py
+-rw-r--r--   0 anton     (1000) users      (100)     1349 2023-05-29 10:25:04.000000 riscemu-2.1.1/riscemu/decoder/formatter.py
+-rw-r--r--   0 anton     (1000) users      (100)     1842 2023-05-29 10:25:04.000000 riscemu-2.1.1/riscemu/decoder/instruction_table.py
+-rw-r--r--   0 anton     (1000) users      (100)      341 2023-05-29 10:25:04.000000 riscemu-2.1.1/riscemu/decoder/regs.py
+-rw-r--r--   0 anton     (1000) users      (100)     3340 2023-05-29 10:25:04.000000 riscemu-2.1.1/riscemu/helpers.py
+drwxr-xr-x   0 anton     (1000) users      (100)        0 2023-08-01 10:30:39.871780 riscemu-2.1.1/riscemu/instructions/
+-rw-r--r--   0 anton     (1000) users      (100)     2908 2023-05-29 10:25:04.000000 riscemu-2.1.1/riscemu/instructions/RV32A.py
+-rw-r--r--   0 anton     (1000) users      (100)    20257 2023-08-01 10:18:56.000000 riscemu-2.1.1/riscemu/instructions/RV32F.py
+-rw-r--r--   0 anton     (1000) users      (100)     9416 2023-05-29 10:25:04.000000 riscemu-2.1.1/riscemu/instructions/RV32I.py
+-rw-r--r--   0 anton     (1000) users      (100)     1325 2023-05-29 10:25:04.000000 riscemu-2.1.1/riscemu/instructions/RV32M.py
+-rw-r--r--   0 anton     (1000) users      (100)     1090 2023-08-01 10:18:56.000000 riscemu-2.1.1/riscemu/instructions/RV_Debug.py
+-rw-r--r--   0 anton     (1000) users      (100)      412 2023-08-01 10:18:56.000000 riscemu-2.1.1/riscemu/instructions/__init__.py
+-rw-r--r--   0 anton     (1000) users      (100)     4901 2023-05-29 10:25:04.000000 riscemu-2.1.1/riscemu/instructions/instruction_set.py
+-rw-r--r--   0 anton     (1000) users      (100)     1027 2023-05-29 11:16:56.000000 riscemu-2.1.1/riscemu/interactive.py
+-rw-r--r--   0 anton     (1000) users      (100)     5042 2023-08-01 10:18:56.000000 riscemu-2.1.1/riscemu/parser.py
+drwxr-xr-x   0 anton     (1000) users      (100)        0 2023-08-01 10:30:39.873780 riscemu-2.1.1/riscemu/priv/
+-rw-r--r--   0 anton     (1000) users      (100)     4604 2023-05-29 10:25:04.000000 riscemu-2.1.1/riscemu/priv/CSR.py
+-rw-r--r--   0 anton     (1000) users      (100)     1981 2023-05-29 10:25:04.000000 riscemu-2.1.1/riscemu/priv/CSRConsts.py
+-rw-r--r--   0 anton     (1000) users      (100)     4414 2023-05-29 10:25:04.000000 riscemu-2.1.1/riscemu/priv/ElfLoader.py
+-rw-r--r--   0 anton     (1000) users      (100)     3159 2023-05-29 10:25:04.000000 riscemu-2.1.1/riscemu/priv/Exceptions.py
+-rw-r--r--   0 anton     (1000) users      (100)     2843 2023-05-29 10:25:04.000000 riscemu-2.1.1/riscemu/priv/ImageLoader.py
+-rw-r--r--   0 anton     (1000) users      (100)     8747 2023-05-29 10:25:04.000000 riscemu-2.1.1/riscemu/priv/PrivCPU.py
+-rw-r--r--   0 anton     (1000) users      (100)     1737 2023-05-29 10:25:04.000000 riscemu-2.1.1/riscemu/priv/PrivMMU.py
+-rw-r--r--   0 anton     (1000) users      (100)     5946 2023-05-29 10:25:04.000000 riscemu-2.1.1/riscemu/priv/PrivRV32I.py
+-rw-r--r--   0 anton     (1000) users      (100)      455 2023-05-29 10:25:04.000000 riscemu-2.1.1/riscemu/priv/__init__.py
+-rw-r--r--   0 anton     (1000) users      (100)     1706 2023-05-29 10:25:04.000000 riscemu-2.1.1/riscemu/priv/__main__.py
+-rw-r--r--   0 anton     (1000) users      (100)       96 2021-10-26 20:05:33.000000 riscemu-2.1.1/riscemu/priv/privmodes.py
+-rw-r--r--   0 anton     (1000) users      (100)     5271 2023-05-29 10:25:04.000000 riscemu-2.1.1/riscemu/priv/types.py
+-rw-r--r--   0 anton     (1000) users      (100)        0 2023-08-01 10:18:56.000000 riscemu-2.1.1/riscemu/py.typed
+-rw-r--r--   0 anton     (1000) users      (100)     6818 2023-08-01 10:18:56.000000 riscemu-2.1.1/riscemu/registers.py
+-rw-r--r--   0 anton     (1000) users      (100)     9491 2023-05-30 08:20:42.000000 riscemu-2.1.1/riscemu/riscemu_main.py
+-rw-r--r--   0 anton     (1000) users      (100)     8444 2023-05-30 08:10:33.000000 riscemu-2.1.1/riscemu/syscall.py
+-rw-r--r--   0 anton     (1000) users      (100)     3278 2023-08-01 10:18:56.000000 riscemu-2.1.1/riscemu/tokenizer.py
+drwxr-xr-x   0 anton     (1000) users      (100)        0 2023-08-01 10:30:39.877780 riscemu-2.1.1/riscemu/tools/
+-rwxr-xr-x   0 anton     (1000) users      (100)       44 2023-05-29 14:29:03.000000 riscemu-2.1.1/riscemu/tools/riscemu
+drwxr-xr-x   0 anton     (1000) users      (100)        0 2023-08-01 10:30:39.876780 riscemu-2.1.1/riscemu/types/
+-rw-r--r--   0 anton     (1000) users      (100)     1193 2023-08-01 10:18:56.000000 riscemu-2.1.1/riscemu/types/__init__.py
+-rw-r--r--   0 anton     (1000) users      (100)     1718 2023-05-29 10:25:04.000000 riscemu-2.1.1/riscemu/types/binary_data_memory_section.py
+-rw-r--r--   0 anton     (1000) users      (100)     3334 2023-05-29 12:57:41.000000 riscemu-2.1.1/riscemu/types/cpu.py
+-rw-r--r--   0 anton     (1000) users      (100)     4807 2023-05-29 10:25:04.000000 riscemu-2.1.1/riscemu/types/exceptions.py
+-rw-r--r--   0 anton     (1000) users      (100)      262 2023-05-29 10:25:04.000000 riscemu-2.1.1/riscemu/types/flags.py
+-rw-r--r--   0 anton     (1000) users      (100)     5702 2023-08-01 10:18:56.000000 riscemu-2.1.1/riscemu/types/float32.py
+-rw-r--r--   0 anton     (1000) users      (100)      642 2022-03-31 20:48:16.000000 riscemu-2.1.1/riscemu/types/instruction.py
+-rw-r--r--   0 anton     (1000) users      (100)     2195 2023-05-29 10:25:04.000000 riscemu-2.1.1/riscemu/types/instruction_context.py
+-rw-r--r--   0 anton     (1000) users      (100)     1496 2023-05-29 10:25:04.000000 riscemu-2.1.1/riscemu/types/instruction_memory_section.py
+-rw-r--r--   0 anton     (1000) users      (100)     8612 2023-08-01 10:18:56.000000 riscemu-2.1.1/riscemu/types/int32.py
+-rw-r--r--   0 anton     (1000) users      (100)     5271 2023-05-29 10:25:04.000000 riscemu-2.1.1/riscemu/types/memory_section.py
+-rw-r--r--   0 anton     (1000) users      (100)     4143 2023-05-29 10:25:04.000000 riscemu-2.1.1/riscemu/types/program.py
+-rw-r--r--   0 anton     (1000) users      (100)     1865 2023-05-29 10:25:04.000000 riscemu-2.1.1/riscemu/types/program_loader.py
+-rw-r--r--   0 anton     (1000) users      (100)      927 2023-05-29 10:25:04.000000 riscemu-2.1.1/riscemu/types/simple_instruction.py
+drwxr-xr-x   0 anton     (1000) users      (100)        0 2023-08-01 10:30:39.877780 riscemu-2.1.1/riscemu.egg-info/
+-rw-r--r--   0 anton     (1000) users      (100)     5579 2023-08-01 10:30:39.000000 riscemu-2.1.1/riscemu.egg-info/PKG-INFO
+-rw-r--r--   0 anton     (1000) users      (100)     2018 2023-08-01 10:30:39.000000 riscemu-2.1.1/riscemu.egg-info/SOURCES.txt
+-rw-r--r--   0 anton     (1000) users      (100)        1 2023-08-01 10:30:39.000000 riscemu-2.1.1/riscemu.egg-info/dependency_links.txt
+-rw-r--r--   0 anton     (1000) users      (100)       17 2023-08-01 10:30:39.000000 riscemu-2.1.1/riscemu.egg-info/requires.txt
+-rw-r--r--   0 anton     (1000) users      (100)        8 2023-08-01 10:30:39.000000 riscemu-2.1.1/riscemu.egg-info/top_level.txt
+-rw-r--r--   0 anton     (1000) users      (100)       38 2023-08-01 10:30:39.879780 riscemu-2.1.1/setup.cfg
+-rw-r--r--   0 anton     (1000) users      (100)     1195 2023-08-01 10:18:56.000000 riscemu-2.1.1/setup.py
+drwxr-xr-x   0 anton     (1000) users      (100)        0 2023-08-01 10:30:39.878780 riscemu-2.1.1/test/
+-rw-r--r--   0 anton     (1000) users      (100)      568 2023-08-01 10:18:56.000000 riscemu-2.1.1/test/test_float32.py
+-rw-r--r--   0 anton     (1000) users      (100)      395 2023-05-29 10:25:04.000000 riscemu-2.1.1/test/test_helpers.py
+-rw-r--r--   0 anton     (1000) users      (100)      468 2023-05-29 10:25:04.000000 riscemu-2.1.1/test/test_integers.py
+-rw-r--r--   0 anton     (1000) users      (100)     2326 2023-05-29 10:25:04.000000 riscemu-2.1.1/test/test_isa.py
+-rw-r--r--   0 anton     (1000) users      (100)      578 2023-08-01 10:18:56.000000 riscemu-2.1.1/test/test_regs.py
+-rw-r--r--   0 anton     (1000) users      (100)     4548 2023-05-29 10:25:04.000000 riscemu-2.1.1/test/test_tokenizer.py
```

### Comparing `riscemu-2.1.0/LICENSE` & `riscemu-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/PKG-INFO` & `riscemu-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: riscemu
-Version: 2.1.0
+Version: 2.1.1
 Summary: RISC-V userspace and machine mode emulator
 Home-page: https://github.com/antonlydike/riscemu
 Author: Anton Lydike <Anton@Lydike.com>
 Author-email: pip@antonlydike.de
 Project-URL: Bug Tracker, https://github.com/AntonLydike/riscemu/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `riscemu-2.1.0/README.md` & `riscemu-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/libc/stdlib.s` & `riscemu-2.1.1/libc/stdlib.s`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/libc/string.s` & `riscemu-2.1.1/libc/string.s`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu/CPU.py` & `riscemu-2.1.1/riscemu/CPU.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu/IO/IOModule.py` & `riscemu-2.1.1/riscemu/IO/IOModule.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu/IO/TextIO.py` & `riscemu-2.1.1/riscemu/IO/TextIO.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu/MMU.py` & `riscemu-2.1.1/riscemu/MMU.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu/__init__.py` & `riscemu-2.1.1/riscemu/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,8 +30,8 @@
 
 from .config import RunConfig
 
 from .parser import tokenize, parse_tokens, AssemblyFileLoader
 
 __author__ = "Anton Lydike <Anton@Lydike.com>"
 __copyright__ = "Copyright 2023 Anton Lydike"
-__version__ = "2.1.0"
+__version__ = "2.1.1"
```

### Comparing `riscemu-2.1.0/riscemu/assembler.py` & `riscemu-2.1.1/riscemu/assembler.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu/colors.py` & `riscemu-2.1.1/riscemu/colors.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu/config.py` & `riscemu-2.1.1/riscemu/config.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu/debug.py` & `riscemu-2.1.1/riscemu/debug.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu/decoder/__main__.py` & `riscemu-2.1.1/riscemu/decoder/__main__.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu/decoder/decoder.py` & `riscemu-2.1.1/riscemu/decoder/decoder.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu/decoder/formats.py` & `riscemu-2.1.1/riscemu/decoder/formats.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu/decoder/formatter.py` & `riscemu-2.1.1/riscemu/decoder/formatter.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu/decoder/instruction_table.py` & `riscemu-2.1.1/riscemu/decoder/instruction_table.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu/helpers.py` & `riscemu-2.1.1/riscemu/helpers.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu/instructions/RV32A.py` & `riscemu-2.1.1/riscemu/instructions/RV32A.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu/instructions/RV32F.py` & `riscemu-2.1.1/riscemu/instructions/RV32F.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,15 @@
 
         :Implementation:
         | f[rd] = f[rs1] + f[rs2]
         """
         rd, rs1, rs2 = self.parse_rd_rs_rs(ins)
         self.regs.set_f(
             rd,
-            self.regs.get_f(rs1) + self.regs.get_f(rs2),
+            rs1 + rs2,
         )
 
     def instruction_fsub_s(self, ins: Instruction):
         """
         +-----+-----+-----+-----+-----+-----+-----+---+
         |31-27|26-25|24-20|19-15|14-12|11-7 |6-2  |1-0|
         +-----+-----+-----+-----+-----+-----+-----+---+
@@ -141,15 +141,15 @@
 
         :Implementation:
         | f[rd] = f[rs1] - f[rs2]
         """
         rd, rs1, rs2 = self.parse_rd_rs_rs(ins)
         self.regs.set_f(
             rd,
-            self.regs.get_f(rs1) - self.regs.get_f(rs2),
+            rs1 - rs2,
         )
 
     def instruction_fmul_s(self, ins: Instruction):
         """
         +-----+-----+-----+-----+-----+-----+-----+---+
         |31-27|26-25|24-20|19-15|14-12|11-7 |6-2  |1-0|
         +-----+-----+-----+-----+-----+-----+-----+---+
@@ -165,15 +165,15 @@
 
         :Implementation:
         | f[rd] = f[rs1] × f[rs2]
         """
         rd, rs1, rs2 = self.parse_rd_rs_rs(ins)
         self.regs.set_f(
             rd,
-            self.regs.get_f(rs1) * self.regs.get_f(rs2),
+            rs1 * rs2,
         )
 
     def instruction_fdiv_s(self, ins: Instruction):
         """
         +-----+-----+-----+-----+-----+-----+-----+---+
         |31-27|26-25|24-20|19-15|14-12|11-7 |6-2  |1-0|
         +-----+-----+-----+-----+-----+-----+-----+---+
@@ -189,15 +189,15 @@
 
         :Implementation:
         | f[rd] = f[rs1] / f[rs2]
         """
         rd, rs1, rs2 = self.parse_rd_rs_rs(ins)
         self.regs.set_f(
             rd,
-            self.regs.get_f(rs1) / self.regs.get_f(rs2),
+            rs1 / rs2,
         )
 
     def instruction_fsqrt_s(self, ins: Instruction):
         """
         +-----+-----+-----+-----+-----+-----+-----+---+
         |31-27|26-25|24-20|19-15|14-12|11-7 |6-2  |1-0|
         +-----+-----+-----+-----+-----+-----+-----+---+
@@ -211,15 +211,15 @@
         :Description:
         | Perform single-precision square root.
 
         :Implementation:
         | f[rd] = sqrt(f[rs1])
         """
         rd, rs = self.parse_rd_rs(ins)
-        self.regs.set_f(self.regs.get_f(rs) ** 0.5)
+        self.regs.set_f(rd, self.regs.get_f(rs) ** 0.5)
 
     def instruction_fsgnj_s(self, ins: Instruction):
         """
         +-----+-----+-----+-----+-----+-----+-----+---+
         |31-27|26-25|24-20|19-15|14-12|11-7 |6-2  |1-0|
         +-----+-----+-----+-----+-----+-----+-----+---+
         |00100|00   |rs2  |rs1  |000  |rd   |10100|11 |
@@ -296,16 +296,16 @@
         | f[rd] = min(f[rs1], f[rs2])
         """
         rd, rs1, rs2 = self.parse_rd_rs_rs(ins)
         self.regs.set_f(
             rd,
             Float32(
                 min(
-                    self.regs.get_f(rs1).value,
-                    self.regs.get_f(rs2).value,
+                    rs1.value,
+                    rs2.value,
                 )
             ),
         )
 
     def instruction_fmax_s(self, ins: Instruction):
         """
         +-----+-----+-----+-----+-----+-----+-----+---+
@@ -324,16 +324,16 @@
         | f[rd] = max(f[rs1], f[rs2])
         """
         rd, rs1, rs2 = self.parse_rd_rs_rs(ins)
         self.regs.set_f(
             rd,
             Float32(
                 max(
-                    self.regs.get_f(rs1).value,
-                    self.regs.get_f(rs2).value,
+                    rs1.value,
+                    rs2.value,
                 )
             ),
         )
 
     def instruction_fcvt_w_s(self, ins: Instruction):
         """
         +-----+-----+-----+-----+-----+-----+-----+---+
@@ -348,15 +348,15 @@
         :Description:
         | Convert a floating-point number in floating-point register rs1 to a signed 32-bit in integer register rd.
 
         :Implementation:
         | x[rd] = sext(s32_{f32}(f[rs1]))
         """
         rd, rs = self.parse_rd_rs(ins)
-        self.regs.set(rd, Int32(self.regs.get_f(rs).value))
+        self.regs.set(rd, Int32(self.regs.get_f(rs).bytes))
 
     def instruction_fcvt_wu_s(self, ins: Instruction):
         """
         +-----+-----+-----+-----+-----+-----+-----+---+
         |31-27|26-25|24-20|19-15|14-12|11-7 |6-2  |1-0|
         +-----+-----+-----+-----+-----+-----+-----+---+
         |11000|00   |00001|rs1  |rm   |rd   |10100|11 |
@@ -368,15 +368,15 @@
         :Description:
         | Convert a floating-point number in floating-point register rs1 to a signed 32-bit in unsigned integer register rd.
 
         :Implementation:
         | x[rd] = sext(u32_{f32}(f[rs1]))
         """
         rd, rs = self.parse_rd_rs(ins)
-        self.regs.set(rd, UInt32(self.regs.get_f(rs).value))
+        self.regs.set(rd, UInt32(self.regs.get_f(rs).bytes))
 
     def instruction_fmv_x_w(self, ins: Instruction):
         """
         +-----+-----+-----+-----+-----+-----+-----+---+
         |31-27|26-25|24-20|19-15|14-12|11-7 |6-2  |1-0|
         +-----+-----+-----+-----+-----+-----+-----+---+
         |11100|00   |00000|rs1  |000  |rd   |10100|11 |
@@ -496,15 +496,15 @@
         :Description:
         | Converts a 32-bit signed integer, in integer register rs1 into a floating-point number in floating-point register rd.
 
         :Implementation:
         | f[rd] = f32_{s32}(x[rs1])
         """
         rd, rs = self.parse_rd_rs(ins)
-        self.regs.set_f(rd, Float32(self.regs.get(rs).signed().value))
+        self.regs.set_f(rd, Float32.from_bytes(self.regs.get(rs).signed().value))
 
     def instruction_fcvt_s_wu(self, ins: Instruction):
         """
         +-----+-----+-----+-----+-----+-----+-----+---+
         |31-27|26-25|24-20|19-15|14-12|11-7 |6-2  |1-0|
         +-----+-----+-----+-----+-----+-----+-----+---+
         |11010|00   |00001|rs1  |rm   |rd   |10100|11 |
@@ -516,15 +516,15 @@
         :Description:
         | Converts a 32-bit unsigned integer, in integer register rs1 into a floating-point number in floating-point register rd.
 
         :Implementation:
         | f[rd] = f32_{u32}(x[rs1])
         """
         rd, rs = self.parse_rd_rs(ins)
-        self.regs.set_f(rd, Float32(self.regs.get(rs).unsigned_value))
+        self.regs.set_f(rd, Float32.from_bytes(self.regs.get(rs).unsigned_value))
 
     def instruction_fmv_w_x(self, ins: Instruction):
         """
         +-----+-----+-----+-----+-----+-----+-----+---+
         |31-27|26-25|24-20|19-15|14-12|11-7 |6-2  |1-0|
         +-----+-----+-----+-----+-----+-----+-----+---+
         |11110|00   |00000|rs1  |000  |rd   |10100|11 |
@@ -558,15 +558,15 @@
         :Description:
           | Load a single-precision floating-point value from memory into floating-point register rd.
 
         :Implementation:
           | f[rd] = M[x[rs1] + sext(offset)][31:0]
         """
         rd, addr = self.parse_mem_ins(ins)
-        self.regs.set_f(rd, self.mmu.read_float(addr))
+        self.regs.set_f(rd, self.mmu.read_float(addr.value))
 
     def instruction_fsw(self, ins: Instruction):
         """
         +-----+-----+-----+-----+-----+--------+-----+---+
         |31-27|26-25|24-20|19-15|14-12|11-7    |6-2  |1-0|
         +-----+-----+-----+-----+-----+--------+-----+---+
         |imm[11:5]  |rs2  |rs1  |010  |imm[4:0]|01001|11 |
@@ -579,15 +579,15 @@
           | Store a single-precision value from floating-point register rs2 to memory.
 
         :Implementation:
           | M[x[rs1] + sext(offset)] = f[rs2][31:0]
         """
         rs, addr = self.parse_mem_ins(ins)
         val = self.regs.get_f(rs)
-        self.mmu.write(addr, 4, bytearray(val.bytes))
+        self.mmu.write(addr.value, 4, bytearray(val.bytes))
 
     def parse_rd_rs(self, ins: Instruction) -> Tuple[str, str]:
         assert len(ins.args) == 2
         return ins.get_reg(0), ins.get_reg(1)
 
     def parse_rd_rs_rs(self, ins: Instruction) -> Tuple[str, Float32, Float32]:
         assert len(ins.args) == 3
```

### Comparing `riscemu-2.1.0/riscemu/instructions/RV32I.py` & `riscemu-2.1.1/riscemu/instructions/RV32I.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu/instructions/RV32M.py` & `riscemu-2.1.1/riscemu/instructions/RV32M.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu/instructions/RV_Debug.py` & `riscemu-2.1.1/riscemu/instructions/RV_Debug.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,25 +2,31 @@
 
 
 class RV_Debug(InstructionSet):
     def instruction_print(self, ins: Instruction):
         reg = ins.get_reg(0)
         print("register {} contains value {}".format(reg, self.regs.get(reg)))
 
+    def instruction_print_float(self, ins: Instruction):
+        reg = ins.get_reg(0)
+        print("register {} contains value {}".format(reg, self.regs.get_f(reg).value))
+
     def instruction_print_uint(self, ins: Instruction):
         reg = ins.get_reg(0)
         print(
             "register {} contains value {}".format(
                 reg, self.regs.get(reg).unsigned_value
             )
         )
 
     def instruction_print_hex(self, ins: Instruction):
         reg = ins.get_reg(0)
-        print("register {} contains value {}".format(reg, hex(self.regs.get(reg))))
+        print(
+            "register {} contains value {}".format(reg, hex(self.regs.get(reg).value))
+        )
 
     def instruction_print_uhex(self, ins: Instruction):
         reg = ins.get_reg(0)
         print(
             "register {} contains value {}".format(
                 reg, hex(self.regs.get(reg).unsigned_value)
             )
```

### Comparing `riscemu-2.1.0/riscemu/instructions/instruction_set.py` & `riscemu-2.1.1/riscemu/instructions/instruction_set.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu/interactive.py` & `riscemu-2.1.1/riscemu/interactive.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu/parser.py` & `riscemu-2.1.1/riscemu/parser.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu/priv/CSR.py` & `riscemu-2.1.1/riscemu/priv/CSR.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu/priv/CSRConsts.py` & `riscemu-2.1.1/riscemu/priv/CSRConsts.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu/priv/ElfLoader.py` & `riscemu-2.1.1/riscemu/priv/ElfLoader.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu/priv/Exceptions.py` & `riscemu-2.1.1/riscemu/priv/Exceptions.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu/priv/ImageLoader.py` & `riscemu-2.1.1/riscemu/priv/ImageLoader.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu/priv/PrivCPU.py` & `riscemu-2.1.1/riscemu/priv/PrivCPU.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu/priv/PrivMMU.py` & `riscemu-2.1.1/riscemu/priv/PrivMMU.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu/priv/PrivRV32I.py` & `riscemu-2.1.1/riscemu/priv/PrivRV32I.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu/priv/__main__.py` & `riscemu-2.1.1/riscemu/priv/__main__.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu/priv/types.py` & `riscemu-2.1.1/riscemu/priv/types.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu/registers.py` & `riscemu-2.1.1/riscemu/registers.py`

 * *Files 4% similar despite different names*

```diff
@@ -143,24 +143,33 @@
         """
         print(
             "Registers[a]:"
             + " ".join(self._reg_repr("a{}".format(i)) for i in range(8))
         )
 
     def _reg_repr(self, reg: str, name_len=4, fmt="08X"):
-        txt = "{:{}}=0x{:{}}".format(reg, name_len, self.get(reg, False), fmt)
+        if reg in self.float_regs:
+            txt = "{:{}}={: .3e}".format(reg, name_len, self.get_f(reg, False))
+        else:
+            txt = "{:{}}=0x{:{}}".format(reg, name_len, self.get(reg, False), fmt)
         if reg == "fp":
             reg = "s0"
         if reg == self.last_set:
             return FMT_ORANGE + FMT_BOLD + txt + FMT_NONE
         if reg == self.last_read:
             return FMT_ORANGE + FMT_UNDERLINE + txt + FMT_NONE
         if reg == "zero":
             return txt
-        if self.get(reg, False) == 0 and reg not in Registers.named_registers():
+        should_grayscale_int = (
+            reg in self.valid_regs
+            and self.get(reg, False) == 0
+            and reg not in Registers.named_registers()
+        )
+        should_grayscale_float = reg in self.float_regs and self.get_f(reg, False) == 0
+        if should_grayscale_int or should_grayscale_float:
             return FMT_GRAY + txt + FMT_NONE
         return txt
 
     def set(self, reg: str, val: "Int32", mark_set: bool = True) -> bool:
         """
         Set a register content to val
         :param reg: The register to set
```

### Comparing `riscemu-2.1.0/riscemu/riscemu_main.py` & `riscemu-2.1.1/riscemu/riscemu_main.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu/syscall.py` & `riscemu-2.1.1/riscemu/syscall.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu/tokenizer.py` & `riscemu-2.1.1/riscemu/tokenizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from riscemu.decoder import RISCV_REGS
 from riscemu.types.exceptions import ParseException
 
 LINE_COMMENT_STARTERS = ("#", ";", "//")
 WHITESPACE_PATTERN = re.compile(r"\s+")
 MEMORY_ADDRESS_PATTERN = re.compile(
-    r"^(0[xX][A-f0-9]+|\d+|0b[0-1]+|[A-z0-9_-]+)\(([A-z]+[0-9]{0,2})\)$"
+    r"^(0[xX][A-f0-9]+|\d+|0b[0-1]+|[A-z0-9_-]+)\(([A-z]+[0-9]*)\)$"
 )
 REGISTER_NAMES = RISCV_REGS
 
 
 class TokenType(Enum):
     COMMA = auto()
     ARGUMENT = auto()
@@ -84,18 +84,17 @@
 
 def parse_arg(arg: str) -> Iterable[Token]:
     comma = arg[-1] == ","
     arg = arg[:-1] if comma else arg
     mem_match_resul = re.match(MEMORY_ADDRESS_PATTERN, arg)
     if mem_match_resul:
         register = mem_match_resul.group(2).lower()
-        if register not in RISCV_REGS:
-            raise ParseException(f'"{register}" is not a valid register!')
+        immediate = mem_match_resul.group(1)
         yield Token(TokenType.ARGUMENT, register)
-        yield Token(TokenType.ARGUMENT, mem_match_resul.group(1))
+        yield Token(TokenType.ARGUMENT, immediate)
     else:
         yield Token(TokenType.ARGUMENT, arg)
     if comma:
         yield COMMA
 
 
 def print_tokens(tokens: Iterable[Token]):
```

### Comparing `riscemu-2.1.0/riscemu/types/__init__.py` & `riscemu-2.1.1/riscemu/types/__init__.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu/types/binary_data_memory_section.py` & `riscemu-2.1.1/riscemu/types/binary_data_memory_section.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu/types/cpu.py` & `riscemu-2.1.1/riscemu/types/cpu.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu/types/exceptions.py` & `riscemu-2.1.1/riscemu/types/exceptions.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu/types/float32.py` & `riscemu-2.1.1/riscemu/types/float32.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         The values bit representation as an int (for easy bit manipulation)
         """
         return int.from_bytes(self.bytes, byteorder="little")
 
     @classmethod
     def from_bytes(cls, val: Union[int, bytes_t, bytearray]):
         if isinstance(val, int):
-            val = int.to_bytes(byteorder="little")
+            val = struct.unpack("!f", struct.pack("!I", val))[0]
         return Float32(val)
 
     def __init__(
         self, val: Union[float, c_float, "Float32", bytes_t, bytearray, int] = 0
     ):
         if isinstance(val, (float, int)):
             self._val = c_float(val)
@@ -130,19 +130,14 @@
         if isinstance(other, Float32):
             other = other.value
         return self.value >= other
 
     def __bool__(self):
         return bool(self.value)
 
-    def __cmp__(self, other: Any):
-        if isinstance(other, Float32):
-            other = other.value
-        return self.value.__cmp__(other)
-
     def __pow__(self, power, modulo=None):
         if modulo is not None:
             raise ValueError("Float32 pow with modulo unsupported")
         return self.__class__(self.value**power)
 
     # right handed binary operators
```

### Comparing `riscemu-2.1.0/riscemu/types/instruction.py` & `riscemu-2.1.1/riscemu/types/instruction.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu/types/instruction_context.py` & `riscemu-2.1.1/riscemu/types/instruction_context.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu/types/instruction_memory_section.py` & `riscemu-2.1.1/riscemu/types/instruction_memory_section.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu/types/int32.py` & `riscemu-2.1.1/riscemu/types/int32.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu/types/memory_section.py` & `riscemu-2.1.1/riscemu/types/memory_section.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu/types/program.py` & `riscemu-2.1.1/riscemu/types/program.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu/types/program_loader.py` & `riscemu-2.1.1/riscemu/types/program_loader.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu/types/simple_instruction.py` & `riscemu-2.1.1/riscemu/types/simple_instruction.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/riscemu.egg-info/PKG-INFO` & `riscemu-2.1.1/riscemu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: riscemu
-Version: 2.1.0
+Version: 2.1.1
 Summary: RISC-V userspace and machine mode emulator
 Home-page: https://github.com/antonlydike/riscemu
 Author: Anton Lydike <Anton@Lydike.com>
 Author-email: pip@antonlydike.de
 Project-URL: Bug Tracker, https://github.com/AntonLydike/riscemu/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `riscemu-2.1.0/riscemu.egg-info/SOURCES.txt` & `riscemu-2.1.1/riscemu.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 ./riscemu/types/instruction_memory_section.py
 ./riscemu/types/int32.py
 ./riscemu/types/memory_section.py
 ./riscemu/types/program.py
 ./riscemu/types/program_loader.py
 ./riscemu/types/simple_instruction.py
 libc/crt0.s
+libc/stdio.s
 libc/stdlib.s
 libc/string.s
 riscemu.egg-info/PKG-INFO
 riscemu.egg-info/SOURCES.txt
 riscemu.egg-info/dependency_links.txt
 riscemu.egg-info/requires.txt
 riscemu.egg-info/top_level.txt
```

### Comparing `riscemu-2.1.0/setup.py` & `riscemu-2.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,13 +32,13 @@
         "riscemu.priv",
         "riscemu.types",
     ],
     package_data={
         "riscemu": ["libc/*.s", "py.typed"],
     },
     data_files=[
-        ('libc', glob('libc/*.s')),
+        ("libc", glob("libc/*.s")),
     ],
     scripts=["riscemu/tools/riscemu"],
     python_requires=">=3.8",
     install_requires=["pyelftools~=0.27"],
 )
```

### Comparing `riscemu-2.1.0/test/test_isa.py` & `riscemu-2.1.1/test/test_isa.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/test/test_regs.py` & `riscemu-2.1.1/test/test_regs.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.1.0/test/test_tokenizer.py` & `riscemu-2.1.1/test/test_tokenizer.py`

 * *Files identical despite different names*

