# Comparing `tmp/chik_dev_tools-1.2.0.tar.gz` & `tmp/chik_dev_tools-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/chik-dev-tools/chik-dev-tools/dist/.tmp-tom4_l5m/chik_dev_tools-1.2.0.tar", last modified: Tue Aug  1 03:04:34 2023, max compression
+gzip compressed data, was "/home/runner/work/chik-dev-tools/chik-dev-tools/dist/.tmp-0usg060m/chik_dev_tools-1.2.1.tar", last modified: Tue Aug  1 03:10:33 2023, max compression
```

## Comparing `chik_dev_tools-1.2.0.tar` & `chik_dev_tools-1.2.1.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:04:34.000000 chik_dev_tools-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:04:34.000000 chik_dev_tools-1.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:04:34.000000 chik_dev_tools-1.2.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:04:34.000000 chik_dev_tools-1.2.0/.github/actions/install/
--rw-r--r--   0 runner    (1001) docker     (122)     1156 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/.github/actions/install/action.yml
--rwxr-xr-x   0 runner    (1001) docker     (122)       51 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/.github/actions/install/install.ps1
--rwxr-xr-x   0 runner    (1001) docker     (122)       65 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/.github/actions/install/install.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:04:34.000000 chik_dev_tools-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      832 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/.github/workflows/codeql-analysis.yml.bak
--rw-r--r--   0 runner    (1001) docker     (122)     1805 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/.github/workflows/precommit.yml.bak
--rw-r--r--   0 runner    (1001) docker     (122)     1485 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3020 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/.github/workflows/run-test-suite.yml.bak
--rw-r--r--   0 runner    (1001) docker     (122)     2063 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/.github/workflows/super-linter.yml.bak
--rw-r--r--   0 runner    (1001) docker     (122)     1193 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/.github/workflows/test-blockchain-main.yml.bak
--rw-r--r--   0 runner    (1001) docker     (122)      108 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1009 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/.markdown-lint.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1693 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    10240 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     4875 2023-08-01 03:04:34.000000 chik_dev_tools-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4151 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (122)      230 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/activated.ps1
--rwxr-xr-x   0 runner    (1001) docker     (122)      588 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/activated.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      230 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/activated.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:04:34.000000 chik_dev_tools-1.2.0/cdv/
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/cdv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:04:34.000000 chik_dev_tools-1.2.0/cdv/clibs/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/cdv/clibs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1114 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/cdv/clibs/condition_codes.clib
--rw-r--r--   0 runner    (1001) docker     (122)     2888 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/cdv/clibs/curry_and_treehash.clib
--rw-r--r--   0 runner    (1001) docker     (122)      244 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/cdv/clibs/sha256tree.clib
--rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/cdv/clibs/singleton_truths.clib
--rw-r--r--   0 runner    (1001) docker     (122)      462 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/cdv/clibs/utility_macros.clib
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:04:34.000000 chik_dev_tools-1.2.0/cdv/cmds/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/cdv/cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    29821 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/cdv/cmds/chik_inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     3809 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/cdv/cmds/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     7401 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/cdv/cmds/clsp.py
--rw-r--r--   0 runner    (1001) docker     (122)    15069 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/cdv/cmds/rpc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1783 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/cdv/cmds/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:04:34.000000 chik_dev_tools-1.2.0/cdv/examples/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/cdv/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:04:34.000000 chik_dev_tools-1.2.0/cdv/examples/clsp/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/cdv/examples/clsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1263 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/cdv/examples/clsp/piggybank.clsp
--rw-r--r--   0 runner    (1001) docker     (122)      503 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/cdv/examples/clsp/piggybank.clsp.hex
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:04:34.000000 chik_dev_tools-1.2.0/cdv/examples/drivers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/cdv/examples/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1324 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/cdv/examples/drivers/piggybank_drivers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:04:34.000000 chik_dev_tools-1.2.0/cdv/examples/klvm/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/cdv/examples/klvm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:04:34.000000 chik_dev_tools-1.2.0/cdv/examples/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     5237 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/cdv/examples/tests/test_piggybank.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:04:34.000000 chik_dev_tools-1.2.0/cdv/test/
--rw-r--r--   0 runner    (1001) docker     (122)    28945 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/cdv/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      478 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/cdv/test/test_skeleton.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:04:34.000000 chik_dev_tools-1.2.0/cdv/util/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/cdv/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1228 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/cdv/util/keys.py
--rw-r--r--   0 runner    (1001) docker     (122)     3545 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/cdv/util/load_klvm.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:04:34.000000 chik_dev_tools-1.2.0/chik_dev_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4875 2023-08-01 03:04:34.000000 chik_dev_tools-1.2.0/chik_dev_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2334 2023-08-01 03:04:34.000000 chik_dev_tools-1.2.0/chik_dev_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-01 03:04:34.000000 chik_dev_tools-1.2.0/chik_dev_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-08-01 03:04:34.000000 chik_dev_tools-1.2.0/chik_dev_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-08-01 03:04:34.000000 chik_dev_tools-1.2.0/chik_dev_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        4 2023-08-01 03:04:34.000000 chik_dev_tools-1.2.0/chik_dev_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      519 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (122)      676 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-01 03:04:34.000000 chik_dev_tools-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1691 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:04:34.000000 chik_dev_tools-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     2229 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/tests/build-init-files.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:04:34.000000 chik_dev_tools-1.2.0/tests/cmds/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:04:34.000000 chik_dev_tools-1.2.0/tests/cmds/object_files/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:04:34.000000 chik_dev_tools-1.2.0/tests/cmds/object_files/coinrecords/
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/tests/cmds/object_files/coinrecords/coinrecord.hex
--rw-r--r--   0 runner    (1001) docker     (122)      325 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/tests/cmds/object_files/coinrecords/coinrecord.json
--rw-r--r--   0 runner    (1001) docker     (122)      336 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/tests/cmds/object_files/coinrecords/coinrecord_invalid.json
--rw-r--r--   0 runner    (1001) docker     (122)      296 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/tests/cmds/object_files/coinrecords/coinrecord_metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:04:34.000000 chik_dev_tools-1.2.0/tests/cmds/object_files/coins/
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/tests/cmds/object_files/coins/coin.json
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/tests/cmds/object_files/coins/coin_invalid.json
--rw-r--r--   0 runner    (1001) docker     (122)      256 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/tests/cmds/object_files/coins/coin_metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:04:34.000000 chik_dev_tools-1.2.0/tests/cmds/object_files/spendbundles/
--rw-r--r--   0 runner    (1001) docker     (122)      348 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/tests/cmds/object_files/spendbundles/spendbundle.hex
--rw-r--r--   0 runner    (1001) docker     (122)      591 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/tests/cmds/object_files/spendbundles/spendbundle.json
--rw-r--r--   0 runner    (1001) docker     (122)      557 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/tests/cmds/object_files/spendbundles/spendbundle_invalid.json
--rw-r--r--   0 runner    (1001) docker     (122)      467 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/tests/cmds/object_files/spendbundles/spendbundle_metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:04:34.000000 chik_dev_tools-1.2.0/tests/cmds/object_files/spends/
--rw-r--r--   0 runner    (1001) docker     (122)      372 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/tests/cmds/object_files/spends/spend.hex
--rw-r--r--   0 runner    (1001) docker     (122)      506 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/tests/cmds/object_files/spends/spend.json
--rw-r--r--   0 runner    (1001) docker     (122)      394 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/tests/cmds/object_files/spends/spend_2.json
--rw-r--r--   0 runner    (1001) docker     (122)      288 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/tests/cmds/object_files/spends/spend_invalid.json
--rw-r--r--   0 runner    (1001) docker     (122)      489 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/tests/cmds/object_files/spends/spend_metadata.json
--rw-r--r--   0 runner    (1001) docker     (122)     2195 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/tests/cmds/test_cdv.py
--rw-r--r--   0 runner    (1001) docker     (122)     8370 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/tests/cmds/test_clsp.py
--rw-r--r--   0 runner    (1001) docker     (122)    17176 2023-08-01 03:03:49.000000 chik_dev_tools-1.2.0/tests/cmds/test_inspect.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:10:33.658149 chik_dev_tools-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:10:33.642148 chik_dev_tools-1.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:10:33.642148 chik_dev_tools-1.2.1/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:10:33.646148 chik_dev_tools-1.2.1/.github/actions/install/
+-rw-r--r--   0 runner    (1001) docker     (122)     1156 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/.github/actions/install/action.yml
+-rwxr-xr-x   0 runner    (1001) docker     (122)       51 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/.github/actions/install/install.ps1
+-rwxr-xr-x   0 runner    (1001) docker     (122)       65 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/.github/actions/install/install.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:10:33.646148 chik_dev_tools-1.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      832 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/.github/workflows/codeql-analysis.yml.bak
+-rw-r--r--   0 runner    (1001) docker     (122)     1805 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/.github/workflows/precommit.yml.bak
+-rw-r--r--   0 runner    (1001) docker     (122)     1489 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3020 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/.github/workflows/run-test-suite.yml.bak
+-rw-r--r--   0 runner    (1001) docker     (122)     2063 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/.github/workflows/super-linter.yml.bak
+-rw-r--r--   0 runner    (1001) docker     (122)     1193 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/.github/workflows/test-blockchain-main.yml.bak
+-rw-r--r--   0 runner    (1001) docker     (122)      108 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1009 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/.markdown-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1693 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    10240 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     4875 2023-08-01 03:10:33.654148 chik_dev_tools-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4151 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (122)      230 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/activated.ps1
+-rwxr-xr-x   0 runner    (1001) docker     (122)      588 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/activated.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      230 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/activated.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:10:33.646148 chik_dev_tools-1.2.1/cdv/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/cdv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:10:33.650148 chik_dev_tools-1.2.1/cdv/clibs/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/cdv/clibs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1114 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/cdv/clibs/condition_codes.clib
+-rw-r--r--   0 runner    (1001) docker     (122)     2888 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/cdv/clibs/curry_and_treehash.clib
+-rw-r--r--   0 runner    (1001) docker     (122)      244 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/cdv/clibs/sha256tree.clib
+-rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/cdv/clibs/singleton_truths.clib
+-rw-r--r--   0 runner    (1001) docker     (122)      462 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/cdv/clibs/utility_macros.clib
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:10:33.650148 chik_dev_tools-1.2.1/cdv/cmds/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/cdv/cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29821 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/cdv/cmds/chik_inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3809 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/cdv/cmds/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7401 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/cdv/cmds/clsp.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15069 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/cdv/cmds/rpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1783 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/cdv/cmds/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:10:33.650148 chik_dev_tools-1.2.1/cdv/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/cdv/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:10:33.650148 chik_dev_tools-1.2.1/cdv/examples/clsp/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/cdv/examples/clsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1263 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/cdv/examples/clsp/piggybank.clsp
+-rw-r--r--   0 runner    (1001) docker     (122)      503 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/cdv/examples/clsp/piggybank.clsp.hex
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:10:33.650148 chik_dev_tools-1.2.1/cdv/examples/drivers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/cdv/examples/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1324 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/cdv/examples/drivers/piggybank_drivers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:10:33.650148 chik_dev_tools-1.2.1/cdv/examples/klvm/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/cdv/examples/klvm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:10:33.650148 chik_dev_tools-1.2.1/cdv/examples/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     5237 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/cdv/examples/tests/test_piggybank.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:10:33.650148 chik_dev_tools-1.2.1/cdv/test/
+-rw-r--r--   0 runner    (1001) docker     (122)    28945 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/cdv/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      478 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/cdv/test/test_skeleton.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:10:33.650148 chik_dev_tools-1.2.1/cdv/util/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/cdv/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1228 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/cdv/util/keys.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3545 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/cdv/util/load_klvm.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:10:33.654148 chik_dev_tools-1.2.1/chik_dev_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4875 2023-08-01 03:10:33.000000 chik_dev_tools-1.2.1/chik_dev_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2334 2023-08-01 03:10:33.000000 chik_dev_tools-1.2.1/chik_dev_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-01 03:10:33.000000 chik_dev_tools-1.2.1/chik_dev_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-08-01 03:10:33.000000 chik_dev_tools-1.2.1/chik_dev_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      233 2023-08-01 03:10:33.000000 chik_dev_tools-1.2.1/chik_dev_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        4 2023-08-01 03:10:33.000000 chik_dev_tools-1.2.1/chik_dev_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      519 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (122)      676 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-01 03:10:33.658149 chik_dev_tools-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:10:33.654148 chik_dev_tools-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     2229 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/tests/build-init-files.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:10:33.654148 chik_dev_tools-1.2.1/tests/cmds/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:10:33.646148 chik_dev_tools-1.2.1/tests/cmds/object_files/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:10:33.654148 chik_dev_tools-1.2.1/tests/cmds/object_files/coinrecords/
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/tests/cmds/object_files/coinrecords/coinrecord.hex
+-rw-r--r--   0 runner    (1001) docker     (122)      325 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/tests/cmds/object_files/coinrecords/coinrecord.json
+-rw-r--r--   0 runner    (1001) docker     (122)      336 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/tests/cmds/object_files/coinrecords/coinrecord_invalid.json
+-rw-r--r--   0 runner    (1001) docker     (122)      296 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/tests/cmds/object_files/coinrecords/coinrecord_metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:10:33.654148 chik_dev_tools-1.2.1/tests/cmds/object_files/coins/
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/tests/cmds/object_files/coins/coin.json
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/tests/cmds/object_files/coins/coin_invalid.json
+-rw-r--r--   0 runner    (1001) docker     (122)      256 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/tests/cmds/object_files/coins/coin_metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:10:33.654148 chik_dev_tools-1.2.1/tests/cmds/object_files/spendbundles/
+-rw-r--r--   0 runner    (1001) docker     (122)      348 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/tests/cmds/object_files/spendbundles/spendbundle.hex
+-rw-r--r--   0 runner    (1001) docker     (122)      591 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/tests/cmds/object_files/spendbundles/spendbundle.json
+-rw-r--r--   0 runner    (1001) docker     (122)      557 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/tests/cmds/object_files/spendbundles/spendbundle_invalid.json
+-rw-r--r--   0 runner    (1001) docker     (122)      467 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/tests/cmds/object_files/spendbundles/spendbundle_metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 03:10:33.654148 chik_dev_tools-1.2.1/tests/cmds/object_files/spends/
+-rw-r--r--   0 runner    (1001) docker     (122)      372 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/tests/cmds/object_files/spends/spend.hex
+-rw-r--r--   0 runner    (1001) docker     (122)      506 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/tests/cmds/object_files/spends/spend.json
+-rw-r--r--   0 runner    (1001) docker     (122)      394 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/tests/cmds/object_files/spends/spend_2.json
+-rw-r--r--   0 runner    (1001) docker     (122)      288 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/tests/cmds/object_files/spends/spend_invalid.json
+-rw-r--r--   0 runner    (1001) docker     (122)      489 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/tests/cmds/object_files/spends/spend_metadata.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2195 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/tests/cmds/test_cdv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8370 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/tests/cmds/test_clsp.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17176 2023-08-01 03:09:41.000000 chik_dev_tools-1.2.1/tests/cmds/test_inspect.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `chik_dev_tools-1.2.0/.github/actions/install/action.yml` & `chik_dev_tools-1.2.1/.github/actions/install/action.yml`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.0/.github/workflows/codeql-analysis.yml.bak` & `chik_dev_tools-1.2.1/.github/workflows/codeql-analysis.yml.bak`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.0/.github/workflows/precommit.yml.bak` & `chik_dev_tools-1.2.1/.github/workflows/precommit.yml.bak`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.0/.github/workflows/publish-to-test-pypi.yml` & `chik_dev_tools-1.2.1/.github/workflows/publish-to-test-pypi.yml`

 * *Files 0% similar despite different names*

```diff
@@ -17,18 +17,18 @@
         fetch-depth: 0
     - run: |
         git fetch origin +refs/tags/*:refs/tags/*
     - name: Set Job Env
       uses: Chik-Network/actions/setjobenv@main
       env:
         GH_TOKEN: ${{ secrets.GITHUB_TOKEN }}
-    - name: Set up Python 3.7
+    - name: Set up Python 3.8.1
       uses: actions/setup-python@v4
       with:
-        python-version: "3.7"
+        python-version: "3.8.1"
     - name: Install build tools (pep517 compatible)
       run: >-
         python -m
         pip install ."[dev]"
         build
         --user
     - name: Build a binary wheel and a source tarball
```

### Comparing `chik_dev_tools-1.2.0/.github/workflows/run-test-suite.yml.bak` & `chik_dev_tools-1.2.1/.github/workflows/run-test-suite.yml.bak`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.0/.github/workflows/super-linter.yml.bak` & `chik_dev_tools-1.2.1/.github/workflows/super-linter.yml.bak`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.0/.github/workflows/test-blockchain-main.yml.bak` & `chik_dev_tools-1.2.1/.github/workflows/test-blockchain-main.yml.bak`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.0/.markdown-lint.yml` & `chik_dev_tools-1.2.1/.markdown-lint.yml`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.0/.pre-commit-config.yaml` & `chik_dev_tools-1.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.0/LICENSE` & `chik_dev_tools-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.0/PKG-INFO` & `chik_dev_tools-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chik_dev_tools
-Version: 1.2.0
+Version: 1.2.1
 Summary: Chik development commands
 Home-page: https://github.com/Chik-Network
 Author: Quexington
 Author-email: admin@chiknetwork.com
 License: https://opensource.org/licenses/Apache-2.0
 Project-URL: Bug Reports, https://github.com/Chik-Network/chik-dev-tools
 Project-URL: Source, https://github.com/Chik-Network/chik-dev-tools
```

### Comparing `chik_dev_tools-1.2.0/README.md` & `chik_dev_tools-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.0/activated.py` & `chik_dev_tools-1.2.1/activated.py`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.0/cdv/clibs/condition_codes.clib` & `chik_dev_tools-1.2.1/cdv/clibs/condition_codes.clib`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.0/cdv/clibs/curry_and_treehash.clib` & `chik_dev_tools-1.2.1/cdv/clibs/curry_and_treehash.clib`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.0/cdv/clibs/singleton_truths.clib` & `chik_dev_tools-1.2.1/cdv/clibs/singleton_truths.clib`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.0/cdv/cmds/chik_inspect.py` & `chik_dev_tools-1.2.1/cdv/cmds/chik_inspect.py`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.0/cdv/cmds/cli.py` & `chik_dev_tools-1.2.1/cdv/cmds/cli.py`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.0/cdv/cmds/clsp.py` & `chik_dev_tools-1.2.1/cdv/cmds/clsp.py`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.0/cdv/cmds/rpc.py` & `chik_dev_tools-1.2.1/cdv/cmds/rpc.py`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.0/cdv/cmds/util.py` & `chik_dev_tools-1.2.1/cdv/cmds/util.py`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.0/cdv/examples/clsp/piggybank.clsp` & `chik_dev_tools-1.2.1/cdv/examples/clsp/piggybank.clsp`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.0/cdv/examples/drivers/piggybank_drivers.py` & `chik_dev_tools-1.2.1/cdv/examples/drivers/piggybank_drivers.py`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.0/cdv/examples/tests/test_piggybank.py` & `chik_dev_tools-1.2.1/cdv/examples/tests/test_piggybank.py`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.0/cdv/test/__init__.py` & `chik_dev_tools-1.2.1/cdv/test/__init__.py`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.0/cdv/util/keys.py` & `chik_dev_tools-1.2.1/cdv/util/keys.py`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.0/cdv/util/load_klvm.py` & `chik_dev_tools-1.2.1/cdv/util/load_klvm.py`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.0/chik_dev_tools.egg-info/PKG-INFO` & `chik_dev_tools-1.2.1/chik_dev_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chik-dev-tools
-Version: 1.2.0
+Version: 1.2.1
 Summary: Chik development commands
 Home-page: https://github.com/Chik-Network
 Author: Quexington
 Author-email: admin@chiknetwork.com
 License: https://opensource.org/licenses/Apache-2.0
 Project-URL: Bug Reports, https://github.com/Chik-Network/chik-dev-tools
 Project-URL: Source, https://github.com/Chik-Network/chik-dev-tools
```

### Comparing `chik_dev_tools-1.2.0/chik_dev_tools.egg-info/SOURCES.txt` & `chik_dev_tools-1.2.1/chik_dev_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.0/mypy.ini` & `chik_dev_tools-1.2.1/mypy.ini`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.0/pyproject.toml` & `chik_dev_tools-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.0/setup.py` & `chik_dev_tools-1.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 dependencies = [
     "packaging",
     "pytest",
     "pytest-asyncio",
     "pytimeparse",
     "anyio",
-    "chik-blockchain==1.8.3rc1",
+    "chik-blockchain==1.8.5",
 ]
 
 dev_dependencies = [
     "anyio",
     "flake8",
     "mypy",
     "types-aiofiles",
```

### Comparing `chik_dev_tools-1.2.0/tests/build-init-files.py` & `chik_dev_tools-1.2.1/tests/build-init-files.py`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.0/tests/cmds/object_files/spendbundles/spendbundle.json` & `chik_dev_tools-1.2.1/tests/cmds/object_files/spendbundles/spendbundle.json`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.0/tests/cmds/object_files/spendbundles/spendbundle_invalid.json` & `chik_dev_tools-1.2.1/tests/cmds/object_files/spendbundles/spendbundle_invalid.json`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.0/tests/cmds/test_cdv.py` & `chik_dev_tools-1.2.1/tests/cmds/test_cdv.py`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.0/tests/cmds/test_clsp.py` & `chik_dev_tools-1.2.1/tests/cmds/test_clsp.py`

 * *Files identical despite different names*

### Comparing `chik_dev_tools-1.2.0/tests/cmds/test_inspect.py` & `chik_dev_tools-1.2.1/tests/cmds/test_inspect.py`

 * *Files identical despite different names*

