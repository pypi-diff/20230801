# Comparing `tmp/fprime_gds-3.2.1a2.tar.gz` & `tmp/fprime_gds-3.3.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fprime_gds-3.2.1a2.tar", last modified: Mon May  8 16:30:37 2023, max compression
+gzip compressed data, was "fprime_gds-3.3.0a1.tar", last modified: Tue Aug  1 20:46:04 2023, max compression
```

## Comparing `fprime_gds-3.2.1a2.tar` & `fprime_gds-3.3.0a1.tar`

### file list

```diff
@@ -1,349 +1,349 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.987830 fprime_gds-3.2.1a2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.951829 fprime_gds-3.2.1a2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.951829 fprime_gds-3.2.1a2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/.github/ISSUE_TEMPLATE/feature-request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.947829 fprime_gds-3.2.1a2/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.951829 fprime_gds-3.2.1a2/.github/actions/codeql/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/.github/actions/codeql/security-pack.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.951829 fprime_gds-3.2.1a2/.github/actions/spelling/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/.github/actions/spelling/excludes.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/.github/actions/spelling/expect.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/.github/actions/spelling/patterns.txt
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.951829 fprime_gds-3.2.1a2/.github/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    87604 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/.github/resources/RefTopologyAppDictionary.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.955829 fprime_gds-3.2.1a2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/.github/workflows/codeql-security-scan.yml
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/.github/workflows/fprime-gds-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/.github/workflows/gds-cli-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/.github/workflows/spelling.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)   106207 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/Doxyfile
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-08 16:30:37.987830 fprime_gds-3.2.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10006 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.955829 fprime_gds-3.2.1a2/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.955829 fprime_gds-3.2.1a2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.947829 fprime_gds-3.2.1a2/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.955829 fprime_gds-3.2.1a2/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/docs/_static/css/rtd_width.css
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/docs/conf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      164 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/docs/gendoc.bash
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.955829 fprime_gds-3.2.1a2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/examples/simple_sequence.bin
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/examples/simple_sequence.seq
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 16:30:37.987830 fprime_gds-3.2.1a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.955829 fprime_gds-3.2.1a2/src/
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fastentrypoints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.955829 fprime_gds-3.2.1a2/src/fprime_gds/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.955829 fprime_gds-3.2.1a2/src/fprime_gds/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.955829 fprime_gds-3.2.1a2/src/fprime_gds/common/communication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/communication/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.955829 fprime_gds-3.2.1a2/src/fprime_gds/common/communication/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/communication/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/communication/adapters/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16064 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/communication/adapters/ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/communication/adapters/uart.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/communication/checksum.py
--rw-r--r--   0 runner    (1001) docker     (123)    10661 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/communication/framing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/communication/ground.py
--rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/communication/updown.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.955829 fprime_gds-3.2.1a2/src/fprime_gds/common/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/controllers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.959829 fprime_gds-3.2.1a2/src/fprime_gds/common/data_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/data_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/data_types/ch_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/data_types/cmd_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/data_types/event_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/data_types/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/data_types/file_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/data_types/pkt_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/data_types/sys_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.959829 fprime_gds-3.2.1a2/src/fprime_gds/common/decoders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/decoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/decoders/ch_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/decoders/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/decoders/event_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/decoders/file_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/decoders/pkt_decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.959829 fprime_gds-3.2.1a2/src/fprime_gds/common/distributor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/distributor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/distributor/distributor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.959829 fprime_gds-3.2.1a2/src/fprime_gds/common/encoders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/encoders/ch_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/encoders/cmd_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/encoders/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/encoders/event_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/encoders/file_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/encoders/pkt_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/encoders/seq_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.959829 fprime_gds-3.2.1a2/src/fprime_gds/common/files/
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/files/File Decoder Documentation.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/files/downlinker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7205 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/files/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13230 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/files/uplinker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.959829 fprime_gds-3.2.1a2/src/fprime_gds/common/gds_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/gds_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9410 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/gds_cli/base_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/gds_cli/channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/gds_cli/command_send.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/gds_cli/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/gds_cli/filtering_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/gds_cli/test_api_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.963829 fprime_gds-3.2.1a2/src/fprime_gds/common/history/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/history/chrono.py
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/history/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/history/ram.py
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/history/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.963829 fprime_gds-3.2.1a2/src/fprime_gds/common/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/loaders/ch_py_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/loaders/ch_xml_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/loaders/cmd_py_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/loaders/cmd_xml_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/loaders/dict_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/loaders/event_py_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/loaders/event_xml_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/loaders/pkt_xml_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/loaders/python_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    14902 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/loaders/xml_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.963829 fprime_gds-3.2.1a2/src/fprime_gds/common/logger/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/logger/data_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/logger/test_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.963829 fprime_gds-3.2.1a2/src/fprime_gds/common/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.963829 fprime_gds-3.2.1a2/src/fprime_gds/common/models/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/models/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/models/common/channel_telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/models/common/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/models/common/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.963829 fprime_gds-3.2.1a2/src/fprime_gds/common/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/parsers/seq_file_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.963829 fprime_gds-3.2.1a2/src/fprime_gds/common/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/pipeline/dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/pipeline/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/pipeline/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/pipeline/histories.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/pipeline/router.py
--rw-r--r--   0 runner    (1001) docker     (123)     8655 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/pipeline/standard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.963829 fprime_gds-3.2.1a2/src/fprime_gds/common/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/templates/ch_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/templates/cmd_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/templates/data_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/templates/event_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/templates/pkt_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.967829 fprime_gds-3.2.1a2/src/fprime_gds/common/testing_fw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/testing_fw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    60456 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/testing_fw/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18371 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/testing_fw/predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/testing_fw/pytest_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.967829 fprime_gds-3.2.1a2/src/fprime_gds/common/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/tools/seqgen.py
--rw-r--r--   0 runner    (1001) docker     (123)    10521 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/transport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.967829 fprime_gds-3.2.1a2/src/fprime_gds/common/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/utils/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/utils/data_desc_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/utils/event_severity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/utils/string_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/common/zmq_transport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.967829 fprime_gds-3.2.1a2/src/fprime_gds/executables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/executables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29973 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/executables/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/executables/comm.py
--rw-r--r--   0 runner    (1001) docker     (123)    12432 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/executables/fprime_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/executables/run_deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)    17533 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/executables/tcpserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/executables/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.967829 fprime_gds-3.2.1a2/src/fprime_gds/flask/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/default_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    19770 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/flask_uploads.py
--rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/sequence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.967829 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.971829 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/.idea/static.iml
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/.idea/vcs.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.971829 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.971829 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/advanced-settings/
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/advanced-settings/addon-templates.js
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/advanced-settings/addon.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.971829 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/channel-render/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/channel-render/addon.js
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/channel-render/channel-render-template.js
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/channel-render/channel-render.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.971829 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/chart-display/
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/chart-display/addon-templates.js
--rw-r--r--   0 runner    (1001) docker     (123)     9185 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/chart-display/addon.js
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/chart-display/config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.971829 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/chart-display/modified-vendor/
--rw-r--r--   0 runner    (1001) docker     (123)    30243 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/chart-display/modified-vendor/chartjs-plugin-streaming.js
--rw-r--r--   0 runner    (1001) docker     (123)    29512 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/chart-display/modified-vendor/chartjs-plugin-zoom.js
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/chart-display/modified-vendor/flat.js
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/chart-display/sibling.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.971829 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/chart-display/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)   184059 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/chart-display/vendor/chart.js
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/chart-display/vendor/chartjs-adapter-luxon.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    20727 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/chart-display/vendor/hammer.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.971829 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/commanding/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/commanding/addon.js
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/commanding/argument-templates.js
--rw-r--r--   0 runner    (1001) docker     (123)    10665 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/commanding/arguments.js
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/commanding/command-history-template.js
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/commanding/command-history.js
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/commanding/command-input-template.js
--rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/commanding/command-input.js
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/commanding/command-string-template.js
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/commanding/command-string.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.971829 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/dictionary/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/dictionary/addon-templates.js
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/dictionary/addon.js
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/enabled.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.971829 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/image-display/
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/image-display/addon.js
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/image-display/dashboard.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.975829 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/sequencer/
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/sequencer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/sequencer/addon-templates.js
--rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/sequencer/addon.js
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/sequencer/autocomplete.js
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/sequencer/lint.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.975829 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/sequencer/third/
--rw-r--r--   0 runner    (1001) docker     (123)   813045 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/sequencer/third/code-mirror.es.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.975829 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/sequencer/third/rollup/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/sequencer/third/rollup/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/sequencer/third/rollup/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/sequencer/third/rollup/language.grammer
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/sequencer/third/rollup/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/sequencer/third/rollup/rollup.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.975829 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)   180390 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/css/fprime.css
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/css/fpstyle.css
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.975829 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/img/
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/img/error.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12470 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/img/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/img/success.svg
--rw-r--r--   0 runner    (1001) docker     (123)    26087 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.975829 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/js/config.js
--rw-r--r--   0 runner    (1001) docker     (123)    14515 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/js/datastore.js
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/js/gds.js
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/js/loader.js
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/js/performance.js
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/js/settings.js
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/js/uploader.js
--rw-r--r--   0 runner    (1001) docker     (123)    12814 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/js/validate.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.979829 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/js/vue-support/
--rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/js/vue-support/channel.js
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/js/vue-support/dashboard-box.js
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/js/vue-support/dashboard-row.js
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/js/vue-support/dashboard.js
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/js/vue-support/downlink.js
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/js/vue-support/event.js
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/js/vue-support/fp-row.js
--rw-r--r--   0 runner    (1001) docker     (123)    18646 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/js/vue-support/fptable.js
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/js/vue-support/log.js
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/js/vue-support/tabetc.js
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/js/vue-support/uplink.js
--rw-r--r--   0 runner    (1001) docker     (123)    16197 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/js/vue-support/utils.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.951829 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.979829 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/css/
--rw-r--r--   0 runner    (1001) docker     (123)    59305 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/css/all.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   161364 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/css/vue-select.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.979829 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/js/
--rw-r--r--   0 runner    (1001) docker     (123)    72827 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/js/luxon.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    16877 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/js/sorttable.js
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/js/v-runtime-template.js
--rw-r--r--   0 runner    (1001) docker     (123)    16999 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/js/vue-select.js
--rw-r--r--   0 runner    (1001) docker     (123)    93675 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/js/vue.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.983829 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/webfonts/
--rw-r--r--   0 runner    (1001) docker     (123)   134294 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/webfonts/fa-brands-400.eot
--rw-r--r--   0 runner    (1001) docker     (123)   747927 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/webfonts/fa-brands-400.svg
--rw-r--r--   0 runner    (1001) docker     (123)   133988 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/webfonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    89988 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/webfonts/fa-brands-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)    76736 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/webfonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    34034 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/webfonts/fa-regular-400.eot
--rw-r--r--   0 runner    (1001) docker     (123)   144714 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/webfonts/fa-regular-400.svg
--rw-r--r--   0 runner    (1001) docker     (123)    33736 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/webfonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    16276 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/webfonts/fa-regular-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13224 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/webfonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   203030 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.eot
--rw-r--r--   0 runner    (1001) docker     (123)   918991 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.svg
--rw-r--r--   0 runner    (1001) docker     (123)   202744 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   101648 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.woff
--rw-r--r--   0 runner    (1001) docker     (123)    78268 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/flask/updown.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/src/fprime_gds/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.955829 fprime_gds-3.2.1a2/src/fprime_gds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-08 16:30:37.000000 fprime_gds-3.2.1a2/src/fprime_gds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12873 2023-05-08 16:30:37.000000 fprime_gds-3.2.1a2/src/fprime_gds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 16:30:37.000000 fprime_gds-3.2.1a2/src/fprime_gds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-08 16:30:37.000000 fprime_gds-3.2.1a2/src/fprime_gds.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 16:30:05.000000 fprime_gds-3.2.1a2/src/fprime_gds.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-08 16:30:37.000000 fprime_gds-3.2.1a2/src/fprime_gds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-08 16:30:37.000000 fprime_gds-3.2.1a2/src/fprime_gds.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.951829 fprime_gds-3.2.1a2/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.951829 fprime_gds-3.2.1a2/test/fprime_gds/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.951829 fprime_gds-3.2.1a2/test/fprime_gds/common/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.983829 fprime_gds-3.2.1a2/test/fprime_gds/common/distributor/
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/test/fprime_gds/common/distributor/test_distributor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.983829 fprime_gds-3.2.1a2/test/fprime_gds/common/encoders/
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/test/fprime_gds/common/encoders/test_ch_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/test/fprime_gds/common/encoders/test_event_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/test/fprime_gds/common/encoders/test_pkt_encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.983829 fprime_gds-3.2.1a2/test/fprime_gds/common/gds_cli/
--rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/test/fprime_gds/common/gds_cli/filtering_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7628 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/test/fprime_gds/common/gds_cli/utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.983829 fprime_gds-3.2.1a2/test/fprime_gds/common/history/
--rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/test/fprime_gds/common/history/chronohistory_unit_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/test/fprime_gds/common/history/testhistory_unit_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.983829 fprime_gds-3.2.1a2/test/fprime_gds/common/testing_fw/
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/test/fprime_gds/common/testing_fw/UnitTestDictionary.xml
--rw-r--r--   0 runner    (1001) docker     (123)    39899 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/test/fprime_gds/common/testing_fw/api_unit_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.983829 fprime_gds-3.2.1a2/test/fprime_gds/common/testing_fw/logs/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/test/fprime_gds/common/testing_fw/logs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/test/fprime_gds/common/testing_fw/predicate_unit_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.983829 fprime_gds-3.2.1a2/test/fprime_gds/common/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/test/fprime_gds/common/tools/seqgen_unit_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.983829 fprime_gds-3.2.1a2/test/fprime_gds/common/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/test/fprime_gds/common/utils/test_string_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.987830 fprime_gds-3.2.1a2/test/fprime_gds/executables/
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/test/fprime_gds/executables/test_run_deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/test/fprime_gds/executables/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:37.987830 fprime_gds-3.2.1a2/test/gui/
--rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-05-08 16:29:58.000000 fprime_gds-3.2.1a2/test/gui/GUI_Test_Procedure.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.658909 fprime_gds-3.3.0a1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.622909 fprime_gds-3.3.0a1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.622909 fprime_gds-3.3.0a1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/.github/ISSUE_TEMPLATE/feature-request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.618909 fprime_gds-3.3.0a1/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.622909 fprime_gds-3.3.0a1/.github/actions/codeql/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/.github/actions/codeql/security-pack.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.626909 fprime_gds-3.3.0a1/.github/actions/spelling/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/.github/actions/spelling/excludes.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/.github/actions/spelling/expect.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/.github/actions/spelling/patterns.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.626909 fprime_gds-3.3.0a1/.github/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    87604 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/.github/resources/RefTopologyAppDictionary.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.626909 fprime_gds-3.3.0a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/.github/workflows/codeql-security-scan.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/.github/workflows/fprime-gds-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/.github/workflows/gds-cli-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/.github/workflows/spelling.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)   106207 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/Doxyfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-08-01 20:46:04.654909 fprime_gds-3.3.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10006 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.626909 fprime_gds-3.3.0a1/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.626909 fprime_gds-3.3.0a1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.618909 fprime_gds-3.3.0a1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.626909 fprime_gds-3.3.0a1/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/docs/_static/css/rtd_width.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/docs/conf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      164 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/docs/gendoc.bash
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.626909 fprime_gds-3.3.0a1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/examples/simple_sequence.bin
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/examples/simple_sequence.seq
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 20:46:04.658909 fprime_gds-3.3.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.626909 fprime_gds-3.3.0a1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fastentrypoints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.626909 fprime_gds-3.3.0a1/src/fprime_gds/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.626909 fprime_gds-3.3.0a1/src/fprime_gds/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.626909 fprime_gds-3.3.0a1/src/fprime_gds/common/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/communication/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.630909 fprime_gds-3.3.0a1/src/fprime_gds/common/communication/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/communication/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/communication/adapters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16082 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/communication/adapters/ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/communication/adapters/uart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/communication/checksum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/communication/framing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/communication/ground.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/communication/updown.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.630909 fprime_gds-3.3.0a1/src/fprime_gds/common/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/controllers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.630909 fprime_gds-3.3.0a1/src/fprime_gds/common/data_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/data_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/data_types/ch_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/data_types/cmd_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/data_types/event_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/data_types/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/data_types/file_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/data_types/pkt_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/data_types/sys_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.630909 fprime_gds-3.3.0a1/src/fprime_gds/common/decoders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/decoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/decoders/ch_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/decoders/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/decoders/event_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/decoders/file_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/decoders/pkt_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.630909 fprime_gds-3.3.0a1/src/fprime_gds/common/distributor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/distributor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/distributor/distributor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.630909 fprime_gds-3.3.0a1/src/fprime_gds/common/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/encoders/ch_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/encoders/cmd_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/encoders/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/encoders/event_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/encoders/file_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/encoders/pkt_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6872 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/encoders/seq_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.630909 fprime_gds-3.3.0a1/src/fprime_gds/common/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/files/File Decoder Documentation.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/files/downlinker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7205 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/files/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13252 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/files/uplinker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.630909 fprime_gds-3.3.0a1/src/fprime_gds/common/gds_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/gds_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9410 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/gds_cli/base_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/gds_cli/channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/gds_cli/command_send.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/gds_cli/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/gds_cli/filtering_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/gds_cli/test_api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.634909 fprime_gds-3.3.0a1/src/fprime_gds/common/history/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/history/chrono.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/history/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/history/ram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/history/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.634909 fprime_gds-3.3.0a1/src/fprime_gds/common/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/loaders/ch_py_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/loaders/ch_xml_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/loaders/cmd_py_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/loaders/cmd_xml_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/loaders/dict_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/loaders/event_py_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/loaders/event_xml_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/loaders/pkt_xml_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/loaders/python_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14921 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/loaders/xml_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.634909 fprime_gds-3.3.0a1/src/fprime_gds/common/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/logger/data_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/logger/test_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.634909 fprime_gds-3.3.0a1/src/fprime_gds/common/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.634909 fprime_gds-3.3.0a1/src/fprime_gds/common/models/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/models/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/models/common/channel_telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/models/common/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/models/common/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.634909 fprime_gds-3.3.0a1/src/fprime_gds/common/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9587 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/parsers/seq_file_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.634909 fprime_gds-3.3.0a1/src/fprime_gds/common/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/pipeline/dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/pipeline/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/pipeline/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/pipeline/histories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/pipeline/router.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8656 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/pipeline/standard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.634909 fprime_gds-3.3.0a1/src/fprime_gds/common/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/templates/ch_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/templates/cmd_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/templates/data_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/templates/event_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/templates/pkt_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.638909 fprime_gds-3.3.0a1/src/fprime_gds/common/testing_fw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/testing_fw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60457 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/testing_fw/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18371 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/testing_fw/predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/testing_fw/pytest_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.638909 fprime_gds-3.3.0a1/src/fprime_gds/common/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/tools/seqgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10565 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.638909 fprime_gds-3.3.0a1/src/fprime_gds/common/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/utils/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/utils/data_desc_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/utils/event_severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/utils/string_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12162 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/common/zmq_transport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.638909 fprime_gds-3.3.0a1/src/fprime_gds/executables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/executables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30110 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/executables/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/executables/comm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12432 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/executables/fprime_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/executables/run_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17555 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/executables/tcpserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/executables/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.638909 fprime_gds-3.3.0a1/src/fprime_gds/flask/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/default_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19778 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/flask_uploads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.638909 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.642909 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/.idea/static.iml
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/.idea/vcs.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.642909 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.642909 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/advanced-settings/
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/advanced-settings/addon-templates.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/advanced-settings/addon.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.642909 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/channel-render/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/channel-render/addon.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/channel-render/channel-render-template.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/channel-render/channel-render.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.642909 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/chart-display/
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/chart-display/addon-templates.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9185 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/chart-display/addon.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/chart-display/config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.642909 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/chart-display/modified-vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)    30243 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/chart-display/modified-vendor/chartjs-plugin-streaming.js
+-rw-r--r--   0 runner    (1001) docker     (123)    29512 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/chart-display/modified-vendor/chartjs-plugin-zoom.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/chart-display/modified-vendor/flat.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/chart-display/sibling.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.642909 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/chart-display/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)   184059 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/chart-display/vendor/chart.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/chart-display/vendor/chartjs-adapter-luxon.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20727 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/chart-display/vendor/hammer.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.642909 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/commanding/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/commanding/addon.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/commanding/argument-templates.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10665 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/commanding/arguments.js
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/commanding/command-history-template.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/commanding/command-history.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/commanding/command-input-template.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/commanding/command-input.js
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/commanding/command-string-template.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/commanding/command-string.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.642909 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/dictionary/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/dictionary/addon-templates.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/dictionary/addon.js
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/enabled.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.642909 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/image-display/
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/image-display/addon.js
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/image-display/dashboard.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.642909 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/sequencer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/sequencer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/sequencer/addon-templates.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/sequencer/addon.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/sequencer/autocomplete.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/sequencer/lint.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.646909 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/sequencer/third/
+-rw-r--r--   0 runner    (1001) docker     (123)   813045 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/sequencer/third/code-mirror.es.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.646909 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/sequencer/third/rollup/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/sequencer/third/rollup/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/sequencer/third/rollup/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/sequencer/third/rollup/language.grammer
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/sequencer/third/rollup/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/sequencer/third/rollup/rollup.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.646909 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   180390 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/css/fprime.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/css/fpstyle.css
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.646909 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/img/
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/img/error.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12470 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/img/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/img/success.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    26087 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.646909 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/js/config.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14515 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/js/datastore.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/js/gds.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15521 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/js/loader.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/js/performance.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/js/settings.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/js/uploader.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12814 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/js/validate.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.650909 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/js/vue-support/
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/js/vue-support/channel.js
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/js/vue-support/dashboard-box.js
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/js/vue-support/dashboard-row.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/js/vue-support/dashboard.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/js/vue-support/downlink.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/js/vue-support/event.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/js/vue-support/fp-row.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18646 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/js/vue-support/fptable.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/js/vue-support/log.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/js/vue-support/tabetc.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/js/vue-support/uplink.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16197 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/js/vue-support/utils.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.622909 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.650909 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    59305 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/css/all.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   161364 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/css/vue-select.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.650909 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    72827 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/js/luxon.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16877 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/js/sorttable.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/js/v-runtime-template.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16999 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/js/vue-select.js
+-rw-r--r--   0 runner    (1001) docker     (123)    93675 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/js/vue.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.654909 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   134294 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/webfonts/fa-brands-400.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   747927 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/webfonts/fa-brands-400.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   133988 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    89988 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/webfonts/fa-brands-400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    76736 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    34034 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/webfonts/fa-regular-400.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   144714 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/webfonts/fa-regular-400.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    33736 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    16276 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/webfonts/fa-regular-400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13224 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   203030 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   918991 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   202744 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   101648 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    78268 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/flask/updown.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/src/fprime_gds/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.626909 fprime_gds-3.3.0a1/src/fprime_gds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-08-01 20:46:04.000000 fprime_gds-3.3.0a1/src/fprime_gds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12873 2023-08-01 20:46:04.000000 fprime_gds-3.3.0a1/src/fprime_gds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:46:04.000000 fprime_gds-3.3.0a1/src/fprime_gds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-08-01 20:46:04.000000 fprime_gds-3.3.0a1/src/fprime_gds.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:45:44.000000 fprime_gds-3.3.0a1/src/fprime_gds.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-08-01 20:46:04.000000 fprime_gds-3.3.0a1/src/fprime_gds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-01 20:46:04.000000 fprime_gds-3.3.0a1/src/fprime_gds.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.622909 fprime_gds-3.3.0a1/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.622909 fprime_gds-3.3.0a1/test/fprime_gds/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.622909 fprime_gds-3.3.0a1/test/fprime_gds/common/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.654909 fprime_gds-3.3.0a1/test/fprime_gds/common/distributor/
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/test/fprime_gds/common/distributor/test_distributor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.654909 fprime_gds-3.3.0a1/test/fprime_gds/common/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/test/fprime_gds/common/encoders/test_ch_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/test/fprime_gds/common/encoders/test_event_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/test/fprime_gds/common/encoders/test_pkt_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.654909 fprime_gds-3.3.0a1/test/fprime_gds/common/gds_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/test/fprime_gds/common/gds_cli/filtering_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/test/fprime_gds/common/gds_cli/utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.654909 fprime_gds-3.3.0a1/test/fprime_gds/common/history/
+-rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/test/fprime_gds/common/history/chronohistory_unit_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/test/fprime_gds/common/history/testhistory_unit_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.654909 fprime_gds-3.3.0a1/test/fprime_gds/common/testing_fw/
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/test/fprime_gds/common/testing_fw/UnitTestDictionary.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    39899 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/test/fprime_gds/common/testing_fw/api_unit_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.654909 fprime_gds-3.3.0a1/test/fprime_gds/common/testing_fw/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/test/fprime_gds/common/testing_fw/logs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/test/fprime_gds/common/testing_fw/predicate_unit_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.654909 fprime_gds-3.3.0a1/test/fprime_gds/common/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/test/fprime_gds/common/tools/seqgen_unit_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.654909 fprime_gds-3.3.0a1/test/fprime_gds/common/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/test/fprime_gds/common/utils/test_string_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.654909 fprime_gds-3.3.0a1/test/fprime_gds/executables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/test/fprime_gds/executables/test_run_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/test/fprime_gds/executables/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:46:04.654909 fprime_gds-3.3.0a1/test/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-08-01 20:45:37.000000 fprime_gds-3.3.0a1/test/gui/GUI_Test_Procedure.md
```

### Comparing `fprime_gds-3.2.1a2/.github/actions/spelling/expect.txt` & `fprime_gds-3.3.0a1/.github/actions/spelling/expect.txt`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/.github/actions/spelling/patterns.txt` & `fprime_gds-3.3.0a1/.github/actions/spelling/patterns.txt`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/.github/pull_request_template.md` & `fprime_gds-3.3.0a1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/.github/resources/RefTopologyAppDictionary.xml` & `fprime_gds-3.3.0a1/.github/resources/RefTopologyAppDictionary.xml`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/.github/workflows/codeql-security-scan.yml` & `fprime_gds-3.3.0a1/.github/workflows/codeql-security-scan.yml`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/.github/workflows/fprime-gds-tests.yml` & `fprime_gds-3.3.0a1/.github/workflows/fprime-gds-tests.yml`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/.github/workflows/gds-cli-tests.yml` & `fprime_gds-3.3.0a1/.github/workflows/gds-cli-tests.yml`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/.github/workflows/publish.yml` & `fprime_gds-3.3.0a1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/.github/workflows/spelling.yml` & `fprime_gds-3.3.0a1/.github/workflows/spelling.yml`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/.gitignore` & `fprime_gds-3.3.0a1/.gitignore`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/Doxyfile` & `fprime_gds-3.3.0a1/Doxyfile`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/LICENSE.txt` & `fprime_gds-3.3.0a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/NOTICE.txt` & `fprime_gds-3.3.0a1/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/PKG-INFO` & `fprime_gds-3.3.0a1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fprime_gds
-Version: 3.2.1a2
+Version: 3.3.0a1
 Summary: F Prime Flight Software Ground Data System layer.
 Home-page: https://github.com/nasa/fprime
 Author: Michael Starch
 Author-email: Michael.D.Starch@jpl.nasa.gov
 License: Apache 2.0 License
 Project-URL: Issue Tracker, https://github.com/nasa/fprime/issues
 Keywords: fprime,gds,embedded,nasa
```

### Comparing `fprime_gds-3.2.1a2/README.md` & `fprime_gds-3.3.0a1/README.md`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/docs/README.md` & `fprime_gds-3.3.0a1/docs/README.md`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/docs/_static/css/rtd_width.css` & `fprime_gds-3.3.0a1/docs/_static/css/rtd_width.css`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/docs/conf.py` & `fprime_gds-3.3.0a1/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import re
 from datetime import datetime
 from importlib import import_module
 from pathlib import Path
 
 import sphinx_rtd_theme  # pylint: disable=unused-import
 
-
 # importlib.metadata is implemented in Python 3.8
 # Previous versions require the backport, https://pypi.org/project/importlib-metadata/
 try:
     metadata = import_module("importlib.metadata")
 except ModuleNotFoundError:
     metadata = import_module("importlib_metadata")
```

### Comparing `fprime_gds-3.2.1a2/docs/index.rst` & `fprime_gds-3.3.0a1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/examples/simple_sequence.seq` & `fprime_gds-3.3.0a1/examples/simple_sequence.seq`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/setup.py` & `fprime_gds-3.3.0a1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 # ```
 # pip install -e ./Gds
 # ```
 ###
 
 from setuptools import find_packages, setup
 
-
 ####
 # GDS Packages:
 #
 # The GDS package 'tkgui' is only allowed as part of a Python 2 distribution. This code
 # excludes the 'fprime_gds.tkgui' package.
 ####
 gds_packages = find_packages("src", exclude=["*tkgui*"])
@@ -105,15 +104,15 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
     ],
     python_requires=">=3.7",
     setup_requires=["setuptools_scm"],
     install_requires=[
-        "flask>=1.1.2",
+        "flask>=1.1.2,<=2.2.3",
         "flask_compress>=1.11",
         "pyzmq>=24.0.1",
         "pexpect>=4.8.0",
         "pytest>=6.2.4",
         "flask_restful>=0.3.8",
         "fprime-tools>=3.1.2a1",
         "argcomplete>=1.12.3",
```

### Comparing `fprime_gds-3.2.1a2/src/fastentrypoints.py` & `fprime_gds-3.3.0a1/src/fastentrypoints.py`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/communication/adapters/base.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/communication/adapters/base.py`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/communication/adapters/ip.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/communication/adapters/ip.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 
 Module containing a comm-layer adapter for the Tcp/UDP/IP stack. This pairs with the F prime component "SocketIpDriver"
 in order to read data being sent via Tcp or Udp. This is the default adapter used by the system to handle data sent
 across a Tcp and/or UDP network interface.
 
 @author lestarch
 """
-import atexit
 import abc
+import atexit
 import logging
 import queue
 import socket
 import threading
 import time
 
-import fprime_gds.common.logger
 import fprime_gds.common.communication.adapters.base
+import fprime_gds.common.logger
 
 LOGGER = logging.getLogger("ip_adapter")
 
 
 def check_port(address, port):
     """
     Checks a given address and port to ensure that it is available. If not available, a ValueError is raised. Note: this
@@ -30,15 +30,16 @@
     :param port: port to bind to
     """
     socket_trial = None
     try:
         socket_trial = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         socket_trial.bind((address, port))
     except OSError as err:
-        raise OSError(f"Error with address/port of '{address}:{port}' : {err}")
+        msg = f"Error with address/port of '{address}:{port}' : {err}"
+        raise OSError(msg)
     finally:
         if socket_trial is not None:
             socket_trial.close()
 
 
 class IpAdapter(fprime_gds.common.communication.adapters.base.BaseAdapter):
     """
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/communication/adapters/uart.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/communication/adapters/uart.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,19 +6,18 @@
 drivers.
 
 @author lestarch
 """
 
 import logging
 
-import fprime_gds.common.communication.adapters.base
-
 import serial
 from serial.tools import list_ports
 
+import fprime_gds.common.communication.adapters.base
 
 LOGGER = logging.getLogger("serial_adapter")
 
 
 class SerialAdapter(fprime_gds.common.communication.adapters.base.BaseAdapter):
     """
     Supplies a data source adapter that is pulling data off from a UART wire using PySerial. This is setup using a
@@ -168,21 +167,24 @@
         Code that should check arguments of this adapter. If there is a problem with this code, then a "ValueError"
         should be raised describing the problem with these arguments.
 
         :param args: arguments as dictionary
         """
         ports = map(lambda info: info.device, list_ports.comports(include_links=True))
         if args["device"] not in ports:
+            msg = f"Serial port '{args['device']}' not valid. Available ports: {ports}"
             raise ValueError(
-                f"Serial port '{args['device']}' not valid. Available ports: {ports}"
+                msg
             )
         # Note: baud rate may not *always* work. These are a superset
         try:
             baud = int(args["baud"])
         except ValueError:
+            msg = f"Serial baud rate '{args['baud']}' not integer. Use one of: {SerialAdapter.BAUDS}"
             raise ValueError(
-                f"""Serial baud rate '{args["baud"]}' not integer. Use one of: {SerialAdapter.BAUDS}"""
+                msg
             )
         if baud not in SerialAdapter.BAUDS:
+            msg = f"Serial baud rate '{baud}' not supported. Use one of: {SerialAdapter.BAUDS}"
             raise ValueError(
-                f"Serial baud rate '{baud}' not supported. Use one of: {SerialAdapter.BAUDS}"
+                msg
             )
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/communication/checksum.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/communication/checksum.py`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/communication/framing.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/communication/framing.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 
 1. FpFramerDeframer: a class used to write the now-standard F prime ground packet format
 2. TcpServerFramerDeframer: a non-symmetric framer/deframer for use interacting with the Tcp Server packet format
 
 @author lestarch
 """
 import abc
-import sys
 import copy
 import struct
+import sys
+
 from .checksum import calculate_checksum
 
 
 class FramerDeframer(abc.ABC):
     """
     Abstract base class of the Framer/Deframer variety. Framers and Deframers have to define two methods, one for
     framing a set of bytes and one for deframing a set of bytes into packets.
@@ -111,15 +112,16 @@
         elif FpFramerDeframer.TOKEN_SIZE == 2:
             FpFramerDeframer.TOKEN_TYPE = "H"
             FpFramerDeframer.START_TOKEN = 0xBEEF
         elif FpFramerDeframer.TOKEN_SIZE == 1:
             FpFramerDeframer.TOKEN_TYPE = "B"
             FpFramerDeframer.START_TOKEN = 0xEF
         else:
-            raise ValueError(f"Invalid TOKEN_SIZE of {FpFramerDeframer.TOKEN_SIZE}")
+            msg = f"Invalid TOKEN_SIZE of {FpFramerDeframer.TOKEN_SIZE}"
+            raise ValueError(msg)
         FpFramerDeframer.HEADER_FORMAT = ">" + (FpFramerDeframer.TOKEN_TYPE * 2)
 
     def frame(self, data):
         """
         Frames outgoing data in the F prime standard format. Expects incoming raw bytes to frame, and adds on the
         needed framing tokens to the front and end of the bytes.
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/communication/ground.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/communication/ground.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 
 @author lestarch
 """
 
 import abc
 import logging
 
-from .framing import TcpServerFramerDeframer
 from fprime_gds.common.communication.adapters.ip import TcpHandler
 
+from .framing import TcpServerFramerDeframer
+
 LOGGER = logging.getLogger("gds_sender")
 
 
 class GroundHandler(abc.ABC):
     """
     Ground handler class interacts upstream from the comm adapter layer to the greater ground system. This
     effectively means handling the following functions:
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/communication/updown.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/communication/updown.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 side where they are and passed into the ground side handler and onto the other GDS processes. Downlink handles multiple
 streams of data the FSW downlink, and loopback data from the uplink adapter.
 
 Uplink is the reverse, it pulls data in from the ground handler, frames it, and sends it up to the waiting FSW. Uplink
 is represented by a single thread, as it is not dealing with multiple streams of data that need to be multiplexed.
 
 """
-import threading
-from queue import Queue, Full, Empty
 import logging
+import threading
+from queue import Empty, Full, Queue
 
 from fprime.common.models.serialize.numerical_types import U32Type
-from fprime_gds.common.utils.data_desc_type import DataDescType
+
 from fprime_gds.common.communication.adapters.base import BaseAdapter
-from fprime_gds.common.communication.ground import GroundHandler
 from fprime_gds.common.communication.framing import FramerDeframer
-
+from fprime_gds.common.communication.ground import GroundHandler
+from fprime_gds.common.utils.data_desc_type import DataDescType
 
 DW_LOGGER = logging.getLogger("downlink")
 UP_LOGGER = logging.getLogger("uplink")
 
 
 class Downlinker:
     """Encapsulates communication downlink functions
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/data_types/ch_data.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/data_types/ch_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 @date Created July 2, 2018
 @author R. Joseph Paetz
 
 @bug No known bugs
 """
 
 from fprime.common.models.serialize import time_type
+from fprime.common.models.serialize.array_type import ArrayType
+from fprime.common.models.serialize.serializable_type import SerializableType
+
 from fprime_gds.common.data_types import sys_data
 from fprime_gds.common.utils.string_util import format_string_template
-from fprime.common.models.serialize.serializable_type import SerializableType
-from fprime.common.models.serialize.array_type import ArrayType
 
 
 class ChData(sys_data.SysData):
     """
     The ChData class stores a specific channel telemetry reading.
     """
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/data_types/cmd_data.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/data_types/cmd_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,32 +6,34 @@
 
 @data Created July 3, 2018
 @author Josef Biberstein
 
 @bug No known bugs
 """
 import json
+
 from fprime.common.models.serialize.array_type import ArrayType
 from fprime.common.models.serialize.bool_type import BoolType
 from fprime.common.models.serialize.enum_type import EnumType
 from fprime.common.models.serialize.numerical_types import (
+    F32Type,
+    F64Type,
     I8Type,
     I16Type,
     I32Type,
     I64Type,
     U8Type,
     U16Type,
     U32Type,
     U64Type,
-    F32Type,
-    F64Type,
 )
 from fprime.common.models.serialize.serializable_type import SerializableType
 from fprime.common.models.serialize.string_type import StringType
 from fprime.common.models.serialize.time_type import TimeBase, TimeType
+
 from fprime_gds.common.data_types import sys_data
 
 
 class CmdData(sys_data.SysData):
     """The CmdData class stores a specific command"""
 
     def __init__(self, cmd_args, cmd_temp, cmd_desc=None, cmd_time=None):
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/data_types/event_data.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/data_types/event_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 @date Created July 2, 2018
 @author R. Joseph Paetz
 
 @bug No known bugs
 """
 
 from fprime.common.models.serialize import time_type
+
 from fprime_gds.common.data_types import sys_data
 from fprime_gds.common.utils.string_util import format_string_template
 
 
 class EventData(sys_data.SysData):
     """
     The EventData class stores a specific event message.
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/data_types/exceptions.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/data_types/exceptions.py`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/data_types/file_data.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/data_types/file_data.py`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/data_types/pkt_data.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/data_types/pkt_data.py`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/data_types/sys_data.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/data_types/sys_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 @date Created July 2, 2018
 @author R. Joseph Paetz (rpaetz@jpl.nasa.gov)
 
 @bug No known bugs
 """
 from fprime.common.models.serialize import time_type
+
 from fprime_gds.common.templates import data_template
 
 
 class SysData:
     """
     The SysData class defines the interface for system data classes which are
     for specific data readings/events
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/decoders/ch_decoder.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/decoders/ch_decoder.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 @date Created July 11, 2018
 @author R. Joseph Paetz
 
 @bug No known bugs
 """
 from fprime.common.models.serialize.time_type import TimeType
+
 from fprime_gds.common.data_types.ch_data import ChData
 from fprime_gds.common.decoders.decoder import Decoder, DecodingException
 from fprime_gds.common.utils import config_manager
 
 
 class ChDecoder(Decoder):
     """Decoder class for Channel data"""
@@ -73,22 +74,24 @@
 
             # Decode time...
             ch_time = TimeType()
             ch_time.deserialize(data, ptr)
             ptr += ch_time.getSize()
 
             if ch_id not in self.__dict:
-                raise DecodingException(f"Channel {ch_id} not found in dictionary")
+                msg = f"Channel {ch_id} not found in dictionary"
+                raise DecodingException(msg)
             # Retrieve the template instance for this channel
             ch_temp = self.__dict[ch_id]
 
             try:
                 val_obj = self.decode_ch_val(data, ptr, ch_temp)
             except Exception as exc:
-                raise DecodingException(f"Channel {ch_temp.name} failed to decode: {exc}")
+                msg = f"Channel {ch_temp.name} failed to decode: {exc}"
+                raise DecodingException(msg)
             ch_list.append(ChData(val_obj, ch_time, ch_temp))
             ptr += val_obj.getSize()
         return ch_list
 
     @staticmethod
     def decode_ch_val(val_data, offset, template):
         """
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/decoders/decoder.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/decoders/decoder.py`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/decoders/event_decoder.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/decoders/event_decoder.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 @date Created June 29, 2018
 @author R. Joseph Paetz
 
 @bug No known bugs
 """
 from fprime.common.models.serialize import time_type
 from fprime.common.models.serialize.type_exceptions import TypeException
+
 from fprime_gds.common.data_types import event_data
 from fprime_gds.common.decoders import decoder
 from fprime_gds.common.utils import config_manager
 
 
 class EventDecoder(decoder.Decoder):
     """Decoder class for event data"""
@@ -71,15 +72,16 @@
 
             # Decode time...
             event_time = time_type.TimeType()
             event_time.deserialize(data, ptr)
             ptr += event_time.getSize()
 
             if event_id not in self.__dict:
-                raise DecodingException(f"Event {event_id} not found in dictionary")
+                msg = f"Event {event_id} not found in dictionary"
+                raise DecodingException(msg)
 
             event_temp = self.__dict[event_id]
 
             (size, arg_vals) = self.decode_args(data, ptr, event_temp)
 
             event_list.append(event_data.EventData(arg_vals, event_time, event_temp))
             # add up argument sizes
@@ -115,12 +117,13 @@
 
             arg_obj = arg_type()
 
             try:
                 arg_obj.deserialize(arg_data, offset)
                 arg_results.append(arg_obj)
             except TypeException as e:
-                raise DecodingException(f"Event argument decoding failed {e.getMsg()}")
+                msg = f"Event argument decoding failed {e.getMsg()}"
+                raise DecodingException(msg)
 
             offset = offset + arg_obj.getSize()
 
         return [offset, tuple(arg_results)]
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/decoders/file_decoder.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/decoders/file_decoder.py`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/decoders/pkt_decoder.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/decoders/pkt_decoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 @date Created July 12, 2018
 @author R. Joseph Paetz
 
 @bug No known bugs
 """
 
 from fprime.common.models.serialize.time_type import TimeType
+
 from fprime_gds.common.data_types.ch_data import ChData
 from fprime_gds.common.decoders.ch_decoder import ChDecoder
 from fprime_gds.common.utils import config_manager
 
 
 class PktDecoder(ChDecoder):
     """Decoder class for Packetized Telemetry data"""
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/distributor/distributor.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/distributor/distributor.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 
 @author Josef Biberstein
 @author Joseph Paetz
 
 @bug No known bugs
 """
 import logging
-from fprime_gds.common.utils import config_manager, data_desc_type
-from fprime_gds.common.handlers import DataHandler
-from fprime_gds.common.decoders.decoder import DecodingException
 
+from fprime_gds.common.decoders.decoder import DecodingException
+from fprime_gds.common.handlers import DataHandler
+from fprime_gds.common.utils import config_manager, data_desc_type
 
 LOGGER = logging.getLogger("distributor")
 
 
 # NOTE decoder function to call is called data_callback(data)
 class Distributor(DataHandler):
     """
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/encoders/ch_encoder.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/encoders/ch_encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,18 +28,19 @@
 
 @date Created August 9, 2018
 @author R. Joseph Paetz
 
 @bug No known bugs
 """
 
-from .encoder import Encoder
 from fprime_gds.common.data_types.ch_data import ChData
 from fprime_gds.common.utils.data_desc_type import DataDescType
 
+from .encoder import Encoder
+
 
 class ChEncoder(Encoder):
     """Encoder class for channel data"""
 
     def __init__(self, config=None):
         """
         Constructor
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/encoders/cmd_encoder.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/encoders/cmd_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,19 +38,21 @@
 @date Created July 9, 2018
 @author R. Joseph Paetz
 
 @bug No known bugs
 """
 
 
-from . import encoder
 from fprime.common.models.serialize.numerical_types import U32Type
+
 from fprime_gds.common.data_types.cmd_data import CmdData
-from fprime_gds.common.utils.data_desc_type import DataDescType
 from fprime_gds.common.utils import config_manager
+from fprime_gds.common.utils.data_desc_type import DataDescType
+
+from . import encoder
 
 
 class CmdEncoder(encoder.Encoder):
     """Encoder class for command data"""
 
     def __init__(self, config=None):
         """
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/encoders/encoder.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/encoders/encoder.py`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/encoders/event_encoder.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/encoders/event_encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,18 +33,19 @@
 
 @date Created August 9, 2018
 @author R. Joseph Paetz
 
 @bug No known bugs
 """
 
-from .encoder import Encoder
 from fprime_gds.common.data_types.event_data import EventData
 from fprime_gds.common.utils.data_desc_type import DataDescType
 
+from .encoder import Encoder
+
 
 class EventEncoder(Encoder):
     """Encoder class for event data"""
 
     def __init__(self, config=None):
         """
         Constructor
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/encoders/file_encoder.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/encoders/file_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 @bug No known bugs
 """
 
 import struct
 
 from fprime.common.models.serialize.numerical_types import U32Type
 from fprime.constants import DATA_ENCODING
+
 from fprime_gds.common.data_types.file_data import FilePacketType
 from fprime_gds.common.utils.data_desc_type import DataDescType
 
 from . import encoder
 
 
 class FileEncoder(encoder.Encoder):
@@ -86,13 +87,14 @@
             out_data += file_dst_enc
         elif data.packetType == FilePacketType.DATA:
             out_data += struct.pack(">IH", data.offset, data.length)
             out_data += data.dataVar
         elif data.packetType == FilePacketType.END:
             out_data += struct.pack(">I", data.hashValue)
         elif data.packetType != FilePacketType.CANCEL:
-            raise Exception(f"Invalid packet type found while encoding: {data.packetType}")
+            msg = f"Invalid packet type found while encoding: {data.packetType}"
+            raise Exception(msg)
         descriptor = U32Type(DataDescType["FW_PACKET_FILE"].value).serialize()
         length_obj = self.config.get_type("msg_len")
         length_obj.val = len(descriptor) + len(out_data)
         header = U32Type(0x5A5A5A5A).serialize() + length_obj.serialize() + descriptor
         return header + out_data
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/encoders/pkt_encoder.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/encoders/pkt_encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,18 +33,19 @@
 
 @date Created August 9, 2018
 @author R. Joseph Paetz
 
 @bug No known bugs
 """
 
-from .encoder import Encoder
 from fprime_gds.common.data_types.pkt_data import PktData
 from fprime_gds.common.utils.data_desc_type import DataDescType
 
+from .encoder import Encoder
+
 
 class PktEncoder(Encoder):
     """Encoder class for packet data"""
 
     def __init__(self, config=None):
         """
         Constructor
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/encoders/seq_writer.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/encoders/seq_writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 
 @author: tcanham
 """
 
 import struct
 import zlib
 
-from fprime.common.models.serialize.type_exceptions import TypeMismatchException
 from fprime.common.models.serialize.numerical_types import U8Type, U16Type, U32Type
+from fprime.common.models.serialize.type_exceptions import TypeMismatchException
+
 from fprime_gds.common.utils import config_manager
 from fprime_gds.common.utils.data_desc_type import DataDescType
 
 
 class SeqBinaryWriter:
     """
     Write out the Binary (ASTERIA) form of sequencer file.
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/files/File Decoder Documentation.txt` & `fprime_gds-3.3.0a1/src/fprime_gds/common/files/File Decoder Documentation.txt`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/files/downlinker.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/files/downlinker.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 @bug No known bugs
 """
 
 import logging
 import os
 
 import fprime.constants
+
 import fprime_gds.common.handlers
 from fprime_gds.common.data_types.file_data import FilePacketType
 from fprime_gds.common.files.helpers import (
     FileStates,
     TransmitFile,
     TransmitFileState,
     file_to_dict,
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/files/helpers.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/files/helpers.py`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/files/uplinker.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/files/uplinker.py`

 * *Files 0% similar despite different names*

```diff
@@ -223,16 +223,17 @@
 
         :param file_obj: file object to upload
         :raises FileUplinkerBusyException: when an upload is already running
         :raises OSError: when file is inaccessible
         """
         # Prevent multiple uplinks at once
         if self.state != FileStates.IDLE:
+            msg = f"Currently uplinking file '{self.active.source}' cannot start uplinking '{file_obj.source}'"
             raise FileUplinkerBusyException(
-                f"Currently uplinking file '{self.active.source}' cannot start uplinking '{file_obj.source}'"
+                msg
             )
         self.state = FileStates.RUNNING
         self.active = file_obj
         self.active.open(TransmitFileState.READ)
         self.send(
             StartPacketData(
                 self.get_next_sequence(),
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/gds_cli/base_commands.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/gds_cli/base_commands.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 A collection of base classes used for the backend implementations of the GDS
 CLI commands
 """
 
 import abc
-import sys
 import json
+import sys
 from typing import Iterable
 
 import fprime_gds.common.gds_cli.filtering_utils as filtering_utils
 import fprime_gds.common.gds_cli.test_api_utils as test_api_utils
 from fprime_gds.common.pipeline.dictionaries import Dictionaries
 from fprime_gds.common.testing_fw import predicates
 from fprime_gds.common.testing_fw.api import IntegrationTestAPI
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/gds_cli/channels.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/gds_cli/channels.py`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/gds_cli/command_send.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/gds_cli/command_send.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
 Handles executing the "command-send" CLI command for the GDS
 """
 
 import difflib
 from typing import Iterable, List
 
-import fprime_gds.common.gds_cli.test_api_utils as test_api_utils
 from fprime.common.models.serialize.type_exceptions import NotInitializedException
+
+import fprime_gds.common.gds_cli.test_api_utils as test_api_utils
 from fprime_gds.common.gds_cli.base_commands import BaseCommand
 from fprime_gds.common.pipeline.dictionaries import Dictionaries
 from fprime_gds.common.templates.cmd_template import CmdTemplate
 from fprime_gds.common.testing_fw import predicates
 from fprime_gds.common.testing_fw.api import IntegrationTestAPI
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/gds_cli/events.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/gds_cli/events.py`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/gds_cli/filtering_utils.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/gds_cli/filtering_utils.py`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/gds_cli/test_api_utils.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/gds_cli/test_api_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """
 A file containing utilities for interacting with the Integration Test API
 """
 
 import types
-from typing import Any, Dict, List
+from typing import Any, Callable, Dict, List
 
 from fprime_gds.common.data_types.ch_data import ChData
 from fprime_gds.common.data_types.event_data import EventData
 from fprime_gds.common.data_types.sys_data import SysData
 from fprime_gds.common.templates.data_template import DataTemplate
 from fprime_gds.common.testing_fw import predicates
 from fprime_gds.common.testing_fw.api import IntegrationTestAPI
-from typing import Callable
 
 
 def get_upcoming_event(
     test_api: IntegrationTestAPI,
     search_filter: predicates.predicate,
     start_time="NOW",
     timeout: float = 5,
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/handlers.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/handlers.py`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/history/chrono.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/history/chrono.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 A chronologically-ordered history that relies on predicates to provide filtering, searching, and
 retrieval operations. This history will re-order itself based on FSW time.
 
 :author: koran
 """
 from fprime.common.models.serialize.time_type import TimeType
+
 from fprime_gds.common.history.history import History
 from fprime_gds.common.testing_fw import predicates
 
 
 class ChronologicalHistory(History):
     """
     A chronological history to support the GDS test api. This history adds support for specifying
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/history/history.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/history/history.py`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/history/ram.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/history/ram.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 robust nor persistent. Given that it is in the RAM, it is driven from the decoders object, which should run off the
 middle-ware layer.
 
 Note: this RAM history treats "start times" as session tokens to remember where it was last fetched from.
 
 :author: lestarch
 """
-import time
 import threading
+import time
 
 from fprime_gds.common.history.history import History
 
 
 class RamHistory(History):
     """
     Chronological variant of history.  This is intended to be registered with the decoders in order
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/history/test.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/history/test.py`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/loaders/ch_py_loader.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/loaders/ch_py_loader.py`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/loaders/ch_xml_loader.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/loaders/ch_xml_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,16 +50,17 @@
         """
         xml_tree = self.get_xml_tree(path)
         versions = xml_tree.attrib.get("framework_version", "unknown"), xml_tree.attrib.get("project_version", "unknown")
 
         # Check if xml dict has channels section
         ch_section = self.get_xml_section(self.CH_SECT, xml_tree)
         if ch_section is None:
+            msg = f"Xml dict did not have a {self.CH_SECT} section"
             raise exceptions.GseControllerParsingException(
-                f"Xml dict did not have a {self.CH_SECT} section"
+                msg
             )
 
         id_dict = {}
         name_dict = {}
         for ch in ch_section:
             ch_dict = ch.attrib
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/loaders/cmd_py_loader.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/loaders/cmd_py_loader.py`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/loaders/cmd_xml_loader.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/loaders/cmd_xml_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,16 +42,17 @@
         """
         xml_tree = self.get_xml_tree(path)
         versions = xml_tree.attrib.get("framework_version", "unknown"), xml_tree.attrib.get("project_version", "unknown")
 
         # Check if xml dict has commands section
         cmd_section = self.get_xml_section(self.CMD_SECT, xml_tree)
         if cmd_section is None:
+            msg = f"Xml dict did not have a {self.EVENT_SECT} section"
             raise exceptions.GseControllerParsingException(
-                f"Xml dict did not have a {self.EVENT_SECT} section"
+                msg
             )
 
         id_dict = {}
         name_dict = {}
 
         for cmd in cmd_section:
             cmd_dict = cmd.attrib
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/loaders/dict_loader.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/loaders/dict_loader.py`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/loaders/event_py_loader.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/loaders/event_py_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 @date Created July 3, 2018
 @author R. Joseph Paetz
 
 @bug No known bugs
 """
 
 from fprime.common.models.serialize.type_exceptions import TypeMismatchException
+
 from fprime_gds.common.templates import event_template
 from fprime_gds.common.utils.event_severity import EventSeverity
 
 # Custom Python Modules
 from . import python_loader
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/loaders/event_xml_loader.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/loaders/event_xml_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,16 +44,17 @@
         """
         xml_tree = self.get_xml_tree(path)
         versions = xml_tree.attrib.get("framework_version", "unknown"), xml_tree.attrib.get("project_version", "unknown")
 
         # Check if xml dict has events section
         event_section = self.get_xml_section(self.EVENT_SECT, xml_tree)
         if event_section is None:
+            msg = f"Xml dict did not have a {self.EVENT_SECT} section"
             raise exceptions.GseControllerParsingException(
-                f"Xml dict did not have a {self.EVENT_SECT} section"
+                msg
             )
 
         id_dict = {}
         name_dict = {}
 
         for event in event_section:
             event_dict = event.attrib
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/loaders/pkt_xml_loader.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/loaders/pkt_xml_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,16 +89,17 @@
         Returns:
             A tuple with two packet dictionaries (type==dict()):
             (id_dict, name_dict). The keys should be the packets' id and name
             fields respectively and the values should be PktTemplate objects.
         """
         packet_list = self.get_xml_tree(path)
         if packet_list.tag != self.PKT_LIST_TAG:
+            msg = f"expected packet list to have tag {self.PKT_LIST_TAG}, but found {packet_list.tag}"
             raise exceptions.GseControllerParsingException(
-                f"expected packet list to have tag {self.PKT_LIST_TAG}, but found {packet_list.tag}"
+                msg
             )
 
         id_dict = {}
         name_dict = {}
 
         for packet in packet_list:
             # check if this is actually a packet, and not something to ignore
@@ -109,16 +110,17 @@
             pkt_id = int(packet.attrib[self.ID_FIELD])
 
             ch_list = []
             for ch in packet:
                 ch_name = ch.attrib[self.CH_NAME_FIELD]
 
                 if ch_name not in ch_name_dict:
+                    msg = f"Channel {ch_name} in pkt {pkt_name}, but cannot be found in channel dictionary"
                     raise exceptions.GseControllerParsingException(
-                        f"Channel {ch_name} in pkt {pkt_name}, but cannot be found in channel dictionary"
+                        msg
                     )
 
                 ch_list.append(ch_name_dict[ch_name])
 
             pkt_temp = PktTemplate(pkt_id, pkt_name, ch_list)
 
             id_dict[pkt_id] = pkt_temp
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/loaders/python_loader.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/loaders/python_loader.py`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/loaders/xml_loader.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/loaders/xml_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,37 +10,38 @@
 
 @date Created July 19, 2018
 @author R. Joseph Paetz
 
 @bug No known bugs
 """
 import os
-from lxml import etree
 
 from fprime.common.models.serialize.array_type import ArrayType
 from fprime.common.models.serialize.bool_type import BoolType
 from fprime.common.models.serialize.enum_type import EnumType
 from fprime.common.models.serialize.numerical_types import (
+    F32Type,
+    F64Type,
     I8Type,
     I16Type,
     I32Type,
     I64Type,
     U8Type,
     U16Type,
     U32Type,
     U64Type,
-    F32Type,
-    F64Type,
 )
 from fprime.common.models.serialize.serializable_type import SerializableType
 from fprime.common.models.serialize.string_type import StringType
+from lxml import etree
+
 from fprime_gds.common.data_types import exceptions
 from fprime_gds.version import (
-    MINIMUM_SUPPORTED_FRAMEWORK_VERSION,
     MAXIMUM_SUPPORTED_FRAMEWORK_VERSION,
+    MINIMUM_SUPPORTED_FRAMEWORK_VERSION,
 )
 
 # Custom Python Modules
 from . import dict_loader
 
 
 class XmlLoader(dict_loader.DictLoader):
@@ -392,16 +393,17 @@
 
         # Now try arrays:
         result = self.get_array_type(type_name, xml_tree)
         if result is not None:
             return result
 
         # Abandon all hope
+        msg = f"Could not find type {type_name}"
         raise exceptions.GseControllerParsingException(
-            f"Could not find type {type_name}"
+            msg
         )
 
 
 class UnsupportedDictionaryVersionException(Exception):
     """Dictionary is of unsupported version"""
 
     def __init__(self, version):
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/logger/__init__.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/logger/data_logger.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/logger/data_logger.py`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/logger/test_logger.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/logger/test_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 import os
 import threading
 import time
 
 # If openpyxl isn't installed, ignore all functionality in this module
 try:
     from openpyxl import Workbook
-    from openpyxl.styles import PatternFill, Font, Alignment
     from openpyxl.cell import WriteOnlyCell
+    from openpyxl.styles import Alignment, Font, PatternFill
     from openpyxl.utils.exceptions import WorkbookAlreadySaved
 
     MODULE_INSTALLED = True
 except ImportError:
     MODULE_INSTALLED = False
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/models/common/channel_telemetry.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/models/common/channel_telemetry.py`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/models/common/command.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/models/common/command.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 
 @author: tcanham
 """
 
 import copy
 from enum import Enum
 
+from fprime.common.models.serialize.numerical_types import U32Type
 from fprime.common.models.serialize.type_base import BaseType
 
 # Import the types this way so they do not need prefixing for execution.
 from fprime.common.models.serialize.type_exceptions import (
     ArgLengthMismatchException,
     ArgNotFoundException,
     TypeMismatchException,
 )
-from fprime.common.models.serialize.numerical_types import U32Type
 
 Descriptor = Enum(value="Descriptor", names="ABSOLUTE RELATIVE")
 
 
 class Command:
     """
     classdocs
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/models/common/event.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/models/common/event.py`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/parsers/seq_file_parser.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/parsers/seq_file_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,16 +167,17 @@
                     print(f"Using timezone {dt.tzinfo.tzname()}")
                     epoch = datetime.fromtimestamp(0, dt.tzinfo)
                 else:
                     print("Using UTC timezone")
                     epoch = datetime.utcfromtimestamp(0)
                 delta = (dt - epoch).total_seconds()
             else:
+                msg = f"Line {lineNumber + 1}: Invalid time descriptor {d} found. Descriptor should either be 'A' for absolute times or 'R' for relative times"
                 raise gseExceptions.GseControllerParsingException(
-                    f"Line {lineNumber + 1}: Invalid time descriptor {d} found. Descriptor should either be 'A' for absolute times or 'R' for relative times"
+                    msg
                 )
             seconds = int(delta)
             useconds = int((delta - seconds) * 1000000)
             return descriptor, seconds, useconds
 
         # Open the sequence file and parse each line:
         with open(filename) as inputFile:
@@ -186,32 +187,35 @@
                     line = line.strip()
                     # ignore blank lines and comments
                     if line and line[0] != ";":
                         line = removeTrailingComments(line)
                         line = splitString(line)
                         length = len(line)
                         if length < 2:
+                            msg = f'Line {i + 1}: Each line must contain a minimum of two fields, time and command mnemonic\n'
                             raise gseExceptions.GseControllerParsingException(
-                                f"Line {i + 1}: Each line must contain a minimum of two fields, time and command mnemonic\n"
+                                msg
                             )
                         try:
                             descriptor, seconds, useconds = parseTime(i, line[0])
                         except Exception:
+                            msg = f'Line {i + 1}: Encountered syntax error parsing timestamp'
                             raise gseExceptions.GseControllerParsingException(
-                                f"Line {i + 1}: Encountered syntax error parsing timestamp"
+                                msg
                             )
                         mnemonic = line[1]
                         args = []
                         if length > 2:
                             args = line[2:]
                             try:
                                 args = parseArgs(args)
                             except Exception:
+                                msg = f'Line {i + 1}: Encountered syntax error parsing arguments'
                                 raise gseExceptions.GseControllerParsingException(
-                                    f"Line {i + 1}: Encountered syntax error parsing arguments"
+                                    msg
                                 )
                         yield i, descriptor, seconds, useconds, mnemonic, args
                 except gseExceptions.GseControllerParsingException as exc:
                     if not cont:
                         raise
                     messages.append(exc.getMsg())
             if cont and messages:
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/pipeline/dictionaries.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/pipeline/dictionaries.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,16 @@
             assert self._versions == command_loader.get_versions(), "Version mismatch while loading"
             # Channels
             channel_loader = fprime_gds.common.loaders.ch_xml_loader.ChXmlLoader()
             self._channel_id_dict = channel_loader.get_id_dict(dictionary)
             self._channel_name_dict = channel_loader.get_name_dict(dictionary)
             assert self._versions == channel_loader.get_versions(), "Version mismatch while loading"
         else:
-            raise Exception(f"[ERROR] Dictionary '{dictionary}' does not exist.")
+            msg = f"[ERROR] Dictionary '{dictionary}' does not exist."
+            raise Exception(msg)
         # Check for packet specification
         if packet_spec is not None:
             packet_loader = fprime_gds.common.loaders.pkt_xml_loader.PktXmlLoader()
             self._packet_dict = packet_loader.get_id_dict(
                 packet_spec, self._channel_name_dict
             )
         else:
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/pipeline/encoding.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/pipeline/encoding.py`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/pipeline/files.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/pipeline/files.py`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/pipeline/histories.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/pipeline/histories.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 Module used to handle the wrangling of histories for the standard pipeline. This allows the standard pipeline, and other
 to compose in this code.
 
 @author mstarch
 """
 from typing import Type
+
 from fprime_gds.common.history.history import History
 from fprime_gds.common.history.ram import RamHistory
 
 
 class Histories:
     """
     Class to handle the individual histories. This handles the following histories:
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/pipeline/router.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/pipeline/router.py`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/pipeline/standard.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/pipeline/standard.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,24 +8,25 @@
 
 :author: lestarch
 """
 import datetime
 import os.path
 from pathlib import Path
 from typing import Type
+
 import fprime.common.models.serialize.time_type
+
 import fprime_gds.common.data_types.cmd_data
 import fprime_gds.common.distributor.distributor
 import fprime_gds.common.logger.data_logger
+from fprime_gds.common.transport import RoutingTag, ThreadedTCPSocketClient
 
 # Local imports for the sake of composition
 from . import dictionaries, encoding, files, histories
 
-from fprime_gds.common.transport import RoutingTag, ThreadedTCPSocketClient
-
 
 class StandardPipeline:
     """
     Class used to encapsulate all of the components of a standard pipeline. The life-cycle of this class follows the
     basic steps:
        1. setup: creates objects needed to read from middle-ware layer and provide data up the stack
        2. register: consumers from this pipeline should register to receive decoder callbacks
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/templates/ch_template.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/templates/ch_template.py`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/templates/cmd_template.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/templates/cmd_template.py`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/templates/data_template.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/templates/data_template.py`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/templates/event_template.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/templates/event_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 @author R. Joseph Paetz
 
 @bug No known bugs
 """
 
 from fprime.common.models.serialize import type_base
 from fprime.common.models.serialize.type_exceptions import TypeMismatchException
+
 from fprime_gds.common.utils.event_severity import EventSeverity
 
 from . import data_template
 
 
 class EventTemplate(data_template.DataTemplate):
     """Class to create event templates to describe specific event types"""
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/templates/pkt_template.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/templates/pkt_template.py`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/testing_fw/api.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/testing_fw/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 :author: koran
 """
 import signal
 import time
 
 from fprime.common.models.serialize.time_type import TimeType
+
 from fprime_gds.common.handlers import DataHandler
 from fprime_gds.common.history.chrono import ChronologicalHistory
 from fprime_gds.common.history.test import TestHistory
 from fprime_gds.common.logger.test_logger import TestLogger
 from fprime_gds.common.testing_fw import predicates
 from fprime_gds.common.utils.event_severity import EventSeverity
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/testing_fw/predicates.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/testing_fw/predicates.py`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/testing_fw/pytest_integration.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/testing_fw/pytest_integration.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 ```
 
 Here a test (defined by starting the name with test_) uses the fprime_test_api fixture to perform the test.
 
 @author lestarch
 """
 import sys
+
 import pytest
 
 from fprime_gds.common.testing_fw.api import IntegrationTestAPI
 from fprime_gds.executables.cli import StandardPipelineParser
 
-
 SEQUENCE_COUNTER = -1
 
 
 def pytest_addoption(parser):
     """ Add fprime-gds options to the pytest parser
 
     Pytest allows users to add options to its parser. These options act very similar to argparse options and thus can be
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/tools/seqgen.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/tools/seqgen.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 # ALL RIGHTS RESERVED. U.S. Government Sponsorship acknowledged.
 # ===============================================================================
 
 import argparse
 import os
 import sys
 
+from fprime.common.models.serialize.time_type import TimeBase, TimeType
+
 from fprime_gds.common.data_types import exceptions as gseExceptions
+from fprime_gds.common.data_types.cmd_data import CmdData, CommandArgumentsException
 from fprime_gds.common.encoders.seq_writer import SeqBinaryWriter
 from fprime_gds.common.loaders.cmd_xml_loader import CmdXmlLoader
 from fprime_gds.common.parsers.seq_file_parser import SeqFileParser
-from fprime_gds.common.data_types.cmd_data import CmdData, CommandArgumentsException
-from fprime.common.models.serialize.time_type import TimeBase, TimeType
-
 
 __author__ = "Tim Canham"
 __version__ = "1.0"
 __email__ = "timothy.canham@jpl.nasa.gov"
 
 
 class SeqGenException(gseExceptions.GseControllerException):
@@ -44,41 +44,45 @@
     Write a binary sequence file from a text sequence file
     @param inputFile: A text input sequence file name (usually a .seq extension)
     @param outputFile: An output binary sequence file name (usually a .bin extension)
     """
 
     # Check for files
     if not os.path.isfile(inputFile):
-        raise SeqGenException(f"Can't open file '{inputFile}'. ")
+        msg = f"Can't open file '{inputFile}'. "
+        raise SeqGenException(msg)
 
     if not os.path.isfile(dictionary):
-        raise SeqGenException(f"Can't open file '{dictionary}'. ")
+        msg = f"Can't open file '{dictionary}'. "
+        raise SeqGenException(msg)
 
     # Check the user environment:
     cmd_xml_dict = CmdXmlLoader()
     try:
         (cmd_id_dict, cmd_name_dict, versions) = cmd_xml_dict.construct_dicts(
             dictionary
         )
     except gseExceptions.GseControllerUndefinedFileException:
-        raise SeqGenException(f"Can't open file '{dictionary}'. ")
+        msg = f"Can't open file '{dictionary}'. "
+        raise SeqGenException(msg)
 
     # Parse the input file:
     command_list = []
     file_parser = SeqFileParser()
 
     parsed_seq = file_parser.parse(inputFile, cont=cont)
 
     messages = []
     try:
         for i, descriptor, seconds, useconds, mnemonic, args in parsed_seq:
             try:
                 if mnemonic not in cmd_name_dict:
+                    msg = f"Line {i + 1}: '{mnemonic}' does not match any command in the command dictionary."
                     raise SeqGenException(
-                        f"Line {i+1}: '{mnemonic}' does not match any command in the command dictionary."
+                        msg
                     )
                 # Set the command arguments:
                 try:
                     cmd_time = TimeType(
                         TimeBase["TB_DONT_CARE"].value,
                         seconds=seconds,
                         useconds=useconds,
@@ -86,16 +90,17 @@
                     cmd_data = CmdData(
                         args,
                         cmd_name_dict[mnemonic],
                         cmd_desc=descriptor,
                         cmd_time=cmd_time,
                     )
                 except CommandArgumentsException as e:
+                    msg = f"Line {i + 1}: {mnemonic} errored: {','.join(e.errors)}"
                     raise SeqGenException(
-                        f"Line { i + 1 }: { mnemonic } errored: { ','.join(e.errors) }"
+                        msg
                     )
                 command_list.append(cmd_data)
             except SeqGenException as exc:
                 if not cont:
                     raise
                 messages.append(exc.getMsg())
     except gseExceptions.GseControllerParsingException as e:
@@ -106,16 +111,17 @@
     # Write to the output file:
     writer = SeqBinaryWriter(timebase=timebase)
     if not outputFile:
         outputFile = f"{os.path.splitext(inputFile)[0]}.bin"
     try:
         writer.open(outputFile)
     except:
+        msg = f"Encountered problem opening output file '{outputFile}'."
         raise SeqGenException(
-            f"Encountered problem opening output file '{outputFile}'."
+            msg
         )
 
     writer.write(command_list)
     writer.close()
 
 
 help_text = "seqgen.py -d"
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/transport.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/transport.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 
 Sets up the classes used to transport data within the GDS system between the few executables that compose the GDS. This
 file defines several base classes used to specify what a client looks like and it defines a basic implementation:
 ThreadedTCPSocketClient used to send data through the threaded tcp server.
 
 @author lestarch
 """
-from abc import abstractmethod, ABC
-from enum import Enum
 import select
 import socket
 import threading
+from abc import ABC, abstractmethod
+from enum import Enum
 
 from fprime_gds.common.handlers import DataHandler, HandlerRegistrar
 
 
 class RoutingTag(Enum):
     """Tag for routing data about the system"""
 
@@ -210,20 +210,22 @@
             host, port = connection_uri.split(":", 1)
             port = int(port)
 
             self.sock.connect((host, port))
             self.sock.send(b"Register %s\n" % incoming_routing.value)
             super().connect(connection_uri, incoming_routing, outgoing_routing)
         except ValueError as vle:
+            msg = f"Failed to parse connection uri: {connection_uri}. {vle}"
             raise TransportationException(
-                f"Failed to parse connection uri: {connection_uri}. {vle}"
+                msg
             )
         except Exception as exc:
+            msg = f"Failed to connect to transportation layer at: {connection_uri}. {exc}"
             raise TransportationException(
-                f"Failed to connect to transportation layer at: {connection_uri}. {exc}"
+                msg
             )
 
     def disconnect(self):
         """Disconnect the socket client"""
         super().disconnect()
         self.sock.close()
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/utils/config_manager.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/utils/config_manager.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 @license Copyright 2018, California Institute of Technology.
          ALL RIGHTS RESERVED. U.S. Government Sponsorship acknowledged.
 """
 import configparser
 
 # Custom type modules
 from fprime.common.models.serialize.numerical_types import (
+    F32Type,
+    F64Type,
     I8Type,
     I16Type,
     I32Type,
     I64Type,
     U8Type,
     U16Type,
     U32Type,
     U64Type,
-    F32Type,
-    F64Type,
 )
 
 
 class ConfigBadTypeException(Exception):
     def __init__(self, config_name, type_str):
         """
         Constructor
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/utils/data_desc_type.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/utils/data_desc_type.py`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/utils/string_util.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/utils/string_util.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 Utility functions to process strings to be used in FPrime GDS
 @Created March 18, 2021
 @`janamian`
 
 Note: This function has an identical copy in fprime-gds
 """
 
-import re
 import logging
+import re
 
 LOGGER = logging.getLogger("string_util_logger")
 
 
 def format_string_template(format_str, given_values):
     r"""
     Function to convert C-string style to python format
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/common/zmq_transport.py` & `fprime_gds-3.3.0a1/src/fprime_gds/common/zmq_transport.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,24 +7,25 @@
 2. ZeroMQ does not require a separate process and may be used w/o tcp sockets
 3. ZeroMQ will not reorder packets at high data rates
 
 @author lestarch
 """
 import logging
 import struct
-import zmq
-
 from typing import Tuple
 
+import zmq
+
 from fprime_gds.common.communication.ground import GroundHandler
 from fprime_gds.common.transport import (
     RoutingTag,
     ThreadedTransportClient,
     TransportationException,
 )
+
 LOGGER = logging.getLogger("transport")
 
 class ZmqWrapper(object):
     """Handler for ZMQ functions for use in other objects"""
 
     def __init__(self):
         """Initialize the ZMQ setup"""
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/executables/cli.py` & `fprime_gds-3.3.0a1/src/fprime_gds/executables/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,40 +6,38 @@
 code that they are importing.
 
 @author mstarch
 """
 import argparse
 import datetime
 import errno
+import getpass
 import itertools
 import os
-import re
 import platform
+import re
 import sys
-import getpass
-
-import fprime_gds.common.logger
-
-# Required to set the checksum as a module variable
-import fprime_gds.common.communication.checksum
-
-from abc import abstractmethod, ABC
+from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import Any, Dict, List, Tuple
 
+# Required to set the checksum as a module variable
+import fprime_gds.common.communication.checksum
+import fprime_gds.common.logger
 from fprime_gds.common.communication.adapters.base import BaseAdapter
 from fprime_gds.common.communication.adapters.ip import check_port
 from fprime_gds.common.pipeline.standard import StandardPipeline
 from fprime_gds.common.transport import ThreadedTCPSocketClient
-from fprime_gds.executables.utils import get_artifacts_root, find_dict, find_app
 from fprime_gds.common.utils.config_manager import ConfigManager
+from fprime_gds.executables.utils import find_app, find_dict, get_artifacts_root
 
 # Optional import: ZeroMQ. Requires package: pyzmq
 try:
     import zmq
+
     from fprime_gds.common.zmq_transport import ZmqClient
 except ImportError:
     zmq = None
     ZmqClient = None
 
 # Optional import: Serial Adapter. Requires package: SerialAdapter
 try:
@@ -217,29 +215,32 @@
     def handle_arguments(self, args, **kwargs):
         """Handle the root, detecting it if necessary"""
         if args.deployment:
             args.deployment = Path(args.deployment)
             return args
         detected_toolchain = get_artifacts_root() / platform.system()
         if not detected_toolchain.exists():
-            raise Exception(f"{detected_toolchain} does not exist. Make sure to build.")
+            msg = f"{detected_toolchain} does not exist. Make sure to build."
+            raise Exception(msg)
         likely_deployment = detected_toolchain / Path.cwd().name
         # Check if the deployment exists
         if likely_deployment.exists():
             args.deployment = likely_deployment
             return args
         child_directories = [child for child in detected_toolchain.iterdir() if child.is_dir()]
         if not child_directories:
-            raise Exception(f"No deployments found in {detected_toolchain}. Specify deployment with: --deployment")
+            msg = f"No deployments found in {detected_toolchain}. Specify deployment with: --deployment"
+            raise Exception(msg)
         # Works for the old structure where the bin, lib, and dict directories live immediately under the platform
         elif len(child_directories) == 3 and set([path.name for path in child_directories]) == {"bin", "lib", "dict"}:
             args.deployment = detected_toolchain
             return args
         elif len(child_directories) > 1:
-            raise Exception(f"Multiple deployments found in {detected_toolchain}. Choose using: --deployment")
+            msg = f"Multiple deployments found in {detected_toolchain}. Choose using: --deployment"
+            raise Exception(msg)
         args.deployment = child_directories[0]
         return args
 
 
 class CompositeParser(ParserBase):
     """Composite parser handles parsing as a composition of multiple other parsers"""
 
@@ -512,15 +513,16 @@
             },
         }
 
     def handle_arguments(self, args, **kwargs):
         """Handle arguments as parsed"""
         # Find dictionary setting via "dictionary" argument or the "deploy" argument
         if args.dictionary is not None and not os.path.exists(args.dictionary):
-            raise ValueError(f"Dictionary file {args.dictionary} does not exist")
+            msg = f"Dictionary file {args.dictionary} does not exist"
+            raise ValueError(msg)
         elif args.dictionary is None:
             args = super().handle_arguments(args, **kwargs)
             args.dictionary = find_dict(args.deployment)
         return args
 
 
 class FileHandlingParser(ParserBase):
@@ -692,16 +694,17 @@
         """
         # No app, stop processing now
         if args.noapp:
             return args
         args = super().handle_arguments(args, **kwargs)
         args.app = Path(args.app) if args.app else Path(find_app(args.deployment))
         if not args.app.is_file():
+            msg = f"F prime binary '{args.app}' does not exist or is not a file"
             raise ValueError(
-                f"F prime binary '{args.app}' does not exist or is not a file"
+                msg
             )
         return args
 
 
 class SearchArgumentsParser(ParserBase):
     """Parser for search arguments"""
 
@@ -721,14 +724,15 @@
                 "help": f"list all possible {self.command_name[:-1]} types the current F Prime instance could produce, based on the {self.command_name} dictionary, sorted by {self.command_name[:-1]} type ID",
             },
             ("-i", "--ids"): {
                 "dest": "ids",
                 "action": "store",
                 "required": False,
                 "type": int,
+                "nargs":'+',
                 "help": f"only show {self.command_name} matching the given type ID(s) 'ID'; can provide multiple IDs to show all given types",
                 "metavar": "ID",
             },
             ("-c", "--components"): {
                 "dest": "components",
                 "nargs": "+",
                 "required": False,
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/executables/comm.py` & `fprime_gds-3.3.0a1/src/fprime_gds/executables/comm.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,30 +14,28 @@
       argument, removing the need to rewrite most of this class to use something different.
 
 @author lestarch
 """
 
 
 import logging
-import sys
 import signal
-
+import sys
 
 # Required adapters built on standard tools
 try:
     from fprime_gds.common.zmq_transport import ZmqGround
 except ImportError:
     ZmqGround = None
 import fprime_gds.common.communication.adapters.base
+import fprime_gds.common.communication.adapters.ip
 import fprime_gds.common.communication.checksum
 import fprime_gds.common.communication.ground
-import fprime_gds.common.communication.adapters.ip
 import fprime_gds.common.logger
 import fprime_gds.executables.cli
-
 from fprime_gds.common.communication.framing import FpFramerDeframer
 from fprime_gds.common.communication.updown import Downlinker, Uplinker
 
 # Uses non-standard PIP package pyserial, so test the waters before getting a hard-import crash
 try:
     import fprime_gds.common.communication.adapters.uart
 except ImportError:
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/executables/fprime_cli.py` & `fprime_gds-3.3.0a1/src/fprime_gds/executables/fprime_cli.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -4,32 +4,32 @@
 """
 Parses the given CLI command for the F' GDS, and then executes the correct
 command with the user-provided arguments on the GDS
 """
 
 import abc
 import argparse
-from copy import deepcopy
 import os
 import sys
-import pkg_resources
+from copy import deepcopy
 from typing import Callable, List, Union
 
 import argcomplete
+import pkg_resources
 
 # NOTE: These modules are now only lazily loaded below as needed, due to slow
 # performance when importing them
 # import fprime_gds.common.gds_cli.channels as channels
 # import fprime_gds.common.gds_cli.command_send as command_send
 # import fprime_gds.common.gds_cli.events as events
 # from fprime_gds.common.pipeline.dictionaries import Dictionaries
 from fprime_gds.executables.cli import (
-    StandardPipelineParser,
-    SearchArgumentsParser,
     RetrievalArgumentsParser,
+    SearchArgumentsParser,
+    StandardPipelineParser,
 )
 
 
 def add_connection_arguments(parser: argparse.ArgumentParser):
     """
     Adds the arguments needed to properly connect to the API, which the user may
     want to specify
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/executables/run_deployment.py` & `fprime_gds-3.3.0a1/src/fprime_gds/executables/run_deployment.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,17 +3,22 @@
 #
 # Runs a deployment. Starts a GUI, a TCPServer, and the deployment application.
 ####
 import os
 import sys
 import webbrowser
 
-from fprime_gds.executables.cli import StandardPipelineParser, GdsParser, BinaryDeployment, CommParser, ParserBase
-from fprime_gds.executables.utils import run_wrapped_application, AppWrapperException
-
+from fprime_gds.executables.cli import (
+    BinaryDeployment,
+    CommParser,
+    GdsParser,
+    ParserBase,
+    StandardPipelineParser,
+)
+from fprime_gds.executables.utils import AppWrapperException, run_wrapped_application
 
 BASE_MODULE_ARGUMENTS = [sys.executable, "-u", "-m"]
 
 
 def parse_args():
     """ Parse command line arguments
     Gets an argument parsers to read the command line and process the arguments. Return
@@ -49,15 +54,16 @@
         try:
             if logfile is not None:
                 with open(logfile) as file_handle:
                     for line in file_handle:
                         print(f"    [LOG] {line.strip()}", file=sys.stderr)
         except Exception:
             pass
-        raise AppWrapperException(f"Failed to run {name}")
+        msg = f"Failed to run {name}"
+        raise AppWrapperException(msg)
 
 
 def launch_tts(parsed_args):
     """ Launch the ThreadedTcpServer middleware application
 
 
     Args:
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/executables/tcpserver.py` & `fprime_gds-3.3.0a1/src/fprime_gds/executables/tcpserver.py`

 * *Files 0% similar despite different names*

```diff
@@ -262,15 +262,16 @@
         elif dst == b"GUI":
             # Read telemetry data here...
             tlm_packet_size = self.recv(4)
             size = struct.unpack(">I", tlm_packet_size)[0]
             data = tlm_packet_size + self.recv(size)
 
         else:
-            raise RuntimeError(f"unrecognized client {dst.decode(DATA_ENCODING)}")
+            msg = f"unrecognized client {dst.decode(DATA_ENCODING)}"
+            raise RuntimeError(msg)
         return data
 
     def processNewPkt(self, header, data):
         """
         Process a single command here header and data here.
         The command must always start with A5A5 except if it is a List.
         Once the entire header tstring is processed send it on queue.
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/executables/utils.py` & `fprime_gds-3.3.0a1/src/fprime_gds/executables/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 """
 import atexit
 import signal
 import subprocess
 import sys
 import time
 from pathlib import Path
+
 from fprime.fbuild.settings import (
-    IniSettings,
     FprimeLocationUnknownException,
     FprimeSettingsException,
+    IniSettings,
 )
 
 # Python 2.7 compatibility, adding in missing error type
 try:
     InterruptedError
 except NameError:
 
@@ -100,15 +101,16 @@
     # Attempt to open a log file
     file_handler = None
     try:
         if logfile is not None:
             print(f"[INFO] Log File: {logfile}")
             file_handler = open(logfile, "wb", 0)
     except OSError as exc:
-        raise AppWrapperException(f"Failed to open: {logfile} with error {str(exc)}.")
+        msg = f"Failed to open: {logfile} with error {str(exc)}."
+        raise AppWrapperException(msg)
     # Spawn the process. Uses pexpect, as this will force the process to output data immediately, rather than buffering
     # the output. That way the log file is fully up-to-date.
     try:
         child = subprocess.Popen(
             arguments, stdout=file_handler, stderr=subprocess.STDOUT, env=env
         )
         register_process_assassin(child, file_handler)
@@ -118,33 +120,47 @@
             child.poll()
             if child.returncode is not None:
                 raise ProcessNotStableException(
                     arguments[0], child.returncode, launch_time
                 )
         return child
     except Exception as exc:
-        raise AppWrapperException(
-            f'Failed to run application: {" ".join(arguments)}. Error: {exc}'
-        )
+        msg = f"Failed to run application: {' '.join(arguments)}. Error: {exc}"
+        raise AppWrapperException(msg)
+
+
+def find_settings(path: Path) -> Path:
+    """
+    Finds the settings file by recursing parent to parent until a matching file is found.
+    """
+    needle = Path("settings.ini")
+    while path != path.parent:
+        if (path / needle).is_file():
+            return path / needle
+        path = path.parent
+    raise FprimeLocationUnknownException()
 
 
 def get_artifacts_root() -> Path:
     try:
-        ini_settings = IniSettings.load(None)
+        ini_file = find_settings(Path.cwd())
+        ini_settings = IniSettings.load(ini_file)
     except FprimeLocationUnknownException:
         print(
             "[ERROR] Not in fprime project and no deployment path provided, unable to find dictionary and/or app"
         )
         sys.exit(-1)
     except FprimeSettingsException as e:
         print("[ERROR]", e)
         sys.exit(-1)
-    assert "install_destination" in ini_settings, "install_destination not in settings.ini"
+    assert (
+        "install_destination" in ini_settings
+    ), "install_destination not in settings.ini"
     print(
-        f"""[INFO] Autodetected artifacts root '{ini_settings["install_destination"]}' from deployment settings.ini file."""
+        f"""[INFO] Autodetected artifacts root '{ini_settings["install_destination"]}' from project settings.ini file."""
     )
     return ini_settings["install_destination"]
 
 
 def find_app(root: Path) -> Path:
     bin_dir = root / "bin"
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/app.py` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,41 +5,39 @@
 # this framework.
 #
 ####
 import logging
 import os
 import sys
 import uuid
+
 import flask
 
 # Try to import Compress, but disable compression if not installed
 try:
     from flask_compress import Compress
 except ImportError:
     Compress = None
 
-from fprime_gds.flask import flask_uploads
-
 import fprime_gds.flask.channels
 
 # Import the Flask API implementations
 import fprime_gds.flask.commands
+import fprime_gds.flask.errors
 import fprime_gds.flask.events
 import fprime_gds.flask.json
 import fprime_gds.flask.logs
-import fprime_gds.flask.updown
 import fprime_gds.flask.sequence
 import fprime_gds.flask.stats
-import fprime_gds.flask.errors
-
+import fprime_gds.flask.updown
 from fprime_gds.executables.cli import ParserBase, StandardPipelineParser
+from fprime_gds.flask import flask_uploads
 
 from . import components
 
-
 # Update logging to avoid redundant messages
 logger = logging.getLogger("werkzeug")
 logger.setLevel(logging.WARN)
 logger = logging.getLogger("downlink")
 logger.setLevel(logging.INFO)
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/channels.py` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/channels.py`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/commands.py` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/commands.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 #             }
 #
 #
 # Note: for commands, these are not true "REST" objects, and thus this is a bit of a stretch to use
 #       a restful interface here. It is done this way to be in-tandem with the events and telemetry
 #       APIs for maintainability.
 ####
-import werkzeug.exceptions
 import flask_restful
 import flask_restful.reqparse
-
 import fprime.common.models.serialize.type_exceptions
+import werkzeug.exceptions
+
 import fprime_gds.common.data_types.cmd_data
 from fprime_gds.flask.resource import DictionaryResource, HistoryResourceBase
 
 
 class CommandDictionary(DictionaryResource):
     """Channel dictionary shares implementation"""
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/components.py` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/components.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 flask/components.py:
 
 This sets up the primary data components that allow Flask to connect into the system. This is where the standard
 pipeline and other components are created to interact with Flask.
 """
 import os
 
-from fprime_gds.common.pipeline.standard import StandardPipeline
 from fprime_gds.common.history.ram import SelfCleaningRamHistory
-
+from fprime_gds.common.pipeline.standard import StandardPipeline
 from fprime_gds.executables.cli import StandardPipelineParser
 
 # Module variables, should remain hidden. These are singleton top-level objects used by Flask, and its various
 # blueprints needed to run the system.
 __PIPELINE = None
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/default_settings.py` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/default_settings.py`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/errors.py` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 Contains the necessary definitions to handle errors across flask in a standard way. This will hopefully make the GDS
 more stable and less likely to fail on errors that occur.
 
 @author lestarch
 """
 
-from flask import jsonify, Flask
+from flask import Flask, jsonify
 from flask_restful import Api
 
 
 def build_error_object(error, args=None):
     """Builds an error object from an error"""
     return {
         "type": str(type(error).__name__),
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/events.py` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/events.py`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/flask_uploads.py` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/flask_uploads.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,22 +18,20 @@
 if PY3:
     string_types = (str,)
 else:
     string_types = (basestring,)
 
 import os.path
 import posixpath
-
-from flask import current_app, send_from_directory, abort, url_for
 from itertools import chain  # lgtm [py/unused-import]
+
+from flask import Blueprint, abort, current_app, send_from_directory, url_for
 from werkzeug.datastructures import FileStorage
 from werkzeug.utils import secure_filename
 
-from flask import Blueprint
-
 # Extension presets
 
 #: This just contains plain text files (.txt).
 TEXT = ("txt",)
 
 #: This contains various office document formats (.rtf, .odf, .ods, .gnumeric,
 #: .abw, .doc, .docx, .xls, .xlsx and .pdf). Note that the macro-enabled versions
@@ -203,15 +201,16 @@
             destination = uset.default_dest(app)
         if destination is None:  # still
             # use the default dest from the config
             if defaults["dest"] is not None:
                 using_defaults = True
                 destination = os.path.join(defaults["dest"], uset.name)
             else:
-                raise RuntimeError(f"no destination for set {uset.name}")
+                msg = f"no destination for set {uset.name}"
+                raise RuntimeError(msg)
 
     if base_url is None and using_defaults and defaults["url"]:
         base_url = addslash(defaults["url"]) + uset.name + "/"
 
     return UploadConfiguration(destination, base_url, allow_extns, deny_extns)
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/json.py` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/json.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 ####
 from abc import ABCMeta
 from enum import Enum
 from inspect import getmembers, isroutine
 from typing import Type
 from uuid import UUID
 
-from fprime.common.models.serialize.type_base import BaseType, ValueType
+import flask.json
 from fprime.common.models.serialize.time_type import TimeType
-from fprime_gds.common.data_types.cmd_data import CmdData
+from fprime.common.models.serialize.type_base import BaseType, ValueType
+
 from fprime_gds.common.data_types.ch_data import ChData
+from fprime_gds.common.data_types.cmd_data import CmdData
 from fprime_gds.common.data_types.event_data import EventData
 from fprime_gds.common.templates.data_template import DataTemplate
 
-import flask.json
-
 
 def jsonify_base_type(input_type: Type[BaseType]) -> dict:
     """ Turn a base type into a JSONable dictionary
 
     Convert a BaseType (the type, not an instance) into a jsonable dictionary. BaseTypes are converted by reading the
     class properties (without __) and creating the object:
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/logs.py` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/logs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 ####
 # Handles GDS logs in a lazy-loading way
 ####
 import os
+
 import flask_restful
 import flask_restful.reqparse
 
 
 class LogList(flask_restful.Resource):
     """A list of log files as produced by the GDS."""
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/resource.py` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 Helper functions used to manage resource endpoints for the fprime_gds. This functions to reduce code duplication,
 establish standard patterns, and prevent replicated errors.
 
 @author lestarch
 """
 from flask_restful import Resource
 from flask_restful.reqparse import RequestParser
+
 from fprime_gds.flask.errors import build_error_object
 
 
 class DictionaryResource(Resource):
     """
     Resource tasked with serving the supplied dictionary through flask. The dictionary will be returned as-is and thus
     should be flask compatible. Errors with the dictionary are a 500 server error and may not be recovered.
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/sequence.py` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/sequence.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 ####
 #
 ####
-from pathlib import Path
 import re
 import sys
 from io import StringIO
+from pathlib import Path
+
 import flask_restful
 import flask_restful.reqparse
 
-from fprime_gds.common.tools.seqgen import generateSequence, SeqGenException
+from fprime_gds.common.tools.seqgen import SeqGenException, generateSequence
 
 
 class StdioTheif(object):
     """
     This class consumes all standard out and error production produced with-in a context block (with :) capturing it.
     """
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/advanced-settings/addon-templates.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/advanced-settings/addon-templates.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/advanced-settings/addon.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/advanced-settings/addon.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/channel-render/channel-render-template.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/channel-render/channel-render-template.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/channel-render/channel-render.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/channel-render/channel-render.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/chart-display/addon-templates.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/chart-display/addon-templates.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/chart-display/addon.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/chart-display/addon.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/chart-display/config.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/chart-display/config.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/chart-display/modified-vendor/chartjs-plugin-streaming.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/chart-display/modified-vendor/chartjs-plugin-streaming.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/chart-display/modified-vendor/chartjs-plugin-zoom.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/chart-display/modified-vendor/chartjs-plugin-zoom.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/chart-display/modified-vendor/flat.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/chart-display/modified-vendor/flat.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/chart-display/sibling.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/chart-display/sibling.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/chart-display/vendor/chart.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/chart-display/vendor/chart.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/chart-display/vendor/chartjs-adapter-luxon.min.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/chart-display/vendor/chartjs-adapter-luxon.min.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/chart-display/vendor/hammer.min.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/chart-display/vendor/hammer.min.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/commanding/argument-templates.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/commanding/argument-templates.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/commanding/arguments.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/commanding/arguments.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/commanding/command-history-template.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/commanding/command-history-template.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/commanding/command-history.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/commanding/command-history.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/commanding/command-input-template.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/commanding/command-input-template.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/commanding/command-input.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/commanding/command-input.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/commanding/command-string-template.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/commanding/command-string-template.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/commanding/command-string.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/commanding/command-string.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/dictionary/addon-templates.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/dictionary/addon-templates.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/dictionary/addon.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/dictionary/addon.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/image-display/addon.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/image-display/addon.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/sequencer/README.md` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/sequencer/README.md`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/sequencer/addon-templates.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/sequencer/addon-templates.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/sequencer/addon.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/sequencer/addon.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/sequencer/autocomplete.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/sequencer/autocomplete.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/sequencer/lint.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/sequencer/lint.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/sequencer/third/code-mirror.es.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/sequencer/third/code-mirror.es.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/sequencer/third/rollup/index.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/sequencer/third/rollup/index.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/sequencer/third/rollup/language.grammer` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/sequencer/third/rollup/language.grammer`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/addons/sequencer/third/rollup/package.json` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/addons/sequencer/third/rollup/package.json`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/css/fprime.css` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/css/fprime.css`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/css/fpstyle.css` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/css/fpstyle.css`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/favicon.ico` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/img/error.svg` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/img/error.svg`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/img/logo.svg` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/img/logo.svg`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/img/success.svg` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/img/success.svg`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/index.html` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/index.html`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/js/config.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/js/config.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/js/datastore.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/js/datastore.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/js/gds.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/js/gds.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/js/loader.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/js/loader.js`

 * *Files 24% similar despite different names*

#### js-beautify {}

```diff
@@ -13,14 +13,17 @@
  */
 import {
     config
 } from "./config.js";
 import {
     _settings
 } from "./settings.js";
+import {
+    _validator
+} from "./validate.js";
 
 /**
  * Function allowing for the saving of some data to a downloadable file.
  * @param data: data to download as file, should be text
  * @return: href link triggering file save
  */
 export function saveTextFileViaHref(data) {
@@ -50,14 +53,126 @@
         } else {
             error("[ERROR] File too large: " + (file.size / 1024 / 1024).toLocaleString(undefined) + " MiB > 1MiB");
         }
     });
 }
 
 /**
+ * Parser to safely handle potential JSON object from Python. Python can produce some non-standard values (infinities,
+ * NaNs, etc.) These values then break on the JS Javascript parser. To localize these faults, they are replaced before
+ * processing with strings and then formally set during parsing.
+ *
+ * This is done by looking for tokens in unquoted text and replacing them with string representations.
+ *
+ */
+class SaferParser {
+    /**
+     * Set up the parser
+     */
+    constructor() {
+        this.STATES = {
+            UNQUOTED: 0,
+            QUOTED: 1
+        };
+        this.FLAG = "-_-您好"; // Extended character usage make collisions less-likely
+        this.MAPPINGS = [
+            ["-Infinity", this.FLAG + "-inf", -Infinity],
+            ["Infinity", this.FLAG + "inf", Infinity],
+            ["NaN", this.FLAG + "nan", NaN],
+            ["null", this.FLAG + "null", null]
+        ];
+        this.state = this.STATES.UNQUOTED;
+    }
+
+    /**
+     * Parse method that will replace JSON.parse. This handles known bad cases and also prints better error messages
+     * including the working snippets of text.
+     * @param rawData: string data
+     * @return {{}|any}: Javascript Object representation of data.
+     */
+    parse(rawData) {
+        let converted_data = this.convert(rawData);
+        try {
+            return JSON.parse(converted_data, this.revert.bind(this));
+        } catch (e) {
+            let message = e.toString();
+            const matcher = /line (\d+) column (\d+)/
+
+            // Process the match
+            let snippet = "";
+            let match = message.match(matcher);
+            if (match != null) {
+                let lines = converted_data.split("\n");
+                let line = lines[Number.parseInt(match[1]) - 1]
+                snippet = line.substring(Number.parseInt(match[2]) - 6, Number.parseInt(match[2]) + 5);
+                message += ". Offending snippet: " + snippet;
+            }
+            _validator.updateErrors([message]);
+        }
+        return {};
+    }
+
+    /**
+     * Convert data from invalid form to strings.
+     * @param rawData: raw data including potentially invalid data
+     * @return {string}: string data in correct JSON format
+     */
+    convert(rawData) {
+        let unprocessed = rawData;
+        let transformed_data = "";
+
+        while (unprocessed.length > 0) {
+            let next_quote = unprocessed.indexOf("\"");
+            let section = (next_quote !== -1) ? unprocessed.substring(0, next_quote + 1) : unprocessed.substring(0);
+            unprocessed = unprocessed.substring(section.length);
+            transformed_data += this.processChunk(section);
+            this.state = (this.state === this.STATES.QUOTED) ? this.STATES.UNQUOTED : this.STATES.QUOTED;
+        }
+        return transformed_data;
+    }
+
+    /**
+     * Inverse of convert removing string and replacing back invalid JSON tokens.
+     * @param key: JSON key
+     * @param value: JSON value search for the converted value.
+     * @return {*}: reverted value or value
+     */
+    revert(key, value) {
+        for (let i = 0; i < this.MAPPINGS.length; i++) {
+            if ((this.MAPPINGS[i][1]) === value) {
+                return this.MAPPINGS[i][2];
+            }
+        }
+        return value;
+    }
+
+    /**
+     * Process a section of the JSON string looking for values to convert. This is intended to handle a section of
+     * quoted or unquoted text but should never handle quoted and unquoted data in one call.
+     * @param section: section of the data
+     * @return {*}: converted data
+     */
+    processChunk(section) {
+        // Replaces all the above mappings with a flagged value
+        let replace_all = (section) => {
+            for (let i = 0; i < this.MAPPINGS.length; i++) {
+                section = section.replace(this.MAPPINGS[i][0], "\"" + this.MAPPINGS[i][1] + "\"");
+            }
+            return section;
+        }
+
+        // When out of quoted space,
+        if (this.state === this.STATES.UNQUOTED) {
+            return replace_all(section);
+        }
+        return section;
+    }
+}
+
+/**
  * Loader:
  *
  * Loader that is used to pull in data from the REST API. This loader is intended to be a singleton and thus will be
  * instantiated and exported once.
  */
 class Loader {
     /**
@@ -195,15 +310,15 @@
         return new Promise(function(resolve, reject) {
             var xhttp = new XMLHttpRequest();
             xhttp.onreadystatechange = function() {
                 // Parse as JSON or send back raw error
                 if (this.readyState === 4 && this.status === 200 && raw) {
                     resolve(this.responseText);
                 } else if (this.readyState === 4 && this.status === 200) {
-                    let dataObj = JSON.parse(this.responseText);
+                    let dataObj = new SaferParser().parse(this.responseText);
                     resolve(dataObj);
                 } else if (this.readyState === 4) {
                     reject(this.responseText);
                 }
             };
             let url = endpoint;
             let session = (_self.endpoints["session"].data || {}).session || null;
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/js/performance.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/js/performance.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/js/settings.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/js/settings.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/js/uploader.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/js/uploader.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/js/validate.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/js/validate.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/js/vue-support/channel.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/js/vue-support/channel.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/js/vue-support/dashboard-box.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/js/vue-support/dashboard-box.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/js/vue-support/dashboard.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/js/vue-support/dashboard.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/js/vue-support/downlink.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/js/vue-support/downlink.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/js/vue-support/event.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/js/vue-support/event.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/js/vue-support/fp-row.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/js/vue-support/fp-row.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/js/vue-support/fptable.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/js/vue-support/fptable.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/js/vue-support/log.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/js/vue-support/log.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/js/vue-support/tabetc.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/js/vue-support/tabetc.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/js/vue-support/uplink.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/js/vue-support/uplink.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/js/vue-support/utils.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/js/vue-support/utils.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/css/all.min.css` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/css/all.min.css`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/css/bootstrap.min.css` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/css/vue-select.css` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/css/vue-select.css`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/js/luxon.min.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/js/luxon.min.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/js/sorttable.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/js/sorttable.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/js/v-runtime-template.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/js/v-runtime-template.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/js/vue-select.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/js/vue-select.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/js/vue.min.js` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/js/vue.min.js`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/webfonts/fa-brands-400.eot` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/webfonts/fa-brands-400.svg` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/webfonts/fa-brands-400.ttf` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/webfonts/fa-brands-400.woff` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/webfonts/fa-brands-400.woff2` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/webfonts/fa-regular-400.eot` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/webfonts/fa-regular-400.svg` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/webfonts/fa-regular-400.ttf` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/webfonts/fa-regular-400.woff` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/webfonts/fa-regular-400.woff2` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.eot` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.svg` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.ttf` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.woff` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.woff2` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/stats.py` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """ stats.py:
 
 Statistics package for the GDS to help diagnose performance issues and give greater visibility into the running GDS.
 """
+from typing import Dict
+
 import flask_restful
 
-from typing import Dict
 from fprime_gds.common.history.history import History
 from fprime_gds.common.history.ram import RamHistory
 
 
 class StatsBlob(flask_restful.Resource):
     """Produces a statistics blob for the upstream webpage"""
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds/flask/updown.py` & `fprime_gds-3.3.0a1/src/fprime_gds/flask/updown.py`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds.egg-info/PKG-INFO` & `fprime_gds-3.3.0a1/src/fprime_gds.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fprime-gds
-Version: 3.2.1a2
+Version: 3.3.0a1
 Summary: F Prime Flight Software Ground Data System layer.
 Home-page: https://github.com/nasa/fprime
 Author: Michael Starch
 Author-email: Michael.D.Starch@jpl.nasa.gov
 License: Apache 2.0 License
 Project-URL: Issue Tracker, https://github.com/nasa/fprime/issues
 Keywords: fprime,gds,embedded,nasa
```

### Comparing `fprime_gds-3.2.1a2/src/fprime_gds.egg-info/SOURCES.txt` & `fprime_gds-3.3.0a1/src/fprime_gds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/test/fprime_gds/common/distributor/test_distributor.py` & `fprime_gds-3.3.0a1/test/fprime_gds/common/distributor/test_distributor.py`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/test/fprime_gds/common/encoders/test_ch_encoder.py` & `fprime_gds-3.3.0a1/test/fprime_gds/common/encoders/test_ch_encoder.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 Tests the channel encoder
 
 Created on Jul 10, 2020
 @author: Joseph Paetz, hpaulson
 """
 
 
+from fprime.common.models.serialize.numerical_types import U16Type, U32Type
+from fprime.common.models.serialize.time_type import TimeType
+from fprime_gds.common.data_types.ch_data import ChData
 from fprime_gds.common.encoders.ch_encoder import ChEncoder
 from fprime_gds.common.templates.ch_template import ChTemplate
 from fprime_gds.common.utils.config_manager import ConfigManager
-from fprime.common.models.serialize.time_type import TimeType
-from fprime.common.models.serialize.numerical_types import U16Type, U32Type
-from fprime_gds.common.data_types.ch_data import ChData
 
 
 def test_ch_encoder():
     """
     Tests the encoding of the channel encoder
     """
     config = ConfigManager()
```

### Comparing `fprime_gds-3.2.1a2/test/fprime_gds/common/encoders/test_event_encoder.py` & `fprime_gds-3.3.0a1/test/fprime_gds/common/encoders/test_event_encoder.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 Tests the event encoder
 
 Created on Jul 10, 2020
 @author: Joseph Paetz, hpaulson
 """
 
 
-from fprime_gds.common.encoders.event_encoder import EventEncoder
+from fprime.common.models.serialize.numerical_types import U8Type, U16Type, U32Type
+from fprime.common.models.serialize.time_type import TimeType
 from fprime_gds.common.data_types.event_data import EventData
-from fprime_gds.common.utils.config_manager import ConfigManager
+from fprime_gds.common.encoders.event_encoder import EventEncoder
 from fprime_gds.common.templates.event_template import EventTemplate
-from fprime.common.models.serialize.time_type import TimeType
-from fprime.common.models.serialize.numerical_types import U8Type, U16Type, U32Type
+from fprime_gds.common.utils.config_manager import ConfigManager
 from fprime_gds.common.utils.event_severity import EventSeverity
 
 
 def test_event_encoder():
     """
     Tests the encoding of the event encoder
     """
```

### Comparing `fprime_gds-3.2.1a2/test/fprime_gds/common/encoders/test_pkt_encoder.py` & `fprime_gds-3.3.0a1/test/fprime_gds/common/encoders/test_pkt_encoder.py`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Tests the packet encoder
 
 Created on Jul 10, 2020
 @author: Joseph Paetz, hpaulson
 """
 
 
-from fprime_gds.common.encoders.pkt_encoder import PktEncoder
+from fprime.common.models.serialize.numerical_types import U8Type, U16Type, U32Type
+from fprime.common.models.serialize.time_type import TimeType
+from fprime_gds.common.data_types.ch_data import ChData
 from fprime_gds.common.data_types.pkt_data import PktData
-from fprime_gds.common.utils.config_manager import ConfigManager
+from fprime_gds.common.encoders.pkt_encoder import PktEncoder
 from fprime_gds.common.templates.ch_template import ChTemplate
 from fprime_gds.common.templates.pkt_template import PktTemplate
-from fprime_gds.common.data_types.ch_data import ChData
-from fprime.common.models.serialize.time_type import TimeType
-from fprime.common.models.serialize.numerical_types import U8Type, U16Type, U32Type
+from fprime_gds.common.utils.config_manager import ConfigManager
 
 
 def test_pkt_encoder():
     """
     Tests the encoding of the packet encoder
     """
     config = ConfigManager()
```

### Comparing `fprime_gds-3.2.1a2/test/fprime_gds/common/gds_cli/filtering_utils_test.py` & `fprime_gds-3.3.0a1/test/fprime_gds/common/gds_cli/filtering_utils_test.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
 A suite of unit tests for testing the predicates and filtering utilities the
 GDS CLI uses
 """
 
-import pytest
-
 import fprime_gds.common.gds_cli.filtering_utils as filtering_utils
+import pytest
 from fprime.common.models.serialize import time_type
 from fprime_gds.common.data_types.event_data import EventData
 from fprime_gds.common.templates.event_template import EventTemplate
 from fprime_gds.common.testing_fw import predicates
 from fprime_gds.common.utils.event_severity import EventSeverity
 
+
 # Pytest fixtures work by reusing outer names, so disable this warning
 # pylint: disable=redefined-outer-name
 @pytest.fixture
 def sample_template():
     return EventTemplate(
         event_id=12345,
         name="Luggage_Combination",
```

### Comparing `fprime_gds-3.2.1a2/test/fprime_gds/common/gds_cli/utils_test.py` & `fprime_gds-3.3.0a1/test/fprime_gds/common/gds_cli/utils_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """
 A suite of unit tests for testing utilities the GDS CLI uses
 """
 
 from copy import deepcopy
 
-import pytest
-
 import fprime_gds.common.gds_cli.filtering_utils as filtering_utils
 import fprime_gds.common.gds_cli.test_api_utils as test_api_utils
+import pytest
 from fprime_gds.common.data_types.pkt_data import PktData
 from fprime_gds.common.data_types.sys_data import SysData
 from fprime_gds.common.templates.data_template import DataTemplate
 from fprime_gds.common.templates.pkt_template import PktTemplate
 from fprime_gds.common.testing_fw import predicates
 
 # ==============================================================================
```

### Comparing `fprime_gds-3.2.1a2/test/fprime_gds/common/history/chronohistory_unit_test.py` & `fprime_gds-3.3.0a1/test/fprime_gds/common/history/chronohistory_unit_test.py`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/test/fprime_gds/common/history/testhistory_unit_test.py` & `fprime_gds-3.3.0a1/test/fprime_gds/common/history/testhistory_unit_test.py`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/test/fprime_gds/common/testing_fw/UnitTestDictionary.xml` & `fprime_gds-3.3.0a1/test/fprime_gds/common/testing_fw/UnitTestDictionary.xml`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/test/fprime_gds/common/testing_fw/api_unit_test.py` & `fprime_gds-3.3.0a1/test/fprime_gds/common/testing_fw/api_unit_test.py`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/test/fprime_gds/common/testing_fw/predicate_unit_test.py` & `fprime_gds-3.3.0a1/test/fprime_gds/common/testing_fw/predicate_unit_test.py`

 * *Files identical despite different names*

### Comparing `fprime_gds-3.2.1a2/test/fprime_gds/common/utils/test_string_util.py` & `fprime_gds-3.3.0a1/test/fprime_gds/common/utils/test_string_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Tests format_string util
 
 @Created on March 18, 2021
 @janamian
 """
 
 import unittest
+
 from fprime_gds.common.utils.string_util import format_string_template
 
 
 class TestFormatString(unittest.TestCase):
     def test_format_with_no_issue(self):
         template = "Opcode 0x%04X dispatched to port %d and value %f"
         values = (181, 8, 1.234)
```

### Comparing `fprime_gds-3.2.1a2/test/fprime_gds/executables/test_run_deployment.py` & `fprime_gds-3.3.0a1/test/fprime_gds/executables/test_run_deployment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import platform
 import tempfile
 import unittest
 from pathlib import Path
-
 from unittest import mock
 
 from fprime_gds.executables import run_deployment
 
 
 class TestRunDeployment(unittest.TestCase):
```

### Comparing `fprime_gds-3.2.1a2/test/gui/GUI_Test_Procedure.md` & `fprime_gds-3.3.0a1/test/gui/GUI_Test_Procedure.md`

 * *Files identical despite different names*

