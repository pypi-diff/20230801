# Comparing `tmp/python-kraken-sdk-1.5.0.tar.gz` & `tmp/python-kraken-sdk-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-kraken-sdk-1.5.0.tar", last modified: Sun Jul 16 13:19:08 2023, max compression
+gzip compressed data, was "python-kraken-sdk-1.6.0.tar", last modified: Tue Aug  1 18:14:49 2023, max compression
```

## Comparing `python-kraken-sdk-1.5.0.tar` & `python-kraken-sdk-1.6.0.tar`

### file list

```diff
@@ -1,142 +1,149 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.290067 python-kraken-sdk-1.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.274067 python-kraken-sdk-1.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.274067 python-kraken-sdk-1.5.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/self-review.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.278067 python-kraken-sdk-1.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/workflows/_build.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/workflows/_build_doc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/workflows/_codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/workflows/_codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/workflows/_pre_commit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/workflows/_pypi_publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/workflows/_test_futures_private.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/workflows/_test_futures_public.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/workflows/_test_spot_private.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/workflows/_test_spot_public.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/workflows/cicd.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/workflows/manual_build.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/workflows/manual_codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/workflows/manual_pre_commit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/workflows/manual_test_futures.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/workflows/manual_test_spot.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    21607 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    21585 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    33066 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    54493 2023-07-16 13:19:08.290067 python-kraken-sdk-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14838 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.278067 python-kraken-sdk-1.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/docs/links.rst
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.278067 python-kraken-sdk-1.5.0/docs/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.278067 python-kraken-sdk-1.5.0/docs/src/about/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/docs/src/about/license.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.278067 python-kraken-sdk-1.5.0/docs/src/base_api/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/docs/src/base_api/base_api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.278067 python-kraken-sdk-1.5.0/docs/src/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/docs/src/examples/futures_bot_template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/docs/src/examples/spot_bot_template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/docs/src/examples/spot_orderbook.rst
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/docs/src/examples/trading_bot_templates.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.282067 python-kraken-sdk-1.5.0/docs/src/futures/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/docs/src/futures/rest.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/docs/src/futures/websockets.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.282067 python-kraken-sdk-1.5.0/docs/src/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/docs/src/getting_started/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/docs/src/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/docs/src/issues.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.282067 python-kraken-sdk-1.5.0/docs/src/krakenexceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/docs/src/krakenexceptions/krakenexceptions.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.282067 python-kraken-sdk-1.5.0/docs/src/spot/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/docs/src/spot/rest.rst
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/docs/src/spot/websockets.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.282067 python-kraken-sdk-1.5.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/examples/futures_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/examples/futures_trading_bot_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/examples/futures_ws_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)   364081 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/examples/market_client_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/examples/spot_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/examples/spot_orderbook.py
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/examples/spot_trading_bot_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/examples/spot_ws_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.282067 python-kraken-sdk-1.5.0/kraken/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/kraken/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-16 13:19:08.000000 python-kraken-sdk-1.5.0/kraken/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.282067 python-kraken-sdk-1.5.0/kraken/base_api/
--rw-r--r--   0 runner    (1001) docker     (123)    21542 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/kraken/base_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.282067 python-kraken-sdk-1.5.0/kraken/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/kraken/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.286067 python-kraken-sdk-1.5.0/kraken/futures/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/kraken/futures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/kraken/futures/funding.py
--rw-r--r--   0 runner    (1001) docker     (123)    39217 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/kraken/futures/market.py
--rw-r--r--   0 runner    (1001) docker     (123)    26338 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/kraken/futures/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)    34957 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/kraken/futures/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.286067 python-kraken-sdk-1.5.0/kraken/futures/websocket/
--rw-r--r--   0 runner    (1001) docker     (123)    10714 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/kraken/futures/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14235 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/kraken/futures/ws_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.286067 python-kraken-sdk-1.5.0/kraken/spot/
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/kraken/spot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14957 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/kraken/spot/funding.py
--rw-r--r--   0 runner    (1001) docker     (123)    15419 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/kraken/spot/market.py
--rw-r--r--   0 runner    (1001) docker     (123)    13906 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/kraken/spot/orderbook.py
--rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/kraken/spot/staking.py
--rw-r--r--   0 runner    (1001) docker     (123)    28957 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/kraken/spot/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)    39336 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/kraken/spot/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.286067 python-kraken-sdk-1.5.0/kraken/spot/websocket/
--rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/kraken/spot/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26546 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/kraken/spot/ws_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.286067 python-kraken-sdk-1.5.0/python_kraken_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    54493 2023-07-16 13:19:08.000000 python-kraken-sdk-1.5.0/python_kraken_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-16 13:19:08.000000 python-kraken-sdk-1.5.0/python_kraken_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 13:19:08.000000 python-kraken-sdk-1.5.0/python_kraken_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-16 13:19:08.000000 python-kraken-sdk-1.5.0/python_kraken_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-16 13:19:08.000000 python-kraken-sdk-1.5.0/python_kraken_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 13:19:08.290067 python-kraken-sdk-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.286067 python-kraken-sdk-1.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.290067 python-kraken-sdk-1.5.0/tests/futures/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/tests/futures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/tests/futures/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/tests/futures/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/tests/futures/test_futures_base_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/tests/futures/test_futures_funding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8714 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/tests/futures/test_futures_market.py
--rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/tests/futures/test_futures_trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/tests/futures/test_futures_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/tests/futures/test_futures_websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.290067 python-kraken-sdk-1.5.0/tests/spot/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/tests/spot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/tests/spot/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:19:08.290067 python-kraken-sdk-1.5.0/tests/spot/fixture/
--rw-r--r--   0 runner    (1001) docker     (123)    22315 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/tests/spot/fixture/orderbook.json
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/tests/spot/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/tests/spot/test_spot_base_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/tests/spot/test_spot_funding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/tests/spot/test_spot_market.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/tests/spot/test_spot_orderbook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/tests/spot/test_spot_staking.py
--rw-r--r--   0 runner    (1001) docker     (123)    11290 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/tests/spot/test_spot_trade.py
--rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/tests/spot/test_spot_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    17385 2023-07-16 13:18:55.000000 python-kraken-sdk-1.5.0/tests/spot/test_spot_websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.809612 python-kraken-sdk-1.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.797612 python-kraken-sdk-1.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.797612 python-kraken-sdk-1.6.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/self-review.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.797612 python-kraken-sdk-1.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/workflows/_build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/workflows/_build_doc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/workflows/_codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/workflows/_codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/workflows/_pre_commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/workflows/_pypi_publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/workflows/_test_futures_private.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/workflows/_test_futures_public.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/workflows/_test_spot_private.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/workflows/_test_spot_public.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/workflows/cicd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/workflows/manual_build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/workflows/manual_codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/workflows/manual_pre_commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/workflows/manual_test_futures.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/workflows/manual_test_spot.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    23697 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    33064 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    56406 2023-08-01 18:14:49.809612 python-kraken-sdk-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16753 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.801612 python-kraken-sdk-1.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/docs/links.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.801612 python-kraken-sdk-1.6.0/docs/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.801612 python-kraken-sdk-1.6.0/docs/src/about/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/docs/src/about/license.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.801612 python-kraken-sdk-1.6.0/docs/src/base_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/docs/src/base_api/base_api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.801612 python-kraken-sdk-1.6.0/docs/src/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/docs/src/examples/futures_bot_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/docs/src/examples/futures_ws_examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/docs/src/examples/spot_bot_templates.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/docs/src/examples/spot_orderbook.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/docs/src/examples/spot_ws_examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/docs/src/examples/trading_bot_templates.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.801612 python-kraken-sdk-1.6.0/docs/src/futures/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/docs/src/futures/rest.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/docs/src/futures/websockets.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.801612 python-kraken-sdk-1.6.0/docs/src/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/docs/src/getting_started/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/docs/src/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/docs/src/issues.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.801612 python-kraken-sdk-1.6.0/docs/src/krakenexceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/docs/src/krakenexceptions/krakenexceptions.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.801612 python-kraken-sdk-1.6.0/docs/src/spot/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/docs/src/spot/rest.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/docs/src/spot/websockets.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.801612 python-kraken-sdk-1.6.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/examples/futures_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/examples/futures_trading_bot_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/examples/futures_ws_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)   364081 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/examples/market_client_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/examples/spot_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/examples/spot_orderbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/examples/spot_trading_bot_template_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8538 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/examples/spot_trading_bot_template_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/examples/spot_ws_examples_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/examples/spot_ws_examples_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.805612 python-kraken-sdk-1.6.0/kraken/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/kraken/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-01 18:14:49.000000 python-kraken-sdk-1.6.0/kraken/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.805612 python-kraken-sdk-1.6.0/kraken/base_api/
+-rw-r--r--   0 runner    (1001) docker     (123)    22158 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/kraken/base_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.805612 python-kraken-sdk-1.6.0/kraken/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/kraken/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.805612 python-kraken-sdk-1.6.0/kraken/futures/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/kraken/futures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/kraken/futures/funding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39483 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/kraken/futures/market.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26413 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/kraken/futures/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35226 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/kraken/futures/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.805612 python-kraken-sdk-1.6.0/kraken/futures/websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)    11207 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/kraken/futures/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14541 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/kraken/futures/ws_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.805612 python-kraken-sdk-1.6.0/kraken/spot/
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/kraken/spot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15198 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/kraken/spot/funding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15711 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/kraken/spot/market.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14501 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/kraken/spot/orderbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9777 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/kraken/spot/staking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29168 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/kraken/spot/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41526 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/kraken/spot/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.805612 python-kraken-sdk-1.6.0/kraken/spot/websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/kraken/spot/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20107 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/kraken/spot/websocket/connectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27560 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/kraken/spot/websocket_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20755 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/kraken/spot/websocket_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7958 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.805612 python-kraken-sdk-1.6.0/python_kraken_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    56406 2023-08-01 18:14:49.000000 python-kraken-sdk-1.6.0/python_kraken_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-08-01 18:14:49.000000 python-kraken-sdk-1.6.0/python_kraken_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 18:14:49.000000 python-kraken-sdk-1.6.0/python_kraken_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-01 18:14:49.000000 python-kraken-sdk-1.6.0/python_kraken_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-01 18:14:49.000000 python-kraken-sdk-1.6.0/python_kraken_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 18:14:49.809612 python-kraken-sdk-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.805612 python-kraken-sdk-1.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.809612 python-kraken-sdk-1.6.0/tests/futures/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/futures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/futures/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/futures/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/futures/test_futures_base_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/futures/test_futures_funding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/futures/test_futures_market.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8059 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/futures/test_futures_trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/futures/test_futures_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/futures/test_futures_websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.809612 python-kraken-sdk-1.6.0/tests/spot/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/spot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/spot/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:14:49.809612 python-kraken-sdk-1.6.0/tests/spot/fixture/
+-rw-r--r--   0 runner    (1001) docker     (123)   204293 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/spot/fixture/orderbook.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/spot/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/spot/test_spot_base_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/spot/test_spot_funding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/spot/test_spot_market.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/spot/test_spot_orderbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/spot/test_spot_staking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11690 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/spot/test_spot_trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12746 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/spot/test_spot_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/spot/test_spot_websocket_internals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27928 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/spot/test_spot_websocket_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-08-01 18:14:39.000000 python-kraken-sdk-1.6.0/tests/spot/test_spot_websocket_v2.py
```

### Comparing `python-kraken-sdk-1.5.0/.github/ISSUE_TEMPLATE/bug_report.md` & `python-kraken-sdk-1.6.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.5.0/.github/ISSUE_TEMPLATE/feature_request.md` & `python-kraken-sdk-1.6.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.5.0/.github/codecov.yml` & `python-kraken-sdk-1.6.0/.github/codecov.yml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.5.0/.github/pull_request_template.md` & `python-kraken-sdk-1.6.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.5.0/.github/release.yaml` & `python-kraken-sdk-1.6.0/.github/release.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) 2023 Benjamin Thomas Schwertfeger
 # GitHub: https://github.com/btschwertfeger
 #
-# Based on https://docs.github.com/en/repositories/releasing-projects-on-github/automatically-generated-release-notes
+# Config file to auto-generate release notes based on
+# https://docs.github.com/en/repositories/releasing-projects-on-github/automatically-generated-release-notes
 
 changelog:
   exclude:
     # labels:
     #   - ignore-for-release
     # authors:
     #   - john-doe
   categories:
-    - title: Breaking Changes 🛠
+    - title: Breaking Changes ⚠️
       labels:
         - breaking
         - Breaking
     - title: Implemented Enhancements 🎉
       labels:
         - Feature
         - enhancement
```

### Comparing `python-kraken-sdk-1.5.0/.github/self-review.md` & `python-kraken-sdk-1.6.0/.github/self-review.md`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.5.0/.github/workflows/_build.yaml` & `python-kraken-sdk-1.6.0/.github/workflows/_build.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -34,9 +34,21 @@
         run: |
           python -m pip install --upgrade pip
           python -m pip install build
 
       - name: Build the package
         run: python -m build --outdir .
 
-      - name: Install the package
+      - name: Install the package on Linux or MacOS
+        if: runner.os != 'Windows'
         run: python -m pip install python_kraken_sdk*.whl
+
+      - name: Install the package on Windows
+        if: runner.os == 'Windows'
+        run: |
+          try {
+              $WHEEL = Get-ChildItem -Path . -Filter "python_kraken_sdk*.whl" -ErrorAction Stop
+              python -m pip install $WHEEL
+          } catch {
+              Write-Error "Error: .whl file not found in the current directory."
+              exit 1
+          }
```

### Comparing `python-kraken-sdk-1.5.0/.github/workflows/_build_doc.yaml` & `python-kraken-sdk-1.6.0/.github/workflows/_build_doc.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.5.0/.github/workflows/_codecov.yaml` & `python-kraken-sdk-1.6.0/.github/workflows/_codecov.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.5.0/.github/workflows/_codeql.yaml` & `python-kraken-sdk-1.6.0/.github/workflows/_codeql.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.5.0/.github/workflows/_pypi_publish.yaml` & `python-kraken-sdk-1.6.0/.github/workflows/_pypi_publish.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.5.0/.github/workflows/_test_futures_private.yaml` & `python-kraken-sdk-1.6.0/.github/workflows/_test_futures_private.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.5.0/.github/workflows/_test_futures_public.yaml` & `python-kraken-sdk-1.6.0/.github/workflows/_test_futures_public.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.5.0/.github/workflows/_test_spot_private.yaml` & `python-kraken-sdk-1.6.0/.github/workflows/_test_spot_private.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # GitHub: https://github.com/btschwertfeger
 #
 # Template workflow to test the private Spot endpoints of the
 # python-kraken-sdk.
 #
 # Runs tests for:
 #   * Spot REST clients
-#   * Spot websocket client
+#   * Spot websocket clients
 #
 
 name: Test Spot
 
 on:
   workflow_call:
     inputs:
@@ -44,24 +44,24 @@
         run: |
           python -m pip install --upgrade pip
           python -m pip install pytest
 
       - name: Install package
         run: python -m pip install .
 
-      ##    Unit tests of the private Spot REST clients and endpoints
+      ##    Unit tests of private Spot REST clients and endpoints
       ##
       - name: Testing Spot REST endpoints
         env:
           SPOT_API_KEY: ${{ secrets.SPOT_API_KEY }}
           SPOT_SECRET_KEY: ${{ secrets.SPOT_SECRET_KEY }}
         run: |
           pytest -vv -m "spot_auth and not spot_websocket" tests
 
-      ##    Unit tests of the Spot websocket client
+      ##    Unit tests of Spot websocket clients
       ##
       - name: Testing Spot websocket client
         env:
           SPOT_API_KEY: ${{ secrets.SPOT_API_KEY }}
           SPOT_SECRET_KEY: ${{ secrets.SPOT_SECRET_KEY }}
         run: |
           pytest -vv -m spot_websocket tests
```

### Comparing `python-kraken-sdk-1.5.0/.github/workflows/_test_spot_public.yaml` & `python-kraken-sdk-1.6.0/.github/workflows/_test_spot_public.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.5.0/.github/workflows/cicd.yaml` & `python-kraken-sdk-1.6.0/.github/workflows/cicd.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -69,17 +69,17 @@
   ##    Builds the package on multiple OS for multiple
   ##    Python versions
   ##
   Build:
     needs: [Pre-Commit]
     uses: ./.github/workflows/_build.yaml
     strategy:
-      fail-fast: false
+      fail-fast: true
       matrix:
-        os: [ubuntu-latest, macos-latest] #, windows-latest]
+        os: [ubuntu-latest, macos-latest, windows-latest]
         python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
     with:
       os: ${{ matrix.os }}
       python-version: ${{ matrix.python-version }}
 
   ## ==========================================================================
   ##    Build the documentation
@@ -112,15 +112,15 @@
   Test-Spot-Private:
     needs: [Build]
     uses: ./.github/workflows/_test_spot_private.yaml
     strategy:
       max-parallel: 1 # to avoid failing tests because of API Rate limits
       fail-fast: false
       matrix:
-        os: [ubuntu-latest]
+        os: [ubuntu-latest] # only ubuntu since this takes to much time ATM
         python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
     with:
       os: ${{ matrix.os }}
       python-version: ${{ matrix.python-version }}
     secrets: inherit
 
   ## ==========================================================================
@@ -143,51 +143,47 @@
   Test-Futures-Private:
     needs: [Build]
     uses: ./.github/workflows/_test_futures_private.yaml
     strategy:
       max-parallel: 1 # to avoid failing tests because of API Rate limits
       fail-fast: false
       matrix:
-        os: [ubuntu-latest]
+        os: [ubuntu-latest, windows-latest]
         python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
     with:
       os: ${{ matrix.os }}
       python-version: ${{ matrix.python-version }}
     secrets: inherit
 
   ## ==========================================================================
   ##    Uploads the package to test.pypi.org on master if triggered by
   ##    a regular commit/push.
   ##
   UploadTestPyPI:
     if: success() && github.actor == 'btschwertfeger' && github.ref == 'refs/heads/master'
     needs:
-      [
-        Test-Spot-Public,
-        Test-Spot-Private,
-        Test-Futures-Public,
-        Test-Futures-Private,
-      ]
+      - Test-Spot-Public
+      - Test-Spot-Private
+      - Test-Futures-Public
+      - Test-Futures-Private
     name: Upload current development version to Test PyPI
     uses: ./.github/workflows/_pypi_publish.yaml
     with:
       REPOSITORY_URL: https://test.pypi.org/legacy/
     secrets:
       API_TOKEN: ${{ secrets.TEST_PYPI_API_TOKEN }}
 
   ## ==========================================================================
   ##    Generates and uploads the coverage statistics to codecov
   ##
   CodeCov:
     if: success() && github.actor == 'btschwertfeger'
     needs:
-      [
-        Test-Spot-Public,
-        Test-Spot-Private,
-        Test-Futures-Public,
-        Test-Futures-Private,
-      ]
+      - Test-Spot-Public
+      - Test-Spot-Private
+      - Test-Futures-Public
+      - Test-Futures-Private
     uses: ./.github/workflows/_codecov.yaml
     with:
       os: "ubuntu-latest"
       python-version: "3.11"
     secrets: inherit
```

### Comparing `python-kraken-sdk-1.5.0/.github/workflows/manual_build.yaml` & `python-kraken-sdk-1.6.0/.github/workflows/manual_build.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.5.0/.github/workflows/manual_test_futures.yaml` & `python-kraken-sdk-1.6.0/.github/workflows/manual_test_futures.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.5.0/.github/workflows/manual_test_spot.yaml` & `python-kraken-sdk-1.6.0/.github/workflows/manual_test_spot.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.5.0/.github/workflows/release.yaml` & `python-kraken-sdk-1.6.0/.github/workflows/release.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -30,17 +30,17 @@
   ## ==========================================================================
   ##    Build the package - for all Python versions
   ##
   Build:
     uses: ./.github/workflows/_build.yaml
     needs: [Pre-Commit]
     strategy:
-      fail-fast: false
+      fail-fast: true
       matrix:
-        os: [macos-latest, ubuntu-latest] #, windows-latest]
+        os: [macos-latest, ubuntu-latest, windows-latest]
         python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
     with:
       os: ${{ matrix.os }}
       python-version: ${{ matrix.python-version }}
 
   ## ==========================================================================
   ##    Build the documentation
@@ -59,15 +59,15 @@
   ##
   Test-Spot-Public:
     needs: [Build]
     uses: ./.github/workflows/_test_spot_public.yaml
     strategy:
       fail-fast: false
       matrix:
-        os: [ubuntu-latest]
+        os: [ubuntu-latest, windows-latest]
         python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
     with:
       os: ${{ matrix.os }}
       python-version: ${{ matrix.python-version }}
   ##
   ##  (private endpoints)
   Test-Spot-Private:
@@ -90,46 +90,44 @@
   ##  (public endpoints)
   Test-Futures-Public:
     needs: [Build]
     uses: ./.github/workflows/_test_futures_public.yaml
     strategy:
       fail-fast: false
       matrix:
-        os: [ubuntu-latest]
+        os: [ubuntu-latest, windows-latest]
         python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
     with:
       os: ${{ matrix.os }}
       python-version: ${{ matrix.python-version }}
   ##
   ##  (private endpoints)
   Test-Futures-Private:
     needs: [Build]
     uses: ./.github/workflows/_test_futures_private.yaml
     strategy:
       max-parallel: 1 # to avoid failing tests because of API Rate limits
       fail-fast: false
       matrix:
-        os: [ubuntu-latest]
+        os: [ubuntu-latest, windows-latest]
         python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
     with:
       os: ${{ matrix.os }}
       python-version: ${{ matrix.python-version }}
     secrets: inherit
 
   ## ==========================================================================
   ##    Upload the python-kraken-sdk to Test PyPI
   ##
   UploadTestPyPI:
     needs:
-      [
-        Test-Spot-Public,
-        Test-Spot-Private,
-        Test-Futures-Public,
-        Test-Futures-Private,
-      ]
+      - Test-Spot-Public
+      - Test-Spot-Private
+      - Test-Futures-Public
+      - Test-Futures-Private
     name: Upload the current release to Test PyPI
     uses: ./.github/workflows/_pypi_publish.yaml
     with:
       REPOSITORY_URL: https://test.pypi.org/legacy/
     secrets:
       API_TOKEN: ${{ secrets.TEST_PYPI_API_TOKEN }}
```

### Comparing `python-kraken-sdk-1.5.0/.gitignore` & `python-kraken-sdk-1.6.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 # Unit test / coverage reports
 htmlcov/
 .tox/
 .nox/
 .coverage
 .coverage.*
 .cache
+.ruff_cache
 nosetests.xml
 coverage.xml
 pytest.xml
 *.cover
 *.py,cover
 .hypothesis/
 .pytest_cache/
```

### Comparing `python-kraken-sdk-1.5.0/.readthedocs.yaml` & `python-kraken-sdk-1.6.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.5.0/CHANGELOG.md` & `python-kraken-sdk-1.6.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,45 @@
 # Changelog
 
 ## [Unreleased](https://github.com/btschwertfeger/python-kraken-sdk/tree/HEAD)
 
-[Full Changelog](https://github.com/btschwertfeger/python-kraken-sdk/compare/v1.4.1...HEAD)
+[Full Changelog](https://github.com/btschwertfeger/python-kraken-sdk/compare/v1.5.0...HEAD)
+
+**Breaking changes:**
+
+- Integrate Websockets API v2 [\#130](https://github.com/btschwertfeger/python-kraken-sdk/issues/130)
+- Let `kraken.spot.OrderbookClient` use Spot Websocket API v2 [\#139](https://github.com/btschwertfeger/python-kraken-sdk/pull/139) ([btschwertfeger](https://github.com/btschwertfeger))
+- Integrate Kraken Websockets API v2; add `kraken.spot.KrakenSpotWebsocketClientV2`; internals [\#131](https://github.com/btschwertfeger/python-kraken-sdk/pull/131) ([btschwertfeger](https://github.com/btschwertfeger))
+
+**Implemented enhancements:**
+
+- Add `/private/AccountTransfer` endpoint to `kraken.spot.User` [\#128](https://github.com/btschwertfeger/python-kraken-sdk/issues/128)
+- Add `/private/AccountTransfer` endpoint -\> `kraken.spot.User.account_transfer` [\#129](https://github.com/btschwertfeger/python-kraken-sdk/pull/129) ([btschwertfeger](https://github.com/btschwertfeger))
+
+**Closed issues:**
+
+- The content of `.pylintrc` can be moved into `pyproject.toml` [\#136](https://github.com/btschwertfeger/python-kraken-sdk/issues/136)
+- Build the package also on Windows within the CI [\#134](https://github.com/btschwertfeger/python-kraken-sdk/issues/134)
+
+Uncategorized merged pull requests:
+
+- Merge `.pylintrc` and `pyproject.toml` [\#137](https://github.com/btschwertfeger/python-kraken-sdk/pull/137) ([btschwertfeger](https://github.com/btschwertfeger))
+- Enable Windows builds within the CI [\#135](https://github.com/btschwertfeger/python-kraken-sdk/pull/135) ([btschwertfeger](https://github.com/btschwertfeger))
+
+## [v1.5.0](https://github.com/btschwertfeger/python-kraken-sdk/tree/v1.5.0) (2023-07-16)
+
+[Full Changelog](https://github.com/btschwertfeger/python-kraken-sdk/compare/v1.4.1...v1.5.0)
+
+**Breaking changes:**
+
+- `kraken.spot.OrderbookClient`: add timestamps to book's ask and bid values [\#124](https://github.com/btschwertfeger/python-kraken-sdk/pull/124) ([btschwertfeger](https://github.com/btschwertfeger))
 
 Uncategorized merged pull requests:
 
+- Adjust project properties [\#123](https://github.com/btschwertfeger/python-kraken-sdk/pull/123) ([btschwertfeger](https://github.com/btschwertfeger))
 - Add "Question" issue template [\#122](https://github.com/btschwertfeger/python-kraken-sdk/pull/122) ([btschwertfeger](https://github.com/btschwertfeger))
 
 ## [v1.4.1](https://github.com/btschwertfeger/python-kraken-sdk/tree/v1.4.1) (2023-06-28)
 
 [Full Changelog](https://github.com/btschwertfeger/python-kraken-sdk/compare/v1.4.0...v1.4.1)
 
 **Fixed bugs:**
```

### Comparing `python-kraken-sdk-1.5.0/CODE_OF_CONDUCT.md` & `python-kraken-sdk-1.6.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.5.0/CONTRIBUTING.md` & `python-kraken-sdk-1.6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.5.0/LICENSE` & `python-kraken-sdk-1.6.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -617,16 +617,16 @@
 an absolute waiver of all civil liability in connection with the
 Program, unless a warranty or assumption of liability accompanies a
 copy of the Program in return for a fee.
 
                      END OF TERMS AND CONDITIONS
 
     The python-kraken-sdk serves as a collection of REST and websocket
-    clients to interact with the Kraken cryptocurrency exchange to
-    access the Spot and Futures API.
+    clients to interact with the Kraken cryptocurrency exchange using it's Spot
+    and Futures APIs.
     Copyright (C) 2023 Benjamin Thomas Schwertfeger
 
     This program is free software: you can redistribute it and/or modify
     it under the terms of the GNU General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
```

### Comparing `python-kraken-sdk-1.5.0/Makefile` & `python-kraken-sdk-1.6.0/Makefile`

 * *Files 18% similar despite different names*

```diff
@@ -1,95 +1,112 @@
 #!make
 # -*- coding: utf-8 -*-
 # Copyright (C) 2023 Benjamin Thomas Schwertfeger
 # GitHub: https://github.com/btschwertfeger
 
 PYTHON := python
-
 PYTEST := $(PYTHON) -m pytest
 PYTEST_OPTS := -vv --junit-xml=pytest.xml
 PYTEST_COV_OPTS := $(PYTEST_OPTS) --cov --cov-report=xml:coverage.xml --cov-report=term
 TEST_DIR := tests
 
-.PHONY := build dev install test tests coverage doc doctest clean changelog pre-commit
+.PHONY := help build rebuild doc install dev test tests test-wip coverage doctest pre-commit ruff ruff-fix changelog clean
 
 help:
 	@grep "^##" Makefile | sed -e "s/##//"
 
 ## ======= B U I L D I N G =======
 ## build		Builds the python-kraken-sdk
 ##
 build:
 	$(PYTHON) -m build .
 
 rebuild: clean build
 
-## dev		Installs the extended package in edit mode
-##
-dev:
-	$(PYTHON) -m pip install -e ".[dev]"
-
 ## doc		Build the documentation
 ##
 doc:
 	cd docs && make html
 
 ## ======= I N S T A L L A T I O N =======
 ## install	Install the package
 ##
 install:
 	$(PYTHON) -m pip install .
 
+## dev		Installs the extended package in edit mode
+##
+dev:
+	$(PYTHON) -m pip install -e ".[dev]"
+
 ## ======= T E S T I N G =======
 ## test		Run the unit tests
 ##
 test:
+	@rm *.log || true
 	$(PYTEST) $(PYTEST_OPTS) $(TEST_DIR)
 
+
 tests: test
 
+## test-wip		Run tests marked as 'wip'
+##
 test-wip:
+	@rm *.log || true
 	$(PYTEST) -m "wip" -vv $(TEST_DIR)
 
+## coverage		Run all tests and generate the coverage report
+##
 coverage:
+	@rm *.log || true
 	$(PYTEST) $(PYTEST_COV_OPTS) $(TEST_DIR)
 
-## doctest	Run the documentation tests
+## doctest	Run the documentation related tests
 ##
 doctest:
 	cd docs && make doctest
 
 ## ======= M I S C E L A N I O U S =======
 ## pre-commit	Run the pre-commit targets
 ##
 pre-commit:
 	@pre-commit run -a
 
+## ruff 	Run ruff without fix
+ruff:
+	ruff check .
+
+## ruff-fix 	Run ruff with fix
+ruff-fix:
+	ruff check . --fix
+
 ## changelog	Generate the changelog
 ##
 changelog:
 	docker run -it --rm \
 		-v $(PWD):/usr/local/src/your-app \
 		githubchangeloggenerator/github-changelog-generator \
 		--user btschwertfeger \
 		--project python-kraken-sdk \
 		--token $(GHTOKEN)  \
 		--breaking-labels Breaking \
-		--enhancement-labels Feature \
+		--enhancement-labels Feature,enhancement \
 		--release-branch master \
 		--pr-label "Uncategorized merged pull requests:"
 
 ## clean		Clean the workspace
 ##
 clean:
 	rm -rf .pytest_cache build/ dist/ \
 		python_kraken_sdk.egg-info \
 		docs/_build \
 		.vscode \
-		.mypy_cache
+		.cache \
+		.mypy_cache \
+		.ruff_cache
 
 	rm -f .coverage coverage.xml pytest.xml mypy.xml \
 		kraken/_version.py \
 		*.log *.csv *.zip \
 		tests/*.zip tests/.csv \
 		python_kraken_sdk-*.whl
```

### Comparing `python-kraken-sdk-1.5.0/PKG-INFO` & `python-kraken-sdk-1.6.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-kraken-sdk
-Version: 1.5.0
+Version: 1.6.0
 Summary: Collection of REST and websocket clients to interact with the Kraken cryptocurrency exchange.
 Author-email: Benjamin Thomas Schwertfeger <contact@b-schwertfeger.de>
 License: GNU GENERAL PUBLIC LICENSE
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
         Everyone is permitted to copy and distribute verbatim copies
@@ -622,16 +622,16 @@
         an absolute waiver of all civil liability in connection with the
         Program, unless a warranty or assumption of liability accompanies a
         copy of the Program in return for a fee.
         
                              END OF TERMS AND CONDITIONS
         
             The python-kraken-sdk serves as a collection of REST and websocket
-            clients to interact with the Kraken cryptocurrency exchange to
-            access the Spot and Futures API.
+            clients to interact with the Kraken cryptocurrency exchange using it's Spot
+            and Futures APIs.
             Copyright (C) 2023 Benjamin Thomas Schwertfeger
         
             This program is free software: you can redistribute it and/or modify
             it under the terms of the GNU General Public License as published by
             the Free Software Foundation, either version 3 of the License, or
             (at your option) any later version.
         
@@ -666,276 +666,327 @@
 Classifier: Operating System :: Unix
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: examples
 License-File: LICENSE
 
-<h1 align="center">Futures and Spot Websocket and REST API Python SDK for the Kraken Cryptocurrency Exchange 🐙</h1>
+<h1 align="center">Futures and Spot - REST and Websocket API Python SDK for the Kraken Cryptocurrency Exchange 🐙</h1>
 
 <div align="center">
 
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/btschwertfeger/python-kraken-sdk)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-orange.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Generic badge](https://img.shields.io/badge/python-3.7_|_3.8_|_3.9_|_3.10_|_3.11-blue.svg)](https://shields.io/)
 [![Downloads](https://static.pepy.tech/personalized-badge/python-kraken-sdk?period=total&units=abbreviation&left_color=grey&right_color=orange&left_text=downloads)](https://pepy.tech/project/python-kraken-sdk)
 
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Typing](https://img.shields.io/badge/typing-mypy-informational)](https://mypy-lang.org/)
 [![CodeQL](https://github.com/btschwertfeger/python-kraken-sdk/actions/workflows/codeql.yaml/badge.svg?branch=master)](https://github.com/btschwertfeger/python-kraken-sdk/actions/workflows/codeql.yaml)
 [![CI/CD](https://github.com/btschwertfeger/python-kraken-sdk/actions/workflows/cicd.yaml/badge.svg?branch=master)](https://github.com/btschwertfeger/python-kraken-sdk/actions/workflows/cicd.yaml)
 [![codecov](https://codecov.io/gh/btschwertfeger/python-kraken-sdk/branch/master/badge.svg)](https://app.codecov.io/gh/btschwertfeger/python-kraken-sdk)
 
 ![release](https://shields.io/github/release-date/btschwertfeger/python-kraken-sdk)
 [![release](https://img.shields.io/pypi/v/python-kraken-sdk)](https://pypi.org/project/python-kraken-sdk/)
 [![DOI](https://zenodo.org/badge/510751854.svg)](https://zenodo.org/badge/latestdoi/510751854)
 [![Documentation Status stable](https://readthedocs.org/projects/python-kraken-sdk/badge/?version=stable)](https://python-kraken-sdk.readthedocs.io/en/stable)
 
 </div>
 
-> ⚠️ This is an unofficial collection of REST and websocket clients for Spot and Futures trading on the Kraken cryptocurrency exchange using Python. Payward Ltd. and Kraken are in no way associated with the authors of this module and documentation.
+> ⚠️ This is an unofficial collection of REST and websocket clients for Spot and
+> Futures trading on the Kraken cryptocurrency exchange using Python. Payward
+> Ltd. and Kraken are in no way associated with the authors of this module and
+> documentation.
 
 ---
 
 ## 📌 Disclaimer
 
-There is no guarantee that this software will work flawlessly at this or later times. Of course, no responsibility is taken for possible profits or losses. This software probably has some errors in it, so use it at your own risk. Also no one should be motivated or tempted to invest assets in speculative forms of investment. By using this software you release the authors from any liability regarding the use of this software.
+There is no guarantee that this software will work flawlessly at this or later
+times. Of course, no responsibility is taken for possible profits or losses.
+This software probably has some errors in it, so use it at your own risk. Also
+no one should be motivated or tempted to invest assets in speculative forms of
+investment. By using this software you release the authors from any liability
+regarding the use of this software.
 
 ---
 
 ## Features
 
-Clients:
+Available Clients:
 
 - Spot REST Clients
-- Spot Websocket Client
+- Spot Websocket Clients (Websocket API v1 and v2)
 - Spot Orderbook Client
 - Futures REST Clients
 - Futures Websocket Client
 
 General:
 
-- access both public and private endpoints
+- access both public and private, REST and websocket endpoints
 - responsive error handling and custom exceptions
 - extensive example scripts (see `/examples` and `/tests`)
 - tested using the [pytest](https://docs.pytest.org/en/7.3.x/) framework
 - releases are permanently archived at [Zenodo](https://zenodo.org/badge/latestdoi/510751854)
 
 Documentation:
 
-- Stable: [https://python-kraken-sdk.readthedocs.io/en/stable](https://python-kraken-sdk.readthedocs.io/en/stable)
-- Latest: [https://python-kraken-sdk.readthedocs.io/en/latest](https://python-kraken-sdk.readthedocs.io/en/latest)
+- [https://python-kraken-sdk.readthedocs.io/en/stable](https://python-kraken-sdk.readthedocs.io/en/stable)
+- [https://python-kraken-sdk.readthedocs.io/en/latest](https://python-kraken-sdk.readthedocs.io/en/latest)
 
 ---
 
 ## ❗️ Attention
 
-**ONLY** tagged releases are available at PyPI. So the content of the master may not match with the content of the latest release. - Please have a look at the release specific READMEs and changelogs.
+**ONLY** tagged releases are available at PyPI. So the content of the master may
+not match with the content of the latest release. - Please have a look at the
+release specific READMEs and changelogs.
 
 ---
 
 ## Table of Contents
 
 - [ Installation and setup ](#installation)
-- [ Spot Client Example Usage ](#spotusage)
+- [ Spot Clients ](#spotusage)
   - [REST API](#spotrest)
-  - [Websockets](#spotws)
-- [ Futures Client Example Usage ](#futuresusage)
+  - [Websocket API V2](#spotws)
+- [ Futures Clients ](#futuresusage)
   - [REST API](#futuresrest)
-  - [Websockets](#futuresws)
+  - [Websocket API](#futuresws)
 - [ Troubleshooting ](#trouble)
 - [ Contributions ](#contribution)
 - [ Notes ](#notes)
 - [ References ](#references)
 
 ---
 
 <a name="installation"></a>
 
 # 🛠 Installation and setup
 
-### 1. Install the Python module:
+### 1. Install the package into the desired environment
 
 ```bash
 python3 -m pip install python-kraken-sdk
 ```
 
-### 2. Register at Kraken and generate API Keys:
+### 2. Register at [Kraken](https://www.kraken.com) and generate API keys
 
 - Spot Trading: https://www.kraken.com/u/security/api
 - Futures Trading: https://futures.kraken.com/trade/settings/api (see _[help](https://docs.futures.kraken.com/#introduction-generate-api-keys)_)
 - Futures Sandbox: https://demo-futures.kraken.com/settings/api
 
 ### 3. Start using the provided example scripts
 
 ### 4. Error handling
 
-If any unexpected behavior occurs, please check <b style="color: yellow">your API permissions</b>, <b style="color: yellow">rate limits</b>, update the python-kraken-sdk, see the [Troubleshooting](#trouble) section, and if the error persists please open an issue.
+If any unexpected behavior occurs, please check <b style="color: yellow">your
+API permissions</b>, <b style="color: yellow">rate limits</b>, update the
+python-kraken-sdk, see the [Troubleshooting](#trouble) section, and if the error
+persists please open an issue.
 
 ---
 
 <a name="spotusage"></a>
 
-# 📍 Spot Client Example Usage
+# 📍 Spot Clients
 
-A template Spot trading bot using both websocket and REST clients can be found in `/examples/spot_trading_bot_template.py`.
+A template for Spot trading using both websocket and REST clients can be
+found in `examples/spot_trading_bot_template_v2.py`.
 
-For those who need a realtime order book - a script that demonstrates how to maintain a valid order book can be found here: `/examples/spot_orderbook.py`.
+For those who need a realtime order book - a script that demonstrates how to
+maintain a valid order book using the Orderbook client can be found in
+`examples/spot_orderbook.py`.
 
 <a name="spotrest"></a>
 
 ## Spot REST API
 
-... can be found in `/examples/spot_examples.py`
+The Kraken Spot REST API offers many endpoints for almost every use-case. The
+python-kraken-sdk aims to provide all of them - split in User, Market,
+Trade, Funding and Staking related clients.
+
+The following code block demonstrates how to use some of them. More examples
+can be found in `examples/spot_examples.py`.
 
 ```python
 from kraken.spot import User, Market, Trade, Funding, Staking
 
 def main():
     key = "kraken-public-key"
     secret = "kraken-secret-key"
 
     # ____USER________________________
     user = User(key=key, secret=secret)
     print(user.get_account_balance())
     print(user.get_open_orders())
-    # ...
+    # …
 
     # ____MARKET____
     market = Market()
     print(market.get_ticker(pair="BTCUSD"))
-    # ...
+    # …
 
     # ____TRADE_________________________
     trade = Trade(key=key, secret=secret)
     print(trade.create_order(
          ordertype="limit",
          side="buy",
          volume=1,
          pair="BTC/EUR",
          price=20000
     ))
-    # ...
+    # …
 
     # ____FUNDING___________________________
     funding = Funding(key=key, secret=secret)
     print(
         funding.withdraw_funds(
             asset="DOT", key="MyPolkadotWallet", amount=200
         )
     )
     print(funding.cancel_withdraw(asset="DOT", refid="<some id>"))
-    # ...
+    # …
 
     # ____STAKING___________________________
     staking = Staking(key=key, secret=secret)
     print(staking.list_stakeable_assets())
     print(
         staking.stake_asset(
             asset="DOT", amount=20, method="polkadot-staked"
         )
     )
-    # ...
+    # …
 
 if __name__ == "__main__":
     main()
 ```
 
 <a name="spotws"></a>
 
-## Websockets
+## Spot Websocket API V2
+
+Kraken offers two versions of their websocket API (V1 and V2). Since V2 is
+offers more possibilities, is way faster and easier to use, only those examples
+are shown below. For using the websocket API V1 please have a look into the
+`examples/spot_ws_examples_v1.py`.
 
-... can be found in `/examples/spot_ws_examples.py`
+The documentation for both API versions can be found here:
+
+- https://docs.kraken.com/websockets
+- https://docs.kraken.com/websockets-v2
+
+Note that authenticated Spot websocket clients can also un-/subscribe from/to
+public feeds.
+
+The example below can be found in an extended way in
+`examples/spot_ws_examples_v2.py`.
 
 ```python
-import time
 import asyncio
-from kraken.spot import KrakenSpotWSClient
+from kraken.spot import KrakenSpotWSClientV2
 
-async def main()
+async def main():
+    key = "spot-api-key"
+    secret = "spot-secret-key"
 
-    key = "kraken-public-key"
-    secret = "kraken-secret-key"
+    class Client(KrakenSpotWSClientV2):
+        """Can be used to create a custom trading strategy"""
 
-    class Bot(KrakenSpotWSClient):
-        async def on_message(self, msg):
-            if isinstance(msg, dict) and "event" in msg:
-                if msg["event"] in ("pong", "heartbeat"):
-                    return
-
-            print(msg)
-            # if condition:
-            #     await self.create_order(
-            #         ordertype="limit",
-            #         side="buy",
-            #         pair="BTC/EUR",
-            #         price=20000,
-            #         volume=1
+        async def on_message(self, message):
+            """Receives the websocket messages"""
+            if message.get("method") == "pong" \
+                or message.get("channel") == "heartbeat":
+                return
+
+            print(message)
+            # here we can access lots of methods, for example to create an order:
+            # if self.is_auth:  # only if the client is authenticated …
+            #     await self.send_message(
+            #         message={
+            #             "method": "add_order",
+            #             "params": {
+            #                 "limit_price": 1234.56,
+            #                 "order_type": "limit",
+            #                 "order_userref": 123456789,
+            #                 "order_qty": 1.0,
+            #                 "side": "buy",
+            #                 "symbol": "BTC/USD",
+            #                 "validate": True,
+            #             },
+            #         }
             #     )
-            # ... it is also possible to call regular Spot REST endpoints
-            # but using the WsClient's functions is more efficient
-            # because the requests will be sent via the ws connection
-
-    # ___Public_Websocket_Feeds__
-    bot = Bot() # only use the unauthenticated client if you don't need private feeds
-    print(bot.public_sub_names) # list public subscription names
-
-    await bot.subscribe(subscription={ "name": "ticker" }, pair=["XBT/EUR", "DOT/EUR"])
-    await bot.subscribe(subscription={ "name": "spread" }, pair=["XBT/EUR", "DOT/EUR"])
-    # await bot.subscribe(subscription={ "name": "book" }, pair=["BTC/EUR"])
-    # await bot.subscribe(subscription={ "name": "book", "depth": 25}, pair=["BTC/EUR"])
-    # await bot.subscribe(subscription={ "name": "ohlc" }, pair=["BTC/EUR"])
-    # await bot.subscribe(subscription={ "name": "ohlc", "interval": 15}, pair=["XBT/EUR", "DOT/EUR"])
-    # await bot.subscribe(subscription={ "name": "trade" }, pair=["BTC/EUR"])
-    # await bot.subscribe(subscription={ "name": "*" } , pair=["BTC/EUR"])
-
-    time.sleep(2) # wait because unsubscribing is faster than subscribing ...
-    await bot.unsubscribe(subscription={ "name": "ticker" }, pair=["XBT/EUR","DOT/EUR"])
-    await bot.unsubscribe(subscription={ "name": "spread" }, pair=["XBT/EUR"])
-    await bot.unsubscribe(subscription={ "name": "spread" }, pair=["DOT/EUR"])
-    # ...
-
-    # ___Authenticated_Websocket_________
-    # when using the authenticated client, you can also subscribe to public feeds
-    auth_bot = Bot(key=key, secret=secret)
-    print(auth_bot.private_sub_names) # list private subscription names
-    await auth_bot.subscribe(subscription={ "name": "ownTrades" })
-    await auth_bot.subscribe(subscription={ "name": "openOrders" })
-
-    time.sleep(2)
-    await auth_bot.unsubscribe(subscription={ "name": "ownTrades" })
-    await auth_bot.unsubscribe(subscription={ "name": "openOrders" })
+            # … it is also possible to call regular REST endpoints
+            # but using the websocket messages is more efficient.
+            # You can also un-/subscribe here using self.subscribe/self.unsubscribe.
 
-    while True:
+    # Public/unauthenticated websocket client
+    client = Client()  # only use this one if you don't need private feeds
+
+    await client.subscribe(
+        params={"channel": "ticker", "symbol": ["BTC/USD", "DOT/USD"]}
+    )
+    await client.subscribe(
+        params={"channel": "book", "depth": 25, "symbol": ["BTC/USD"]}
+    )
+    # wait because unsubscribing is faster than unsubscribing … (just for that example)
+    await asyncio.sleep(3)
+    # print(client.active_public_subscriptions) # to list active subscriptions
+    await client.unsubscribe(
+        params={"channel": "ticker", "symbol": ["BTC/USD", "DOT/USD"]}
+    )
+    # …
+
+    # Per default, the authenticated client starts two websocket connections,
+    # one for authenticated and one for public messages. If there is no need
+    # for a public connection, it can be disabled using the ``no_public``
+    # parameter.
+    client_auth = Client(key=key, secret=secret, no_public=True)
+    await client_auth.subscribe(params={"channel": "executions"})
+
+    while not client.exception_occur and not client_auth.exception_occur:
         await asyncio.sleep(6)
+    return
+
 
 if __name__ == "__main__":
     try:
         asyncio.run(main())
     except KeyboardInterrupt:
-        # do some exception handling ...
         pass
+        # The websocket client will send {'event': 'asyncio.CancelledError'}
+        # via on_message so you can handle the behavior/next actions
+        # individually within your strategy.
 ```
 
-Note: Authenticated Spot websocket clients can also un/subscribe from/to public feeds.
-
 ---
 
 <a name="futuresusage"></a>
 
-# 📍 Futures Client Example Usage
+# 📍 Futures Clients
 
-Kraken provides a sandbox environment at https://demo-futures.kraken.com for paper trading. When using this API keys you have to set the `sandbox` parameter to `True` when instantiating the respective client.
+Kraken provides a sandbox environment at https://demo-futures.kraken.com for
+Futures paper trading. When using these API keys you have to set the `sandbox`
+parameter to `True` when instantiating the respective client.
 
-A template Futures trading bot using both websocket and REST clients can be found in `/examples/futures_trading_bot_template.py`.
+A template for Futures trading using both websocket and REST clients can be
+found in `examples/futures_trading_bot_template.py`.
+
+The Kraken Futures API documentation can be found here:
+
+- https://docs.futures.kraken.com
+- https://support.kraken.com/hc/en-us/sections/360012894412-Futures-API
 
 <a name="futuresrest"></a>
 
 ## Futures REST API
 
-The following example can be found in `/examples/futures_examples.py`.
+As the Spot API, Kraken also offers a REST API for Futures. Examples on how to
+use the python-kraken-sdk fot Futures are shown in
+`examples/futures_examples.py` and listed in a shorter ways below.
 
 ```python
 from kraken.futures import Market, User, Trade, Funding
 
 def main():
 
     key = "futures-api-key"
@@ -943,24 +994,24 @@
 
     # ____USER________________________
     user = User(key=key, secret=secret) # optional: sandbox=True
     print(user.get_wallets())
     print(user.get_open_orders())
     print(user.get_open_positions())
     print(user.get_subaccounts())
-    # ...
+    # …
 
     # ____MARKET____
     market = Market()
     print(market.get_ohlc(tick_type="trade", symbol="PI_XBTUSD", resolution="5m"))
 
     priv_market = Market(key=key, secret=secret)
     print(priv_market.get_fee_schedules_vol())
     print(priv_market.get_execution_events())
-    # ...
+    # …
 
     # ____TRADE_________________________
     trade = Trade(key=key, secret=secret)
     print(trade.get_fills())
     print(trade.create_batch_order(
         batchorder_list = [{
             "order": "send",
@@ -994,118 +1045,137 @@
             orderType="lmt",
             side="buy",
             size=1,
             limitPrice=4,
             symbol="pf_bchusd"
         )
     )
-    # ...
+    # …
 
     # ____FUNDING___________________________
     funding = Funding(key=key, secret=secret)
-    # ...
+    # …
 
 if __name__ == "__main__":
     main()
 ```
 
 <a name="futuresws"></a>
 
-## Futures Websocket Client
+## Futures Websocket API
+
+Not only REST, also the websocket API for Kraken Futures is available. Examples
+are shown below and demonstrated in `examples/futures_ws_examples.py`.
 
-The following example can be found in `/examples/futures_ws_examples.py`.
+- https://docs.futures.kraken.com/#websocket-api
+
+Note: Authenticated Futures websocket clients can also un-/subscribe from/to
+public feeds.
 
 ```python
 import asyncio
 from kraken.futures import KrakenFuturesWSClient
 
 async def main():
 
     key = "futures-api-key"
     secret = "futures-secret-key"
 
-    # ___Custom_Trading_Bot________
-    class Bot(KrakenFuturesWSClient):
+    class Client(KrakenFuturesWSClient):
 
         async def on_message(self, event):
             print(event)
-            # >> apply your trading strategy here <<
-            # you can also combine this with the Futures REST clients
 
-    # ___Public_Websocket_Feeds____
-    bot = Bot()
-    # print(bot.get_available_public_subscription_feeds())
+    # Public/unauthenticated websocket connection
+    client = Client()
 
     products = ["PI_XBTUSD", "PF_ETHUSD"]
 
     # subscribe to a public websocket feed
-    await bot.subscribe(feed="ticker", products=products)
-    # await bot.subscribe(feed="book", products=products)
-    # ...
+    await client.subscribe(feed="ticker", products=products)
+    # await client.subscribe(feed="book", products=products)
+    # …
 
     # unsubscribe from a public websocket feed
-    # await bot.unsubscribe(feed="ticker", products=products)
+    # await client.unsubscribe(feed="ticker", products=products)
 
-    # ___Authenticated_Websocket_________
-    auth_bot = Bot(key=key, secret=secret)
-    # print(auth_bot.get_available_private_subscription_feeds())
+    # Private/authenticated websocket connection (+public)
+    client_auth = Client(key=key, secret=secret)
+    # print(client_auth.get_available_private_subscription_feeds())
 
     # subscribe to a private/authenticated websocket feed
-    await auth_bot.subscribe(feed="fills")
-    await auth_bot.subscribe(feed="open_positions")
-    await auth_bot.subscribe(feed="open_orders")
-    # ...
+    await client_auth.subscribe(feed="fills")
+    await client_auth.subscribe(feed="open_positions")
+    await client_auth.subscribe(feed="open_orders")
+    # …
 
     # unsubscribe from a private/authenticated websocket feed
-    await auth_bot.unsubscribe(feed="fills")
+    await client_auth.unsubscribe(feed="fills")
 
     while True:
         await asyncio.sleep(6)
 
 if __name__ == "__main__":
     try:
         asyncio.run(main())
     except KeyboardInterrupt:
-        # do some exception handling ...
+        # do some exception handling …
         pass
 ```
 
-Note: Authenticated Futures websocket clients can also un-/subscribe from/to public feeds.
-
 ---
 
 <a name="contribution"></a>
 
 # 🆕 Contributions
 
 … are welcome! - Please have a look at [CONTRIBUTION.md](./CONTRIBUTING.md).
 
 ---
 
 <a name="trouble"></a>
 
 # 🚨 Troubleshooting
 
-- Check if you downloaded and installed the **latest version** of the python-kraken-sdk.
-- Check the **permissions of your API keys** and the required permissions on the respective endpoints.
-- If you get some Cloudflare or **rate limit errors**, please check your Kraken Tier level and maybe apply for a higher rank if required.
-- **Use different API keys for different algorithms**, because the nonce calculation is based on timestamps and a sent nonce must always be the highest nonce ever sent of that API key. Having multiple algorithms using the same keys will result in invalid nonce errors.
+- Check if you downloaded and installed the **latest version** of the
+  python-kraken-sdk.
+- Check the **permissions of your API keys** and the required permissions on the
+  respective endpoints.
+- If you get some Cloudflare or **rate limit errors**, please check your Kraken
+  Tier level and maybe apply for a higher rank if required.
+- **Use different API keys for different algorithms**, because the nonce
+  calculation is based on timestamps and a sent nonce must always be the highest
+  nonce ever sent of that API key. Having multiple algorithms using the same
+  keys will result in invalid nonce errors.
 
 ---
 
 <a name="notes"></a>
 
 # 📝 Notes
 
-- Coding standards are not always followed to make arguments and function names as similar as possible to those in the Kraken API documentations.
+- The version scheme is `<Major>.<Minor>.<Service Level>` where:
+
+  - **Major** will affect everything and there will be breaking changes
+    in any case. This could be for example a change to Python 3.11+ only.
+
+  - **Minor** introduces features and enhancements which may bring breaking
+    changes in some cases. These breaking changes could be renaming or
+    addition of parameters, change in order of parameters or even renaming
+    a function.
+  - **Service Level** includes bug fixes, documentation or CI related changes.
+
+- Coding standards are not always followed to make arguments and function names
+  as similar as possible to those of the Kraken API documentations.
 
 <a name="references"></a>
 
 # 🔭 References
 
 - https://python-kraken-sdk.readthedocs.io/en/stable
 - https://docs.kraken.com/rest
 - https://docs.kraken.com/websockets
+- https://docs.kraken.com/websockets-v2
 - https://docs.futures.kraken.com
 - https://support.kraken.com/hc/en-us/sections/360012894412-Futures-API
 
 ---
```

### Comparing `python-kraken-sdk-1.5.0/README.md` & `python-kraken-sdk-1.6.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,269 +1,320 @@
-<h1 align="center">Futures and Spot Websocket and REST API Python SDK for the Kraken Cryptocurrency Exchange 🐙</h1>
+<h1 align="center">Futures and Spot - REST and Websocket API Python SDK for the Kraken Cryptocurrency Exchange 🐙</h1>
 
 <div align="center">
 
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/btschwertfeger/python-kraken-sdk)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-orange.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Generic badge](https://img.shields.io/badge/python-3.7_|_3.8_|_3.9_|_3.10_|_3.11-blue.svg)](https://shields.io/)
 [![Downloads](https://static.pepy.tech/personalized-badge/python-kraken-sdk?period=total&units=abbreviation&left_color=grey&right_color=orange&left_text=downloads)](https://pepy.tech/project/python-kraken-sdk)
 
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Typing](https://img.shields.io/badge/typing-mypy-informational)](https://mypy-lang.org/)
 [![CodeQL](https://github.com/btschwertfeger/python-kraken-sdk/actions/workflows/codeql.yaml/badge.svg?branch=master)](https://github.com/btschwertfeger/python-kraken-sdk/actions/workflows/codeql.yaml)
 [![CI/CD](https://github.com/btschwertfeger/python-kraken-sdk/actions/workflows/cicd.yaml/badge.svg?branch=master)](https://github.com/btschwertfeger/python-kraken-sdk/actions/workflows/cicd.yaml)
 [![codecov](https://codecov.io/gh/btschwertfeger/python-kraken-sdk/branch/master/badge.svg)](https://app.codecov.io/gh/btschwertfeger/python-kraken-sdk)
 
 ![release](https://shields.io/github/release-date/btschwertfeger/python-kraken-sdk)
 [![release](https://img.shields.io/pypi/v/python-kraken-sdk)](https://pypi.org/project/python-kraken-sdk/)
 [![DOI](https://zenodo.org/badge/510751854.svg)](https://zenodo.org/badge/latestdoi/510751854)
 [![Documentation Status stable](https://readthedocs.org/projects/python-kraken-sdk/badge/?version=stable)](https://python-kraken-sdk.readthedocs.io/en/stable)
 
 </div>
 
-> ⚠️ This is an unofficial collection of REST and websocket clients for Spot and Futures trading on the Kraken cryptocurrency exchange using Python. Payward Ltd. and Kraken are in no way associated with the authors of this module and documentation.
+> ⚠️ This is an unofficial collection of REST and websocket clients for Spot and
+> Futures trading on the Kraken cryptocurrency exchange using Python. Payward
+> Ltd. and Kraken are in no way associated with the authors of this module and
+> documentation.
 
 ---
 
 ## 📌 Disclaimer
 
-There is no guarantee that this software will work flawlessly at this or later times. Of course, no responsibility is taken for possible profits or losses. This software probably has some errors in it, so use it at your own risk. Also no one should be motivated or tempted to invest assets in speculative forms of investment. By using this software you release the authors from any liability regarding the use of this software.
+There is no guarantee that this software will work flawlessly at this or later
+times. Of course, no responsibility is taken for possible profits or losses.
+This software probably has some errors in it, so use it at your own risk. Also
+no one should be motivated or tempted to invest assets in speculative forms of
+investment. By using this software you release the authors from any liability
+regarding the use of this software.
 
 ---
 
 ## Features
 
-Clients:
+Available Clients:
 
 - Spot REST Clients
-- Spot Websocket Client
+- Spot Websocket Clients (Websocket API v1 and v2)
 - Spot Orderbook Client
 - Futures REST Clients
 - Futures Websocket Client
 
 General:
 
-- access both public and private endpoints
+- access both public and private, REST and websocket endpoints
 - responsive error handling and custom exceptions
 - extensive example scripts (see `/examples` and `/tests`)
 - tested using the [pytest](https://docs.pytest.org/en/7.3.x/) framework
 - releases are permanently archived at [Zenodo](https://zenodo.org/badge/latestdoi/510751854)
 
 Documentation:
 
-- Stable: [https://python-kraken-sdk.readthedocs.io/en/stable](https://python-kraken-sdk.readthedocs.io/en/stable)
-- Latest: [https://python-kraken-sdk.readthedocs.io/en/latest](https://python-kraken-sdk.readthedocs.io/en/latest)
+- [https://python-kraken-sdk.readthedocs.io/en/stable](https://python-kraken-sdk.readthedocs.io/en/stable)
+- [https://python-kraken-sdk.readthedocs.io/en/latest](https://python-kraken-sdk.readthedocs.io/en/latest)
 
 ---
 
 ## ❗️ Attention
 
-**ONLY** tagged releases are available at PyPI. So the content of the master may not match with the content of the latest release. - Please have a look at the release specific READMEs and changelogs.
+**ONLY** tagged releases are available at PyPI. So the content of the master may
+not match with the content of the latest release. - Please have a look at the
+release specific READMEs and changelogs.
 
 ---
 
 ## Table of Contents
 
 - [ Installation and setup ](#installation)
-- [ Spot Client Example Usage ](#spotusage)
+- [ Spot Clients ](#spotusage)
   - [REST API](#spotrest)
-  - [Websockets](#spotws)
-- [ Futures Client Example Usage ](#futuresusage)
+  - [Websocket API V2](#spotws)
+- [ Futures Clients ](#futuresusage)
   - [REST API](#futuresrest)
-  - [Websockets](#futuresws)
+  - [Websocket API](#futuresws)
 - [ Troubleshooting ](#trouble)
 - [ Contributions ](#contribution)
 - [ Notes ](#notes)
 - [ References ](#references)
 
 ---
 
 <a name="installation"></a>
 
 # 🛠 Installation and setup
 
-### 1. Install the Python module:
+### 1. Install the package into the desired environment
 
 ```bash
 python3 -m pip install python-kraken-sdk
 ```
 
-### 2. Register at Kraken and generate API Keys:
+### 2. Register at [Kraken](https://www.kraken.com) and generate API keys
 
 - Spot Trading: https://www.kraken.com/u/security/api
 - Futures Trading: https://futures.kraken.com/trade/settings/api (see _[help](https://docs.futures.kraken.com/#introduction-generate-api-keys)_)
 - Futures Sandbox: https://demo-futures.kraken.com/settings/api
 
 ### 3. Start using the provided example scripts
 
 ### 4. Error handling
 
-If any unexpected behavior occurs, please check <b style="color: yellow">your API permissions</b>, <b style="color: yellow">rate limits</b>, update the python-kraken-sdk, see the [Troubleshooting](#trouble) section, and if the error persists please open an issue.
+If any unexpected behavior occurs, please check <b style="color: yellow">your
+API permissions</b>, <b style="color: yellow">rate limits</b>, update the
+python-kraken-sdk, see the [Troubleshooting](#trouble) section, and if the error
+persists please open an issue.
 
 ---
 
 <a name="spotusage"></a>
 
-# 📍 Spot Client Example Usage
+# 📍 Spot Clients
 
-A template Spot trading bot using both websocket and REST clients can be found in `/examples/spot_trading_bot_template.py`.
+A template for Spot trading using both websocket and REST clients can be
+found in `examples/spot_trading_bot_template_v2.py`.
 
-For those who need a realtime order book - a script that demonstrates how to maintain a valid order book can be found here: `/examples/spot_orderbook.py`.
+For those who need a realtime order book - a script that demonstrates how to
+maintain a valid order book using the Orderbook client can be found in
+`examples/spot_orderbook.py`.
 
 <a name="spotrest"></a>
 
 ## Spot REST API
 
-... can be found in `/examples/spot_examples.py`
+The Kraken Spot REST API offers many endpoints for almost every use-case. The
+python-kraken-sdk aims to provide all of them - split in User, Market,
+Trade, Funding and Staking related clients.
+
+The following code block demonstrates how to use some of them. More examples
+can be found in `examples/spot_examples.py`.
 
 ```python
 from kraken.spot import User, Market, Trade, Funding, Staking
 
 def main():
     key = "kraken-public-key"
     secret = "kraken-secret-key"
 
     # ____USER________________________
     user = User(key=key, secret=secret)
     print(user.get_account_balance())
     print(user.get_open_orders())
-    # ...
+    # …
 
     # ____MARKET____
     market = Market()
     print(market.get_ticker(pair="BTCUSD"))
-    # ...
+    # …
 
     # ____TRADE_________________________
     trade = Trade(key=key, secret=secret)
     print(trade.create_order(
          ordertype="limit",
          side="buy",
          volume=1,
          pair="BTC/EUR",
          price=20000
     ))
-    # ...
+    # …
 
     # ____FUNDING___________________________
     funding = Funding(key=key, secret=secret)
     print(
         funding.withdraw_funds(
             asset="DOT", key="MyPolkadotWallet", amount=200
         )
     )
     print(funding.cancel_withdraw(asset="DOT", refid="<some id>"))
-    # ...
+    # …
 
     # ____STAKING___________________________
     staking = Staking(key=key, secret=secret)
     print(staking.list_stakeable_assets())
     print(
         staking.stake_asset(
             asset="DOT", amount=20, method="polkadot-staked"
         )
     )
-    # ...
+    # …
 
 if __name__ == "__main__":
     main()
 ```
 
 <a name="spotws"></a>
 
-## Websockets
+## Spot Websocket API V2
+
+Kraken offers two versions of their websocket API (V1 and V2). Since V2 is
+offers more possibilities, is way faster and easier to use, only those examples
+are shown below. For using the websocket API V1 please have a look into the
+`examples/spot_ws_examples_v1.py`.
 
-... can be found in `/examples/spot_ws_examples.py`
+The documentation for both API versions can be found here:
+
+- https://docs.kraken.com/websockets
+- https://docs.kraken.com/websockets-v2
+
+Note that authenticated Spot websocket clients can also un-/subscribe from/to
+public feeds.
+
+The example below can be found in an extended way in
+`examples/spot_ws_examples_v2.py`.
 
 ```python
-import time
 import asyncio
-from kraken.spot import KrakenSpotWSClient
+from kraken.spot import KrakenSpotWSClientV2
 
-async def main()
+async def main():
+    key = "spot-api-key"
+    secret = "spot-secret-key"
 
-    key = "kraken-public-key"
-    secret = "kraken-secret-key"
+    class Client(KrakenSpotWSClientV2):
+        """Can be used to create a custom trading strategy"""
 
-    class Bot(KrakenSpotWSClient):
-        async def on_message(self, msg):
-            if isinstance(msg, dict) and "event" in msg:
-                if msg["event"] in ("pong", "heartbeat"):
-                    return
-
-            print(msg)
-            # if condition:
-            #     await self.create_order(
-            #         ordertype="limit",
-            #         side="buy",
-            #         pair="BTC/EUR",
-            #         price=20000,
-            #         volume=1
+        async def on_message(self, message):
+            """Receives the websocket messages"""
+            if message.get("method") == "pong" \
+                or message.get("channel") == "heartbeat":
+                return
+
+            print(message)
+            # here we can access lots of methods, for example to create an order:
+            # if self.is_auth:  # only if the client is authenticated …
+            #     await self.send_message(
+            #         message={
+            #             "method": "add_order",
+            #             "params": {
+            #                 "limit_price": 1234.56,
+            #                 "order_type": "limit",
+            #                 "order_userref": 123456789,
+            #                 "order_qty": 1.0,
+            #                 "side": "buy",
+            #                 "symbol": "BTC/USD",
+            #                 "validate": True,
+            #             },
+            #         }
             #     )
-            # ... it is also possible to call regular Spot REST endpoints
-            # but using the WsClient's functions is more efficient
-            # because the requests will be sent via the ws connection
-
-    # ___Public_Websocket_Feeds__
-    bot = Bot() # only use the unauthenticated client if you don't need private feeds
-    print(bot.public_sub_names) # list public subscription names
-
-    await bot.subscribe(subscription={ "name": "ticker" }, pair=["XBT/EUR", "DOT/EUR"])
-    await bot.subscribe(subscription={ "name": "spread" }, pair=["XBT/EUR", "DOT/EUR"])
-    # await bot.subscribe(subscription={ "name": "book" }, pair=["BTC/EUR"])
-    # await bot.subscribe(subscription={ "name": "book", "depth": 25}, pair=["BTC/EUR"])
-    # await bot.subscribe(subscription={ "name": "ohlc" }, pair=["BTC/EUR"])
-    # await bot.subscribe(subscription={ "name": "ohlc", "interval": 15}, pair=["XBT/EUR", "DOT/EUR"])
-    # await bot.subscribe(subscription={ "name": "trade" }, pair=["BTC/EUR"])
-    # await bot.subscribe(subscription={ "name": "*" } , pair=["BTC/EUR"])
-
-    time.sleep(2) # wait because unsubscribing is faster than subscribing ...
-    await bot.unsubscribe(subscription={ "name": "ticker" }, pair=["XBT/EUR","DOT/EUR"])
-    await bot.unsubscribe(subscription={ "name": "spread" }, pair=["XBT/EUR"])
-    await bot.unsubscribe(subscription={ "name": "spread" }, pair=["DOT/EUR"])
-    # ...
-
-    # ___Authenticated_Websocket_________
-    # when using the authenticated client, you can also subscribe to public feeds
-    auth_bot = Bot(key=key, secret=secret)
-    print(auth_bot.private_sub_names) # list private subscription names
-    await auth_bot.subscribe(subscription={ "name": "ownTrades" })
-    await auth_bot.subscribe(subscription={ "name": "openOrders" })
-
-    time.sleep(2)
-    await auth_bot.unsubscribe(subscription={ "name": "ownTrades" })
-    await auth_bot.unsubscribe(subscription={ "name": "openOrders" })
+            # … it is also possible to call regular REST endpoints
+            # but using the websocket messages is more efficient.
+            # You can also un-/subscribe here using self.subscribe/self.unsubscribe.
 
-    while True:
+    # Public/unauthenticated websocket client
+    client = Client()  # only use this one if you don't need private feeds
+
+    await client.subscribe(
+        params={"channel": "ticker", "symbol": ["BTC/USD", "DOT/USD"]}
+    )
+    await client.subscribe(
+        params={"channel": "book", "depth": 25, "symbol": ["BTC/USD"]}
+    )
+    # wait because unsubscribing is faster than unsubscribing … (just for that example)
+    await asyncio.sleep(3)
+    # print(client.active_public_subscriptions) # to list active subscriptions
+    await client.unsubscribe(
+        params={"channel": "ticker", "symbol": ["BTC/USD", "DOT/USD"]}
+    )
+    # …
+
+    # Per default, the authenticated client starts two websocket connections,
+    # one for authenticated and one for public messages. If there is no need
+    # for a public connection, it can be disabled using the ``no_public``
+    # parameter.
+    client_auth = Client(key=key, secret=secret, no_public=True)
+    await client_auth.subscribe(params={"channel": "executions"})
+
+    while not client.exception_occur and not client_auth.exception_occur:
         await asyncio.sleep(6)
+    return
+
 
 if __name__ == "__main__":
     try:
         asyncio.run(main())
     except KeyboardInterrupt:
-        # do some exception handling ...
         pass
+        # The websocket client will send {'event': 'asyncio.CancelledError'}
+        # via on_message so you can handle the behavior/next actions
+        # individually within your strategy.
 ```
 
-Note: Authenticated Spot websocket clients can also un/subscribe from/to public feeds.
-
 ---
 
 <a name="futuresusage"></a>
 
-# 📍 Futures Client Example Usage
+# 📍 Futures Clients
 
-Kraken provides a sandbox environment at https://demo-futures.kraken.com for paper trading. When using this API keys you have to set the `sandbox` parameter to `True` when instantiating the respective client.
+Kraken provides a sandbox environment at https://demo-futures.kraken.com for
+Futures paper trading. When using these API keys you have to set the `sandbox`
+parameter to `True` when instantiating the respective client.
 
-A template Futures trading bot using both websocket and REST clients can be found in `/examples/futures_trading_bot_template.py`.
+A template for Futures trading using both websocket and REST clients can be
+found in `examples/futures_trading_bot_template.py`.
+
+The Kraken Futures API documentation can be found here:
+
+- https://docs.futures.kraken.com
+- https://support.kraken.com/hc/en-us/sections/360012894412-Futures-API
 
 <a name="futuresrest"></a>
 
 ## Futures REST API
 
-The following example can be found in `/examples/futures_examples.py`.
+As the Spot API, Kraken also offers a REST API for Futures. Examples on how to
+use the python-kraken-sdk fot Futures are shown in
+`examples/futures_examples.py` and listed in a shorter ways below.
 
 ```python
 from kraken.futures import Market, User, Trade, Funding
 
 def main():
 
     key = "futures-api-key"
@@ -271,24 +322,24 @@
 
     # ____USER________________________
     user = User(key=key, secret=secret) # optional: sandbox=True
     print(user.get_wallets())
     print(user.get_open_orders())
     print(user.get_open_positions())
     print(user.get_subaccounts())
-    # ...
+    # …
 
     # ____MARKET____
     market = Market()
     print(market.get_ohlc(tick_type="trade", symbol="PI_XBTUSD", resolution="5m"))
 
     priv_market = Market(key=key, secret=secret)
     print(priv_market.get_fee_schedules_vol())
     print(priv_market.get_execution_events())
-    # ...
+    # …
 
     # ____TRADE_________________________
     trade = Trade(key=key, secret=secret)
     print(trade.get_fills())
     print(trade.create_batch_order(
         batchorder_list = [{
             "order": "send",
@@ -322,118 +373,137 @@
             orderType="lmt",
             side="buy",
             size=1,
             limitPrice=4,
             symbol="pf_bchusd"
         )
     )
-    # ...
+    # …
 
     # ____FUNDING___________________________
     funding = Funding(key=key, secret=secret)
-    # ...
+    # …
 
 if __name__ == "__main__":
     main()
 ```
 
 <a name="futuresws"></a>
 
-## Futures Websocket Client
+## Futures Websocket API
+
+Not only REST, also the websocket API for Kraken Futures is available. Examples
+are shown below and demonstrated in `examples/futures_ws_examples.py`.
 
-The following example can be found in `/examples/futures_ws_examples.py`.
+- https://docs.futures.kraken.com/#websocket-api
+
+Note: Authenticated Futures websocket clients can also un-/subscribe from/to
+public feeds.
 
 ```python
 import asyncio
 from kraken.futures import KrakenFuturesWSClient
 
 async def main():
 
     key = "futures-api-key"
     secret = "futures-secret-key"
 
-    # ___Custom_Trading_Bot________
-    class Bot(KrakenFuturesWSClient):
+    class Client(KrakenFuturesWSClient):
 
         async def on_message(self, event):
             print(event)
-            # >> apply your trading strategy here <<
-            # you can also combine this with the Futures REST clients
 
-    # ___Public_Websocket_Feeds____
-    bot = Bot()
-    # print(bot.get_available_public_subscription_feeds())
+    # Public/unauthenticated websocket connection
+    client = Client()
 
     products = ["PI_XBTUSD", "PF_ETHUSD"]
 
     # subscribe to a public websocket feed
-    await bot.subscribe(feed="ticker", products=products)
-    # await bot.subscribe(feed="book", products=products)
-    # ...
+    await client.subscribe(feed="ticker", products=products)
+    # await client.subscribe(feed="book", products=products)
+    # …
 
     # unsubscribe from a public websocket feed
-    # await bot.unsubscribe(feed="ticker", products=products)
+    # await client.unsubscribe(feed="ticker", products=products)
 
-    # ___Authenticated_Websocket_________
-    auth_bot = Bot(key=key, secret=secret)
-    # print(auth_bot.get_available_private_subscription_feeds())
+    # Private/authenticated websocket connection (+public)
+    client_auth = Client(key=key, secret=secret)
+    # print(client_auth.get_available_private_subscription_feeds())
 
     # subscribe to a private/authenticated websocket feed
-    await auth_bot.subscribe(feed="fills")
-    await auth_bot.subscribe(feed="open_positions")
-    await auth_bot.subscribe(feed="open_orders")
-    # ...
+    await client_auth.subscribe(feed="fills")
+    await client_auth.subscribe(feed="open_positions")
+    await client_auth.subscribe(feed="open_orders")
+    # …
 
     # unsubscribe from a private/authenticated websocket feed
-    await auth_bot.unsubscribe(feed="fills")
+    await client_auth.unsubscribe(feed="fills")
 
     while True:
         await asyncio.sleep(6)
 
 if __name__ == "__main__":
     try:
         asyncio.run(main())
     except KeyboardInterrupt:
-        # do some exception handling ...
+        # do some exception handling …
         pass
 ```
 
-Note: Authenticated Futures websocket clients can also un-/subscribe from/to public feeds.
-
 ---
 
 <a name="contribution"></a>
 
 # 🆕 Contributions
 
 … are welcome! - Please have a look at [CONTRIBUTION.md](./CONTRIBUTING.md).
 
 ---
 
 <a name="trouble"></a>
 
 # 🚨 Troubleshooting
 
-- Check if you downloaded and installed the **latest version** of the python-kraken-sdk.
-- Check the **permissions of your API keys** and the required permissions on the respective endpoints.
-- If you get some Cloudflare or **rate limit errors**, please check your Kraken Tier level and maybe apply for a higher rank if required.
-- **Use different API keys for different algorithms**, because the nonce calculation is based on timestamps and a sent nonce must always be the highest nonce ever sent of that API key. Having multiple algorithms using the same keys will result in invalid nonce errors.
+- Check if you downloaded and installed the **latest version** of the
+  python-kraken-sdk.
+- Check the **permissions of your API keys** and the required permissions on the
+  respective endpoints.
+- If you get some Cloudflare or **rate limit errors**, please check your Kraken
+  Tier level and maybe apply for a higher rank if required.
+- **Use different API keys for different algorithms**, because the nonce
+  calculation is based on timestamps and a sent nonce must always be the highest
+  nonce ever sent of that API key. Having multiple algorithms using the same
+  keys will result in invalid nonce errors.
 
 ---
 
 <a name="notes"></a>
 
 # 📝 Notes
 
-- Coding standards are not always followed to make arguments and function names as similar as possible to those in the Kraken API documentations.
+- The version scheme is `<Major>.<Minor>.<Service Level>` where:
+
+  - **Major** will affect everything and there will be breaking changes
+    in any case. This could be for example a change to Python 3.11+ only.
+
+  - **Minor** introduces features and enhancements which may bring breaking
+    changes in some cases. These breaking changes could be renaming or
+    addition of parameters, change in order of parameters or even renaming
+    a function.
+  - **Service Level** includes bug fixes, documentation or CI related changes.
+
+- Coding standards are not always followed to make arguments and function names
+  as similar as possible to those of the Kraken API documentations.
 
 <a name="references"></a>
 
 # 🔭 References
 
 - https://python-kraken-sdk.readthedocs.io/en/stable
 - https://docs.kraken.com/rest
 - https://docs.kraken.com/websockets
+- https://docs.kraken.com/websockets-v2
 - https://docs.futures.kraken.com
 - https://support.kraken.com/hc/en-us/sections/360012894412-Futures-API
 
 ---
```

### Comparing `python-kraken-sdk-1.5.0/docs/Makefile` & `python-kraken-sdk-1.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.5.0/docs/conf.py` & `python-kraken-sdk-1.6.0/docs/conf.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # -*- coding: utf-8 -*-
+# Copyright (C) 2023 Benjamin Thomas Schwertfeger
+# GitHub: https://github.com/btschwertfeger
+#
 # Configuration file for the Sphinx documentation builder.
 #
 # For the full list of built-in configuration values, see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
+# pylint: disable=invalid-name
 
 """This module is the configuration for the Sphinx documentation building process"""
-# pylint: disable=invalid-name
 
 import os
 import sys
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = "python-kraken-sdk"
-copyright = "2023, Benjamin Thomas Schwertfeger"  # pylint: disable=redefined-builtin
+copyright = "2023, Benjamin Thomas Schwertfeger"  # noqa: A001
 author = "Benjamin Thomas Schwertfeger"
 
 # to import the package
 sys.path.insert(0, os.path.abspath(".."))
 
-# import links
 rst_epilog = ""
 # Read link all targets from file
 with open("links.rst", encoding="utf-8") as f:
     rst_epilog += f.read()
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
@@ -37,19 +39,14 @@
     "sphinx.ext.napoleon",
     "sphinx.ext.autosectionlabel",
 ]
 
 templates_path = ["_templates"]
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store", "links.rst"]
 
-
-def setup(app):
-    """Run during the Sphinx building process"""
-
-
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 html_theme = "sphinx_rtd_theme"
 html_static_path = ["_static"]
 html_context = {
     "display_github": True,
```

### Comparing `python-kraken-sdk-1.5.0/docs/index.rst` & `python-kraken-sdk-1.6.0/docs/index.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+.. -*- coding: utf-8 -*-
+.. Copyright (C) 2023 Benjamin Thomas Schwertfeger
+.. GitHub: https://github.com/btschwertfeger
+..
 .. Python Kraken SDK documentation master file, created by
    sphinx-quickstart on Sun Apr  2 11:32:02 2023.
    You can adapt this file completely to your liking, but it should at least
    contain the root ``toctree``` directive.
 
 
 Welcome to Python Kraken SDK's documentation!
```

### Comparing `python-kraken-sdk-1.5.0/docs/make.bat` & `python-kraken-sdk-1.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.5.0/docs/src/examples/trading_bot_templates.rst` & `python-kraken-sdk-1.6.0/docs/src/examples/trading_bot_templates.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,25 @@
-.. Some Headline
+.. -*- coding: utf-8 -*-
+.. Copyright (C) 2023 Benjamin Thomas Schwertfeger
+.. GitHub: https://github.com/btschwertfeger
 
 .. _section-trading-bot-templates:
 
 Trading Bot Templates
 =====================
 
-The `python-kraken-sdk`_ is perfectly suited to develop automated trading algorithms. To facilitate the start here directly
-for Spot trading as well as for the Futures enthusiasts templates are provided, which can serve as the basis for dynamic trading algorithms.
-In both cases the websocket endpoints are used to capture the live data. In addition REST clients are integrated,
-so that their endpoints can be reached at any time.
+The `python-kraken-sdk`_ is perfectly suited to develop automated trading
+algorithms. To facilitate the start here directly for Spot trading as well as
+for the Futures enthusiasts, templates are provided which can serve as the basis
+for dynamic trading algorithms. In both cases websockets are used to capture the
+live data. In addition REST clients are integrated, so that their endpoints can
+also be reached at any time.
 
-For questions, feedback, suggestions for improvement or problems `python-kraken-sdk/discussions`_ or `python-kraken-sdk/issues`_ may be helpful.
+For questions, feedback, additions, suggestions or problems
+`python-kraken-sdk/discussions`_ or `python-kraken-sdk/issues`_ may be helpful.
 
 .. toctree::
     :maxdepth: 2
 
-    spot_bot_template.rst
+    spot_bot_templates.rst
     spot_orderbook.rst
     futures_bot_template.rst
```

### Comparing `python-kraken-sdk-1.5.0/docs/src/getting_started/getting_started.rst` & `python-kraken-sdk-1.6.0/docs/src/getting_started/getting_started.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+.. -*- coding: utf-8 -*-
+.. Copyright (C) 2023 Benjamin Thomas Schwertfeger
+.. GitHub: https://github.com/btschwertfeger
+
 Getting Started
 ===============
 
 1. Install the Python module
 
 .. code-block:: bash
 
@@ -12,15 +16,17 @@
 
 - Spot Trading: https://www.kraken.com/u/security/api
 - Futures Trading: https://futures.kraken.com/trade/settings/api
 - Futures Sandbox: https://demo-futures.kraken.com/settings/api
 
 3. Start using the provided example scripts
 
-The examples can be found within the repository of the `python-kraken-sdk`_ and obviously in this documentation.
-For trading algorithms templates see the :ref:`section-trading-bot-templates` section.
+The examples can be found within the repository of the `python-kraken-sdk`_ and
+obviously in this documentation. For trading algorithms templates see the
+:ref:`section-trading-bot-templates` section.
 
 4. Error handling
 
-If any unexpected behavior occurs, please check **your API permissions**, **rate limits**,
-update the `python-kraken-sdk`_, see the :ref:`section-troubleshooting` section, and if the error
-persists please open an issue at `python-kraken-sdk/issues`_.
+If any unexpected behavior occurs, please check **your API permissions**,
+**rate limits**, update the `python-kraken-sdk`_, see the
+:ref:`section-troubleshooting` section, and if the error persists please open an
+issue at `python-kraken-sdk/issues`_.
```

### Comparing `python-kraken-sdk-1.5.0/docs/src/introduction.rst` & `python-kraken-sdk-1.6.0/docs/src/introduction.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,71 +1,101 @@
-.. This is the introduction
+.. -*- coding: utf-8 -*-
+.. Copyright (C) 2023 Benjamin Thomas Schwertfeger
+.. GitHub: https://github.com/btschwertfeger
 
 Introduction
 =============
 
 |GitHub badge| |License badge| |PyVersions badge| |Downloads badge|
 |CodeQL badge| |CI/CD badge| |codecov badge| |Typing badge|
 |Release date badge| |Release version badge| |DOI badge|
 
 
-**This is the documentation of the unofficial Python SDK to interact with the Kraken cryptocurrency exchange. Payward Ltd. and Kraken are in
-no way associated with the authors of this module and documentation.**
-
-This documentation refers to the `python-kraken-sdk`_ and serves to simplify the application of trading strategies,
-in which as far as possible all interaction possibilities with the cryptocurrency exchange Kraken are implemented, tested and documented.
-
-- Gladly open an issue on GitHub on make if something is incorrect or missing (`python-kraken-sdk/issues`_).
-- The output in the examples may differ, as these are only intended as examples and may change in the future.
-- If a certain endpoint is not reachable, the function :func:`kraken.base_api.KrakenBaseSpotAPI._request` or :func:`kraken.base_api.KrakenBaseFuturesAPI._request`,
-  which is also available in all derived REST clients, can be used to reach an endpoint with the appropriate parameters. Here private content can also be accessed,
-  provided that either the base class or one of the clients has been initialized with valid credentials.
+**This is the documentation of the unofficial Python SDK to interact with the
+Kraken cryptocurrency exchange. Payward Ltd. and Kraken are in no way associated
+with the authors of this module and documentation.**
+
+This documentation refers to the `python-kraken-sdk`_ and serves to simplify the
+application of trading strategies, in which as far as possible all interaction
+possibilities with the cryptocurrency exchange Kraken are implemented, tested
+and documented.
+
+- Gladly open an issue on GitHub on make if something is incorrect or missing
+  (`python-kraken-sdk/issues`_).
+- The output in the examples may differ, as these are only intended as examples
+  and may change in the future.
+- If a certain endpoint is not reachable, the function
+  :func:`kraken.base_api.KrakenBaseSpotAPI._request` or
+  :func:`kraken.base_api.KrakenBaseFuturesAPI._request`,
+  which is also available in all derived REST clients, can be used to reach an
+  endpoint with the appropriate parameters. Here private content can also be
+  accessed, provided that either the base class or one of the clients has been
+  initialized with valid credentials.
+- For Futures there is only one websocket client -
+  :class:`kraken.futures.KrakenFuturesWSClient`. For Spot there are two:
+  :class:`kraken.spot.KrakenSpotWSClient` (for API version 1) and
+  :class:`kraken.spot.KrakenSpotWSClientV2` (for API version 2).
 
 
 Disclaimer
 -------------
 
-There is no guarantee that this software will work flawlessly at this or later times. Of course,
-no responsibility is taken for possible profits or losses. This software probably has some errors in it, so use it at your own risk.
-Also no one should be motivated or tempted to invest assets in speculative forms of investment. By using this software you release the author(s)
-from any liability regarding the use of this software.
+There is no guarantee that this software will work flawlessly at this or later
+times. Of course, no responsibility is taken for possible profits or losses.
+This software probably has some errors in it, so use it at your own risk. Also
+no one should be motivated or tempted to invest assets in speculative forms of
+investment. By using this software you release the author(s) from any liability
+regarding the use of this software.
 
 
 Features
 --------
 
-Clients:
+Available Clients:
 
 - Spot REST Clients
-- Spot Websocket Client
+- Spot Websocket Clients (Websocket API v1 and v2)
+- Spot Orderbook Client
 - Futures REST Clients
 - Futures Websocket Client
 
 General:
 
-- access both public and private endpoints
-- responsive error handling, custom exceptions and logging
+- access both public and private, REST and websocket endpoints
+- responsive error handling and custom exceptions
 - extensive examples
-- all clients can be used as context manager
+- tested using the `pytest <https://docs.pytest.org/en/7.3.x/>`_ framework
+- releases are permanently archived at `Zenodo <https://zenodo.org/badge/latestdoi/510751854>`_
+
 
 Important Notice
 -----------------
-**ONLY tagged releases are available at PyPI**. The content of the master branch may not match with the content of the latest release.  - Please have a look at the release specific READMEs and changelogs.
+**ONLY tagged releases are available at PyPI**. The content of the master branch
+may not match with the content of the latest release. - Please have a look at
+the release specific READMEs and changelogs.
 
 .. _section-troubleshooting:
 
 Troubleshooting
 ---------------
-- Check if you downloaded and installed the **latest version** of the python-kraken-sdk.
-- Check the **permissions of your API keys** and the required permissions on the respective endpoints.
-- If you get some Cloudflare or **rate limit errors**, please check your Kraken Tier level and maybe apply for a higher rank if required.
-- **Use different API keys for different algorithms**, because the nonce calculation is based on timestamps and a sent nonce must always be the highest nonce ever sent of that API key. Having multiple algorithms using the same keys will result in invalid nonce errors.
+- Check if you downloaded and installed the **latest version** of the
+  python-kraken-sdk.
+- Check the **permissions of your API keys** and the required permissions on the
+  respective endpoints.
+- If you get some Cloudflare or **rate limit errors**, please check your
+  `Kraken`_ Tier level and maybe apply for a higher rank if required.
+- **Use different API keys for different algorithms**, because the nonce
+  calculation is based on timestamps and a sent nonce must always be the highest
+  nonce ever sent of that API key. Having multiple algorithms using the same
+  keys will result in invalid nonce errors.
 - Feel free to open an issue at `python-kraken-sdk/issues`_.
 
 
 References
 ----------
+
 - https://python-kraken-sdk.readthedocs.io/en/stable
 - https://docs.kraken.com/rest
 - https://docs.kraken.com/websockets
+- https://docs.kraken.com/websockets-v2
 - https://docs.futures.kraken.com
 - https://support.kraken.com/hc/en-us/sections/360012894412-Futures-API
```

### Comparing `python-kraken-sdk-1.5.0/docs/src/issues.rst` & `python-kraken-sdk-1.6.0/docs/src/issues.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,22 @@
+.. -*- coding: utf-8 -*-
+.. Copyright (C) 2023 Benjamin Thomas Schwertfeger
+.. GitHub: https://github.com/btschwertfeger
+
 Known Issues
 ============
 
 Issues listed here: `python-kraken-sdk/issues`_
 
 Futures Trading
 ---------------
 
-- Kraken's API doesn't seem to know the ``trailing_stop`` order type and raises an error if this type
-  is part of an order. This order type is documented here https://docs.futures.kraken.com/#http-api-trading-v3-api-order-management-send-order
+- Kraken's API doesn't seem to know the ``trailing_stop`` order type and raises
+  an error if this type is part of an order. This order type is documented here
+  https://docs.futures.kraken.com/#http-api-trading-v3-api-order-management-send-order
 
   .. code-block:: python
     :linenos:
     :caption: ``trailing_stop`` order type not working in Kraken Futures
 
     from kraken.futures import Trade
```

### Comparing `python-kraken-sdk-1.5.0/examples/futures_examples.py` & `python-kraken-sdk-1.6.0/examples/futures_examples.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,24 +17,25 @@
     datefmt="%Y/%m/%d %H:%M:%S",
     level=logging.INFO,
 )
 logging.getLogger().setLevel(logging.INFO)
 logging.getLogger("requests").setLevel(logging.WARNING)
 logging.getLogger("urllib3").setLevel(logging.WARNING)
 
-key = os.getenv("Futures_SANDBOX_KEY")
-secret = os.getenv("Futures_SANDBOX_SECRET")
+key = os.getenv("FUTURES_SANDBOX_KEY")
+secret = os.getenv("FUTURES_SANDBOX_SECRET")
 
 #  _   _  ___ _____ _____
 # | \ | |/ _ \_   _| ____|_
 # |  \| | | | || | |  _| (_)
 # | |\  | |_| || | | |___ _
 # |_| \_|\___/ |_| |_____(_)
 # ----> More examples can be found in kraken/tests/*.py
-# examples may not be updated regularly
+#
+# Examples may not be updated regularly
 
 
 def market_examples() -> None:
     """Example market client usage"""
     # market = Market()
     # print(market.get_tick_types())
     # print(market.get_tradeable_products(tick_type='trade'))
@@ -88,15 +89,15 @@
             if chunk:
                 file.write(chunk)
 
 
 def trade_examples() -> None:
     """Example Trade client usage"""
     raise ValueError(
-        "Attention: Please check if you really want to test the trade endpoints!"
+        "Attention: Please check if you really want to test the trade endpoints!",
     )
     trade = Trade(key=key, secret=secret, sandbox=True)
     print(trade.get_fills())
     print(trade.get_fills(lastFillTime="2020-07-21T12:41:52.790Z"))
     print(
         trade.create_batch_order(
             batchorder_list=[
@@ -124,45 +125,48 @@
                     "order_id": "e35d61dd-8a30-4d5f-a574-b5593ef0c050",
                 },
                 {
                     "order": "cancel",
                     "cliOrdId": 123456789,
                 },
             ],
-        )
+        ),
     )
     print(trade.cancel_all_orders())
     print(trade.cancel_all_orders(symbol="pi_xbtusd"))
     print(trade.dead_mans_switch(timeout=60))
     print(trade.dead_mans_switch(timeout=0))  # to deactivate
     print(trade.cancel_order(order_id="some order id"))
     print(
         trade.edit_order(
-            orderId="some order id", size=300, limitPrice=401, stopPrice=350
-        )
+            orderId="some order id",
+            size=300,
+            limitPrice=401,
+            stopPrice=350,
+        ),
     )
     print(trade.get_orders_status(orderIds=["orderid1", "orderid2"]))
     print(
         trade.create_order(
             orderType="lmt",
             side="buy",
             size=1,
             limitPrice=4,
             symbol="pf_bchusd",
-        )
+        ),
     )
     print(
         trade.create_order(
             orderType="take_profit",
             side="buy",
             size=1,
             symbol="pf_bchusd",
             stopPrice=100,
             triggerSignal="mark",
-        )
+        ),
     )
 
 
 def funding_examples() -> None:
     """Example Funding client usage"""
     funding = Funding(key=key, secret=secret, sandbox=True)
     print(funding.get_historical_funding_rates(symbol="PF_SOLUSD"))
```

### Comparing `python-kraken-sdk-1.5.0/examples/futures_trading_bot_template.py` & `python-kraken-sdk-1.6.0/examples/futures_trading_bot_template.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) 2023 Benjamin Thomas Schwertfeger
 # GitHub: https://github.com/btschwertfeger
 #
 
-"""Module that provides an example Futures trading bot data structure."""
+"""
+Module that provides a template to build a Futures trading algorithm using the
+python-kraken-sdk.
+"""
 
 from __future__ import annotations
 
 import asyncio
 import logging
 import logging.config
 import os
@@ -32,178 +35,191 @@
 logging.getLogger("urllib3").setLevel(logging.WARNING)
 
 
 class TradingBot(KrakenFuturesWSClient):
     """
     Class that implements the trading strategy
 
-    * The on_message function gets all events from the websocket feed
-    * Decisions can be made based on these events
+    * The on_message function gets all messages sent by the websocket feeds.
+    * Decisions can be made based on these messages
     * Can place trades using the self.__trade client
     * Do everything you want
 
     ====== P A R A M E T E R S ======
     config: dict
         configuration like: {
             'key' 'kraken-futures-key',
             'secret': 'kraken-secret-key',
             'products': ['PI_XBTUSD']
         }
     """
 
-    def __init__(self: "TradingBot", config: dict) -> None:
-        super().__init__(
-            key=config["key"], secret=config["secret"]
-        )  # initialize the KrakenFuturesWSClient
+    def __init__(self: TradingBot, config: dict) -> None:
+        super().__init__(  # initialize the KrakenFuturesWSClient
+            key=config["key"],
+            secret=config["secret"],
+        )
         self.__config: dict = config
 
         self.__user: User = User(key=config["key"], secret=config["secret"])
         self.__trade: Trade = Trade(key=config["key"], secret=config["secret"])
         self.__market: Market = Market(key=config["key"], secret=config["secret"])
         self.__funding: Funding = Funding(key=config["key"], secret=config["secret"])
 
-    async def on_message(self: "TradingBot", event: Union[list, dict]) -> None:
-        """Receives all events that came form the websocket feed(s)"""
-        logging.info(event)
-        # ... apply your trading strategy here
-
-        # call functions from self.__trade and other clients if conditions met...
-
-        # response = self.__trade.create_order(
-        #     orderType='lmt',
-        #     size=2,
-        #     symbol='PI_XBTUSD',
-        #     side='buy',
-        #     limitPrice=10000
+    async def on_message(self: TradingBot, msg: Union[list, dict]) -> None:
+        """Receives all messages that came form the websocket feed(s)"""
+        logging.info(msg)
+
+        # == apply your trading strategy here ==
+
+        # Call functions of `self.__trade` and other clients if conditions met …
+        # print(
+        #     self.__trade.create_order(
+        #         orderType='lmt',
+        #         size=2,
+        #         symbol='PI_XBTUSD',
+        #         side='buy',
+        #         limitPrice=10000
+        #     )
         # )
-        # ...
 
-        # you can also un-/subscribe here using `self.subscribe(...)` or `self.unsubscribe(...)`
+        # You can also un-/subscribe here using `self.subscribe(...)` or
+        # `self.unsubscribe(...)`
+        # … more can be found in the documentation
+        #        (https://python-kraken-sdk.readthedocs.io/en/stable/).
 
-    # add more functions to customize the trading strategy
-    # ...
-    # ...
+    # Add more functions to customize the trading strategy …
 
-    def save_exit(self: "TradingBot", reason: Optional[str] = "") -> None:
+    def save_exit(self: TradingBot, reason: Optional[str] = "") -> None:
         """Controlled shutdown of the strategy"""
-        logging.warning(f"Save exit triggered, reason: {reason}")
-        # ideas:
+        logging.warning(
+            "Save exit triggered, reason: {reason}",
+            extra={"reason": reason},
+        )
+        # some ideas:
         #   * save the bots data
         #   * maybe close trades
         #   * enable dead man's switch
         sys.exit(1)
 
 
 class ManagedBot:
     """
     Class to manage the trading strategy
 
-    Subscribes to desired feeds, instantiates the strategy and runs until condition met
+    … subscribes to desired feeds, instantiates the strategy and runs as long
+    as there is no error.
 
     ====== P A R A M E T E R S ======
     config: dict
         bot configuration like: {
             'key' 'kraken-futures-key',
             'secret': 'kraken-secret-key',
             'products': ['PI_XBTUSD']
         }
     """
 
-    def __init__(self: "ManagedBot", config: dict) -> None:
+    def __init__(self: ManagedBot, config: dict) -> None:
         self.__config: dict = config
         self.__trading_strategy: Optional[TradingBot] = None
 
-    def run(self: "ManagedBot") -> None:
+    def run(self: ManagedBot) -> None:
         """Runner function"""
         if not self.__check_credentials():
             sys.exit(1)
 
         try:
             asyncio.run(self.__main())
         except KeyboardInterrupt:
-            pass
-        finally:
-            if self.__trading_strategy is not None:
-                self.__trading_strategy.save_exit(reason="Asyncio loop left")
+            self.save_exit(reason="KeyboardInterrupt")
+        else:
+            self.save_exit(reason="Asyncio loop left")
 
-    async def __main(self: "ManagedBot") -> None:
+    async def __main(self: ManagedBot) -> None:
         """
         Instantiates the trading strategy/algorithm and subscribes to the
         desired websocket feeds. Run the loop while no exception occur.
 
-        Thi variable `exception_occur` which is an attribute of the KrakenFuturesWSClient
-        can be set individually but is also being set to `True` if the websocket connection
-        has some fatal error. This is used to exit the asyncio loop.
+        Thi variable `exception_occur` which is an attribute of the
+        KrakenFuturesWSClient can be set individually but is also being set to
+        `True` if the websocket connection has some fatal error. This is used to
+        exit the asyncio loop - but you can also apply your own reconnect rules.
         """
         self.__trading_strategy = TradingBot(config=self.__config)
 
         await self.__trading_strategy.subscribe(
-            feed="ticker", products=self.__config["products"]
+            feed="ticker",
+            products=self.__config["products"],
         )
         await self.__trading_strategy.subscribe(
-            feed="book", products=self.__config["products"]
+            feed="book",
+            products=self.__config["products"],
         )
 
         await self.__trading_strategy.subscribe(feed="fills")
         await self.__trading_strategy.subscribe(feed="open_positions")
         await self.__trading_strategy.subscribe(feed="open_orders")
         await self.__trading_strategy.subscribe(feed="balances")
 
         while not self.__trading_strategy.exception_occur:
             try:
-                # check if bot feels good
+                # check if the strategy feels good
                 # maybe send a status update every day
-                # ...
+                # …
                 pass
 
             except Exception as exc:
                 message: str = f"Exception in main: {exc} {traceback.format_exc()}"
                 logging.error(message)
                 self.__trading_strategy.save_exit(reason=message)
 
             await asyncio.sleep(6)
         self.__trading_strategy.save_exit(
-            reason="Left main loop because of exception in strategy."
+            reason="Left main loop because of exception in strategy.",
         )
-        return
 
-    def __check_credentials(self: "ManagedBot") -> bool:
+    def __check_credentials(self: ManagedBot) -> bool:
         """Checks the user credentials and the connection to Kraken"""
         try:
             User(self.__config["key"], self.__config["secret"]).get_wallets()
-            logging.info("Client credentials are valid")
+            logging.info("Client credentials are valid.")
             return True
         except urllib3.exceptions.MaxRetryError:
             logging.error("MaxRetryError, cannot connect.")
             return False
         except requests.exceptions.ConnectionError:
             logging.error("ConnectionError, Kraken not available.")
             return False
         except KrakenException.KrakenAuthenticationError:
             logging.error("Invalid credentials!")
             return False
 
-    def save_exit(self: "ManagedBot", reason: str = "") -> None:
+    def save_exit(self: ManagedBot, reason: str = "") -> None:
         """Calls the save exit function of the trading strategy"""
         print(f"Save exit triggered - {reason}")
         if self.__trading_strategy is not None:
             self.__trading_strategy.save_exit(reason=reason)
+        else:
+            sys.exit(1)
 
 
 def main() -> None:
-    """Main"""
-    bot_config: dict = {
-        "key": os.getenv("FUTURES_API_KEY"),
-        "secret": os.getenv("FUTURES_SECRET_KEY"),
-        "products": ["PI_XBTUSD", "PF_SOLUSD"],
-    }
+    """Example main - load environment variables and run the strategy."""
+
+    managed_bot: ManagedBot = ManagedBot(
+        config={
+            "key": os.getenv("FUTURES_API_KEY"),
+            "secret": os.getenv("FUTURES_SECRET_KEY"),
+            "products": ["PI_XBTUSD", "PF_SOLUSD"],
+        },
+    )
+
     try:
-        managed_bot: ManagedBot = ManagedBot(config=bot_config)
         managed_bot.run()
     except Exception:
         managed_bot.save_exit(
-            reason=f"manageBot.run() has ended: {traceback.format_exc()}"
+            reason=f"manageBot.run() has ended: {traceback.format_exc()}",
         )
 
 
 if __name__ == "__main__":
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `python-kraken-sdk-1.5.0/examples/futures_ws_examples.py` & `python-kraken-sdk-1.6.0/examples/futures_ws_examples.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) 2023 Benjamin Thomas Schwertfeger
 # GitHub: https://github.com/btschwertfeger
 #
 
-"""Module that provides an example usage for the Kraken Futures websocket client"""
+"""
+Module that provides an example usage for the Kraken Futures websocket client.
+"""
 
 from __future__ import annotations
 
 import asyncio
 import logging
 import logging.config
 import os
 import time
+from contextlib import suppress
 from typing import Union
 
 from kraken.futures import KrakenFuturesWSClient
 
 logging.basicConfig(
     format="%(asctime)s %(module)s,line: %(lineno)d %(levelname)8s | %(message)s",
     datefmt="%Y/%m/%d %H:%M:%S",
@@ -24,89 +27,82 @@
 )
 logging.getLogger().setLevel(logging.INFO)
 logging.getLogger("requests").setLevel(logging.WARNING)
 logging.getLogger("urllib3").setLevel(logging.WARNING)
 
 
 async def main() -> None:
-    """Create bot and subscribe to topics/feeds"""
+    """Create a client and subscribe to channels/feeds"""
 
-    key = os.getenv("Futures_API_KEY")
-    secret = os.getenv("Futures_SECRET_KEY")
+    key = os.getenv("FUTURES_API_KEY")
+    secret = os.getenv("FUTURES_SECRET_KEY")
 
-    # ___Custom_Trading_Bot__________
-    class Bot(KrakenFuturesWSClient):
-        """Can be used to create a custom trading strategy/bot"""
+    # Custom client
+    class Client(KrakenFuturesWSClient):
+        """Can be used to create a custom trading strategy"""
 
-        async def on_message(self: "Bot", msg: Union[list, dict]) -> None:
-            """receives the websocket messages"""
+        async def on_message(self: "Client", msg: Union[list, dict]) -> None:
+            """Receives the websocket messages"""
             logging.info(msg)
-            # ... apply your trading strategy here
-            # you can also combine this with the Futures REST clients
+            # … apply your trading strategy here
+            # … you can also combine this with the Futures REST clients
 
     # _____Public_Websocket_Feeds___________________
-    bot = Bot()
-    # print(bot.get_available_public_subscription_feeds())
+    client = Client()
+    # print(client.get_available_public_subscription_feeds())
 
     products = ["PI_XBTUSD", "PF_SOLUSD"]
     # subscribe to a public websocket feed
-    await bot.subscribe(feed="ticker", products=products)
-    await bot.subscribe(feed="book", products=products)
-    # await bot.subscribe(feed='trade', products=products)
-    # await bot.subscribe(feed='ticker_lite', products=products)
-    # await bot.subscribe(feed='heartbeat')
+    await client.subscribe(feed="ticker", products=products)
+    await client.subscribe(feed="book", products=products)
+    # await client.subscribe(feed='trade', products=products)
+    # await client.subscribe(feed='ticker_lite', products=products)
+    # await client.subscribe(feed='heartbeat')
     # time.sleep(2)
 
     # unsubscribe from a websocket feed
     time.sleep(2)  # in case subscribe is not done yet
-    # await bot.unsubscribe(feed='ticker', products=['PI_XBTUSD'])
-    await bot.unsubscribe(feed="ticker", products=["PF_XBTUSD"])
-    await bot.unsubscribe(feed="book", products=products)
+    # await client.unsubscribe(feed='ticker', products=['PI_XBTUSD'])
+    await client.unsubscribe(feed="ticker", products=["PF_XBTUSD"])
+    await client.unsubscribe(feed="book", products=products)
     # ...
 
     # _____Private_Websocket_Feeds_________________
-    auth_bot = Bot(key=key, secret=secret)
-    # print(auth_bot.get_available_private_subscription_feeds())
+    client_auth = Client(key=key, secret=secret)
+    # print(client_auth.get_available_private_subscription_feeds())
 
     # subscribe to a private/authenticated websocket feed
-    await auth_bot.subscribe(feed="fills")
-    await auth_bot.subscribe(feed="open_positions")
-    # await auth_bot.subscribe(feed='open_orders')
-    # await auth_bot.subscribe(feed='open_orders_verbose')
-    # await auth_bot.subscribe(feed='deposits_withdrawals')
-    # await auth_bot.subscribe(feed='account_balances_and_margins')
-    # await auth_bot.subscribe(feed='balances')
-    # await auth_bot.subscribe(feed='account_log')
-    # await auth_bot.subscribe(feed='notifications_auth')
+    await client_auth.subscribe(feed="fills")
+    await client_auth.subscribe(feed="open_positions")
+    # await client_auth.subscribe(feed='open_orders')
+    # await client_auth.subscribe(feed='open_orders_verbose')
+    # await client_auth.subscribe(feed='deposits_withdrawals')
+    # await client_auth.subscribe(feed='account_balances_and_margins')
+    # await client_auth.subscribe(feed='balances')
+    # await client_auth.subscribe(feed='account_log')
+    # await client_auth.subscribe(feed='notifications_auth')
 
     # authenticated clients can also subscribe to public feeds
-    # await auth_bot.subscribe(feed='ticker', products=['PI_XBTUSD', 'PF_ETHUSD'])
+    # await client_auth.subscribe(feed='ticker', products=['PI_XBTUSD', 'PF_ETHUSD'])
 
     # time.sleep(1)
-    # unsubscribe from a private/authenticaed websocket feed
-    await auth_bot.unsubscribe(feed="fills")
-    await auth_bot.unsubscribe(feed="open_positions")
+    # unsubscribe from a private/authenticated websocket feed
+    await client_auth.unsubscribe(feed="fills")
+    await client_auth.unsubscribe(feed="open_positions")
     # ...
 
-    while not bot.exception_occur and not auth_bot.exception_occur:
+    while not client.exception_occur and not client_auth.exception_occur:
         await asyncio.sleep(6)
-    return
 
 
 if __name__ == "__main__":
-    loop = asyncio.new_event_loop()
-    asyncio.set_event_loop(loop)
-    try:
+    with suppress(KeyboardInterrupt):
         asyncio.run(main())
-    except KeyboardInterrupt:
-        # the websocket client will send {'event': 'asyncio.CancelledError'} via on_message
-        # so you can handle the behavior/next actions individually within you bot
-        pass
-    finally:
-        loop.close()
+    # the websocket client will send {'event': 'asyncio.CancelledError'} via on_message
+    # so you can handle the behavior/next actions individually within you strategy
 
 # ============================================================
 # Alternative - as ContextManager:
 
 # from kraken.futures import KrakenFuturesWSClient
 # import asyncio
 
@@ -120,9 +116,7 @@
 #         await asyncio.sleep(6)
 
 # if __name__ == "__main__":
 #     try:
 #         asyncio.run(main())
 #     except KeyboardInterrupt:
 #         pass
-#     finally:
-#         loop.close()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `python-kraken-sdk-1.5.0/examples/market_client_example.ipynb` & `python-kraken-sdk-1.6.0/examples/market_client_example.ipynb`

 * *Files identical despite different names*

### Comparing `python-kraken-sdk-1.5.0/examples/spot_examples.py` & `python-kraken-sdk-1.6.0/examples/spot_examples.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,54 +27,58 @@
 secret = os.getenv("SECRET_KEY")
 
 #  _   _  ___ _____ _____
 # | \ | |/ _ \_   _| ____|_
 # |  \| | | | || | |  _| (_)
 # | |\  | |_| || | | |___ _
 # |_| \_|\___/ |_| |_____(_)
-# ----> More examples can be found in kraken/tests/*.py, the doc and in the doc strings
-# examples may not be updated regularly
+# ----> More examples can be found in kraken/tests/*.py, the doc and in the
+# doc strings
+#
+# Examples may not be updated regularly.
 
 
 def user_examples() -> None:
     """Example usage of the User client"""
     user = User(key=key, secret=secret)
 
     print(user.get_account_balance())
     print(user.get_trade_balance())  # asset='BTC'
     print(user.get_open_orders())
     print(user.get_closed_orders())
     print(
-        user.get_orders_info(txid="OBQFM7-JNVKS-H3ULEH")
+        user.get_orders_info(txid="OBQFM7-JNVKS-H3ULEH"),
     )  # or txid='id1,id2,id3' or txid=['id1','id2']
     print(user.get_trades_history())
     time.sleep(3)
     print(user.get_trades_info(txid="TCNTTR-QBEVO-E5H5UK"))
     print(user.get_open_positions())  # txid='someid'
     print(
-        user.get_ledgers_info()
+        user.get_ledgers_info(),
     )  # asset='BTC' or asset='BTC,EUR' or asset=['BTC','EUR']
     print(user.get_ledgers(id_="LIORGR-33NXH-LBUS5Z"))
     print(user.get_trade_volume())  # pair='BTC/EUR'
 
     # ____export_report____
     response = user.request_export_report(
-        report="ledgers", description="myLedgers1", format="CSV"
+        report="ledgers",
+        description="myLedgers1",
+        format="CSV",
     )  # report='trades'
     print(user.get_export_report_status(report="ledgers"))
 
     # save report to file
     response_data = user.retrieve_export(id_=response["id"])
     with open("myExport.zip", "wb") as file:
         for chunk in response_data.iter_content(chunk_size=512):
             if chunk:
                 file.write(chunk)
 
     print(
-        user.delete_export_report(id_=response["id"], type_="delete")
+        user.delete_export_report(id_=response["id"], type_="delete"),
     )  # alternative: type_=cancel
 
 
 def market_examples() -> None:
     """Example usage of the Market client"""
     market = Market()
 
@@ -88,23 +92,27 @@
     print(market.get_system_status())
     time.sleep(2)
 
 
 def trade_examples() -> None:
     """Example usage of the Trade client"""
     raise ValueError(
-        "Attention: Please check if you really want to execute trade functions."
+        "Attention: Please check if you really want to execute trade functions.",
     )
     trade = Trade(key=key, secret=secret)
 
     if False:
         print(
             trade.create_order(
-                ordertype="limit", side="buy", volume=1, pair="BTC/EUR", price=0.01
-            )
+                ordertype="limit",
+                side="buy",
+                volume=1,
+                pair="BTC/EUR",
+                price=0.01,
+            ),
         )
         print(
             trade.create_order_batch(
                 orders=[
                     {
                         "close": {
                             "ordertype": "stop-loss-limit",
@@ -126,71 +134,74 @@
                         "type": "sell",
                         "userref": "1dfgesggwe5t3",
                         "volume": 123,
                     },
                 ],
                 pair="BTC/USD",
                 validate=True,
-            )
+            ),
         )
 
         print(
-            trade.edit_order(txid="sometxid", pair="BTC/EUR", volume=4.2, price=17000)
+            trade.edit_order(txid="sometxid", pair="BTC/EUR", volume=4.2, price=17000),
         )
         time.sleep(2)
 
         print(trade.cancel_order(txid="O2JLFP-VYFIW-35ZAAE"))
         print(trade.cancel_all_orders())
         print(trade.cancel_all_orders_after_x(timeout=6))
 
     print(
         trade.cancel_order_batch(
             orders=[
                 "O2JLFP-VYFIW-35ZAAE",
                 "O523KJ-DO4M2-KAT243",
                 "OCDIAL-YC66C-DOF7HS",
                 "OVFPZ2-DA2GV-VBFVVI",
-            ]
-        )
+            ],
+        ),
     )
 
 
 def funding_examples() -> None:
     """Example usage of the Funding client"""
     funding = Funding(key=key, secret=secret)
     print(funding.get_deposit_methods(asset="DOT"))
     # print(funding.get_deposit_address(asset='DOT', method='Polkadot'))
     # print(funding.get_recent_deposits_status(asset='DOT'))
     print(
-        funding.get_withdrawal_info(asset="DOT", key="MyPolkadotWallet", amount="200")
+        funding.get_withdrawal_info(asset="DOT", key="MyPolkadotWallet", amount="200"),
     )
 
     raise ValueError(
-        "Attention: Please check if you really want to execute funding functions."
+        "Attention: Please check if you really want to execute funding functions.",
     )
     if False:
         time.sleep(2)
         print(funding.withdraw_funds(asset="DOT", key="MyPolkadotWallet", amount=200))
         print(funding.get_recent_withdraw_status(asset="DOT"))
         print(funding.cancel_widthdraw(asset="DOT", refid="12345"))
         print(
             funding.wallet_transfer(
-                asset="ETH", amount=0.100, from_="Spot Wallet", to_="Futures Wallet"
-            )
+                asset="ETH",
+                amount=0.100,
+                from_="Spot Wallet",
+                to_="Futures Wallet",
+            ),
         )
 
 
 def staking_examples() -> None:
     """Example usage of the Staking client"""
     staking = Staking(key=key, secret=secret)
     print(staking.list_stakeable_assets())
     print(staking.list_staking_transactions())
     print(staking.get_pending_staking_transactions())
     raise ValueError(
-        "Attention: Please check if you really want to execute staking functions."
+        "Attention: Please check if you really want to execute staking functions.",
     )
     if False:
         print(staking.stake_asset(asset="DOT", amount=2000, method="polkadot-staked"))
         print(staking.unstake_asset(asset="DOT", amount=200, method="polkadot-staked"))
         time.sleep(2)
```

### Comparing `python-kraken-sdk-1.5.0/examples/spot_orderbook.py` & `python-kraken-sdk-1.6.0/examples/spot_orderbook.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) 2023 Benjamin Thomas Schwertfeger
 # GitHub: https://github.com/btschwertfeger
 #
 
 """
-This module provides an example on how to use the Spot Orderbook
-client of the python-kraken-sdk (https://github.com/btschwertfeger/python-kraken-sdk)
-to retrieve and maintain a valid Spot order book for (a) specific
-asset pair(s). It can be run directly without any credentials if the
-python-kraken-sdk is installed.
+This module provides an example on how to use the Spot Orderbook client of the
+python-kraken-sdk (https://github.com/btschwertfeger/python-kraken-sdk) to
+retrieve and maintain a valid Spot order book for (a) specific asset pair(s).
+It can be run directly without any credentials if the python-kraken-sdk is
+installed.
 
     python3 -m pip install python-kraken-sdk
 
-The output when running this snippet looks like the following table and
-updates the book as soon as Kraken sent any order book update.
+The output when running this snippet looks like the following table and updates
+the book as soon as Kraken sent any order book update.
 
 Bid         Volume               Ask         Volume
 27076.00000 (8.28552127)         27076.10000 (2.85897056)
 27075.90000 (3.75748052)         27077.30000 (0.57243521)
 27074.40000 (0.57249652)         27080.80000 (0.00100000)
 27072.90000 (0.01200917)         27081.00000 (0.00012345)
 27072.80000 (0.25000000)         27081.70000 (0.30000000)
 27072.30000 (4.89735970)         27082.70000 (0.05539777)
 27072.20000 (2.65896716)         27082.80000 (0.00400000)
 27072.10000 (2.77037635)         27082.90000 (0.57231684)
 27072.00000 (0.81770000)         27083.00000 (0.38934000)
 27071.50000 (0.07194657)         27083.80000 (2.76918992)
 
-This can be the basis of an order book based trading strategy where
-realtime data and fast price movements are considered.
+This can be the basis of an order book based trading strategy where realtime
+data and fast price movements are considered.
 """
 
 from __future__ import annotations
 
 import asyncio
 from typing import Any, Dict, List, Tuple
 
@@ -45,59 +45,62 @@
     This is a wrapper class that is used to overload the :func:`on_book_update`
     function. It can also be used as a base for trading strategy. Since the
     :class:`OrderbookClient` is derived from :class:`KrakenSpotWSClient`
     it can also be used to access the :func:`subscribe` function and any
     other provided utility.
     """
 
-    async def on_book_update(self: "Orderbook", pair: str, message: list) -> None:
+    async def on_book_update(self: Orderbook, pair: str, message: list) -> None:
         """
         This function is called every time the order book of ``pair`` gets
         updated.
 
-        The ``pair`` parameter can be used to access the updated order book
-        as shown in the function body below.
+        The ``pair`` parameter can be used to access the updated order book as
+        shown in the function body below.
 
         :param pair: The currency pair of the updated order book
         :type pair: str
         :param message: The message sent by Kraken (not needed in most cases)
         :type message: list
         """
         book: Dict[str, Any] = self.get(pair=pair)
         bid: List[Tuple[str, str]] = list(book["bid"].items())
         ask: List[Tuple[str, str]] = list(book["ask"].items())
 
-        print("Bid         Volume\t\t Ask         Volume")
+        print("Bid     Volume\t\t  Ask     Volume")
         for level in range(self.depth):
             print(
-                f"{bid[level][0]} ({bid[level][1][0]}) \t {ask[level][0]} ({ask[level][1][0]})"
+                f"{bid[level][0]} ({bid[level][1][0]}) \t {ask[level][0]} ({ask[level][1][0]})",
             )
 
         assert book["valid"]  # ensure that the checksum is valid
+        # … the client will automatically resubscribe to a book feed if the
+        #   checksum is not valid. The user must not do anything for that, but
+        #   will get informed.
 
 
 async def main() -> None:
     """
     Here we depth of the order book and also a pair. We could
     subscribe to multiple pairs, but for simplicity only XBT/USD is chosen.
 
     The Orderbook class can be instantiated, which receives the order
     book-related messages, after we subscribed to the book feed.
 
     Finally we need some "game loop" - so we create a while loop
     that runs as long as there is no error.
     """
-    orderbook: Orderbook = Orderbook()
+    orderbook: Orderbook = Orderbook(depth=10)
 
     await orderbook.add_book(
-        pairs=["XBT/USD"]  # we can also subscribe to more currency pairs
+        pairs=["BTC/USD"],  # we can also subscribe to more currency pairs
     )
 
     while not orderbook.exception_occur:
         await asyncio.sleep(10)
 
 
 if __name__ == "__main__":
     try:
         asyncio.run(main())
     except KeyboardInterrupt:
-        pass
+        print("KeyboardInterrupt!")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `python-kraken-sdk-1.5.0/examples/spot_trading_bot_template.py` & `python-kraken-sdk-1.6.0/examples/spot_trading_bot_template_v2.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,225 +1,251 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) 2023 Benjamin Thomas Schwertfeger
 # GitHub: https://github.com/btschwertfeger
 
-
-"""Module that provides an example Futures trading bot data structure."""
+"""
+Module that provides a template to build a Spot trading algorithm using the
+python-kraken-sdk and Kraken Spot websocket API v1.
+"""
 
 from __future__ import annotations
 
 import asyncio
 import logging
 import logging.config
 import os
 import sys
 import traceback
-from typing import Optional, Union
+from typing import Any, Optional
 
 import requests
 import urllib3
 
 from kraken.exceptions import KrakenException
-from kraken.spot import Funding, KrakenSpotWSClient, Market, Staking, Trade, User
+from kraken.spot import Funding, KrakenSpotWSClientV2, Market, Staking, Trade, User
+
+logging.basicConfig(
+    format="%(asctime)s %(module)s,line: %(lineno)d %(levelname)8s | %(message)s",
+    datefmt="%Y/%m/%d %H:%M:%S",
+    level=logging.INFO,
+)
+logging.getLogger().setLevel(logging.INFO)
+logging.getLogger("requests").setLevel(logging.WARNING)
+logging.getLogger("urllib3").setLevel(logging.WARNING)
 
 
-class TradingBot(KrakenSpotWSClient):
+class TradingBot(KrakenSpotWSClientV2):
     """
     Class that implements the trading strategy
 
-    * The on_message function gets all events from the websocket feed
-    * Decisions can be made based on these events
-    * Can place trades using the self.__trade client
+    * The on_message function gets all messages sent by the websocket feeds.
+    * Decisions can be made based on these messages
+    * Can place trades using the self.__trade client or self.send_message
     * Do everything you want
 
     ====== P A R A M E T E R S ======
     config: dict
         configuration like: {
-            'key' 'kraken-futures-key',
-            'secret': 'kraken-secret-key',
-            'products': ['PI_XBTUSD']
+            "key": "kraken-spot-key",
+            "secret": "kraken-spot-secret",
+            "pairs": ["DOT/USD", "BTC/USD"],
         }
     """
 
-    def __init__(self: "TradingBot", config: dict) -> None:
-        super().__init__(
-            key=config["key"], secret=config["secret"]
-        )  # initialize the KakenFuturesWSClient
+    def __init__(self: TradingBot, config: dict, **kwargs: Any) -> None:
+        super().__init__(  # initialize the KrakenSpotWSClientV2
+            key=config["key"],
+            secret=config["secret"],
+            **kwargs,
+        )
         self.__config: dict = config
 
         self.__user: User = User(key=config["key"], secret=config["secret"])
         self.__trade: Trade = Trade(key=config["key"], secret=config["secret"])
         self.__market: Market = Market(key=config["key"], secret=config["secret"])
         self.__funding: Funding = Funding(key=config["key"], secret=config["secret"])
         self.__staking: Staking = Staking(key=config["key"], secret=config["secret"])
 
-    async def on_message(self: "TradingBot", event: Union[dict, list]) -> None:
-        """Receives all events that came form the websocket connection"""
-        if isinstance(event, dict) and "event" in event:
-            if event["event"] == "heartbeat":
-                return
-            if event["event"] == "pong":
-                return
-            if "error" in event:
-                # handle exceptions/errors sent by websocket connection ...
-                pass
-
-        logging.info(event)
+    async def on_message(self: TradingBot, message: dict) -> None:
+        """Receives all messages of the websocket connection(s)"""
+        if message.get("method") == "pong" or message.get("channel") == "heartbeat":
+            return
+        if "error" in message:
+            # handle exceptions/errors sent by websocket connection …
+            pass
 
-        # ... apply your trading strategy here
+        logging.info(message)
 
-        # call functions from self.__trade and other clients if conditions met...
+        # == apply your trading strategy here ==
 
+        # Call functions of `self.__trade` and other clients if conditions met …
         # try:
         #     print(self.__trade.create_order(
         #         ordertype='limit',
         #         side='buy',
         #         volume=2,
         #         pair='XBTUSD',
         #         price=12000
         #     ))
         # except KrakenException.KrakenPermissionDeniedError:
-        #    # ... handle exceptions
+        #    # … handle exceptions
         #    pass
 
         # The spot websocket client also allow sending orders via websockets
         # this is way faster than using REST endpoints.
-
-        # await self.create_order(
-        #     ordertype='limit',
-        #     side='buy',
-        #     pair='BTC/EUR',
-        #     price=20000,
-        #     volume=200
+        # await self.send_message(
+        #     message={
+        #         "method": "add_order",
+        #         "params": {
+        #             "limit_price": 1234.56,
+        #             "order_type": "limit",
+        #             "order_userref": 123456789,
+        #             "order_qty": 1.0,
+        #             "side": "buy",
+        #             "symbol": "BTC/USD",
+        #             "validate": True,
+        #         },
+        #     }
         # )
 
-        # you can also un-/subscribe here using `self.subscribe(...)` or `self.unsubscribe(...)`
-
-        # more can be found in the documentation
+        # You can also un-/subscribe here using `self.subscribe(...)` or
+        # `self.unsubscribe(...)`.
+        #
+        # … more can be found in the documentation
+        #        (https://python-kraken-sdk.readthedocs.io/en/stable/).
 
-    # add more functions to customize the trading strategy
-    # ...
+    # Add more functions to customize the trading strategy …
 
-    def save_exit(self: "TradingBot", reason: Optional[str] = "") -> None:
+    def save_exit(self: TradingBot, reason: Optional[str] = "") -> None:
         """controlled shutdown of the strategy"""
-        logging.warning(f"Save exit triggered, reason: {reason}")
-        # ideas:
-        #   * save the bots data
+        logging.warning(
+            "Save exit triggered, reason: {reason}",
+            extra={"reason": reason},
+        )
+        # some ideas:
+        #   * save the current data
         #   * maybe close trades
         #   * enable dead man's switch
         sys.exit(1)
 
 
 class ManagedBot:
     """
     Class to manage the trading strategy
 
-    subscribes to desired feeds, instantiates the strategy and runs until condition met
+    … subscribes to desired feeds, instantiates the strategy and runs as long
+    as there is no error.
 
     ====== P A R A M E T E R S ======
     config: dict
         configuration like: {
-            'key' 'kraken-futures-key',
-            'secret': 'kraken-secret-key',
-            'products': ['PI_XBTUSD']
+            "key" "kraken-spot-key",
+            "secret": "kraken-secret-key",
+            "pairs": ["DOT/USD", "BTC/USD"],
         }
     """
 
-    def __init__(self: "ManagedBot", config: dict):
+    def __init__(self: ManagedBot, config: dict):
         self.__config: dict = config
         self.__trading_strategy: Optional[TradingBot] = None
 
-    def run(self: "ManagedBot") -> None:
+    def run(self: ManagedBot) -> None:
         """Starts the event loop and bot"""
         if not self.__check_credentials():
             sys.exit(1)
 
         try:
             asyncio.run(self.__main())
         except KeyboardInterrupt:
-            pass
-        finally:
-            if self.__trading_strategy is not None:
-                self.__trading_strategy.save_exit(reason="Asyncio loop left")
+            self.save_exit(reason="KeyboardInterrupt")
+        else:
+            self.save_exit(reason="Asyncio loop left")
 
-    async def __main(self: "ManagedBot") -> None:
+    async def __main(self: ManagedBot) -> None:
         """
-        Instantiates the trading strategy (bot) and subscribes to the
-        desired websocket feeds. While no exception within the strategy occur
-        run the loop.
-
-        This variable `exception_occur` which is an attribute of the KrakenSpotWSClient
-        can be set individually but is also being set to True if the websocket connection
-        has some fatal error. This is used to exit the asyncio loop.
+        Instantiates the trading strategy and subscribes to the desired
+        websocket feeds. While no exception within the strategy occur run the
+        loop.
+
+        The variable `exception_occur` which is an attribute of the
+        KrakenSpotWSClient can be set individually but is also being set to
+        `True` if the websocket connection has some fatal error. This is used to
+        exit the asyncio loop - but you can also apply your own reconnect rules.
         """
         self.__trading_strategy = TradingBot(config=self.__config)
 
         await self.__trading_strategy.subscribe(
-            subscription={"name": "ticker"}, pair=self.__config["pairs"]
+            params={"channel": "ticker", "symbol": self.__config["pairs"]},
         )
         await self.__trading_strategy.subscribe(
-            subscription={"name": "ohlc", "interval": 15}, pair=self.__config["pairs"]
+            params={
+                "channel": "ohlc",
+                "interval": 15,
+                "symbol": self.__config["pairs"],
+            },
         )
 
-        await self.__trading_strategy.subscribe(subscription={"name": "ownTrades"})
-        await self.__trading_strategy.subscribe(subscription={"name": "openOrders"})
+        await self.__trading_strategy.subscribe(params={"channel": "executions"})
 
         while not self.__trading_strategy.exception_occur:
             try:
-                # check if bot feels good
-                # maybe send a status update every day
-                # ...
+                # check if the algorithm feels good
+                # maybe send a status update every day via Telegram or Mail
+                # …
                 pass
 
             except Exception as exc:
                 message: str = f"Exception in main: {exc} {traceback.format_exc()}"
                 logging.error(message)
                 self.__trading_strategy.save_exit(reason=message)
 
             await asyncio.sleep(6)
         self.__trading_strategy.save_exit(
-            reason="Left main loop because of exception in strategy."
+            reason="Left main loop because of exception in strategy.",
         )
-        return
 
-    def __check_credentials(self: "ManagedBot") -> bool:
+    def __check_credentials(self: ManagedBot) -> bool:
         """Checks the user credentials and the connection to Kraken"""
         try:
             User(self.__config["key"], self.__config["secret"]).get_account_balance()
-            logging.info("Client credentials are valid")
+            logging.info("Client credentials are valid.")
             return True
         except urllib3.exceptions.MaxRetryError:
             logging.error("MaxRetryError, cannot connect.")
             return False
         except requests.exceptions.ConnectionError:
             logging.error("ConnectionError, Kraken not available.")
             return False
         except KrakenException.KrakenAuthenticationError:
             logging.error("Invalid credentials!")
             return False
 
-    def save_exit(self: "ManagedBot", reason: str = "") -> None:
+    def save_exit(self: ManagedBot, reason: str = "") -> None:
         """Invoke the save exit function of the trading strategy"""
         print(f"Save exit triggered - {reason}")
         if self.__trading_strategy is not None:
             self.__trading_strategy.save_exit(reason=reason)
+        else:
+            sys.exit(1)
 
 
 def main() -> None:
-    """Main"""
-    bot_config: dict = {
-        "key": os.getenv("API_KEY"),
-        "secret": os.getenv("SECRET_KEY"),
-        "pairs": ["DOT/EUR", "XBT/USD"],
-    }
-    managed_bot: ManagedBot = ManagedBot(config=bot_config)
+    """Example main - load environment variables and run the strategy."""
+    managed_bot: ManagedBot = ManagedBot(
+        config={
+            "key": os.getenv("SPOT_API_KEY"),
+            "secret": os.getenv("SPOT_SECRET_KEY"),
+            "pairs": ["DOT/USD", "BTC/USD"],
+        },
+    )
+
     try:
         managed_bot.run()
     except Exception:
         managed_bot.save_exit(
-            reason=f"manageBot.run() has ended: {traceback.format_exc()}"
+            reason=f"manageBot.run() has ended: {traceback.format_exc()}",
         )
 
 
 if __name__ == "__main__":
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `python-kraken-sdk-1.5.0/examples/spot_ws_examples.py` & `python-kraken-sdk-1.6.0/examples/spot_ws_examples_v1.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) 2023 Benjamin Thomas Schwertfeger
 # GitHub: https://github.com/btschwertfeger
 #
 
-"""Module that provides an example usage for the Kraken Spot websocket client."""
+"""
+Module that provides an example usage for the KrakenSpotWebsocketClient.
+It uses the Kraken Websocket API v1.
+"""
 
 from __future__ import annotations
 
 import asyncio
 import logging
 import logging.config
 import os
-import time
+from contextlib import suppress
 from typing import Union
 
 from kraken.spot import KrakenSpotWSClient
 
 logging.basicConfig(
     format="%(asctime)s %(module)s,line: %(lineno)d %(levelname)8s | %(message)s",
     datefmt="%Y/%m/%d %H:%M:%S",
@@ -24,86 +27,86 @@
 )
 logging.getLogger().setLevel(logging.INFO)
 logging.getLogger("requests").setLevel(logging.WARNING)
 logging.getLogger("urllib3").setLevel(logging.WARNING)
 
 
 async def main() -> None:
-    """Create bot and subscribe to topics/feeds"""
+    """Create a client and subscribe to channels/feeds"""
 
     key: str = os.getenv("SPOT_API_KEY")
     secret: str = os.getenv("SPOT_SECRET_KEY")
 
-    # ___Custom_Trading_Bot______________
-    class Bot(KrakenSpotWSClient):
-        """Can be used to create a custom trading strategy/bot"""
+    class Client(KrakenSpotWSClient):
+        """Can be used to create a custom trading strategy"""
 
-        async def on_message(self: "Bot", msg: Union[list, dict]) -> None:
+        async def on_message(self: Client, message: Union[list, dict]) -> None:
             """Receives the websocket messages"""
-            if isinstance(msg, dict) and "event" in msg:
-                topic = msg["event"]
+            if isinstance(message, dict) and "event" in message:
+                topic = message["event"]
                 if topic in ("heartbeat", "pong"):
                     return
 
-            print(msg)
+            print(message)
             # if condition:
             #     await self.create_order(
             #         ordertype="limit",
             #         side="buy",
-            #         pair="BTC/EUR",
+            #         pair="BTC/USD",
             #         price=20000,
             #         volume=200
             #     )
             # ... it is also possible to call regular REST endpoints
-            # but using the websocket messages is more efficient
-            # you can also un/subscribe here using self.subscribe/self-unsubscribe
+            # but using the websocket messages is more efficient.
+            # You can also un-/subscribe here using self.subscribe/self.unsubscribe.
 
     # ___Public_Websocket_Feed_____
-    bot: Bot = Bot()  # only use this one if you don't need private feeds
-    # print(bot.public_sub_names) # list public subscription names
+    client: Client = Client()  # only use this one if you don't need private feeds
+    # print(client.public_channel_names) # list public subscription names
 
-    await bot.subscribe(subscription={"name": "ticker"}, pair=["XBT/EUR", "DOT/EUR"])
-    await bot.subscribe(subscription={"name": "spread"}, pair=["XBT/EUR", "DOT/EUR"])
-    await bot.subscribe(subscription={"name": "book"}, pair=["BTC/EUR"])
-    # await bot.subscribe(subscription={ "name": "book", "depth": 25}, pair=["BTC/EUR"])
-    # await bot.subscribe(subscription={ "name": "ohlc" }, pair=["BTC/EUR"])
-    # await bot.subscribe(subscription={ "name": "ohlc", "interval": 15}, pair=["XBT/EUR", "DOT/EUR"])
-    # await bot.subscribe(subscription={ "name": "trade" }, pair=["BTC/EUR"])
-    # await bot.subscribe(subscription={ "name": "*"} , pair=["BTC/EUR"])
-
-    time.sleep(2)  # wait because unsubscribing is faster than subscribing ...
-    # print(bot.active_public_subscriptions)
-    await bot.unsubscribe(subscription={"name": "ticker"}, pair=["XBT/EUR", "DOT/EUR"])
-    await bot.unsubscribe(subscription={"name": "spread"}, pair=["XBT/EUR"])
-    await bot.unsubscribe(subscription={"name": "spread"}, pair=["DOT/EUR"])
-    # ....
-
-    auth_bot = Bot(key=key, secret=secret)
-    # print(bot.active_private_subscriptions)
-    # print(auth_bot.private_sub_names) # list private subscription names
-    # when using the authenticated bot, you can also subscribe to public feeds
-    await auth_bot.subscribe(subscription={"name": "ownTrades"})
-    await auth_bot.subscribe(subscription={"name": "openOrders"})
-
-    time.sleep(2)
-    await auth_bot.unsubscribe(subscription={"name": "ownTrades"})
-    await auth_bot.unsubscribe(subscription={"name": "openOrders"})
+    await client.subscribe(subscription={"name": "ticker"}, pair=["XBT/USD", "DOT/USD"])
+    await client.subscribe(subscription={"name": "spread"}, pair=["XBT/USD", "DOT/USD"])
+    await client.subscribe(subscription={"name": "book"}, pair=["BTC/USD"])
+    # await client.subscribe(subscription={ "name": "book", "depth": 25}, pair=["BTC/USD"])
+    # await client.subscribe(subscription={ "name": "ohlc" }, pair=["BTC/USD"])
+    # await client.subscribe(subscription={ "name": "ohlc", "interval": 15}, pair=["XBT/USD", "DOT/USD"])
+    # await client.subscribe(subscription={ "name": "trade" }, pair=["BTC/USD"])
+    # await client.subscribe(subscription={ "name": "*"} , pair=["BTC/USD"])
+
+    await asyncio.sleep(2)  # wait because unsubscribing is faster than subscribing ...
+    # print(client.active_public_subscriptions)
+    await client.unsubscribe(
+        subscription={"name": "ticker"},
+        pair=["XBT/USD", "DOT/USD"],
+    )
+    await client.unsubscribe(subscription={"name": "spread"}, pair=["XBT/USD"])
+    await client.unsubscribe(subscription={"name": "spread"}, pair=["DOT/USD"])
+    # ...
+
+    client_auth = Client(key=key, secret=secret)
+    # print(client_auth.active_private_subscriptions)
+    # print(client_auth.private_channel_names) # list private channel names
+    # when using the authenticated client, you can also subscribe to public feeds
+    await client_auth.subscribe(subscription={"name": "ownTrades"})
+    await client_auth.subscribe(subscription={"name": "openOrders"})
+
+    await asyncio.sleep(2)
+    await client_auth.unsubscribe(subscription={"name": "ownTrades"})
+    await client_auth.unsubscribe(subscription={"name": "openOrders"})
 
-    while not bot.exception_occur and not auth_bot.exception_occur:
+    while not client.exception_occur and not client_auth.exception_occur:
         await asyncio.sleep(6)
-    return
 
 
 if __name__ == "__main__":
-    try:
+    with suppress(KeyboardInterrupt):
         asyncio.run(main())
-    except KeyboardInterrupt:
-        pass
-        # the websocket client will send {'event': 'asyncio.CancelledError'} via on_message
-        # so you can handle the behavior/next actions individually within you bot
+    # The websocket client will send {'event': 'asyncio.CancelledError'}
+    # via on_message so you can handle the behavior/next actions
+    # individually within your strategy.
 
 # ============================================================
 # Alternative - as ContextManager:
 
 # from kraken.spot import KrakenSpotWSClient
 # import asyncio
 
@@ -118,9 +121,7 @@
 #         await asyncio.sleep(6)
 
 # if __name__ == "__main__":
 #     try:
 #         asyncio.run(main())
 #     except KeyboardInterrupt:
 #         pass
-#     finally:
-#         loop.close()
```

### Comparing `python-kraken-sdk-1.5.0/kraken/base_api/__init__.py` & `python-kraken-sdk-1.6.0/kraken/base_api/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) 2023 Benjamin Thomas Schwertfeger
 # GitHub: https://github.com/btschwertfeger
 
 """Module that implements the base classes for all Spot and Futures clients"""
 
+from __future__ import annotations
+
 import base64
 import hashlib
 import hmac
 import json
 import time
 import urllib.parse
 from functools import wraps
@@ -60,99 +62,102 @@
             if parameter_name in kwargs:
                 value: Any = kwargs[parameter_name]
                 if isinstance(value, str) or value is None:
                     pass
                 elif isinstance(value, list):
                     kwargs[parameter_name] = ",".join(value)
                 else:
-                    raise ValueError(
-                        f"{parameter_name} cannot be {type(kwargs[parameter_name])}!"
+                    raise TypeError(
+                        f"{parameter_name} can't be {type(kwargs[parameter_name])}!",
                     )
 
             return func(*args, **kwargs)
 
         return wrapper
 
     return decorator
 
 
 class KrakenErrorHandler:
     """
     Class that checks if the response of a request contains error messages and
-    returns either message if there is no error or raises a custom KrakenException
-    based on the error message.
+    returns either message if there is no error or raises a custom
+    KrakenException based on the error message.
     """
 
-    def __init__(self: "KrakenErrorHandler") -> None:
+    def __init__(self: KrakenErrorHandler) -> None:
         self.__kexceptions: KrakenException = KrakenException()
 
-    def __get_exception(self: "KrakenErrorHandler", msg: str) -> Optional[Any]:
+    def __get_exception(self: KrakenErrorHandler, msg: str) -> Optional[Any]:
         """
         Must be called when an error was found in the message, so the corresponding
         KrakenException will be returned.
         """
         return self.__kexceptions.get_exception(msg)
 
-    def check(self: "KrakenErrorHandler", data: dict) -> Union[dict, Any]:
+    def check(self: KrakenErrorHandler, data: dict) -> Union[dict, Any]:
         """
-        Check if the error message is a known KrakenError response and than raise
-        a custom exception or return the data containing the "error".
+        Check if the error message is a known KrakenError response and than
+        raise a custom exception or return the data containing the "error".
         This is only for the Spot REST endpoints, since the Futures API
         serves kinds of errors.
 
         :param data: The response as dict to check for an error
         :type data: dict
-        :raise kraken.exceptions.KrakenException.*: raises a KrakenError if the response contains an error
+        :raise kraken.exceptions.KrakenException.*: raises a KrakenError if the
+            response contains an error
         :return: The response as dict
         :rtype: dict
         :raises KrakenError: If is the error keyword in the response
         """
         if len(data.get("error", [])) == 0 and "result" in data:
             return data["result"]
 
         exception = self.__get_exception(data["error"])
         if exception:
             raise exception(data)
         return data
 
-    def check_send_status(self: "KrakenErrorHandler", data: dict) -> dict:
+    def check_send_status(self: KrakenErrorHandler, data: dict) -> dict:
         """
         Checks the responses of Futures REST endpoints
 
         :param data: The response as dict to check for an error
         :type data: dict
-        :raise kraken.exceptions.KrakenException.*: raises a KrakenError if the response contains an error
+        :raise kraken.exceptions.KrakenException.*: raises a KrakenError if the
+            response contains an error
         :return: The response as dict
         :rtype: dict
         """
         if "sendStatus" in data and "status" in data["sendStatus"]:
             exception: Type[KrakenException] = self.__get_exception(
-                data["sendStatus"]["status"]
+                data["sendStatus"]["status"],
             )
             if exception:
                 raise exception(data)
             return data
         return data
 
-    def check_batch_status(self: "KrakenErrorHandler", data: dict) -> dict:
+    def check_batch_status(self: KrakenErrorHandler, data: dict) -> dict:
         """
         Used to check the Futures batch order responses for errors
 
         :param data: The response as dict to check for an error
         :type data: dict
-        :raise kraken.exceptions.KrakenException.*: raises a KrakenError if the response contains an error
-        :return: The response as List[dict]
+        :raise kraken.exceptions.KrakenException.*: raises a KrakenError if the
+            response contains an error
+        :return: The response as list[dict]
         :rtype: dict
         """
         if "batchStatus" in data:
             batch_status: List[Dict[str, Any]] = data["batchStatus"]
             for status in batch_status:
                 if "status" in status:
                     exception: Type[KrakenException] = self.__get_exception(
-                        status["status"]
+                        status["status"],
                     )
                     if exception:
                         raise exception(data)
         return data
 
 
 class KrakenBaseSpotAPI:
@@ -162,23 +167,24 @@
 
     :param key: Spot API public key (default: ``""``)
     :type key: str, optional
     :param secret: Spot API secret key (default: ``""``)
     :type secret: str, optional
     :param url: URL to access the Kraken API (default: https://api.kraken.com)
     :type url: str, optional
-    :param sandbox: Use the sandbox (not supported for Spot trading so far, default: ``False``)
+    :param sandbox: Use the sandbox (not supported for Spot trading so far,
+        default: ``False``)
     :type sandbox: bool, optional
     """
 
     URL: str = "https://api.kraken.com"
     API_V: str = "/0"
 
     def __init__(
-        self: "KrakenBaseSpotAPI",
+        self: KrakenBaseSpotAPI,
         key: str = "",
         secret: str = "",
         url: str = "",
         sandbox: bool = False,
         use_custom_exceptions: bool = True,
     ):
         if sandbox:
@@ -193,55 +199,59 @@
         self.__use_custom_exceptions: bool = use_custom_exceptions
 
         self.__err_handler: KrakenErrorHandler = KrakenErrorHandler()
         self.__session: requests.Session = requests.Session()
         self.__session.headers.update({"User-Agent": "python-kraken-sdk"})
 
     def _request(
-        self: "KrakenBaseSpotAPI",
+        self: KrakenBaseSpotAPI,
         method: str,
         uri: str,
         timeout: int = 10,
         auth: bool = True,
         params: Optional[dict] = None,
         do_json: bool = False,
         return_raw: bool = False,
     ) -> Union[Dict[str, Any], List[str], List[Dict[str, Any]], requests.Response]:
         """
-        Handles the requested requests, by sending the request, handling the response,
-        and returning the message or in case of an error the respective Exception.
+        Handles the requested requests, by sending the request, handling the
+        response, and returning the message or in case of an error the
+        respective Exception.
 
         :param method:  The request method, e.g., ``GET``, ``POST``, and ``PUT``
         :type method: str
         :param uri: The endpoint to send the message
         :type uri: str
         :param timeout: Timeout for the request (default: ``10``)
         :type timeout: int
         :param auth: If the requests needs authentication (default: ``True``)
         :type auth: bool
-        :param params: The query or post parameter of the request (default: ``None``)
-        :type params: Optional[dict]
-        :param do_json: If the ``params`` must be "jsonified" - in case of nested dict style
+        :param params: The query or post parameter of the request (default:
+            ``None``)
+        :type params: dict, optional
+        :param do_json: If the ``params`` must be "jsonified" - in case of
+            nested dict style
         :type do_json: bool
-        :param return_raw: If the response should be returned without parsing. This is used
-         for example when requesting an export of the trade history as .zip archive.
-        :type return_raw: bool
-        :raise kraken.exceptions.KrakenException.*: If the response contains errors
+        :param return_raw: If the response should be returned without parsing.
+            This is used for example when requesting an export of the trade
+            history as .zip archive.
+        :type return_raw: bool, optional
+        :raise kraken.exceptions.KrakenException.*: If the response contains
+            errors
         :return: The response
-        :rtype: Union[Dict[str, Any], List[str], List[Dict[str, Any]], requests.Response]
+        :rtype: dict[str, Any] | list[str] | list[dict[str, Any]] | requests.Response
         """
         if params is None:
             params = {}
 
         method = method.upper()
         data_json: str = ""
-        if method in ("GET", "DELETE"):
-            if params:
-                data_json = "&".join([f"{key}={params[key]}" for key in sorted(params)])
-                uri += f"?{data_json}".replace(" ", "%20")
+        if method in ("GET", "DELETE") and params:
+            data_json = "&".join([f"{key}={params[key]}" for key in sorted(params)])
+            uri += f"?{data_json}".replace(" ", "%20")
 
         headers: dict = {}
         if auth:
             if (
                 not self.__key
                 or self.__key == ""
                 or not self.__secret
@@ -265,22 +275,25 @@
                     "Content-Type": content_type,
                     "API-Key": self.__key,
                     "API-Sign": self._get_kraken_signature(
                         url_path=f"{self.API_V}{uri}",
                         data=sign_data,
                         nonce=params["nonce"],
                     ),
-                }
+                },
             )
 
         url: str = f"{self.url}{uri}"
         if method in ("GET", "DELETE"):
             return self.__check_response_data(
                 self.__session.request(
-                    method=method, url=url, headers=headers, timeout=timeout
+                    method=method,
+                    url=url,
+                    headers=headers,
+                    timeout=timeout,
                 ),
                 return_raw,
             )
 
         if do_json:
             return self.__check_response_data(
                 self.__session.request(
@@ -291,25 +304,32 @@
                     timeout=timeout,
                 ),
                 return_raw,
             )
 
         return self.__check_response_data(
             self.__session.request(
-                method=method, url=url, headers=headers, data=params, timeout=timeout
+                method=method,
+                url=url,
+                headers=headers,
+                data=params,
+                timeout=timeout,
             ),
             return_raw,
         )
 
     def _get_kraken_signature(
-        self: "KrakenBaseSpotAPI", url_path: str, data: str, nonce: int
+        self: KrakenBaseSpotAPI,
+        url_path: str,
+        data: str,
+        nonce: int,
     ) -> str:
         """
-        Creates the signature of the data. This is required for authenticated requests
-        to verify the user.
+        Creates the signature of the data. This is required for authenticated
+        requests to verify the user.
 
         :param url_path: The endpoint including the api version
         :type url_path: str
         :param data: Data of the request to sign, including the nonce.
         :type data: str
         :param nonce: The nonce to sign with
         :type nonce: int
@@ -318,29 +338,31 @@
         """
         return base64.b64encode(
             hmac.new(
                 base64.b64decode(self.__secret),
                 url_path.encode()
                 + hashlib.sha256((str(nonce) + data).encode()).digest(),
                 hashlib.sha512,
-            ).digest()
+            ).digest(),
         ).decode()
 
     def __check_response_data(
-        self: "KrakenBaseSpotAPI", response: requests.Response, return_raw: bool = False
+        self: KrakenBaseSpotAPI,
+        response: requests.Response,
+        return_raw: bool = False,
     ) -> Union[dict, list, requests.Response]:
         """
         Checks the response, handles the error (if exists) and returns the response data.
 
         :param response: The response of a request, requested by the requests module
         :type response: requests.Response
         :param return_raw: Defines if the return should be the raw response if there is no error
-        :type data: bool
+        :type data: bool, optional
         :return: The response in raw or parsed to dict
-        :rtype: Union[dict, list, requests.Response]
+        :rtype: dict | list | requests.Response
         """
         if not self.__use_custom_exceptions:
             return response
 
         if response.status_code in ("200", 200):
             if return_raw:
                 return response
@@ -353,27 +375,29 @@
                 # can only be dict if error is present:
                 return self.__err_handler.check(data)  # type: ignore[arg-type]
             return data
 
         raise Exception(f"{response.status_code} - {response.text}")
 
     @property
-    def return_unique_id(self: "KrakenBaseSpotAPI") -> str:
+    def return_unique_id(self: KrakenBaseSpotAPI) -> str:
         """Returns a unique uuid string
 
         :return: uuid
         :rtype: str
         """
         return "".join(str(uuid1()).split("-"))
 
-    def __enter__(self: "KrakenBaseSpotAPI") -> "KrakenBaseSpotAPI":
+    def __enter__(self: KrakenBaseSpotAPI) -> KrakenBaseSpotAPI:
         return self
 
     def __exit__(
-        self: "KrakenBaseSpotAPI", *exc: tuple, **kwargs: Dict[str, Any]
+        self: KrakenBaseSpotAPI,
+        *exc: tuple,
+        **kwargs: Dict[str, Any],
     ) -> None:
         pass
 
 
 class KrakenBaseFuturesAPI:
     """
     The base class for all Futures clients handles un-/signed requests
@@ -392,15 +416,15 @@
     :type sandbox: bool, optional
     """
 
     URL: str = "https://futures.kraken.com"
     SANDBOX_URL: str = "https://demo-futures.kraken.com"
 
     def __init__(
-        self: "KrakenBaseFuturesAPI",
+        self: KrakenBaseFuturesAPI,
         key: str = "",
         secret: str = "",
         url: str = "",
         sandbox: bool = False,
         use_custom_exceptions: bool = True,
     ):
         self.sandbox: bool = sandbox
@@ -417,47 +441,53 @@
         self.__use_custom_exceptions: bool = use_custom_exceptions
 
         self.__err_handler: KrakenErrorHandler = KrakenErrorHandler()
         self.__session: requests.Session = requests.Session()
         self.__session.headers.update({"User-Agent": "python-kraken-sdk"})
 
     def _request(
-        self: "KrakenBaseFuturesAPI",
+        self: KrakenBaseFuturesAPI,
         method: str,
         uri: str,
         timeout: int = 10,
         auth: bool = True,
         post_params: Optional[dict] = None,
         query_params: Optional[dict] = None,
         return_raw: bool = False,
     ) -> Union[Dict[str, Any], List[Dict[str, Any]], List[str], requests.Response]:
         """
-        Handles the requested requests, by sending the request, handling the response,
-        and returning the message or in case of an error the respective Exception.
+        Handles the requested requests, by sending the request, handling the
+        response, and returning the message or in case of an error the
+        respective Exception.
 
         :param method:  The request method, e.g., ``GET``, ``POST``, and ``PUT``
         :type method: str
         :param uri: The endpoint to send the message
         :type uri: str
         :param timeout: Timeout for the request (default: ``10``)
         :type timeout: int
         :param auth: If the request needs authentication (default: ``True``)
         :type auth: bool
-        :param post_params: The query parameter of the request (default: ``None``)
-        :type post_params: Optional[dict]
-        :param query_params: The query parameter of the request (default: ``None``)
-        :type query_params: Optional[dict]
-        :param do_json: If the ``post_params`` must be "jsonified" - in case of nested dict style
-        :type do_json: bool
+        :param post_params: The query parameter of the request (default:
+            ``None``)
+        :type post_params: dict, optional
+        :param query_params: The query parameter of the request (default:
+            ``None``)
+        :type query_params: dict, optional
+        :param do_json: If the ``post_params`` must be "jsonified" - in case of
+            nested dict style
+        :type do_json: bool, optional
         :param return_raw: If the response should be returned without parsing.
-            This is used for example when requesting an export of the trade history as .zip archive.
-        :type return_raw: bool
-        :raise kraken.exceptions.KrakenException.*: If the response contains errors
+            This is used for example when requesting an export of the trade
+            history as .zip archive.
+        :type return_raw: bool, optional
+        :raise kraken.exceptions.KrakenException.*: If the response contains
+            errors
         :return: The response
-        :rtype: Union[Dict[str, Any], List[Dict[str, Any]], List[str], requests.Response]
+        :rtype: dict[str, Any] | list[dict[str, Any]] | list[str] | requests.Response
         """
         method = method.upper()
 
         post_string: str = ""
         strl: List[str]
         if post_params is not None:
             strl = [f"{key}={post_params[key]}" for key in sorted(post_params)]
@@ -484,17 +514,19 @@
             nonce: str = str(int(time.time() * 100_000_000))
             headers.update(
                 {
                     "Content-Type": "application/x-www-form-urlencoded; charset=utf-8",
                     "Nonce": nonce,
                     "APIKey": self.__key,
                     "Authent": self._get_kraken_futures_signature(
-                        uri, query_string + post_string, nonce
+                        uri,
+                        query_string + post_string,
+                        nonce,
                     ),
-                }
+                },
             )
 
         if method in ("GET", "DELETE"):
             return self.__check_response_data(
                 self.__session.request(
                     method=method,
                     url=f"{self.url}{uri}"
@@ -526,19 +558,22 @@
                 headers=headers,
                 timeout=timeout,
             ),
             return_raw,
         )
 
     def _get_kraken_futures_signature(
-        self: "KrakenBaseFuturesAPI", endpoint: str, data: str, nonce: str
+        self: KrakenBaseFuturesAPI,
+        endpoint: str,
+        data: str,
+        nonce: str,
     ) -> str:
         """
-        Creates the signature of the data. This is required for authenticated requests
-        to verify the user.
+        Creates the signature of the data. This is required for authenticated
+        requests to verify the user.
 
         :param endpoint: The endpoint including the api version
         :type endpoint: str
         :param data: Data of the request to sign, including the nonce.
         :type data: dict
         :param nonce: The nonce to use for this signature
         :type nonce: str
@@ -548,33 +583,39 @@
         if endpoint.startswith("/derivatives"):
             endpoint = endpoint[len("/derivatives") :]
 
         sha256_hash = hashlib.sha256()
         sha256_hash.update((data + nonce + endpoint).encode("utf8"))
         return base64.b64encode(
             hmac.new(
-                base64.b64decode(self.__secret), sha256_hash.digest(), hashlib.sha512
-            ).digest()
+                base64.b64decode(self.__secret),
+                sha256_hash.digest(),
+                hashlib.sha512,
+            ).digest(),
         ).decode()
 
     def __check_response_data(
-        self: "KrakenBaseFuturesAPI",
+        self: KrakenBaseFuturesAPI,
         response: requests.Response,
         return_raw: bool = False,
     ) -> Union[dict, requests.Response]:
         """
-        Checks the response, handles the error (if exists) and returns the response data.
+        Checks the response, handles the error (if exists) and returns the
+        response data.
 
-        :param response: The response of a request, requested by the requests module
+        :param response: The response of a request, requested by the requests
+            module
         :type response: requests.Response
-        :param return_raw: Defines if the return should be the raw response if there is no error
-        :type return_raw: dict
-        :raise kraken.exceptions.KrakenException.*: If the response contains the error key
+        :param return_raw: Defines if the return should be the raw response if
+            there is no error
+        :type return_raw: dict, optional
+        :raise kraken.exceptions.KrakenException.*: If the response contains the
+            error key
         :return: The signed string
-        :rtype: Union[dict, Response]
+        :rtype: dict | requests.Response
         """
         if not self.__use_custom_exceptions:
             return response
 
         if response.status_code in ("200", 200):
             if return_raw:
                 return response
@@ -589,12 +630,15 @@
                 return self.__err_handler.check_send_status(data)
             if "batchStatus" in data:
                 return self.__err_handler.check_batch_status(data)
             return data
 
         raise Exception(f"{response.status_code} - {response.text}")
 
-    def __enter__(self: "KrakenBaseFuturesAPI") -> "KrakenBaseFuturesAPI":
+    def __enter__(self: KrakenBaseFuturesAPI) -> KrakenBaseFuturesAPI:
         return self
 
     def __exit__(self, *exc: tuple, **kwargs: Dict[str, Any]) -> None:
         pass
+
+
+__all__ = ["defined", "ensure_string", "KrakenBaseSpotAPI", "KrakenBaseFuturesAPI"]
```

### Comparing `python-kraken-sdk-1.5.0/kraken/exceptions/__init__.py` & `python-kraken-sdk-1.6.0/kraken/exceptions/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) 2023 Benjamin Thomas Schwertfeger
 # GitHub: https://github.com/btschwertfeger
 
+"""
+Module that provides custom exceptions for the python-kraken-sdk
+
+TODO: make each Error separate
+"""
+
+from __future__ import annotations
 
-"""Module that provides custom exceptions for the python-kraken-sdk"""
 import functools
 from typing import Any, Dict, List, Optional, Union
 
 
 def docstring_message(cls: Any) -> Any:
     """
     Decorates an exception to make its docstring its default message.
 
     - https://stackoverflow.com/a/66491013/13618168
     """
     cls_init = cls.__init__
 
     @functools.wraps(cls.__init__)
     def wrapped_init(
-        self: "KrakenException",
+        self: KrakenException,
         msg: Optional[Union[str, dict]] = None,
         *args: tuple,
         **kwargs: Dict[str, Any],
     ) -> None:
         err_message: str = (
             self.__doc__ if not msg else f"{self.__doc__}\nDetails: {msg}"
         )
@@ -39,15 +45,15 @@
     Class that provides custom exceptions for the python-kraken-sdk based on the
     error messages that can be received from the Kraken Spot and Futures API.
 
     - https://docs.kraken.com/rest/#section/General-Usage/Requests-Responses-and-Errors
     """
 
     def __init__(
-        self: "KrakenException",
+        self: KrakenException,
         msg: Optional[Union[str, dict]] = None,
         *args: tuple,
         **kwargs: Dict[str, Any],
     ) -> None:
         self.EXCEPTION_ASSIGNMENT: Dict[str, Any] = {
             ##      Spot, Margin, and Futures trading Errors
             ##
@@ -56,14 +62,15 @@
             "EGeneral:Permission denied": self.KrakenPermissionDeniedError,
             "EGeneral:Unknown method": self.KrakenUnknownMethodError,
             "EGeneral:Temporary lockout": self.KrakenTemporaryLockoutError,
             "EService:Unavailable": self.KrakenServiceUnavailableError,
             "EService:Market in cancel_only mode": self.KrakenMarketInOnlyCancelModeError,
             "EService:Market in post_only mode": self.KrakenMarketInOnlyPostModeError,
             "EService:Deadline elapsed": self.KrakenDeadlineElapsedError,
+            "EAuth:Failed": self.KrakenAuthenticationFailedError,
             "EAPI:Invalid key": self.KrakenInvalidAPIKeyError,
             "EAPI:Invalid signature": self.KrakenInvalidSignatureError,
             "EAPI:Invalid nonce": self.KrakenInvalidNonceError,
             "EAPI:Rate limit exceeded": self.KrakenApiLimitExceededError,
             "EAPI:Bad request": self.KrakenBadRequestError,
             "EOrder:Invalid order": self.KrakenInvalidOrderError,
             "EOrder:Invalid price": self.KrakenInvalidPriceError,
@@ -101,15 +108,16 @@
             "Unavailable": self.KrakenUnavailableError,
             "invalidAccount": self.KrakenInvalidAccountError,
             "notFound": self.KrakenNotFoundError,
             "orderForEditNotFound": self.KrakenOrderForEditNotFoundError,
         }
 
     def get_exception(
-        self: "KrakenException", data: Union[str, List[str]]
+        self: KrakenException,
+        data: Union[str, List[str]],
     ) -> Optional[Any]:
         """Returns the exception given by name if available"""
         is_list: bool = isinstance(data, list)
         for name, exception in self.EXCEPTION_ASSIGNMENT.items():
             if is_list:
                 if name in data:
                     return exception
@@ -177,14 +185,18 @@
         """Price is invalid."""
 
     @docstring_message
     class KrakenAuthenticationError(Exception):
         """Credentials are invalid."""
 
     @docstring_message
+    class KrakenAuthenticationFailedError(Exception):
+        """The account or its permissions could not be authenticated."""
+
+    @docstring_message
     class KrakenCannotOpenPositionError(Exception):
         """User/tier is ineligible for margin trading."""
 
     @docstring_message
     class KrakenMarginAllowedExceededError(Exception):
         """User has exceeded their margin allowance."""
 
@@ -304,7 +316,10 @@
     class KrakenTemporaryLockoutError(Exception):
         """The account was temporary locked out."""
 
     # ? ____CUSTOM_EXCEPTIONS_________
     @docstring_message
     class MaxReconnectError(Exception):
         """To many reconnect tries."""
+
+
+__all__ = ["KrakenException"]
```

### Comparing `python-kraken-sdk-1.5.0/kraken/futures/funding.py` & `python-kraken-sdk-1.6.0/kraken/futures/funding.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) 2023 Benjamin Thomas Schwertfeger
 # GitHub: https://github.com/btschwertfeger
 
 """Module that implements the Kraken Futures Funding client"""
 
+from __future__ import annotations
+
 from typing import Optional, Union
 
-from ..base_api import KrakenBaseFuturesAPI
+from kraken.base_api import KrakenBaseFuturesAPI
 
 
 class Funding(KrakenBaseFuturesAPI):
     """
     Class that implements the Kraken Futures Funding client
 
     If the sandbox environment is chosen, the keys must be generated from here:
@@ -48,19 +50,19 @@
         key: str = "",
         secret: str = "",
         url: str = "",
         sandbox: bool = False,
     ) -> None:
         super().__init__(key=key, secret=secret, url=url, sandbox=sandbox)
 
-    def __enter__(self: "Funding") -> "Funding":
+    def __enter__(self: Funding) -> Funding:
         super().__enter__()
         return self
 
-    def get_historical_funding_rates(self, symbol: str) -> dict:
+    def get_historical_funding_rates(self: Funding, symbol: str) -> dict:
         """
         Retrieve information about the historical funding rates of a specific ``symbol``
 
         - https://docs.futures.kraken.com/#http-api-trading-v3-api-historical-funding-rates-historicalfundingrates
 
         :param symbol: The futures symbol to filter for
         :type symbol: str
@@ -91,15 +93,15 @@
             method="GET",
             uri="/derivatives/api/v4/historicalfundingrates",
             query_params={"symbol": symbol},
             auth=False,
         )
 
     def initiate_wallet_transfer(
-        self,
+        self: Funding,
         amount: Union[str, int, float],
         fromAccount: str,
         toAccount: str,
         unit: str,
     ) -> dict:
         """
         Submit a wallet transfer request to transfer funds between margin accounts.
@@ -144,15 +146,15 @@
                 "toAccount": toAccount,
                 "unit": unit,
             },
             auth=True,
         )
 
     def initiate_subaccount_transfer(
-        self,
+        self: Funding,
         amount: Union[str, int, float],
         fromAccount: str,
         fromUser: str,
         toAccount: str,
         toUser: str,
         unit: str,
     ) -> dict:
@@ -201,15 +203,15 @@
                 "toUser": toUser,
                 "unit": unit,
             },
             auth=True,
         )
 
     def initiate_withdrawal_to_spot_wallet(
-        self,
+        self: Funding,
         amount: Union[str, int, float],
         currency: str,
         sourceWallet: Optional[str] = None,
         **kwargs: dict,
     ) -> dict:
         """
         Enables the transfer of funds between the futures and spot wallet.
@@ -250,7 +252,10 @@
         params.update(kwargs)
         return self._request(  # type: ignore[return-value]
             method="POST",
             uri="/derivatives/api/v3/withdrawal",
             post_params=params,
             auth=True,
         )
+
+
+__all__ = ["Funding"]
```

### Comparing `python-kraken-sdk-1.5.0/kraken/futures/market.py` & `python-kraken-sdk-1.6.0/kraken/futures/market.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) 2023 Benjamin Thomas Schwertfeger
 # GitHub: https://github.com/btschwertfeger
 
 """Module that implements the Kraken Futures market client"""
 
+from __future__ import annotations
+
 from functools import lru_cache
 from typing import List, Optional, Union
 
-from ..base_api import KrakenBaseFuturesAPI, defined
+from kraken.base_api import KrakenBaseFuturesAPI, defined
 
 
 class Market(KrakenBaseFuturesAPI):
 
     """
     Class that implements the Kraken Futures market client
 
@@ -42,28 +44,28 @@
 
         >>> from kraken.futures import Market
         >>> with Market() as market:
         ...     print(market.get_tick_types())
     """
 
     def __init__(
-        self: "Market",
+        self: Market,
         key: str = "",
         secret: str = "",
         url: str = "",
         sandbox: bool = False,
     ) -> None:
         super().__init__(key=key, secret=secret, url=url, sandbox=sandbox)
 
-    def __enter__(self: "Market") -> "Market":
+    def __enter__(self: Market) -> Market:
         super().__enter__()
         return self
 
     def get_ohlc(
-        self: "Market",
+        self: Market,
         tick_type: str,
         symbol: str,
         resolution: int,
         from_: Optional[int] = None,
         to: Optional[int] = None,
     ) -> dict:
         """
@@ -124,15 +126,15 @@
             method="GET",
             uri=f"/api/charts/v1/{tick_type}/{symbol}/{resolution}",
             query_params=params,
             auth=False,
         )
 
     @lru_cache()
-    def get_tick_types(self: "Market") -> List[str]:
+    def get_tick_types(self: Market) -> List[str]:
         """
         Retrieve the available tick types that can be used for example to access
         the :func:`kraken.futures.Market.get_ohlc` endpoint.
 
         - https://docs.futures.kraken.com/#http-api-charts-ohlc-get-tick-types
 
         This function uses caching. Run ``get_tick_types.cache_clear()`` to clear.
@@ -147,15 +149,15 @@
             >>> from kraken.futures import Market
             >>> Market().get_tick_types()
             ['mark', 'spot', 'trade']
         """
         return self._request(method="GET", uri="/api/charts/v1/", auth=False)  # type: ignore[return-value]
 
     @lru_cache()
-    def get_tradeable_products(self: "Market", tick_type: str) -> List[str]:
+    def get_tradeable_products(self: Market, tick_type: str) -> List[str]:
         """
         Retrieve a list containing the tradeable assets on the futures market.
 
         - https://docs.futures.kraken.com/#http-api-charts-ohlc-get-tradeable-products
 
         This function uses caching. Run ``get_tradeable_products.cache_clear()`` to clear.
 
@@ -169,19 +171,21 @@
             :caption: Futures Market: Get the tradeable products
 
             >>> from kraken.futures import Market
             >>> Market().get_tradeable_products(tick_type="trade")
             ["PI_XBTUSD", "PF_XBTUSD", "PF_SOLUSD", ...]
         """
         return self._request(  # type: ignore[return-value]
-            method="GET", uri=f"/api/charts/v1/{tick_type}", auth=False
+            method="GET",
+            uri=f"/api/charts/v1/{tick_type}",
+            auth=False,
         )
 
     @lru_cache()
-    def get_resolutions(self: "Market", tick_type: str, tradeable: str) -> List[str]:
+    def get_resolutions(self: Market, tick_type: str, tradeable: str) -> List[str]:
         """
         Retrieve the list of available resolutions for a specific asset.
 
         - https://docs.futures.kraken.com/#http-api-charts-ohlc-get-resolutions
 
         This function uses caching. Run ``get_resolutions.cache_clear()`` to clear.
 
@@ -197,19 +201,21 @@
             :caption: Futures Market: Get the available resolutions
 
             >>> from kraken.futures import Market
             >>> Market().get_resolutions(tick_type="mark", tradeable="PI_XBTUSD")
             ['1h', '12h', '1w', '15m', '1d', '5m', '30m', '4h', '1m']
         """
         return self._request(  # type: ignore[return-value]
-            method="GET", uri=f"/api/charts/v1/{tick_type}/{tradeable}", auth=False
+            method="GET",
+            uri=f"/api/charts/v1/{tick_type}/{tradeable}",
+            auth=False,
         )
 
     @lru_cache()
-    def get_fee_schedules(self: "Market") -> dict:
+    def get_fee_schedules(self: Market) -> dict:
         """
         Retrieve information about the current fees
 
         - https://docs.futures.kraken.com/#http-api-trading-v3-api-fee-schedules-get-fee-schedules
 
         - https://support.kraken.com/hc/en-us/articles/360049269572-Fee-Schedules
 
@@ -238,18 +244,20 @@
                         {'makerFee': 0.0025, 'takerFee': 0.0125, 'usdVolume': 50000000.0},
                         {'makerFee': 0.0, 'takerFee': 0.01, 'usdVolume': 100000000.0}
                     ]}, ...
                 ]
             }
         """
         return self._request(  # type: ignore[return-value]
-            method="GET", uri="/derivatives/api/v3/feeschedules", auth=False
+            method="GET",
+            uri="/derivatives/api/v3/feeschedules",
+            auth=False,
         )
 
-    def get_fee_schedules_vol(self: "Market") -> dict:
+    def get_fee_schedules_vol(self: Market) -> dict:
         """
         Get the personal volumes per fee schedule
 
         Requires the ``General API - Full Access`` permission in the API key settings.
 
         - https://docs.futures.kraken.com/#http-api-trading-v3-api-fee-schedules-get-fee-schedule-volumes
 
@@ -266,18 +274,20 @@
                     '5b755fea-c5b0-4307-a66e-b392cd5bd931': 0,
                     'eef90775-995b-4596-9257-0917f6134766': 0
                 }
             }
 
         """
         return self._request(  # type: ignore[return-value]
-            method="GET", uri="/derivatives/api/v3/feeschedules/volumes", auth=True
+            method="GET",
+            uri="/derivatives/api/v3/feeschedules/volumes",
+            auth=True,
         )
 
-    def get_orderbook(self: "Market", symbol: Optional[str] = None) -> dict:
+    def get_orderbook(self: Market, symbol: Optional[str] = None) -> dict:
         """
         Get the orderbook of a specific asset/symbol. Even if the official kraken documentation
         states that the parameter ``symbol`` is not required, they will always respond with an error
         message, so it is recommended to use the ``symbol`` parameter until they don't fix this issue.
 
         - https://docs.futures.kraken.com/#http-api-trading-v3-api-market-data-get-orderbook
 
@@ -320,15 +330,15 @@
         return self._request(  # type: ignore[return-value]
             method="GET",
             uri="/derivatives/api/v3/orderbook",
             query_params=params,
             auth=False,
         )
 
-    def get_tickers(self: "Market") -> dict:
+    def get_tickers(self: Market) -> dict:
         """
         Retrieve information about the current tickers of all futures contracts.
 
         - https://docs.futures.kraken.com/#http-api-trading-v3-api-market-data-get-tickers
 
         - https://support.kraken.com/hc/en-us/articles/360022839531-Tickers
 
@@ -363,18 +373,20 @@
                     'fundingRate': 0.000220714078888884,
                     'fundingRatePrediction': 6.3914700437486e-05,
                     'postOnly': False
                 }, ...]
             }
         """
         return self._request(  # type: ignore[return-value]
-            method="GET", uri="/derivatives/api/v3/tickers", auth=False
+            method="GET",
+            uri="/derivatives/api/v3/tickers",
+            auth=False,
         )
 
-    def get_instruments(self: "Market") -> dict:
+    def get_instruments(self: Market) -> dict:
         """
         Retrieve more specific information about the tradeable assets on the Futures market
 
         - https://docs.futures.kraken.com/#http-api-trading-v3-api-instrument-details-get-instruments
 
         - https://support.kraken.com/hc/en-us/articles/360022635672-Instruments
 
@@ -445,20 +457,20 @@
                     }],
                     'category': '', 'tags': []
                 }
             }
 
         """
         return self._request(  # type: ignore[return-value]
-            method="GET", uri="/derivatives/api/v3/instruments", auth=False
+            method="GET",
+            uri="/derivatives/api/v3/instruments",
+            auth=False,
         )
 
-    def get_instruments_status(
-        self: "Market", instrument: Optional[str] = None
-    ) -> dict:
+    def get_instruments_status(self: Market, instrument: Optional[str] = None) -> dict:
         """
         Retrieve status information of a specific or all futures contracts.
 
         - https://docs.futures.kraken.com/#http-api-trading-v3-api-instrument-details-get-instrument-status-list
 
         - https://docs.futures.kraken.com/#http-api-trading-v3-api-instrument-details-get-instrument-status
 
@@ -485,19 +497,21 @@
             return self._request(  # type: ignore[return-value]
                 method="GET",
                 uri=f"/derivatives/api/v3/instruments/{instrument}/status",
                 auth=False,
             )
 
         return self._request(  # type: ignore[return-value]
-            method="GET", uri="/derivatives/api/v3/instruments/status", auth=False
+            method="GET",
+            uri="/derivatives/api/v3/instruments/status",
+            auth=False,
         )
 
     def get_trade_history(
-        self: "Market",
+        self: Market,
         symbol: Optional[str] = None,
         lastTime: Optional[str] = None,
         **kwargs: dict,
     ) -> dict:
         """
         Retrieve the trade history (max 100 entries), can be filtered using the parameters.
 
@@ -545,15 +559,15 @@
         return self._request(  # type: ignore[return-value]
             method="GET",
             uri="/derivatives/api/v3/history",
             query_params=params,
             auth=False,
         )
 
-    def get_historical_funding_rates(self: "Market", symbol: str) -> dict:
+    def get_historical_funding_rates(self: Market, symbol: str) -> dict:
         """
         Retrieve information about the historical funding rates for a specific asset.
 
         - https://support.kraken.com/hc/en-us/articles/360061979852-Historical-Funding-Rates
 
         :param symbol: The symbol/asset/futures contract
         :type symbol: str
@@ -586,15 +600,15 @@
         return self._request(  # type: ignore[return-value]
             method="GET",
             uri="/derivatives/api/v4/historicalfundingrates",
             query_params={"symbol": symbol},
             auth=False,
         )
 
-    def get_leverage_preference(self: "Market") -> dict:
+    def get_leverage_preference(self: Market) -> dict:
         """
         Get the current leverage preferences of the user.
 
         Requires at least the ``General API - Read Only`` permission in the API key settings.
 
         - https://docs.futures.kraken.com/#http-api-trading-v3-api-multi-collateral-get-the-leverage-setting-for-a-market
 
@@ -612,19 +626,21 @@
                 'leveragePreferences': [
                     {'symbol': 'PF_XBTUSD', 'maxLeverage': 5.0},
                     ...
                 ]
             }
         """
         return self._request(  # type: ignore[return-value]
-            method="GET", uri="/derivatives/api/v3/leveragepreferences", auth=True
+            method="GET",
+            uri="/derivatives/api/v3/leveragepreferences",
+            auth=True,
         )
 
     def set_leverage_preference(
-        self: "Market",
+        self: Market,
         symbol: str,
         maxLeverage: Optional[Union[str, int, float]] = None,
     ) -> dict:
         """
         Set a new leverage preference for a specific futures contract.
 
         Requires the ``General API - Full Access`` permission in the API key settings.
@@ -654,15 +670,15 @@
         return self._request(  # type: ignore[return-value]
             method="PUT",
             uri="/derivatives/api/v3/leveragepreferences",
             post_params=params,
             auth=True,
         )
 
-    def get_pnl_preference(self: "Market") -> dict:
+    def get_pnl_preference(self: Market) -> dict:
         """
         Get the current PNL (profit & loss) preferences. This can be used to define the currency
         in which the profits and losses are realized.
 
         Requires at least the ``General API - Read Only`` permission in the API key settings.
 
         - https://docs.futures.kraken.com/#http-api-trading-v3-api-multi-collateral-get-pnl-currency-preference-for-a-market
@@ -676,18 +692,20 @@
 
             >>> from kraken.futures import Market
             >>> market = Market(key="api-key", secret="secret-key")
             >>> market.get_pnl_preference()
             {'result': 'success', 'serverTime': '2023-04-04T15:21:29.413Z', 'preferences': []}
         """
         return self._request(  # type: ignore[return-value]
-            method="GET", uri="/derivatives/api/v3/pnlpreferences", auth=True
+            method="GET",
+            uri="/derivatives/api/v3/pnlpreferences",
+            auth=True,
         )
 
-    def set_pnl_preference(self: "Market", symbol: str, pnlPreference: str) -> dict:
+    def set_pnl_preference(self: Market, symbol: str, pnlPreference: str) -> dict:
         """
         Modify or set the current PNL preference of the user. This can be used to define a
         specific currency that should be used to realize profits and losses. The default is
         the quote currency of the futures contract.
 
         Requires the ``General API - Full Access`` permission in the API key settings.
 
@@ -713,15 +731,15 @@
             method="PUT",
             uri="/derivatives/api/v3/pnlpreferences",
             post_params={"symbol": symbol, "pnlPreference": pnlPreference},
             auth=True,
         )
 
     def _get_historical_events(
-        self: "Market",
+        self: Market,
         endpoint: str,
         before: Optional[int] = None,
         continuation_token: Optional[str] = None,
         since: Optional[int] = None,
         sort: Optional[str] = None,
         tradeable: Optional[str] = None,
         **kwargs: dict,
@@ -755,19 +773,22 @@
             params["since"] = since
         if defined(sort):
             params["sort"] = sort
         if defined(tradeable):
             params["tradeable"] = tradeable
         params.update(kwargs)
         return self._request(  # type: ignore[return-value]
-            method="GET", uri=endpoint, post_params=params, auth=False
+            method="GET",
+            uri=endpoint,
+            post_params=params,
+            auth=False,
         )
 
     def get_public_execution_events(
-        self: "Market",
+        self: Market,
         tradeable: str,
         before: Optional[int] = None,
         continuation_token: Optional[str] = None,
         since: Optional[int] = None,
         sort: Optional[str] = None,
     ) -> dict:
         """
@@ -849,15 +870,15 @@
             before=before,
             continuation_token=continuation_token,
             since=since,
             sort=sort,
         )
 
     def get_public_order_events(
-        self: "Market",
+        self: Market,
         tradeable: str,
         before: Optional[int] = None,
         continuation_token: Optional[str] = None,
         since: Optional[int] = None,
         sort: Optional[str] = None,
     ) -> dict:
         """
@@ -920,15 +941,15 @@
             before=before,
             continuation_token=continuation_token,
             since=since,
             sort=sort,
         )
 
     def get_public_mark_price_events(
-        self: "Market",
+        self: Market,
         tradeable: str,
         before: Optional[int] = None,
         continuation_token: Optional[str] = None,
         since: Optional[int] = None,
         sort: Optional[str] = None,
     ) -> dict:
         """
@@ -985,7 +1006,10 @@
         return self._get_historical_events(
             endpoint=f"/api/history/v2/market/{tradeable}/price",
             before=before,
             continuation_token=continuation_token,
             since=since,
             sort=sort,
         )
+
+
+__all__ = ["Market"]
```

### Comparing `python-kraken-sdk-1.5.0/kraken/futures/trade.py` & `python-kraken-sdk-1.6.0/kraken/futures/trade.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) 2023 Benjamin Thomas Schwertfeger
 # GitHub: https://github.com/btschwertfeger
 #
 
 """Module that implements the Kraken Futures trade client"""
 
+from __future__ import annotations
+
 from typing import List, Optional, Tuple, Union
 
-from ..base_api import KrakenBaseFuturesAPI, defined
+from kraken.base_api import KrakenBaseFuturesAPI, defined
 
 
 class Trade(KrakenBaseFuturesAPI):
     """
     Class that implements the Kraken Futures trade client
 
     If the sandbox environment is chosen, the keys must be generated from here:
@@ -41,27 +43,27 @@
 
         >>> from kraken.futures import Trade
         >>> with Trade(key="api-key", secret="secret-key") as trade:
         ...     print(trade.get_fills())
     """
 
     def __init__(
-        self: "Trade",
+        self: Trade,
         key: str = "",
         secret: str = "",
         url: str = "",
         sandbox: bool = False,
     ) -> None:
         super().__init__(key=key, secret=secret, url=url, sandbox=sandbox)
 
-    def __enter__(self: "Trade") -> "Trade":
+    def __enter__(self: Trade) -> Trade:
         super().__enter__()
         return self
 
-    def get_fills(self: "Trade", lastFillTime: Optional[str] = None) -> dict:
+    def get_fills(self: Trade, lastFillTime: Optional[str] = None) -> dict:
         """
         Return the current fills of the user.
 
         Requires at least the ``General API - Read Only`` permission in the API key settings.
 
         - https://docs.futures.kraken.com/#http-api-trading-v3-api-historical-data-get-your-fills
 
@@ -98,15 +100,15 @@
         return self._request(  # type: ignore[return-value]
             method="GET",
             uri="/derivatives/api/v3/fills",
             query_params=query_params,
             auth=True,
         )
 
-    def create_batch_order(self: "Trade", batchorder_list: List[dict]) -> dict:
+    def create_batch_order(self: Trade, batchorder_list: List[dict]) -> dict:
         """
         Create multiple orders at once using the batch order endpoint.
 
         Requires the ``General API - Full Access`` permission in the API key settings.
 
         - https://docs.futures.kraken.com/#http-api-trading-v3-api-order-management-batch-order-management
 
@@ -205,15 +207,15 @@
         return self._request(  # type: ignore[return-value]
             method="POST",
             uri="/derivatives/api/v3/batchorder",
             post_params={"json": f"{batchorder}"},
             auth=True,
         )
 
-    def cancel_all_orders(self: "Trade", symbol: Optional[str] = None) -> dict:
+    def cancel_all_orders(self: Trade, symbol: Optional[str] = None) -> dict:
         """
         Cancels all open orders, can be filtered by symbol.
 
         Requires the ``General API - Full Access`` permission in the API key settings.
 
         - https://docs.futures.kraken.com/#http-api-trading-v3-api-order-management-cancel-all-orders
 
@@ -253,15 +255,15 @@
         return self._request(  # type: ignore[return-value]
             method="POST",
             uri="/derivatives/api/v3/cancelallorders",
             post_params=params,
             auth=True,
         )
 
-    def dead_mans_switch(self: "Trade", timeout: Optional[int] = 0) -> dict:
+    def dead_mans_switch(self: Trade, timeout: Optional[int] = 0) -> dict:
         """
         The Death Man's Switch can be used to cancel all orders after a specific timeout.
         If the timeout is set to 60, all orders will be cancelled after 60 seconds. The timeout
         can be pushed back by accessing this endpoint over and over again. Set the timeout to zero
         to reset.
 
         Requires the ``General API - Full Access`` permission in the API key settings.
@@ -292,15 +294,17 @@
         return self._request(  # type: ignore[return-value]
             method="POST",
             uri="/derivatives/api/v3/cancelallordersafter",
             post_params={"timeout": timeout},
         )
 
     def cancel_order(
-        self: "Trade", order_id: Optional[str] = None, cliOrdId: Optional[str] = None
+        self: Trade,
+        order_id: Optional[str] = None,
+        cliOrdId: Optional[str] = None,
     ) -> dict:
         """
         This endpoint can be used to cancel a specific order by ``order_id`` or ``cliOrdId``.
 
         Requires the ``General API - Full Access`` permission in the API key settings.
 
         - https://docs.futures.kraken.com/#http-api-trading-v3-api-order-management-cancel-order
@@ -342,15 +346,15 @@
             method="POST",
             uri="/derivatives/api/v3/cancelorder",
             post_params=params,
             auth=True,
         )
 
     def edit_order(
-        self: "Trade",
+        self: Trade,
         orderId: Optional[str] = None,
         cliOrdId: Optional[str] = None,
         limitPrice: Optional[Union[str, int, float]] = None,
         size: Optional[Union[str, int, float]] = None,
         stopPrice: Optional[Union[str, int, float]] = None,
     ) -> dict:
         """
@@ -412,15 +416,15 @@
             method="POST",
             uri="/derivatives/api/v3/editorder",
             post_params=params,
             auth=True,
         )
 
     def get_orders_status(
-        self: "Trade",
+        self: Trade,
         orderIds: Optional[Union[str, List[str]]] = None,
         cliOrdIds: Optional[Union[str, List[str]]] = None,
     ) -> dict:
         """
         Get the status of multiple orders.
 
         Requires at least the ``General API - Read Only`` permission in the API key settings.
@@ -456,16 +460,16 @@
         return self._request(  # type: ignore[return-value]
             method="POST",
             uri="/derivatives/api/v3/orders/status",
             post_params=params,
             auth=True,
         )
 
-    def create_order(
-        self: "Trade",
+    def create_order(  # noqa: PLR0913
+        self: Trade,
         orderType: str,
         size: Union[str, int, float],
         symbol: str,
         side: str,
         cliOrdId: Optional[str] = None,
         limitPrice: Optional[Union[str, int, float]] = None,
         reduceOnly: Optional[bool] = None,
@@ -667,7 +671,10 @@
 
         return self._request(  # type: ignore[return-value]
             method="POST",
             uri="/derivatives/api/v3/sendorder",
             post_params=params,
             auth=True,
         )
+
+
+__all__ = ["Trade"]
```

### Comparing `python-kraken-sdk-1.5.0/kraken/futures/user.py` & `python-kraken-sdk-1.6.0/kraken/futures/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,22 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) 2023 Benjamin Thomas Schwertfeger
 # GitHub: https://github.com/btschwertfeger
 #
 
 """Module that implements the Kraken Futures user client"""
 
-from typing import Optional, Union
+from __future__ import annotations
 
-import requests
+from typing import TYPE_CHECKING, Optional, Union
 
-from ..base_api import KrakenBaseFuturesAPI, defined
+if TYPE_CHECKING:
+    import requests
+
+from kraken.base_api import KrakenBaseFuturesAPI, defined
 
 
 class User(KrakenBaseFuturesAPI):
     """
     Class that implements the Kraken Futures user client
 
     If the sandbox environment is chosen, the keys must be generated from here:
@@ -43,27 +46,27 @@
 
         >>> from kraken.futures import User
         >>> with User(key="api-key", secret="secret-key") as user:
         ...     print(user.get_wallets())
     """
 
     def __init__(
-        self: "User",
+        self: User,
         key: str = "",
         secret: str = "",
         url: str = "",
         sandbox: bool = False,
     ) -> None:
         super().__init__(key=key, secret=secret, url=url, sandbox=sandbox)
 
-    def __enter__(self: "User") -> "User":
+    def __enter__(self: User) -> User:
         super().__enter__()
         return self
 
-    def get_wallets(self: "User") -> dict:
+    def get_wallets(self: User) -> dict:
         """
         Lists the current wallet balances of the user.
 
         Requires at least the ``General API - Read Only`` permission in the API key settings.
 
         - https://docs.futures.kraken.com/#http-api-trading-v3-api-account-information-get-wallets
 
@@ -138,18 +141,20 @@
                         'type': 'multiCollateralMarginAccount'
                     }
                 },
                 'serverTime': '2023-04-04T17:56:49.027Z'
             }
         """
         return self._request(  # type: ignore[return-value]
-            method="GET", uri="/derivatives/api/v3/accounts", auth=True
+            method="GET",
+            uri="/derivatives/api/v3/accounts",
+            auth=True,
         )
 
-    def get_subaccounts(self: "User") -> dict:
+    def get_subaccounts(self: User) -> dict:
         """
         List the subaccounts of the user.
 
         Requires at least the ``General API - Read Only`` permission in the API key settings.
 
         - https://docs.futures.kraken.com/#http-api-trading-v3-api-account-information-get-subaccounts
 
@@ -167,18 +172,20 @@
                 'result': 'success',
                 'serverTime': '2023-04-04T18:03:33.696Z',
                 'masterAccountUid': 'f7d5571c-6d10-4cf1-944a-048d25682ed0',
                 'subaccounts': []
             }
         """
         return self._request(  # type: ignore[return-value]
-            method="GET", uri="/derivatives/api/v3/subaccounts", auth=True
+            method="GET",
+            uri="/derivatives/api/v3/subaccounts",
+            auth=True,
         )
 
-    def get_unwind_queue(self: "User") -> dict:
+    def get_unwind_queue(self: User) -> dict:
         """
         Retrieve information about the percentile of the open position in case of unwinding.
 
         Requires at least the ``General API - Read Only`` permission in the API key settings.
 
         - https://docs.futures.kraken.com/#http-api-trading-v3-api-account-information-get-position-percentile-of-unwind-queue
 
@@ -197,18 +204,20 @@
                 'serverTime': '2023-04-04T18:05:01.328Z',
                 'queue': [
                     { 'symbol': 'PF_UNIUSD', 'percentile': 20 }
                 ]
             }
         """
         return self._request(  # type: ignore[return-value]
-            method="GET", uri="/derivatives/api/v3/unwindqueue", auth=True
+            method="GET",
+            uri="/derivatives/api/v3/unwindqueue",
+            auth=True,
         )
 
-    def get_notifications(self: "User") -> dict:
+    def get_notifications(self: User) -> dict:
         """
         Retrieve the latest notifications from the Kraken Futures API
 
         Requires at least the ``General API - Read Only`` permission in the API key settings.
 
         - https://docs.futures.kraken.com/#http-api-trading-v3-api-general-get-notifications
 
@@ -229,19 +238,21 @@
                     'priority': 'high',
                     'note': 'Market in post only mode until 4pm.'
                 }],
                 'serverTime': '2023-04-04T18:01:39.729Z'
             }
         """
         return self._request(  # type: ignore[return-value]
-            method="GET", uri="/derivatives/api/v3/notifications", auth=True
+            method="GET",
+            uri="/derivatives/api/v3/notifications",
+            auth=True,
         )
 
     def get_account_log(
-        self: "User",
+        self: User,
         before: Optional[Union[str, int]] = None,
         count: Optional[Union[str, int]] = None,
         from_: Optional[Union[str, int]] = None,
         info: Optional[str] = None,
         since: Optional[Union[str, int]] = None,
         sort: Optional[str] = None,
         to: Optional[str] = None,
@@ -325,15 +336,15 @@
         return self._request(  # type: ignore[return-value]
             method="GET",
             uri="/api/history/v2/account-log",
             query_params=params,
             auth=True,
         )
 
-    def get_account_log_csv(self: "User") -> requests.Response:
+    def get_account_log_csv(self: User) -> requests.Response:
         """
         Return the account log as csv, for example to export it. This is not available in the
         Kraken demo/sandbox environment.
 
         Requires at least the ``General API - Read Only`` permission in the API key settings.
 
         - https://docs.futures.kraken.com/#http-api-history-account-log-get-recent-account-log-csv
@@ -355,15 +366,15 @@
             method="GET",
             uri="/api/history/v2/accountlogcsv",
             auth=True,
             return_raw=True,
         )
 
     def _get_historical_events(
-        self: "User",
+        self: User,
         endpoint: str,
         before: Optional[int] = None,
         continuation_token: Optional[str] = None,
         since: Optional[int] = None,
         sort: Optional[str] = None,
         tradeable: Optional[str] = None,
         **kwargs: dict,
@@ -397,19 +408,22 @@
             params["since"] = since
         if defined(sort):
             params["sort"] = sort
         if defined(tradeable):
             params["tradeable"] = tradeable
         params.update(kwargs)
         return self._request(  # type: ignore[return-value]
-            method="GET", uri=endpoint, query_params=params, auth=True
+            method="GET",
+            uri=endpoint,
+            query_params=params,
+            auth=True,
         )
 
     def get_execution_events(
-        self: "User",
+        self: User,
         before: Optional[int] = None,
         continuation_token: Optional[str] = None,
         since: Optional[int] = None,
         sort: Optional[str] = None,
         tradeable: Optional[str] = None,
     ) -> dict:
         """
@@ -523,15 +537,15 @@
             continuation_token=continuation_token,
             since=since,
             sort=sort,
             tradeable=tradeable,
         )
 
     def get_order_events(
-        self: "User",
+        self: User,
         before: Optional[int] = None,
         continuation_token: Optional[str] = None,
         since: Optional[int] = None,
         sort: Optional[str] = None,
         tradeable: Optional[str] = None,
     ) -> dict:
         """
@@ -599,15 +613,15 @@
             continuation_token=continuation_token,
             since=since,
             sort=sort,
             tradeable=tradeable,
         )
 
     def get_trigger_events(
-        self: "User",
+        self: User,
         before: Optional[int] = None,
         continuation_token: Optional[str] = None,
         since: Optional[int] = None,
         sort: Optional[str] = None,
         tradeable: Optional[str] = None,
     ) -> dict:
         """
@@ -683,15 +697,15 @@
             before=before,
             continuation_token=continuation_token,
             since=since,
             sort=sort,
             tradeable=tradeable,
         )
 
-    def get_open_positions(self: "User") -> dict:
+    def get_open_positions(self: User) -> dict:
         """
         List the open positions of the user.
 
         Requires at least the ``General API - Read Only`` permission in the API key settings.
 
         - https://docs.futures.kraken.com/#http-api-trading-v3-api-account-information-get-open-positions
 
@@ -717,18 +731,20 @@
                         'unrealizedFunding': 0.00005879463852989987
                     },
                 ],
                 'serverTime': '2023-04-06T16:12:15.410Z'
             }
         """
         return self._request(  # type: ignore[return-value]
-            method="GET", uri="/derivatives/api/v3/openpositions", auth=True
+            method="GET",
+            uri="/derivatives/api/v3/openpositions",
+            auth=True,
         )
 
-    def get_open_orders(self: "User") -> dict:
+    def get_open_orders(self: User) -> dict:
         """
         Retrieve the open orders.
 
         Requires at least the ``General API - Read Only`` permission in the API key settings.
 
         - https://docs.futures.kraken.com/#http-api-trading-v3-api-order-management-get-open-orders
 
@@ -799,18 +815,20 @@
                     'triggerSignal': 'last',
                     'lastUpdateTime': '2023-04-07T14:57:37.849Z'
                 }, ...],
                 'serverTime': '2023-04-07T15:30:29.911Z'
             }
         """
         return self._request(  # type: ignore[return-value]
-            method="GET", uri="/derivatives/api/v3/openorders", auth=True
+            method="GET",
+            uri="/derivatives/api/v3/openorders",
+            auth=True,
         )
 
-    def check_trading_enabled_on_subaccount(self: "User", subaccountUid: str) -> dict:
+    def check_trading_enabled_on_subaccount(self: User, subaccountUid: str) -> dict:
         """
         Checks if trading is enabled or disabled on the specified subaccount.
 
         Requires the ``General API - Full Access`` permission in the API key settings.
 
         This endpoint is only available for institutional clients and is not tested so far and
         results in ``KrakenAuthenticationError``.
@@ -836,15 +854,17 @@
         return self._request(  # type: ignore[return-value]
             method="GET",
             uri=f"/derivatives/api/v3/subaccount/{subaccountUid}/trading-enabled",
             auth=True,
         )
 
     def set_trading_on_subaccount(
-        self: "User", subaccountUid: str, trading_enabled: bool
+        self: User,
+        subaccountUid: str,
+        trading_enabled: bool,
     ) -> dict:
         """
         Enable or disable trading on a subaccount.
 
         Requires the ``General API - Full Access`` permission in the API key settings.
 
         This endpoint is only available for institutional clients and is not tested so far and
@@ -871,7 +891,10 @@
         """
         return self._request(  # type: ignore[return-value]
             method="PUT",
             uri=f"/derivatives/api/v3/subaccount/{subaccountUid}/trading-enabled",
             post_params={"tradingEnabled": trading_enabled},
             auth=True,
         )
+
+
+__all__ = ["User"]
```

### Comparing `python-kraken-sdk-1.5.0/kraken/futures/websocket/__init__.py` & `python-kraken-sdk-1.6.0/kraken/futures/websocket/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 import traceback
 from copy import deepcopy
 from random import random
 from typing import TYPE_CHECKING, Any, List, Optional
 
 import websockets
 
-from ...exceptions import KrakenException
+from kraken.exceptions import KrakenException
 
 if TYPE_CHECKING:
     # to avoid circular import for type checking
-    from ...futures import KrakenFuturesWSClient
+    from kraken.futures import KrakenFuturesWSClient
 
 
 class ConnectFuturesWebsocket:
     """
     This class is only called by the :class:`kraken.futures.KrakenFuturesWSClient`
     to establish the websocket connection.
 
@@ -37,15 +37,15 @@
     :param callback: The function that is used to receive the message objects
     :type callback: function
     """
 
     MAX_RECONNECT_NUM: int = 2
 
     def __init__(
-        self: "ConnectFuturesWebsocket",
+        self: ConnectFuturesWebsocket,
         client: KrakenFuturesWSClient,
         endpoint: str,
         callback: Any,
     ):
         self.__client: KrakenFuturesWSClient = client
         self.__ws_endpoint: str = endpoint
         self.__callback: Any = callback
@@ -55,141 +55,157 @@
         self.__last_challenge: Optional[str] = None
         self.__new_challenge: Optional[str] = None
         self.__challenge_ready: bool = False
 
         self.__socket: Any = None
         self.__subscriptions: List[dict] = []
 
-        asyncio.ensure_future(self.__run_forever(), loop=asyncio.get_running_loop())
+        self.task = asyncio.ensure_future(
+            self.__run_forever(),
+            loop=asyncio.get_running_loop(),
+        )
 
     @property
-    def subscriptions(self: "ConnectFuturesWebsocket") -> List[dict]:
+    def subscriptions(self: ConnectFuturesWebsocket) -> List[dict]:
         """Returns the active subscriptions"""
         return self.__subscriptions
 
-    async def __run(self: "ConnectFuturesWebsocket", event: asyncio.Event) -> None:
+    async def __run(self: ConnectFuturesWebsocket, event: asyncio.Event) -> None:
         keep_alive: bool = True
         self.__new_challenge = None
         self.__last_challenge = None
 
         async with websockets.connect(  # pylint: disable=no-member
-            f"wss://{self.__ws_endpoint}", ping_interval=30
+            f"wss://{self.__ws_endpoint}",
+            ping_interval=30,
         ) as socket:
             logging.info("Websocket connected!")
             self.__socket = socket
 
             if not event.is_set():
                 event.set()
             self.__reconnect_num = 0
 
             while keep_alive:
                 try:
                     _msg = await asyncio.wait_for(self.__socket.recv(), timeout=15)
                 except asyncio.TimeoutError:
-                    pass  # important
+                    logging.debug(
+                        "Timeout error in {endpoint}",
+                        extra={"endpoint": self.__ws_endpoint},
+                    )  # important
                 except asyncio.CancelledError:
                     logging.exception("asyncio.CancelledError")
                     keep_alive = False
                     await self.__callback({"error": "asyncio.CancelledError"})
                 else:
                     try:
-                        msg: dict = json.loads(_msg)
+                        message: dict = json.loads(_msg)
                     except ValueError:
                         logging.warning(_msg)
                     else:
                         forward: bool = True
-                        if "event" in msg:
-                            _event: str = msg["event"]
-                            if _event == "challenge" and "message" in msg:
+                        if "event" in message:
+                            _event: str = message["event"]
+                            if _event == "challenge" and "message" in message:
                                 forward = False
-                                self.__handle_new_challenge(msg)
+                                self.__handle_new_challenge(message)
                             elif _event == "subscribed":
-                                self.__append_subscription(msg)
+                                self.__append_subscription(message)
                             elif _event == "unsubscribed":
-                                self.__remove_subscription(msg)
+                                self.__remove_subscription(message)
                         if forward:
-                            await self.__callback(msg)
+                            await self.__callback(message)
 
-    async def __run_forever(self: "ConnectFuturesWebsocket") -> None:
+    async def __run_forever(self: ConnectFuturesWebsocket) -> None:
         try:
             while True:
                 await self.__reconnect()
         except KrakenException.MaxReconnectError:
             await self.__callback(
-                {"error": "kraken.exceptions.KrakenException.MaxReconnectError"}
+                {"error": "kraken.exceptions.KrakenException.MaxReconnectError"},
             )
         except Exception:
-            # for task in asyncio.all_tasks(): task.cancel()
-            logging.error(traceback.format_exc())
-        # except asyncio.CancelledError: pass
+            logging.exception(traceback.format_exc())
         finally:
             self.__client.exception_occur = True
 
-    async def __reconnect(self: "ConnectFuturesWebsocket") -> None:
+    async def __reconnect(self: ConnectFuturesWebsocket) -> None:
         logging.info("Websocket start connect/reconnect")
 
         self.__reconnect_num += 1
         if self.__reconnect_num >= self.MAX_RECONNECT_NUM:
-            raise KrakenException.MaxReconnectError()
+            raise KrakenException.MaxReconnectError
 
         reconnect_wait: float = self.__get_reconnect_wait(self.__reconnect_num)
         logging.debug(
-            f"asyncio sleep reconnect_wait={reconnect_wait} s reconnect_num={self.__reconnect_num}"
+            "asyncio sleep reconnect_wait={wait} s reconnect_num={num}",
+            extra={"wait": reconnect_wait, "num": self.__reconnect_num},
         )
         await asyncio.sleep(reconnect_wait)
         logging.debug("asyncio sleep done")
         event: asyncio.Event = asyncio.Event()
 
         tasks: dict = {
             asyncio.ensure_future(
-                self.__recover_subscription_req_msg(event)
+                self.__recover_subscription_req_msg(event),
             ): self.__recover_subscription_req_msg,
             asyncio.ensure_future(self.__run(event)): self.__run,
         }
 
         while set(tasks.keys()):
             finished, pending = await asyncio.wait(
-                tasks.keys(), return_when=asyncio.FIRST_EXCEPTION
+                tasks.keys(),
+                return_when=asyncio.FIRST_EXCEPTION,
             )
             exception_occur: bool = False
             for task in finished:
                 if task.exception():
                     exception_occur = True
                     traceback.print_stack()
                     message = f"{task} got an exception {task.exception()}\n {task.get_stack()}"
                     logging.warning(message)
                     for process in pending:
-                        logging.warning(f"pending {process}")
+                        logging.warning("pending {proc}", extra={"proc": process})
                         try:
                             process.cancel()
                         except asyncio.CancelledError:
                             logging.exception("CancelledError")
                         logging.warning("cancel ok")
                     await self.__callback({"error": message})
             if exception_occur:
                 break
         logging.warning("reconnect over")
 
     async def __recover_subscription_req_msg(
-        self: "ConnectFuturesWebsocket", event: asyncio.Event
+        self: ConnectFuturesWebsocket,
+        event: asyncio.Event,
     ) -> None:
-        logging.info(f"Recover subscriptions {self.__subscriptions} waiting.")
+        logging.info(
+            "Recover subscriptions {subscriptions} waiting.",
+            extra={"subscriptions": self.__subscriptions},
+        )
         await event.wait()
 
         for sub in self.__subscriptions:
             if sub["feed"] in self.__client.get_available_private_subscription_feeds():
                 await self.send_message(deepcopy(sub), private=True)
             elif sub["feed"] in self.__client.get_available_public_subscription_feeds():
                 await self.send_message(deepcopy(sub), private=False)
-            logging.info(f"{sub}: OK")
+            logging.info("{sub}: OK", extra={"sub": sub})
 
-        logging.info(f"Recover subscriptions {self.__subscriptions} done.")
+        logging.info(
+            "Recover subscriptions {subscriptions} done.",
+            extra={"subscriptions": self.__subscriptions},
+        )
 
     async def send_message(
-        self: "ConnectFuturesWebsocket", msg: dict, private: bool = False
+        self: ConnectFuturesWebsocket,
+        msg: dict,
+        private: bool = False,
     ) -> None:
         """
         Enables sending a message via the websocket connection
 
         :param msg: The message as dictionary
         :type msg: dict
         :param private: If the message requires authentication (default: ``False``)
@@ -197,64 +213,67 @@
         :rtype: Coroutine
         """
         while not self.__socket:
             await asyncio.sleep(0.4)
 
         if private:
             if not self.__client.is_auth:
-                raise ValueError(
-                    "Cannot access private endpoints with unauthenticated client!"
+                raise AttributeError(
+                    "Cannot access private endpoints with unauthenticated client!",
                 )
             if not self.__challenge_ready:
                 await self.__check_challenge_ready()
 
-            msg["api_key"] = self.__client._key
+            msg["api_key"] = self.__client.key
             msg["original_challenge"] = self.__last_challenge
             msg["signed_challenge"] = self.__new_challenge
 
         await self.__socket.send(json.dumps(msg))
 
-    def __handle_new_challenge(self: "ConnectFuturesWebsocket", msg: dict) -> None:
+    def __handle_new_challenge(self: ConnectFuturesWebsocket, msg: dict) -> None:
         self.__last_challenge = msg["message"]
-        self.__new_challenge = self.__client._get_sign_challenge(self.__last_challenge)
+        self.__new_challenge = self.__client.get_sign_challenge(self.__last_challenge)
         self.__challenge_ready = True
 
-    async def __check_challenge_ready(self: "ConnectFuturesWebsocket") -> None:
+    async def __check_challenge_ready(self: ConnectFuturesWebsocket) -> None:
         await self.__socket.send(
-            json.dumps({"event": "challenge", "api_key": self.__client._key})
+            json.dumps({"event": "challenge", "api_key": self.__client.key}),
         )
 
         logging.debug("Awaiting challenge...")
         while not self.__challenge_ready:
             await asyncio.sleep(0.2)
 
     def __get_reconnect_wait(self, attempts: int) -> float:
-        return round(random() * min(60 * 3, (2**attempts) - 1) + 1)  # type: ignore[no-any-return]
+        return round(  # type: ignore[no-any-return]
+            random() * min(60 * 3, (2**attempts) - 1) + 1,  # noqa: S311
+        )
 
-    def __append_subscription(self: "ConnectFuturesWebsocket", msg: dict) -> None:
+    def __append_subscription(self: ConnectFuturesWebsocket, msg: dict) -> None:
         self.__remove_subscription(msg=msg)  # remove from list, to avoid duplicates
         sub: dict = self.__build_subscription(msg)
         self.__subscriptions.append(sub)
 
-    def __remove_subscription(self: "ConnectFuturesWebsocket", msg: dict) -> None:
+    def __remove_subscription(self: ConnectFuturesWebsocket, msg: dict) -> None:
         sub: dict = self.__build_subscription(msg)
         self.__subscriptions = [x for x in self.__subscriptions if x != sub]
 
     def __build_subscription(
-        self: "ConnectFuturesWebsocket", subscription: dict
+        self: ConnectFuturesWebsocket,
+        subscription: dict,
     ) -> dict:
         sub: dict = {"event": "subscribe"}
 
         if (
             "event" not in subscription
             or subscription["event"] not in ["subscribed", "unsubscribed"]
             or "feed" not in subscription
         ):
-            raise ValueError(
-                "Cannot append/remove subscription with missing attributes."
+            raise AttributeError(
+                "Cannot append/remove subscription with missing attributes.",
             )
 
         if (
             subscription["feed"]
             in self.__client.get_available_public_subscription_feeds()
         ):
             # public subscribe
@@ -269,14 +288,17 @@
             subscription["feed"]
             in self.__client.get_available_private_subscription_feeds()
         ):
             # private subscription
             sub["feed"] = subscription["feed"]
         else:
             logging.warning(
-                "Feed not implemented. Please contact the python-kraken-sdk package author."
+                "Feed not implemented. Please contact the python-kraken-sdk package author.",
             )
         return sub
 
-    def _get_active_subscriptions(self: "ConnectFuturesWebsocket") -> List[dict]:
+    def get_active_subscriptions(self: ConnectFuturesWebsocket) -> List[dict]:
         """Returns the active subscriptions"""
         return self.__subscriptions
+
+
+__all__ = ["ConnectFuturesWebsocket"]
```

### Comparing `python-kraken-sdk-1.5.0/kraken/futures/ws_client.py` & `python-kraken-sdk-1.6.0/kraken/futures/ws_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,34 +2,36 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) 2023 Benjamin Thomas Schwertfeger
 # GitHub: https://github.com/btschwertfeger
 #
 
 """Provides the websocket client for Kraken Futures"""
 
+from __future__ import annotations
+
 import base64
 import hashlib
 import hmac
 import logging
 from copy import deepcopy
 from typing import Any, Dict, List, Optional
 
-from ..base_api import KrakenBaseFuturesAPI
-from ..exceptions import KrakenException
-from .websocket import ConnectFuturesWebsocket
+from kraken.base_api import KrakenBaseFuturesAPI
+from kraken.exceptions import KrakenException
+from kraken.futures.websocket import ConnectFuturesWebsocket
 
 
 class KrakenFuturesWSClient(KrakenBaseFuturesAPI):
     """
     Class to access public and (optional)
     private/authenticated websocket connection.
 
-    So far there are no trade endpoints that can be accessed using the
-    Futures Kraken API. If this has changed and not implemented yet,
-    please open an issue: https://github.com/btschwertfeger/python-kraken-sdk/issues
+    So far there are no trade endpoints that can be accessed using the Futures
+    Kraken API. If this has changed and is not implemented yet, please open an
+    issue at https://github.com/btschwertfeger/python-kraken-sdk/issues
 
     - https://docs.futures.kraken.com/#websocket-api
 
     :param key: The Kraken Futures API key to access private endpoints
     :type key: str, optional
     :param secret: The Kraken Futures Secret key to access private endpoints
     :type secret: str, optional
@@ -44,45 +46,40 @@
         :caption: Futures Websocket: Create the websocket client
 
         import asyncio
         from kraken.futures import KrakenFuturesWSClient
 
         async def main() -> None:
 
-            # Create a custom bot
-            class Bot(KrakenFuturesWSClient):
+            # Create the custom client
+            class Client(KrakenFuturesWSClient):
                 async def on_message(self, event: dict) -> None:
                     print(event)
 
-            bot = Bot()     # unauthenticated
-            auth_bot = Bot( # authenticated
+            client = Client()     # unauthenticated
+            auth_client = Client( # authenticated
                 key="api-key",
                 secret="secret-key"
             )
 
             # now you can subscribe to channels using
-            await bot.subscribe(
+            await client.subscribe(
                 feed='ticker',
                 products=["XBTUSD", "DOT/EUR"]
             )
             # the messages can be used within the `on_message` callback method
 
             while True:
                 await asyncio.sleep(6)
 
         if __name__ == "__main__":
-            loop = asyncio.new_event_loop()
-            asyncio.set_event_loop(loop)
             try:
                 asyncio.run(main())
             except KeyboardInterrupt:
-                loop.close()
-
-
-                from kraken.futures import KrakenFuturesWSClient
+                pass
 
     .. code-block:: python
         :linenos:
         :caption: Futures Websocket: Create the websocket client as context manager
 
         import asyncio
         from kraken.futures import KrakenFuturesWSClient
@@ -108,93 +105,105 @@
                 loop.close()
     """
 
     PROD_ENV_URL: str = "futures.kraken.com/ws/v1"
     DEMO_ENV_URL: str = "demo-futures.kraken.com/ws/v1"
 
     def __init__(
-        self: "KrakenFuturesWSClient",
+        self: KrakenFuturesWSClient,
         key: str = "",
         secret: str = "",
         url: str = "",
         callback: Optional[Any] = None,
         sandbox: bool = False,
     ):
         super().__init__(key=key, secret=secret, url=url, sandbox=sandbox)
 
-        self._key: str = key
-        self._secret: str = secret
+        self.__key: str = key
+        self.__secret: str = secret
 
         self.exception_occur: bool = False
         self.__callback: Any = callback
         self._conn: ConnectFuturesWebsocket = ConnectFuturesWebsocket(
             client=self,
             endpoint=url
             if url != ""
             else self.DEMO_ENV_URL
             if sandbox
             else self.PROD_ENV_URL,
             callback=self.on_message,
         )
 
-    def _get_sign_challenge(self: "KrakenFuturesWSClient", challenge: str) -> str:
+    @property
+    def key(self: KrakenBaseFuturesAPI) -> str:
+        """Returns the API key"""
+        return self.__key
+
+    def get_sign_challenge(self: KrakenFuturesWSClient, challenge: str) -> str:
         """
         Sign the challenge/message using the secret key
 
         :param challenge: The challenge/message to sign
         :type challenge: str
         :return: The signed message
         :raises kraken.exceptions.KrakenAuthenticationError: If the credentials are not valid
         :rtype: str
         """
         if not self.is_auth:
-            raise KrakenException.KrakenAuthenticationError()
+            raise KrakenException.KrakenAuthenticationError
 
         sha256_hash = hashlib.sha256()
         sha256_hash.update(challenge.encode("utf-8"))
         return base64.b64encode(
             hmac.new(
-                base64.b64decode(self._secret), sha256_hash.digest(), hashlib.sha512
-            ).digest()
+                base64.b64decode(self.__secret),
+                sha256_hash.digest(),
+                hashlib.sha512,
+            ).digest(),
         ).decode("utf-8")
 
-    async def on_message(self: "KrakenFuturesWSClient", msg: dict) -> None:
+    async def on_message(self: KrakenFuturesWSClient, msg: dict) -> None:
         """
         Method that serves as the default callback function Calls the defined callback function (if defined)
         or overload this function.
 
         This is the default method  which just logs the messages. In production you want to overload this
         with your custom methods, as shown in the Example of :class:`kraken.futures.KrakenFuturesWSClient`.
 
         :param msg: The message that was send by Kraken via the websocket connection.
         :type msg: dict
         :rtype: NOne
         """
+        # todo: rename the msg parameter to message
         if self.__callback is not None:
             await self.__callback(msg)
         else:
             logging.warning("Received event but no callback is defined")
             logging.info(msg)
 
     async def subscribe(
-        self: "KrakenFuturesWSClient", feed: str, products: Optional[List[str]] = None
+        self: KrakenFuturesWSClient,
+        feed: str,
+        products: Optional[List[str]] = None,
     ) -> None:
         """
         Subscribe to a Futures websocket channel/feed. For some feeds authentication is required.
 
         - https://docs.futures.kraken.com/#websocket-api-websocket-api-introduction-subscriptions
 
         :param feed: The websocket feed/channel to subscribe to
         :type feed: str
         :param products: The products/futures contracts to subscribe to
-        :type products: List[str], optional
-        :raises ValueError: If the parameters don't match the requirements set by the Kraken API
-
-        Initialize your client as described in :class:`kraken.futures.KrakenFuturesWSClient` to
-        run the following example:
+        :type products: list[str], optional
+        :raises TypeError: If the parameters don't match the requirements set
+            by the Kraken API
+
+        Initialize your client as described in
+        :class:`kraken.futures.KrakenFuturesWSClient` to run the following
+        example:
 
         .. code-block:: python
             :linenos:
             :caption: Futures Websocket: Subscribe to a feed
 
             >>> await bot.subscribe(feed='ticker', products=["XBTUSD", "DOT/EUR"])
 
@@ -203,16 +212,17 @@
         or a custom callback function.
         """
 
         message: dict = {"event": "subscribe", "feed": feed}
 
         if products is not None:
             if not isinstance(products, list):
-                raise ValueError(
-                    'Parameter products must be type of List[str] (e.g. products=["PI_XBTUSD"])'
+                raise TypeError(
+                    "Parameter products must be type of list[str] "
+                    '(e.g. products=["PI_XBTUSD"])',
                 )
             message["product_ids"] = products
 
         if feed in self.get_available_private_subscription_feeds():
             if products is not None:
                 raise ValueError("There is no private feed that accepts products!")
             await self._conn.send_message(message, private=True)
@@ -224,48 +234,54 @@
                     await self._conn.send_message(sub, private=False)
             else:
                 await self._conn.send_message(message, private=False)
         else:
             raise ValueError(f"Feed: {feed} not found. Not subscribing to it.")
 
     async def unsubscribe(
-        self: "KrakenFuturesWSClient", feed: str, products: Optional[List[str]] = None
+        self: KrakenFuturesWSClient,
+        feed: str,
+        products: Optional[List[str]] = None,
     ) -> None:
         """
-        Subscribe to a Futures websocket channel/feed. For some feeds authentication is required.
+        Subscribe to a Futures websocket channel/feed. For some feeds
+        authentication is required.
 
         - https://docs.futures.kraken.com/#websocket-api-websocket-api-introduction-subscriptions
 
         :param feed: The websocket feed/channel to unsubscribe from
         :type feed: str
         :param products: The products/futures contracts to unsubscribe from
         :type products: List[str], optional
-        :raises ValueError: If the parameters don't match the requirements set by the Kraken API
+        :raises TypeError: If the parameters don't match the requirements set
+            by the Kraken API
 
-        Initialize your client as described in :class:`kraken.futures.KrakenFuturesWSClient` to
-        run the following example:
+        Initialize your client as described in
+        :class:`kraken.futures.KrakenFuturesWSClient` to run the following
+        example:
 
         .. code-block:: python
             :linenos:
             :caption: Futures Websocket: Unsubscribe from a feed
 
             >>> await bot.unsubscribe(feed='ticker', products=["XBTUSD", "DOT/EUR"])
 
         Success or failures are sent over the websocket connection and can be
-        received via the default :func:`kraken.futures.KrakenFuturesWSClient.on_message``
-        or a custom callback function.
+        received via the default
+        :func:`kraken.futures.KrakenFuturesWSClient.on_message`` or a custom
+        callback function.
         """
 
         message: dict = {"event": "unsubscribe", "feed": feed}
 
         if products is not None:
             if not isinstance(products, list):
-                raise ValueError(
-                    'Parameter products must be type of List[str]\
-                    (e.g. products=["PI_XBTUSD"])'
+                raise TypeError(
+                    'Parameter products must be type of list[str]\
+                    (e.g. products=["PI_XBTUSD"])',
                 )
             message["product_ids"] = products
 
         if feed in self.get_available_private_subscription_feeds():
             if products is not None:
                 raise ValueError("There is no private feed that accepts products!")
             await self._conn.send_message(message, private=True)
@@ -279,15 +295,16 @@
                 await self._conn.send_message(message, private=False)
         else:
             raise ValueError(f"Feed: {feed} not found. Not unsubscribing it.")
 
     @staticmethod
     def get_available_public_subscription_feeds() -> List[str]:
         """
-        Return all available public feeds that can be un-/subscribed using the Kraken Futures API.
+        Return all available public feeds that can be un-/subscribed using the
+        Kraken Futures API.
 
         :return: List of available public feeds
         :rtype: List[str]
 
         .. code-block:: python
             :linenos:
             :caption: Futures Websocket: Get the available public subscription feeds
@@ -300,16 +317,16 @@
             ]
         """
         return ["trade", "book", "ticker", "ticker_lite", "heartbeat"]
 
     @staticmethod
     def get_available_private_subscription_feeds() -> List[str]:
         """
-        Return all available private feeds that can be un-/subscribed to/from using the
-        Kraken Futures API
+        Return all available private feeds that can be un-/subscribed to/from
+        using the Kraken Futures API
 
         :return: List of available private feeds
         :rtype: List[str]
 
         .. code-block:: python
             :linenos:
             :caption: Futures Websocket: Get the available private subscription feeds
@@ -332,15 +349,15 @@
             "deposits_withdrawals",
             "account_balances_and_margins",
             "account_log",
             "notifications_auth",
         ]
 
     @property
-    def is_auth(self: "KrakenFuturesWSClient") -> bool:
+    def is_auth(self: KrakenFuturesWSClient) -> bool:
         """
         Checks if key and secret are set.
 
         :return: ``True`` if the credentials are set, else ``False``
         :rtype: bool
 
         .. code-block:: python
@@ -348,25 +365,26 @@
             :caption: Futures Websocket: Check if the credentials are set
 
             >>> from kraken.futures import KrakenFuturesWSClient
             >>> KrakenFuturesWSClient().is_auth()
             False
         """
         return (
-            self._key is not None
-            and self._key != ""
-            and self._secret is not None
-            and self._secret != ""
+            self.__key is not None
+            and self.__key != ""
+            and self.__secret is not None
+            and self.__secret != ""
         )
 
-    def get_active_subscriptions(self: "KrakenFuturesWSClient") -> List[dict]:
+    def get_active_subscriptions(self: KrakenFuturesWSClient) -> List[dict]:
         """
         Returns the list of active subscriptions.
 
-        :return: List of active subscriptions including the feed names, products and additional information.
+        :return: List of active subscriptions including the feed names, products
+            and additional information.
         :rtype: List[dict]
 
         Initialize your client as described in :class:`kraken.futures.KrakenFuturesWSClient` to
         run the following example:
 
         .. code-block:: python
             :linenos:
@@ -382,16 +400,21 @@
                     "product_ids": ["PI_XBTUSD"]
                 }, {
                     "event": "subscribe",
                     "feed": "open_orders,
                 }, ...
             ]
         """
-        return self._conn._get_active_subscriptions()
+        return self._conn.get_active_subscriptions()
 
-    async def __aenter__(self: "KrakenFuturesWSClient") -> "KrakenFuturesWSClient":
+    async def __aenter__(self: KrakenFuturesWSClient) -> KrakenFuturesWSClient:
         return self
 
     async def __aexit__(
-        self: "KrakenFuturesWSClient", *exc: tuple, **kwargs: Dict[str, Any]
+        self: KrakenFuturesWSClient,
+        *exc: tuple,
+        **kwargs: Dict[str, Any],
     ) -> None:
         pass
+
+
+__all__ = ["KrakenFuturesWSClient"]
```

### Comparing `python-kraken-sdk-1.5.0/kraken/spot/funding.py` & `python-kraken-sdk-1.6.0/kraken/spot/funding.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) 2023 Benjamin Thomas Schwertfeger
 # GitHub: https://github.com/btschwertfeger
 #
 
 """Module that implements the Spot Funding client"""
 
+from __future__ import annotations
+
 from typing import List, Optional, Union
 
-from ..base_api import KrakenBaseSpotAPI, defined
+from kraken.base_api import KrakenBaseSpotAPI, defined
 
 
 class Funding(KrakenBaseSpotAPI):
     """
     Class that implements the Spot Funding client. Currently there
     are no funding endpoints that could be accesses without authentication.
 
@@ -39,26 +41,26 @@
 
         >>> from kraken.spot import Funding
         >>> with Funding(key="api-key", secret="secret-key") as funding:
         ...     print(funding.get_deposit_methods(asset="XLM"))
     """
 
     def __init__(
-        self: "Funding",
+        self: Funding,
         key: str = "",
         secret: str = "",
         url: str = "",
     ) -> None:
         super().__init__(key=key, secret=secret, url=url)
 
-    def __enter__(self: "Funding") -> "Funding":
+    def __enter__(self: Funding) -> Funding:
         super().__enter__()
         return self
 
-    def get_deposit_methods(self: "Funding", asset: str) -> List[dict]:
+    def get_deposit_methods(self: Funding, asset: str) -> List[dict]:
         """
         Get the available deposit methods for a specific asset.
 
         - https://docs.kraken.com/rest/#operation/getDepositMethods
 
         :param asset: Asset being deposited
         :type asset: str
@@ -81,19 +83,24 @@
                     'method': 'Stellar XLM Multi',
                     'limit': False,
                     'gen-address': True
                 }
             ]
         """
         return self._request(
-            method="POST", uri="/private/DepositMethods", params={"asset": asset}  # type: ignore
+            method="POST",
+            uri="/private/DepositMethods",
+            params={"asset": asset},  # type: ignore[return-value]
         )
 
     def get_deposit_address(
-        self: "Funding", asset: str, method: str, new: Optional[bool] = False
+        self: Funding,
+        asset: str,
+        method: str,
+        new: Optional[bool] = False,
     ) -> List[dict]:
         """
         Get the deposit addresses for a specific asset. New deposit addresses can be generated.
 
         Requires the ``Deposit funds`` API key permission.
 
         - https://docs.kraken.com/rest/#operation/getDepositAddresses
@@ -131,15 +138,17 @@
         return self._request(  # type: ignore[return-value]
             method="POST",
             uri="/private/DepositAddresses",
             params={"asset": asset, "method": method, "new": new},
         )
 
     def get_recent_deposits_status(
-        self: "Funding", asset: Optional[str] = None, method: Optional[str] = None
+        self: Funding,
+        asset: Optional[str] = None,
+        method: Optional[str] = None,
     ) -> List[dict]:
         """
         Get information about the recent deposit status. The look back period is 90 days and
         only the last 25 deposits will be returned.
 
         Requires the ``Query funds`` and ``Deposit funds`` API key permissions.
 
@@ -198,19 +207,24 @@
         """
         params: dict = {}
         if defined(asset):
             params["asset"] = asset
         if defined(method):
             params["method"] = method
         return self._request(  # type: ignore[return-value]
-            method="POST", uri="/private/DepositStatus", params=params
+            method="POST",
+            uri="/private/DepositStatus",
+            params=params,
         )
 
     def get_withdrawal_info(
-        self: "Funding", asset: str, key: str, amount: Union[str, int, float]
+        self: Funding,
+        asset: str,
+        key: str,
+        amount: Union[str, int, float],
     ) -> dict:
         """
         Get information about a possible withdraw, including fee and limit information.
         The ``key`` must be the name of the key defined in the account. You can add
         a new key for any asset listed on Kraken here: https://www.kraken.com/u/funding/withdraw.
 
         Requires the ``Query funds`` and ``Withdraw funds`` API key permissions.
@@ -248,15 +262,18 @@
         return self._request(  # type: ignore[return-value]
             method="POST",
             uri="/private/WithdrawInfo",
             params={"asset": asset, "key": str(key), "amount": str(amount)},
         )
 
     def withdraw_funds(
-        self: "Funding", asset: str, key: str, amount: Union[str, int, float]
+        self: Funding,
+        asset: str,
+        key: str,
+        amount: Union[str, int, float],
     ) -> dict:
         """
         Create a new withdraw. The key must be the name of the withdraw key
         defined in the withdraw section of the Kraken WebUI.
 
         Requires the ``Withdraw funds`` API key permissions.
 
@@ -287,15 +304,17 @@
         return self._request(  # type: ignore[return-value]
             method="POST",
             uri="/private/Withdraw",
             params={"asset": asset, "key": str(key), "amount": str(amount)},
         )
 
     def get_recent_withdraw_status(
-        self: "Funding", asset: Optional[str] = None, method: Optional[str] = None
+        self: Funding,
+        asset: Optional[str] = None,
+        method: Optional[str] = None,
     ) -> List[dict]:
         """
         Get information about the recent withdraw status, including withdraws of the
         past 90 days but at max 500 results.
 
         - https://docs.kraken.com/rest/#operation/getStatusRecentWithdrawals
 
@@ -330,18 +349,20 @@
         """
         params: dict = {}
         if defined(asset):
             params["asset"] = asset
         if defined(method):
             params["method"] = method
         return self._request(  # type: ignore[return-value]
-            method="POST", uri="/private/WithdrawStatus", params=params
+            method="POST",
+            uri="/private/WithdrawStatus",
+            params=params,
         )
 
-    def cancel_withdraw(self: "Funding", asset: str, refid: str) -> dict:
+    def cancel_withdraw(self: Funding, asset: str, refid: str) -> dict:
         """
         Cancel a requested withdraw. This will only be successful if the withdraw
         is not being processed so far.
 
         Requires the ``Withdraw funds`` API key permissions.
 
         - https://docs.kraken.com/rest/#operation/cancelWithdrawal
@@ -365,15 +386,15 @@
         return self._request(  # type: ignore[return-value]
             method="POST",
             uri="/private/WithdrawCancel",
             params={"asset": asset, "refid": str(refid)},
         )
 
     def wallet_transfer(
-        self: "Funding",
+        self: Funding,
         asset: str,
         from_: str,
         to_: str,
         amount: Union[str, int, float],
     ) -> dict:
         """
         Transfer assets between the Spot and Futures wallet.
@@ -408,7 +429,10 @@
             { 'refid': "ANS1EE5-SKACR4-PENGVP" }
         """
         return self._request(  # type: ignore[return-value]
             method="POST",
             uri="/private/WalletTransfer",
             params={"asset": asset, "from": from_, "to": to_, "amount": str(amount)},
         )
+
+
+__all__ = ["Funding"]
```

### Comparing `python-kraken-sdk-1.5.0/kraken/spot/market.py` & `python-kraken-sdk-1.6.0/kraken/spot/market.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) 2023 Benjamin Thomas Schwertfeger
 # GitHub: https://github.com/btschwertfeger
 #
 
 """Module that implements the Kraken Spot Market client"""
 
+from __future__ import annotations
+
 from functools import lru_cache
 from typing import List, Optional, Union
 
-from ..base_api import KrakenBaseSpotAPI, defined, ensure_string
+from kraken.base_api import KrakenBaseSpotAPI, defined, ensure_string
 
 
 class Market(KrakenBaseSpotAPI):
     """
     Class that implements the Kraken Spot Market client. Can be used to access
     the Kraken Spot market data.
 
@@ -40,29 +42,29 @@
 
         >>> from kraken.spot import Market
         >>> with Market() as market:
         ...     print(market.get_assets())
     """
 
     def __init__(
-        self: "Market",
+        self: Market,
         key: str = "",
         secret: str = "",
         url: str = "",
     ) -> None:
         super().__init__(key=key, secret=secret, url=url)
 
-    def __enter__(self: "Market") -> "Market":
+    def __enter__(self: Market) -> Market:
         super().__enter__()
         return self
 
     @ensure_string("assets")
     @lru_cache()
     def get_assets(
-        self: "Market",
+        self: Market,
         assets: Optional[Union[str, List[str]]] = None,
         aclass: Optional[str] = None,
     ) -> dict:
         """
         Get information about one or more assets.
         If ``assets`` is not specified, all assets will be returned.
 
@@ -115,21 +117,24 @@
         """
         params: dict = {}
         if defined(assets):
             params["asset"] = assets
         if defined(aclass):
             params["aclass"] = aclass
         return self._request(  # type: ignore[return-value]
-            method="GET", uri="/public/Assets", params=params, auth=False
+            method="GET",
+            uri="/public/Assets",
+            params=params,
+            auth=False,
         )
 
     @ensure_string("pair")
     @lru_cache()
     def get_asset_pairs(
-        self: "Market",
+        self: Market,
         pair: Optional[Union[str, List[str]]] = None,
         info: Optional[str] = None,
     ) -> dict:
         """
         Get information about a single or multiple asset/currency pair(s).
         If ``pair`` is left blank, all currency pairs will be returned.
 
@@ -190,21 +195,22 @@
         """
         params: dict = {}
         if defined(pair):
             params["pair"] = pair
         if defined(info):
             params["info"] = info
         return self._request(  # type: ignore[return-value]
-            method="GET", uri="/public/AssetPairs", params=params, auth=False
+            method="GET",
+            uri="/public/AssetPairs",
+            params=params,
+            auth=False,
         )
 
     @ensure_string("pair")
-    def get_ticker(
-        self: "Market", pair: Optional[Union[str, List[str]]] = None
-    ) -> dict:
+    def get_ticker(self: Market, pair: Optional[Union[str, List[str]]] = None) -> dict:
         """
         Returns all tickers if pair is not specified - else just
         the ticker of the ``pair``. Multiple pairs can be specified.
 
         https://docs.kraken.com/rest/#operation/getTickerInformation
 
         :param pair: Filter by pair(s)
@@ -232,19 +238,22 @@
                 }
             }
         """
         params: dict = {}
         if defined(pair):
             params["pair"] = pair
         return self._request(  # type: ignore[return-value]
-            method="GET", uri="/public/Ticker", params=params, auth=False
+            method="GET",
+            uri="/public/Ticker",
+            params=params,
+            auth=False,
         )
 
     def get_ohlc(
-        self: "Market",
+        self: Market,
         pair: str,
         interval: Union[int, str] = 1,
         since: Optional[Union[int, str]] = None,
     ) -> dict:
         """
         Get the open, high, low, and close data for a specific trading pair.
         Returns at max 720 time stamps per request.
@@ -281,18 +290,21 @@
                 ]
             }
         """
         params: dict = {"pair": pair, "interval": interval}
         if defined(since):
             params["since"] = since
         return self._request(  # type: ignore[return-value]
-            method="GET", uri="/public/OHLC", params=params, auth=False
+            method="GET",
+            uri="/public/OHLC",
+            params=params,
+            auth=False,
         )
 
-    def get_order_book(self: "Market", pair: str, count: Optional[int] = 100) -> dict:
+    def get_order_book(self: Market, pair: str, count: Optional[int] = 100) -> dict:
         """
         Get the current orderbook of a specified trading pair.
 
         - https://docs.kraken.com/rest/#operation/getOrderBook
 
         :param pair: The pair to get the orderbook from
         :type pair: str
@@ -325,15 +337,15 @@
             method="GET",
             uri="/public/Depth",
             params={"pair": pair, "count": count},
             auth=False,
         )
 
     def get_recent_trades(
-        self: "Market",
+        self: Market,
         pair: str,
         since: Optional[Union[str, int]] = None,
         count: Optional[int] = None,
     ) -> dict:
         """
         Get the latest trades for a specific trading pair (up to 1000).
 
@@ -366,19 +378,24 @@
         """
         params: dict = {"pair": pair}
         if defined(since):
             params["since"] = since
         if defined(count):
             params["count"] = count
         return self._request(  # type: ignore[return-value]
-            method="GET", uri="/public/Trades", params=params, auth=False
+            method="GET",
+            uri="/public/Trades",
+            params=params,
+            auth=False,
         )
 
     def get_recent_spreads(
-        self: "Market", pair: str, since: Optional[Union[str, int]] = None
+        self: Market,
+        pair: str,
+        since: Optional[Union[str, int]] = None,
     ) -> dict:
         """
         Get the latest spreads for a specific trading pair.
 
         - https://docs.kraken.com/rest/#operation/getRecentSpreads
 
         :param pair: Pair to get the recent spreads
@@ -403,18 +420,21 @@
                 ]
             }
         """
         params: dict = {"pair": pair}
         if defined(since):
             params["since"] = since
         return self._request(  # type: ignore[return-value]
-            method="GET", uri="/public/Spread", params=params, auth=False
+            method="GET",
+            uri="/public/Spread",
+            params=params,
+            auth=False,
         )
 
-    def get_system_status(self: "Market") -> dict:
+    def get_system_status(self: Market) -> dict:
         """
         Returns the system status of the Kraken Spot API.
 
         - https://docs.kraken.com/rest/#section/General-Usage/Requests-Responses-and-Errors
 
         :return: Success or failure
         :rtype: dict
@@ -424,9 +444,14 @@
             :caption: Spot Market: Get the Kraken API system status
 
             >>> from kraken.spot import Market
             >>> Market().get_system_status()
             {'status': 'online', 'timestamp': '2023-04-05T17:12:31Z'}
         """
         return self._request(  # type: ignore[return-value]
-            method="GET", uri="/public/SystemStatus", auth=False
+            method="GET",
+            uri="/public/SystemStatus",
+            auth=False,
         )
+
+
+__all__ = ["Market"]
```

### Comparing `python-kraken-sdk-1.5.0/kraken/spot/staking.py` & `python-kraken-sdk-1.6.0/kraken/spot/staking.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) 2023 Benjamin Thomas Schwertfeger
 # GitHub: https://github.com/btschwertfeger
 #
 
 """Module that implements the Kraken Spot Staking client"""
 
+from __future__ import annotations
+
 from typing import List, Optional, Union
 
-from ..base_api import KrakenBaseSpotAPI, defined
+from kraken.base_api import KrakenBaseSpotAPI, defined
 
 
 class Staking(KrakenBaseSpotAPI):
     """
     Class that implements the Kraken Spot Staking client. Currently there
     are no staking endpoints that could be accesses without authentication.
 
@@ -46,20 +48,23 @@
         self,
         key: str = "",
         secret: str = "",
         url: str = "",
     ) -> None:
         super().__init__(key=key, secret=secret, url=url)
 
-    def __enter__(self: "Staking") -> "Staking":
+    def __enter__(self: Staking) -> Staking:
         super().__enter__()
         return self
 
     def stake_asset(
-        self: "Staking", asset: str, amount: Union[str, int, float], method: str
+        self: Staking,
+        asset: str,
+        amount: Union[str, int, float],
+        method: str,
     ) -> dict:
         """
         Stake the specified asset from the Spot wallet.
 
         Requires the ``Withdraw funds`` permission in the API key settings.
 
         Have a look at :func:`kraken.spot.Staking.list_stakeable_assets` to get
@@ -93,15 +98,15 @@
             method="POST",
             uri="/private/Stake",
             params={"asset": asset, "amount": amount, "method": method},
             auth=True,
         )
 
     def unstake_asset(
-        self: "Staking",
+        self: Staking,
         asset: str,
         amount: Union[str, int, float],
         method: Optional[str] = None,
     ) -> dict:
         """
         Unstake an asset and transfer the amount to the Spot wallet.
 
@@ -135,18 +140,21 @@
             { 'refid': 'BOG5AE5-KSCNR4-VPNPEV' }
         """
         params: dict = {"asset": asset, "amount": amount}
         if defined(method):
             params["method"] = method
 
         return self._request(  # type: ignore[return-value]
-            method="POST", uri="/private/Unstake", params=params, auth=True
+            method="POST",
+            uri="/private/Unstake",
+            params=params,
+            auth=True,
         )
 
-    def list_stakeable_assets(self: "Staking") -> List[dict]:
+    def list_stakeable_assets(self: Staking) -> List[dict]:
         """
         Get a list of stakeable assets. Only assets that the user is able to stake
         will be shown.
 
         Requires the ``Withdraw funds`` and ``Query funds`` API key permissions.
 
         https://docs.kraken.com/rest/#operation/getStakingAssetInfo
@@ -192,18 +200,20 @@
                         "staking": "0.0000000000",
                         "unstaking": "0.0000000000"
                     }
                 }, ...
             ]
         """
         return self._request(  # type: ignore[return-value]
-            method="POST", uri="/private/Staking/Assets", auth=True
+            method="POST",
+            uri="/private/Staking/Assets",
+            auth=True,
         )
 
-    def get_pending_staking_transactions(self: "Staking") -> List[dict]:
+    def get_pending_staking_transactions(self: Staking) -> List[dict]:
         """
         Get the list of pending staking transactions of the user.
 
         Requires the ``Withdraw funds`` and ``Query funds`` API key permissions.
 
         - https://docs.kraken.com/rest/#operation/getStakingPendingDeposits
 
@@ -228,18 +238,20 @@
                     'time': 1623653613,
                     'status': 'Initial',
                     'type': 'bonding'
                 }, ...
             ]
         """
         return self._request(  # type: ignore[return-value]
-            method="POST", uri="/private/Staking/Pending", auth=True
+            method="POST",
+            uri="/private/Staking/Pending",
+            auth=True,
         )
 
-    def list_staking_transactions(self: "Staking") -> List[dict]:
+    def list_staking_transactions(self: Staking) -> List[dict]:
         """
         List the last 1000 staking transactions of the past 90 days.
 
         Requires the ``Query funds`` API key permission.
 
         - https://docs.kraken.com/rest/#operation/getStakingTransactions
 
@@ -267,9 +279,14 @@
                     'bond_start': 1623234684,
                     'bond_end': 1632345316
                 }, ...
             ]
 
         """
         return self._request(  # type: ignore[return-value]
-            method="POST", uri="/private/Staking/Transactions", auth=True
+            method="POST",
+            uri="/private/Staking/Transactions",
+            auth=True,
         )
+
+
+__all__ = ["Staking"]
```

### Comparing `python-kraken-sdk-1.5.0/kraken/spot/trade.py` & `python-kraken-sdk-1.6.0/kraken/spot/trade.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,21 +2,23 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) 2023 Benjamin Thomas Schwertfeger
 # GitHub: https://github.com/btschwertfeger
 #
 
 """Module that implements the Kraken Trade Spot client"""
 
+from __future__ import annotations
+
 from decimal import Decimal
 from functools import lru_cache
 from math import floor
 from typing import List, Optional, Union
 
-from ..base_api import KrakenBaseSpotAPI, defined, ensure_string
-from .market import Market
+from kraken.base_api import KrakenBaseSpotAPI, defined, ensure_string
+from kraken.spot.market import Market
 
 
 class Trade(KrakenBaseSpotAPI):
     """
     Class that implements the Kraken Trade Spot client
 
     :param key: Spot API public key (default: ``""``)
@@ -43,29 +45,29 @@
         >>> from kraken.spot import Trade
         >>> with Trade(key="api-key", secret="secret-key") as trade:
         ...     print(trade.create_order(...))
 
     """
 
     def __init__(
-        self: "Trade",
+        self: Trade,
         key: str = "",
         secret: str = "",
         url: str = "",
     ) -> None:
         super().__init__(key=key, secret=secret, url=url)
         self.__market: Market = Market()
 
-    def __enter__(self: "Trade") -> "Trade":
+    def __enter__(self: Trade) -> Trade:
         super().__enter__()
         return self
 
     @ensure_string("oflags")
-    def create_order(
-        self: "Trade",
+    def create_order(  # noqa: PLR0913 PLR0912
+        self: Trade,
         ordertype: str,
         side: str,
         pair: str,
         volume: Union[str, int, float],
         price: Optional[Union[str, int, float]] = None,
         price2: Optional[Union[str, int, float]] = None,
         truncate: bool = False,
@@ -324,20 +326,20 @@
                 price
                 if not truncate
                 else self.truncate(amount=price, amount_type="price", pair=pair)
             )
         if ordertype in ("stop-loss-limit", "take-profit-limit"):
             if not defined(price2):
                 raise ValueError(
-                    f"Ordertype {ordertype} requires a secondary price (price2)!"
+                    f"Ordertype {ordertype} requires a secondary price (price2)!",
                 )
             params["price2"] = str(price2)
         elif price2 is not None:
             raise ValueError(
-                f"Ordertype {ordertype} dos not allow a second price (price2)!"
+                f"Ordertype {ordertype} dos not allow a second price (price2)!",
             )
         if defined(leverage):
             params["leverage"] = str(leverage)
         if defined(oflags):
             params["oflags"] = oflags
         if defined(close_ordertype):
             params["close[ordertype]"] = close_ordertype
@@ -349,19 +351,21 @@
             params["deadline"] = deadline
         if defined(userref):
             params["userref"] = userref
         if defined(displayvol):
             params["displayvol"] = str(displayvol)
 
         return self._request(  # type: ignore[return-value]
-            method="POST", uri="/private/AddOrder", params=params
+            method="POST",
+            uri="/private/AddOrder",
+            params=params,
         )
 
     def create_order_batch(
-        self: "Trade",
+        self: Trade,
         orders: List[dict],
         pair: str,
         deadline: Optional[str] = None,
         validate: bool = False,
     ) -> dict:
         """
         Create a batch of max 15 orders for a specific asset pair.
@@ -424,20 +428,23 @@
                 }]
             }
         """
         params: dict = {"orders": orders, "pair": pair, "validate": validate}
         if defined(deadline):
             params["deadline"] = deadline
         return self._request(  # type: ignore[return-value]
-            method="POST", uri="/private/AddOrderBatch", params=params, do_json=True
+            method="POST",
+            uri="/private/AddOrderBatch",
+            params=params,
+            do_json=True,
         )
 
     @ensure_string("oflags")
-    def edit_order(
-        self: "Trade",
+    def edit_order(  # noqa: PLR0913
+        self: Trade,
         txid: str,
         pair: str,
         volume: Optional[Union[str, int, float]] = None,
         price: Optional[Union[str, int, float]] = None,
         price2: Optional[Union[str, int, float]] = None,
         truncate: bool = False,
         oflags: Optional[str] = None,
@@ -464,15 +471,16 @@
         :type price: str | int | float, optional
         :param price2: Set a new second price
         :type price2: str | int | float, optional
         :param truncate: If enabled: round the ``price`` and ``volume`` to Kraken's
             maximum allowed decimal places. See https://support.kraken.com/hc/en-us/articles/4521313131540
             fore more information about decimals.
         :type truncate: bool, optional
-        :param oflags: Order flags like ``post``, ``fcib``, ``fciq``, ``nomp``, ``viqc`` (see the referenced Kraken documentation for more information)
+        :param oflags: Order flags like ``post``, ``fcib``, ``fciq``, ``nomp``,
+            ``viqc`` (see the referenced Kraken documentation for more information)
         :type oflags: str | List[str], optional
         :param deadline: (see the referenced Kraken documentation for more information)
         :type deadline: string
         :param cancel_response: See the referenced Kraken documentation for more information
         :type cancel_response: bool, optional
         :param validate: Validate the order without placing on the market (default: ``False``)
         :type validate: bool, optional
@@ -524,19 +532,21 @@
         if defined(oflags):
             params["oflags"] = oflags
         if defined(cancel_response):
             params["cancel_response"] = cancel_response
         if defined(deadline):
             params["deadline"] = deadline
         return self._request(  # type: ignore[return-value]
-            "POST", uri="/private/EditOrder", params=params
+            "POST",
+            uri="/private/EditOrder",
+            params=params,
         )
 
     @ensure_string("txid")
-    def cancel_order(self: "Trade", txid: str) -> dict:
+    def cancel_order(self: Trade, txid: str) -> dict:
         """
         Cancel a specific order by ``txid``. Instead of a transaction id
         a user reference id can be passed.
 
         Requires the ``Cancel/close orders`` permission in
         the API key settings.
 
@@ -558,15 +568,15 @@
         """
         return self._request(  # type: ignore[return-value]
             method="POST",
             uri="/private/CancelOrder",
             params={"txid": txid},
         )
 
-    def cancel_all_orders(self: "Trade") -> dict:
+    def cancel_all_orders(self: Trade) -> dict:
         """
         Cancel all open orders.
 
         Requires the ``Cancel/close orders`` permission in
         the API key settings.
 
         - https://docs.kraken.com/rest/#operation/cancelAllOrders
@@ -580,18 +590,19 @@
 
             >>> from kraken.spot import Trade
             >>> trade = Trade(key="api-key", secret="secret-key")
             >>> trade.cancel_all_orders()
             { 'count': 2 }
         """
         return self._request(  # type: ignore[return-value]
-            method="POST", uri="/private/CancelAll"
+            method="POST",
+            uri="/private/CancelAll",
         )
 
-    def cancel_all_orders_after_x(self: "Trade", timeout: int = 0) -> dict:
+    def cancel_all_orders_after_x(self: Trade, timeout: int = 0) -> dict:
         """
         Cancel all orders after a timeout. This can be used as Dead Man's Switch.
 
         Requires the ``Create and modify orders`` permission in
         the API key settings.
 
         - https://docs.kraken.com/rest/#operation/cancelAllOrdersAfter
@@ -615,15 +626,15 @@
         """
         return self._request(  # type: ignore[return-value]
             method="POST",
             uri="/private/CancelAllOrdersAfter",
             params={"timeout": timeout},
         )
 
-    def cancel_order_batch(self: "Trade", orders: List[Union[str, int]]) -> dict:
+    def cancel_order_batch(self: Trade, orders: List[Union[str, int]]) -> dict:
         """
         Cancel a a list of orders by ``txid`` or ``userref``
 
         Requires the ``Cancel/close orders`` permission in
         the API key settings.
 
         - https://docs.kraken.com/rest/#operation/cancelOrderBatch
@@ -649,15 +660,15 @@
             uri="/private/CancelOrderBatch",
             params={"orders": orders},
             do_json=True,
         )
 
     @lru_cache()
     def truncate(
-        self: "Trade",
+        self: Trade,
         amount: Union[Decimal, float, int, str],
         amount_type: str,
         pair: str,
     ) -> str:
         """
         Kraken only allows volume and price amounts to be specified with a specific number of
         decimal places, and these vary depending on the currency pair used.
@@ -715,15 +726,15 @@
             ... ))
             21123.0
         """
         if amount_type not in ("price", "volume"):
             raise ValueError("Amount type must be 'volume' or 'price'!")
 
         pair_data: dict = self.__market.get_asset_pairs(pair=pair)
-        data: dict = pair_data[list(pair_data)[0]]
+        data: dict = pair_data[next(iter(pair_data))]
 
         pair_decimals: int = int(data["pair_decimals"])
         lot_decimals: int = int(data["lot_decimals"])
 
         ordermin: Decimal = Decimal(data["ordermin"])
         costmin: Decimal = Decimal(data["costmin"])
 
@@ -737,7 +748,10 @@
         else:  # amount_type == "volume":
             if ordermin > amount:
                 raise ValueError(f"Volume is less than the ordermin: {ordermin}!")
             decimals = lot_decimals
 
         amount_rounded: float = floor(float(amount) * 10**decimals) / 10**decimals
         return f"{amount_rounded:.{decimals}f}"
+
+
+__all__ = ["Trade"]
```

### Comparing `python-kraken-sdk-1.5.0/kraken/spot/user.py` & `python-kraken-sdk-1.6.0/kraken/spot/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) 2023 Benjamin Thomas Schwertfeger
 # GitHub: https://github.com/btschwertfeger
 #
 
 """ Module that implements the Kraken Spot User client"""
+
+from __future__ import annotations
+
 from decimal import Decimal
 from typing import List, Optional, Union
 
-from ..base_api import KrakenBaseSpotAPI, defined, ensure_string
+from kraken.base_api import KrakenBaseSpotAPI, defined, ensure_string
 
 
 class User(KrakenBaseSpotAPI):
     """
     Class that implements the Kraken Spot User client
 
     Requires the ``Query funds`` permission in the API key settings.
@@ -40,26 +43,26 @@
 
         >>> from kraken.spot import User
         >>> with User(key="api-key", secret="secret-key") as user:
         ...     print(user.get_account_balances())
     """
 
     def __init__(
-        self: "User",
+        self: User,
         key: str = "",
         secret: str = "",
         url: str = "",
     ) -> None:
         super().__init__(key=key, secret=secret, url=url)
 
-    def __enter__(self: "User") -> "User":
+    def __enter__(self: User) -> User:
         super().__enter__()
         return self
 
-    def get_account_balance(self: "User") -> dict:
+    def get_account_balance(self: User) -> dict:
         """
         Get the current balances of the user.
 
         Requires the ``Query funds`` permission in the API key settings.
 
         - https://docs.kraken.com/rest/#operation/getAccountBalance
 
@@ -78,18 +81,19 @@
                 'XXLM': '0.00000000',
                 'ZEUR': '0.0000',
                 'DOT': '32011.21197000',
                 ...
             }
         """
         return self._request(  # type: ignore[return-value]
-            method="POST", uri="/private/Balance"
+            method="POST",
+            uri="/private/Balance",
         )
 
-    def get_balances(self: "User") -> dict:
+    def get_balances(self: User) -> dict:
         """
         Retrieve the user's asset balances and the
         the corresponding amount held by open orders.
 
         Requires the ``Query funds`` permission in the API key settings.
 
         :return: Dictionary containing the ``currency`` as keys, that
@@ -119,18 +123,19 @@
                 'KFEE': {
                     'balance': '1407.73', 'hold_trade': '0.00'
                 },
                 ...
             }
         """
         return self._request(  # type: ignore[return-value]
-            method="POST", uri="/private/BalanceEx"
+            method="POST",
+            uri="/private/BalanceEx",
         )
 
-    def get_balance(self: "User", currency: str) -> dict:
+    def get_balance(self: User, currency: str) -> dict:
         """
         Returns the balance and available balance of a given currency.
 
         Requires the ``Query funds`` permission in the API key settings.
 
         :param currency: The currency to get the balances from
         :type currency: str
@@ -165,15 +170,15 @@
 
         return {
             "currency": currency,
             "balance": float(balance),
             "available_balance": float(available_balance),
         }
 
-    def get_trade_balance(self: "User", asset: Optional[str] = "ZUSD") -> dict:
+    def get_trade_balance(self: User, asset: Optional[str] = "ZUSD") -> dict:
         """
         Get the summary of all collateral balances.
 
         Requires the ``Query funds``, ``Query open orders & trades``,
         and ``Query closed orders & trades`` permissions in the API key settings.
 
         - https://docs.kraken.com/rest/#operation/getTradeBalance
@@ -200,28 +205,34 @@
                 'mf': '322296.9914'  # Free margin ( tb / initial margin ) * 100
             }
         """
         params: dict = {}
         if defined(asset):
             params["asset"] = asset
         return self._request(  # type: ignore[return-value]
-            method="POST", uri="/private/TradeBalance", params=params
+            method="POST",
+            uri="/private/TradeBalance",
+            params=params,
         )
 
     def get_open_orders(
-        self: "User", trades: Optional[bool] = False, userref: Optional[int] = None
+        self: User,
+        trades: Optional[bool] = False,
+        userref: Optional[int] = None,
     ) -> dict:
         """
         Get information about the open orders.
 
-        Requires the ``Query open orders & trades`` permission in the API key settings.
+        Requires the ``Query open orders & trades`` permission in the API key
+        settings.
 
         - https://docs.kraken.com/rest/#operation/getOpenOrders
 
-        :param trades: Include trades related to position or not into the response (default: ``False``)
+        :param trades: Include trades related to position or not into the
+            response (default: ``False``)
         :type trades: bool
         :param userref: Filter the results by user reference id
         :type userref: int, optional
 
         .. code-block:: python
             :linenos:
             :caption: Spot User: Get the open orders
@@ -265,44 +276,49 @@
                 }
             }
         """
         params: dict = {"trades": trades}
         if defined(userref):
             params["userref"] = userref
         return self._request(  # type: ignore[return-value]
-            method="POST", uri="/private/OpenOrders", params=params
+            method="POST",
+            uri="/private/OpenOrders",
+            params=params,
         )
 
     def get_closed_orders(
-        self: "User",
+        self: User,
         trades: Optional[bool] = False,
         userref: Optional[int] = None,
         start: Optional[int] = None,
         end: Optional[int] = None,
         ofs: Optional[int] = None,
         closetime: Optional[str] = "both",
     ) -> dict:
         """
         Get the 50 latest closed (filled or canceled) orders.
 
-        Requires the ``Query closed orders & trades`` permission in the API key settings.
+        Requires the ``Query closed orders & trades`` permission in the API key
+        settings.
 
         - https://docs.kraken.com/rest/#operation/getClosedOrders
 
-        :param trades: Include trades related to position into the response or not (default: ``False``)
+        :param trades: Include trades related to position into the response or
+        not (default: ``False``)
         :type trades: bool
         :param userref: Filter the results by user reference id
         :type userref: int, optional
         :param start: Unix timestamp to start the search from
         :type start: int, optional
         :param end: Unix timestamp to define the last result to include
         :type end: int, optional
         :param ofs: Offset for pagination
         :type ofs: int, optional
-        :param closetime: Specify the exact time frame, one of: ``both``, ``open``, ``close`` (default: ``both``)
+        :param closetime: Specify the exact time frame, one of: ``both``,
+            ``open``, ``close`` (default: ``both``)
         :type closetime: str, optional
 
         .. code-block:: python
             :linenos:
             :caption: Spot User: Get the closed orders
 
             >>> from kraken.spot import User
@@ -352,40 +368,44 @@
             params["start"] = start
         if defined(end):
             params["end"] = end
         if defined(ofs):
             params["ofs"] = ofs
 
         return self._request(  # type: ignore[return-value]
-            method="POST", uri="/private/ClosedOrders", params=params
+            method="POST",
+            uri="/private/ClosedOrders",
+            params=params,
         )
 
     @ensure_string("txid")
     def get_orders_info(
-        self: "User",
+        self: User,
         txid: Union[List[str], str],
         trades: Optional[bool] = False,
         userref: Optional[int] = None,
         consolidate_taker: Optional[bool] = True,
     ) -> dict:
         """
         Get information about one or more orders.
 
-        Requires the ``Query open orders & trades`` and ``Query closed orders & trades``
-        permissions in the API key settings.
+        Requires the ``Query open orders & trades`` and
+        ``Query closed orders & trades`` permissions in the API key settings.
 
         - https://docs.kraken.com/rest/#tag/User-Data/operation/getOrdersInfo
 
-        :param txid: A transaction id of a specific order, a list of txids or a string containing a comma delimited list of txids
+        :param txid: A transaction id of a specific order, a list of txids or a
+            string containing a comma delimited list of txids
         :type txid: str | List[str]
         :param trades: Include trades in the result or not (default: ``False``)
         :type trades: bool, optional
         :param userref: Filter results by user reference id
         :type userref: int, optional
-        :param consolidate_taker: Consolidate trades by individual taker trades (default: ``True``)
+        :param consolidate_taker: Consolidate trades by individual taker trades
+            (default: ``True``)
         :type consolidate_taker: bool, optional
 
         .. code-block:: python
             :linenos:
             :caption: Spot User: Get order information
 
             >>> from kraken.spot import User
@@ -458,34 +478,38 @@
             "txid": txid,
             "trades": trades,
             "consolidate_taker": consolidate_taker,
         }
         if defined(userref):
             params["userref"] = userref
         return self._request(  # type: ignore[return-value]
-            method="POST", uri="/private/QueryOrders", params=params
+            method="POST",
+            uri="/private/QueryOrders",
+            params=params,
         )
 
     def get_trades_history(
-        self: "User",
+        self: User,
         type_: Optional[str] = "all",
         trades: Optional[bool] = False,
         start: Optional[int] = None,
         end: Optional[int] = None,
         ofs: Optional[int] = None,
         consolidate_taker: bool = True,
     ) -> dict:
         """
         Get information about the latest 50 trades and fills. Can be paginated.
 
         Requires the ``Query closed orders & trades`` permission in the API key settings.
 
         - https://docs.kraken.com/rest/#operation/getTradeHistory
 
-        :param type_: Filter by type of trade, one of: ``all``, ``any position``, ``closed position``, ``closing position``, and ``no position`` (default: ``all``)
+        :param type_: Filter by type of trade, one of: ``all``,
+            ``any position``, ``closed position``, ``closing position``, and
+            ``no position`` (default: ``all``)
         :type type_: str, optional
         :param trades: Include trades related to a position or not (default: ``False``)
         :type trades: bool, optional
         :param start: Timestamp or txid to start the search
         :type start: int, optional
         :param end: Timestamp or txid to define the last included result
         :type end: int, optional
@@ -531,20 +555,24 @@
         if defined(start):
             params["start"] = start
         if defined(end):
             params["end"] = end
         if defined(ofs):
             params["ofs"] = ofs
         return self._request(  # type: ignore[return-value]
-            method="POST", uri="/private/TradesHistory", params=params
+            method="POST",
+            uri="/private/TradesHistory",
+            params=params,
         )
 
     @ensure_string("txid")
     def get_trades_info(
-        self: "User", txid: Union[str, List[str]], trades: Optional[bool] = False
+        self: User,
+        txid: Union[str, List[str]],
+        trades: Optional[bool] = False,
     ) -> dict:
         """
         Get information about specific trades/filled orders. 20 txids can be queried maximum.
 
         Requires the ``Query open orders & trades`` and ``Query closed orders & trades``
         permission in the API key settings.
 
@@ -588,15 +616,15 @@
                 "trades": trades,
                 "txid": txid,
             },
         )
 
     @ensure_string("txid")
     def get_open_positions(
-        self: "User",
+        self: User,
         txid: Optional[Union[str, List[str]]] = None,
         docalcs: Optional[bool] = False,
         consolidation: Optional[str] = "market",
     ) -> dict:
         """
         Get information about the open margin positions.
 
@@ -642,20 +670,22 @@
                 }, ...
             }
         """
         params: dict = {"docalcs": docalcs, "consolidation": consolidation}
         if defined(txid):
             params["txid"] = txid
         return self._request(  # type: ignore[return-value]
-            method="POST", uri="/private/OpenPositions", params=params
+            method="POST",
+            uri="/private/OpenPositions",
+            params=params,
         )
 
     @ensure_string("asset")
     def get_ledgers_info(
-        self: "User",
+        self: User,
         asset: Optional[Union[str, List[str]]] = "all",
         aclass: Optional[str] = "currency",
         type_: Optional[str] = "all",
         start: Optional[int] = None,
         end: Optional[int] = None,
         ofs: Optional[int] = None,
     ) -> dict:
@@ -712,32 +742,38 @@
         if defined(start):
             params["start"] = start
         if defined(end):
             params["end"] = end
         if defined(ofs):
             params["ofs"] = ofs
         return self._request(  # type: ignore[return-value]
-            method="POST", uri="/private/Ledgers", params=params
+            method="POST",
+            uri="/private/Ledgers",
+            params=params,
         )
 
     @ensure_string("id_")
     def get_ledgers(
-        self: "User", id_: Union[str, List[str]], trades: Optional[bool] = False
+        self: User,
+        id_: Union[str, List[str]],
+        trades: Optional[bool] = False,
     ) -> dict:
         """
         Get information about specific ledeger entries.
 
         Requires the ``Query funds`` and ``Query ledger entries`` permissions in
         the API key settings.
 
         - https://docs.kraken.com/rest/#operation/getLedgersInfo
 
-        :param id_: Ledger id as string, list of strings, or comma delimited list of ledger ids as string
+        :param id_: Ledger id as string, list of strings, or comma delimited
+            list of ledger ids as string
         :type id_: str | List[str]
-        :param trades: Include trades related to a position or not (default: ``False``)
+        :param trades: Include trades related to a position or not
+            (default: ``False``)
         :type trades: bool, optional
 
         .. code-block:: python
             :linenos:
             :caption: Spot User: Get ledgers
 
             >>> from kraken.spot import User
@@ -761,26 +797,27 @@
             method="POST",
             uri="/private/QueryLedgers",
             params={"trades": trades, "id": id_},
         )
 
     @ensure_string("pair")
     def get_trade_volume(
-        self: "User",
+        self: User,
         pair: Optional[Union[str, List[str]]] = None,
         fee_info: bool = True,
     ) -> dict:
         """
         Get the 30-day user specific trading volume in USD.
 
         Requires the ``Query funds`` permission in the API key settings.
 
         - https://docs.kraken.com/rest/#operation/getTradeVolume
 
-        :param pair: Asset pair, list of asset pairs or comma delimited list (as string) of asset pairs to filter
+        :param pair: Asset pair, list of asset pairs or comma delimited list
+            (as string) of asset pairs to filter
         :type pair: str | List[str], optional
         :param fee_info: Include fee information or not (default: ``True``)
         :type fee_info: bool, optional
 
         .. code-block:: python
             :linenos:
             :caption: Spot User: Get the 30-day trade volume
@@ -821,20 +858,22 @@
             }
 
         """
         params: dict = {"fee-info": fee_info}
         if defined(pair):
             params["pair"] = pair
         return self._request(  # type: ignore[return-value]
-            method="POST", uri="/private/TradeVolume", params=params
+            method="POST",
+            uri="/private/TradeVolume",
+            params=params,
         )
 
     @ensure_string("fields")
     def request_export_report(
-        self: "User",
+        self: User,
         report: str,
         description: str,
         format_: Optional[str] = "CSV",
         fields: Optional[Union[str, List[str]]] = "all",
         starttm: Optional[int] = None,
         endtm: Optional[int] = None,
         **kwargs: dict,
@@ -847,15 +886,16 @@
         ``Query closed orders & trades`` must be set. For exporting ledgers the
         ``Query funds`` and ``Query ledger entries`` must be set.
 
         - https://docs.kraken.com/rest/#operation/addExport
 
         :param report: Kind of report, one of: ``trades`` and ``ledgers``
         :type report: str
-        :param format_: The export format of the requesting report, one of ``CSV`` and ``TSV`` (default: ``CSV``)
+        :param format_: The export format of the requesting report, one of
+            ``CSV`` and ``TSV`` (default: ``CSV``)
         :type format_: str
         :param fields: Fields to include in the report (default: ``all``)
         :type fields: str | List[str], optional
         :param starttm: Unix timestamp to start
         :type starttm: int, optional
         :param endtm: Unix timestamp of the last result
         :type endtm: int, optional
@@ -869,33 +909,35 @@
             >>> from kraken.spot import User
             >>> user = User(key="api-key", secret="secret-key")
             >>> user.request_export_report(
             ...     report="ledgers", description="myLedgers1", format="CSV"
             ... )
             { 'id': 'GEHI' }
         """
-        if report not in ["trades", "ledgers"]:
-            raise ValueError('report must be one of "trades", "ledgers"')
+        if report not in ("trades", "ledgers"):
+            raise ValueError('`report` must be either "trades" or "ledgers".')
 
         params: dict = {
             "report": report,
             "description": description,
             "format": format_,
             "fields": fields,
         }
         params.update(kwargs)
         if defined(starttm):
             params["starttm"] = starttm
         if defined(endtm):
             params["endtm"] = endtm
         return self._request(  # type: ignore[return-value]
-            method="POST", uri="/private/AddExport", params=params
+            method="POST",
+            uri="/private/AddExport",
+            params=params,
         )
 
-    def get_export_report_status(self: "User", report: str) -> dict:
+    def get_export_report_status(self: User, report: str) -> dict:
         """
         Get the status of the current pending report.
 
         Requires the ``Export data`` permission. In addition for exporting trades
         data the permissions ``Query open orders & trades`` and
         ``Query closed orders & trades`` must be set. For exporting ledgers the
         ``Query funds`` and ``Query ledger entries`` must be set.
@@ -939,18 +981,20 @@
                     'flags': '0'
                 }
             ]
         """
         if report not in ("trades", "ledgers"):
             raise ValueError('report must be one of "trades", "ledgers"')
         return self._request(  # type: ignore[return-value]
-            method="POST", uri="/private/ExportStatus", params={"report": report}
+            method="POST",
+            uri="/private/ExportStatus",
+            params={"report": report},
         )
 
-    def retrieve_export(self: "User", id_: str) -> dict:
+    def retrieve_export(self: User, id_: str) -> dict:
         """
         Retrieve the requested report export.
 
         Requires the ``Export data`` permission. In addition for exporting trades
         data the permissions ``Query open orders & trades`` and
         ``Query closed orders & trades`` must be set. For exporting ledgers the
         ``Query funds`` and ``Query ledger entries`` must be set.
@@ -983,15 +1027,17 @@
             method="POST",
             uri="/private/RetrieveExport",
             params={"id": id_},
             return_raw=True,
         )
 
     def delete_export_report(
-        self: "User", id_: str, type_: Optional[str] = "delete"
+        self: User,
+        id_: str,
+        type_: Optional[str] = "delete",
     ) -> dict:
         """
         Delete a report from the Kraken server.
 
         Requires the ``Export data`` permission. In addition for exporting trades
         data the permissions ``Query open orders & trades`` and
         ``Query closed orders & trades`` must be set. For exporting ledgers the
@@ -1017,15 +1063,15 @@
         """
         return self._request(  # type: ignore[return-value]
             method="POST",
             uri="/private/RemoveExport",
             params={"id": id_, "type": type_},
         )
 
-    def create_subaccount(self: "User", username: str, email: str) -> dict:
+    def create_subaccount(self: User, username: str, email: str) -> dict:
         """
         Create a subaccount for trading. This is currently *only available
         for institutional clients*.
 
         - https://docs.kraken.com/rest/#tag/User-Subaccounts
 
         :param username: The username for the new subaccount
@@ -1045,7 +1091,60 @@
             { 'result': True }
         """
         return self._request(  # type: ignore[return-value]
             method="POST",
             uri="/private/CreateSubaccount",
             params={"username": username, "email": email},
         )
+
+    def account_transfer(
+        self: "User",
+        asset: str,
+        amount: Union[str, int, float],
+        from_: str,
+        to_: str,
+    ) -> dict:
+        """
+        Transfer funds between master and subaccounts. This is currently *only
+        available for institutional clients and must be called by the
+        master account*.
+
+        - https://docs.kraken.com/rest/#tag/User-Subaccounts/operation/accountTransfer
+
+        :param asset: The asset to transfer
+        :type asset: str
+        :param amount: The amount of that asset to transfer
+        :type amount: str | int | float
+        :param from_: The source account (IIBAN)
+        :type from_: str
+        :param to_: The destination account (IIBAN)
+        :type to_: str
+        :return: Success or failure
+        :rtype: dict
+
+        .. code-block:: python
+            :linenos:
+            :caption: Spot User: Transfer funds between accounts
+
+            >>> from kraken.spot import User
+            >>> user = User(key="api-key", secret="secret-key")
+            >>> user.account_transfer(
+            ...     "asset": "XBT",
+            ...     "amount": 1.0,
+            ...     "from": "ABCD 1234 EFGH 5678"
+            ...     "to": "IJKL 0987 MNOP 6543"
+            ... )
+            {
+                'result': {
+                    'transfer_id': 'TOH3AS2-LPCWR8-JDQGEU',
+                    'status': 'complete'
+                }
+            }
+        """
+        return self._request(  # type: ignore[return-value]
+            method="POST",
+            uri="/private/AccountTransfer",
+            params={"asset": asset, "amount": amount, "from": from_, "to": to_},
+        )
+
+
+__all__ = ["User"]
```

### Comparing `python-kraken-sdk-1.5.0/kraken/spot/ws_client.py` & `python-kraken-sdk-1.6.0/kraken/spot/websocket_v1.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,373 +1,390 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) 2023 Benjamin Thomas Schwertfeger
 # GitHub: https://github.com/btschwertfeger
 #
 
-"""This module provides the Spot websocket client. """
+"""
+This module provides the Spot websocket client (Websocket API V1 as
+documented in https://docs.kraken.com/websockets).
+"""
 
 from __future__ import annotations
 
-import logging
+import asyncio
+import json
 from copy import deepcopy
 from typing import Any, Callable, List, Optional, Union
 
-from ..base_api import KrakenBaseSpotAPI, defined, ensure_string
-from .trade import Trade
-from .websocket import ConnectSpotWebsocket
+from kraken.base_api import defined, ensure_string
+from kraken.exceptions import KrakenException
+from kraken.spot.trade import Trade
+from kraken.spot.websocket import KrakenSpotWSClientBase
 
 
-class KrakenSpotWSClient(KrakenBaseSpotAPI):
+class KrakenSpotWSClient(KrakenSpotWSClientBase):
     """
-    Class to access public and (optional)
-    private/authenticated websocket connection.
+    Class to access public and private/authenticated websocket connections.
 
-    - https://docs.kraken.com/websockets/#overview
+    **This client only supports the Kraken Websocket API v1.**
+
+    - https://docs.kraken.com/websockets
+
+    … please use :class:`KrakenSpotWSClientV2` for accessing the Kraken
+    Websockets API v2.
 
     This class holds up to two websocket connections, one private
     and one public.
 
     When accessing private endpoints that need authentication make sure,
     that the ``Access WebSockets API`` API key permission is set in the user's
-    account.
+    account. To place or cancel orders, querying ledger information or accessing
+    live portfolio changes (fills, new orders, ...) there are separate
+    permissions that must be enabled if required.
 
     :param key: API Key for the Kraken Spot API (default: ``""``)
     :type key: str, optional
     :param secret: Secret API Key for the Kraken Spot API (default: ``""``)
     :type secret: str, optional
-    :param url: Set a specific/custom url to access the Kraken API
+    :param url: Set a specific URL to access the Kraken REST API
     :type url: str, optional
-    :param beta: Use the beta websocket channels (maybe not supported anymore, default: ``False``)
+    :param no_public: Disables public connection (default: ``False``).
+        If not set or set to ``False``, the client will create a public and
+        a private connection per default. If only a private connection is
+        required, this parameter should be set to ``True``.
+    :param beta: Use the beta websocket channels (maybe not supported anymore,
+        default: ``False``)
     :type beta: bool
 
     .. code-block:: python
         :linenos:
-        :caption: HowTo: Create a Bot and integrate the python-kraken-sdk Spot Websocket Client
+        :caption: HowTo: Use the Kraken Spot websocket client (v1)
 
         import asyncio
         from kraken.spot import KrakenSpotWSClient
 
-        async def main() -> None:
-            class Bot(KrakenSpotWSClient):
 
-                async def on_message(self, event: dict) -> None:
-                    print(event)
+        class Client(KrakenSpotWSClient):
+
+            async def on_message(self, message):
+                print(message)
+
+
+        async def main():
 
-            bot = Bot()         # unauthenticated
-            auth_bot = Bot(     # authenticated
-                key='kraken-api-key',
-                secret='kraken-secret-key'
+            client = Client()         # unauthenticated
+            client_auth = Client(     # authenticated
+                key="kraken-api-key",
+                secret="kraken-secret-key"
             )
 
             # subscribe to the desired feeds:
-            await bot.subscribe(
+            await client.subscribe(
                 subscription={"name": ticker},
                 pair=["XBTUSD", "DOT/EUR"]
             )
             # from now on the on_message function receives the ticker feed
 
-            while not bot.exception_occur:
+            while not client.exception_occur:
                 await asyncio.sleep(6)
 
-        if __name__ == '__main__':
+        if __name__ == "__main__":
+            try:
+                asyncio.run(main())
+            except KeyboardInterrupt:
+                pass
+
+    .. code-block:: python
+        :linenos:
+        :caption: HowTo: Use the websocket client (v1) as instance
+
+        import asyncio
+        from kraken.spot import KrakenSpotWSClient
+
+
+        async def main() -> None:
+            async def on_message(message) -> None:
+                print(message)
+
+            client = KrakenSpotWSClient(callback=on_message)
+            await client.subscribe(
+                subscription={"name": "ticker"},
+                pair=["XBT/USD"]
+            )
+
+            while not client.exception_occur:
+                await asyncio.sleep(10)
+
+
+        if __name__ == "__main__":
             try:
                 asyncio.run(main())
             except KeyboardInterrupt:
                 pass
 
+
     .. code-block:: python
         :linenos:
-        :caption: HowTo: Use the websocket client as context manager
+        :caption: HowTo: Use the websocket client (v1) as context manager
 
         import asyncio
         from kraken.spot import KrakenSpotWSClient
 
-        async def on_message(msg):
-            print(msg)
+        async def on_message(message):
+            print(message)
 
         async def main() -> None:
             async with KrakenSpotWSClient(
                 key="api-key",
                 secret="secret-key",
                 callback=on_message
             ) as session:
                 await session.subscribe(
                     subscription={"name": "ticker"},
                     pair=["XBT/USD"]
                 )
 
-            while not bot.exception_occur::
+            while True
                 await asyncio.sleep(6)
 
 
         if __name__ == "__main__":
             try:
                 asyncio.run(main())
             except KeyboardInterrupt:
                 pass
     """
 
-    LOG: logging.Logger = logging.getLogger(__name__)
-
-    PROD_ENV_URL: str = "ws.kraken.com"
-    AUTH_PROD_ENV_URL: str = "ws-auth.kraken.com"
-    BETA_ENV_URL: str = "beta-ws.kraken.com"
-    AUTH_BETA_ENV_URL: str = "beta-ws-auth.kraken.com"
-
     def __init__(
-        self: "KrakenSpotWSClient",
+        self: KrakenSpotWSClient,
         key: str = "",
         secret: str = "",
-        url: str = "",
         callback: Optional[Callable] = None,
+        no_public: bool = False,
         beta: bool = False,
     ):
-        super().__init__(key=key, secret=secret, url=url, sandbox=beta)
-        self.__callback: Any = callback
-        self.__is_auth: bool = bool(key and secret)
-        self.exception_occur: bool = False
-
-        self._pub_conn: ConnectSpotWebsocket = ConnectSpotWebsocket(
-            client=self,
-            endpoint=self.PROD_ENV_URL if not beta else self.BETA_ENV_URL,
-            is_auth=False,
-            callback=self.on_message,
-        )
-
-        self._priv_conn: Optional[ConnectSpotWebsocket] = (
-            ConnectSpotWebsocket(
-                client=self,
-                endpoint=self.AUTH_PROD_ENV_URL if not beta else self.AUTH_BETA_ENV_URL,
-                is_auth=True,
-                callback=self.on_message,
-            )
-            if self.__is_auth
-            else None
+        super().__init__(
+            key=key,
+            secret=secret,
+            callback=callback,
+            no_public=no_public,
+            beta=beta,
+            api_version="v1",
         )
 
-    async def on_message(self: "KrakenSpotWSClient", msg: Union[dict, list]) -> None:
+    async def send_message(  # pylint: disable=arguments-differ
+        self: KrakenSpotWSClient,
+        message: dict,
+        private: bool = False,
+        raw: bool = False,
+    ) -> None:
         """
-        Calls the defined callback function (if defined)
-        or overload this function.
-
-        Can be overloaded as described in :class:`kraken.spot.KrakenSpotWSClient`
+        Sends a message via the websocket connection. For private messages
+        the authentication token will be assigned automatically if
+        ``raw=False``.
+
+        The user can specify a ``reqid`` within the message to identify
+        corresponding responses via websocket feed.
+
+        :param message: The content to send
+        :type message: dict
+        :param private: Use authentication (default: ``False``)
+        :type private: bool, optional
+        :param raw: If set to ``True`` the ``message`` will be sent directly.
+        :type raw: bool, optional
+        """
+
+        if private and not self._is_auth:
+            raise KrakenException.KrakenAuthenticationError
+
+        socket: Any = self._get_socket(private=private)
+        while not socket:
+            socket = self._get_socket(private=private)
+            await asyncio.sleep(0.4)
 
-        :param msg: The message received sent by Kraken via the websocket connection
-        :type msg: dict | list
-        """
-        if self.__callback is not None:
-            await self.__callback(msg)
-        else:
-            self.LOG.warning("Received event but no callback is defined.")
-            print(msg)
+        if raw:
+            await socket.send(json.dumps(message))
+            return
 
-    async def subscribe(
-        self: "KrakenSpotWSClient", subscription: dict, pair: List[str] = None
+        if private and "subscription" in message:
+            message["subscription"]["token"] = self._priv_conn.ws_conn_details["token"]
+        elif private:
+            message["token"] = self._priv_conn.ws_conn_details["token"]
+        await socket.send(json.dumps(message))
+
+    async def subscribe(  # pylint: disable=arguments-differ
+        self: KrakenSpotWSClient,
+        subscription: dict,
+        pair: Optional[List[str]] = None,
     ) -> None:
         """
         Subscribe to a channel
 
         Success or failures are sent over the websocket connection and can be
         received via the on_message callback function.
 
-        When accessing private endpoints and subscription feeds that need authentication
-        make sure, that the ``Access WebSockets API`` API key permission is set
-        in the users Kraken account.
+        When accessing private endpoints and subscription feeds that need
+        authentication make sure, that the ``Access WebSockets API`` API key
+        permission is set in the users Kraken account.
 
         - https://docs.kraken.com/websockets/#message-subscribe
 
         :param subscription: The subscription message
         :type subscription: dict
         :param pair: The pair to subscribe to
-        :type pair: List[str] | None, optional
+        :type pair: list[str], optional
 
-        Initialize your client as described in :class:`kraken.spot.KrakenSpotWSClient` to
-        run the following example:
+        Initialize your client as described in
+        :class:`kraken.spot.KrakenSpotWSClient` to run the following example:
 
         .. code-block:: python
             :linenos:
-            :caption: Spot Websocket: Subscribe to a websocket feed
+            :caption: Spot Websocket v1: Subscribe to a websocket feed
 
-            >>> await bot.subscribe(
+            >>> await client.subscribe(
             ...     subscription={"name": ticker},
             ...     pair=["XBTUSD", "DOT/EUR"]
             ... )
         """
 
         if "name" not in subscription:
             raise AttributeError('Subscription requires a "name" key."')
-        private: bool = bool(subscription["name"] in self.private_sub_names)
+        private: bool = bool(subscription["name"] in self.private_channel_names)
 
         payload: dict = {"event": "subscribe", "subscription": subscription}
         if pair is not None:
             if not isinstance(pair, list):
-                raise ValueError(
-                    'Parameter pair must be type of List[str] (e.g. pair=["XBTUSD"])'
+                raise TypeError(
+                    'Parameter pair must be type of list[str] (e.g. pair=["XBTUSD"])',
                 )
             payload["pair"] = pair
 
         if private:  # private == without pair
-            if not self.__is_auth:
-                raise ValueError(
-                    "Cannot subscribe to private feeds without valid credentials!"
+            if not self._is_auth:
+                raise KrakenException.KrakenAuthenticationError(
+                    "Cannot subscribe to private feeds without valid credentials!",
                 )
             if pair is not None:
                 raise ValueError(
-                    "Cannot subscribe to private endpoint with specific pair!"
+                    "Cannot subscribe to private endpoint with specific pair!",
                 )
-            await self._priv_conn.send_message(payload, private=True)
+            await self.send_message(payload, private=True)
 
         elif pair is not None:  # public with pair
             for symbol in pair:
                 sub = deepcopy(payload)
                 sub["pair"] = [symbol]
-                await self._pub_conn.send_message(sub, private=False)
+                await self.send_message(sub, private=False)
 
         else:
-            await self._pub_conn.send_message(payload, private=False)
-
-    async def unsubscribe(
-        self: "KrakenSpotWSClient", subscription: dict, pair: Optional[List[str]] = None
+            raise ValueError(
+                "At least one pair must be specified when subscribing to public feeds.",
+            )
+            # Currently there is no possibility to public subscribe without a
+            # pair (July 2023).
+            # await self.send_message(payload, private=False)
+
+    async def unsubscribe(  # pylint: disable=arguments-differ
+        self: KrakenSpotWSClient,
+        subscription: dict,
+        pair: Optional[List[str]] = None,
     ) -> None:
         """
-        Unsubscribe from a topic
+        Unsubscribe from a feed
 
-        Success or failures are sent over the websocket connection and can be
-        received via the on_message callback function.
+        Success or failures are sent via the websocket connection and can be
+        received via the on_message or callback function.
 
-        When accessing private endpoints and subscription feeds that need authentication
-        make sure, that the ``Access WebSockets API`` API key permission is set
-        in the users Kraken account.
+        When accessing private endpoints and subscription feeds that need
+        authentication make sure, that the ``Access WebSockets API`` API key
+        permission is set in the users Kraken account.
 
         - https://docs.kraken.com/websockets/#message-unsubscribe
 
         :param subscription: The subscription to unsubscribe from
         :type subscription: dict
         :param pair: The pair or list of pairs to unsubscribe
-        :type pair: List[str], optional
+        :type pair: list[str], optional
 
-        Initialize your client as described in :class:`kraken.spot.KrakenSpotWSClient` to
-        run the following example:
+        Initialize your client as described in
+        :class:`kraken.spot.KrakenSpotWSClient` to run the following example:
 
         .. code-block:: python
             :linenos:
-            :caption: Spot Websocket: Unsubscribe from a websocket feed
+            :caption: Spot Websocket v1: Unsubscribe from a websocket feed
 
-            >>> await bot.unsubscribe(
+            >>> await client.unsubscribe(
             ...     subscription={"name": ticker},
             ...     pair=["XBTUSD", "DOT/EUR"]
             ... )
         """
         if "name" not in subscription:
-            raise AttributeError('Subscription requires a "name" key."')
-        private: bool = bool(subscription["name"] in self.private_sub_names)
+            raise AttributeError('Subscription requires a "name" key.')
+        private: bool = bool(subscription["name"] in self.private_channel_names)
 
         payload: dict = {"event": "unsubscribe", "subscription": subscription}
         if pair is not None:
             if not isinstance(pair, list):
-                raise ValueError(
-                    'Parameter pair must be type of List[str] (e.g. pair=["XBTUSD"])'
+                raise TypeError(
+                    'Parameter pair must be type of list[str] (e.g. pair=["XBTUSD"])',
                 )
             payload["pair"] = pair
 
         if private:  # private == without pair
-            if not self.__is_auth:
-                raise ValueError(
-                    "Cannot unsubscribe from private feeds without valid credentials!"
+            if not self._is_auth:
+                raise KrakenException.KrakenAuthenticationError(
+                    "Cannot unsubscribe from private feeds without valid credentials!",
                 )
             if pair is not None:
                 raise ValueError(
-                    "Cannot unsubscribe from private endpoint with specific pair!"
+                    "Cannot unsubscribe from private endpoint with specific pair!",
                 )
-            await self._priv_conn.send_message(payload, private=True)
+            await self.send_message(payload, private=True)
 
         elif pair is not None:  # public with pair
             for symbol in pair:
                 sub = deepcopy(payload)
                 sub["pair"] = [symbol]
-                await self._pub_conn.send_message(sub, private=False)
+                await self.send_message(sub, private=False)
 
         else:
-            await self._pub_conn.send_message(payload, private=False)
-
-    @property
-    def private_sub_names(self: "KrakenSpotWSClient") -> List[str]:
-        """
-        Returns the private subscription names
-
-        :return: List of private subscription names (``ownTrades``, ``openOrders``)
-        :rtype: List[str]
-        """
-        return ["ownTrades", "openOrders"]
+            raise ValueError(
+                "At least one pair must be specified when unsubscribing "
+                "from public feeds.",
+            )
+            # Currently there is no possibility to public unsubscribe without a
+            # pair (July 2023).
+            # await self.send_message(payload, private=False)
 
     @property
-    def public_sub_names(self: "KrakenSpotWSClient") -> List[str]:
+    def public_channel_names(self: KrakenSpotWSClient) -> List[str]:
         """
         Returns the public subscription names
 
         :return: List of public subscription names (``ticker``,
-         ``spread``, ``book``, ``ohlc``, ``trade``, ``*``)
-        :rtype: List[str]
+            ``spread``, ``book``, ``ohlc``, ``trade``, ``*``)
+        :rtype: list[str]
         """
         return ["ticker", "spread", "book", "ohlc", "trade", "*"]
 
     @property
-    def active_public_subscriptions(
-        self: "KrakenSpotWSClient",
-    ) -> Union[List[dict], Any]:
-        """
-        Returns the active public subscriptions
-
-        :return: List of active public subscriptions
-        :rtype: Union[List[dict], Any]
-        :raises ConnectionError: If there is no public connection.
-        """
-        if self._pub_conn is not None:
-            return self._pub_conn.subscriptions
-        raise ConnectionError("Public connection does not exist!")
-
-    @property
-    def active_private_subscriptions(
-        self: "KrakenSpotWSClient",
-    ) -> Union[List[dict], Any]:
+    def private_channel_names(self: KrakenSpotWSClient) -> List[str]:
         """
-        Returns the active private subscriptions
-
-        :return: List of active private subscriptions
-        :rtype: Union[List[dict], Any]
-        :raises ConnectionError: If there is no private connection
-        """
-        if self._priv_conn is not None:
-            return self._priv_conn.subscriptions
-        raise ConnectionError("Private connection does not exist!")
-
-    async def __aenter__(self: "KrakenSpotWSClient") -> "KrakenSpotWSClient":
-        return self
-
-    async def __aexit__(self, *exc: tuple, **kwargs: dict) -> None:
-        pass
-
-    def get_ws_token(self: "KrakenSpotWSClient") -> dict:
-        """
-        Get the authentication token to establish the authenticated
-        websocket connection.
-
-        - https://docs.kraken.com/rest/#tag/Websockets-Authentication
+        Returns the private subscription names
 
-        :returns: The authentication token
-        :rtype: dict
+        :return: List of private subscription names (``ownTrades``,
+            ``openOrders``)
+        :rtype: list[str]
         """
-        return self._request(  # type: ignore[return-value]
-            "POST", "/private/GetWebSocketsToken"
-        )
+        return ["ownTrades", "openOrders"]
 
     @ensure_string("oflags")
-    async def create_order(
-        self: "KrakenSpotWSClient",
+    async def create_order(  # noqa: PLR0912 PLR0913
+        self: KrakenSpotWSClient,
         ordertype: str,
         side: str,
         pair: str,
         volume: Union[str, int, float],
         price: Optional[Union[str, int, float]] = None,
         price2: Optional[Union[str, int, float]] = None,
         truncate: bool = False,
@@ -382,97 +399,108 @@
         close_price: Optional[Union[str, int, float]] = None,
         close_price2: Optional[Union[str, int, float]] = None,
         timeinforce: Optional[Union[str, int]] = None,
     ) -> None:
         """
         Create an order and submit it.
 
-        Requires the ``Access WebSockets API`` and ``Create and modify orders`` API key permissions.
+        Requires the ``Access WebSockets API`` and ``Create and modify orders``
+        API key permissions.
 
         - https://docs.kraken.com/websockets/#message-addOrder
 
-        :param ordertype: The type of order, one of: ``limit``, ``market`` ``stop-loss``,
-            ``take-profit``, ``stop-loss-limit``, ``settle-position``, ``take-profit-limit``
-            (see: https://support.kraken.com/hc/en-us/sections/200577136-Order-types)
+        :param ordertype: The type of order, one of: ``limit``, ``market``,
+            ``stop-loss``, ``take-profit``, ``stop-loss-limit``,
+            ``settle-position``, ``take-profit-limit`` (see:
+            https://support.kraken.com/hc/en-us/sections/200577136-Order-types)
         :type ordertype: str
         :param side: The side - one of ``buy``, ``sell``
         :type side: str
         :param pair: The asset pair to trade
         :type pair: str
         :param volume: The volume of the order that is being created
         :type volume: str | int | float
-        :param price: The limit price for ``limit`` orders or the trigger price for orders with
-            ``ordertype`` one of ``stop-loss``, ``stop-loss-limit``, ``take-profit``, and ``take-profit-limit``
+        :param price: The limit price for ``limit`` orders or the trigger price
+            for orders with ``ordertype`` one of ``stop-loss``,
+            ``stop-loss-limit``, ``take-profit``, and ``take-profit-limit``
         :type price: str | int | float, optional
-        :param price2: The second price for ``stop-loss-limit`` and ``take-profit-limit``
-            orders (see the referenced Kraken documentation for more information)
+        :param price2: The second price for ``stop-loss-limit`` and
+            ``take-profit-limit`` orders (see the referenced Kraken
+            documentation for more information)
         :type price2: str | int | float, optional
-        :param truncate: If enabled: round the ``price`` and ``volume`` to Kraken's
-            maximum allowed decimal places. See https://support.kraken.com/hc/en-us/articles/4521313131540
+        :param truncate: If enabled: round the ``price`` and ``volume`` to
+            Kraken's maximum allowed decimal places. See
+            https://support.kraken.com/hc/en-us/articles/4521313131540
             fore more information about decimals.
         :type truncate: bool, optional
         :param leverage: The leverage
         :type leverage: str | int | float, optional
-        :param oflags: Order flags like ``post``, ``fcib``, ``fciq``, ``nomp``, ``viqc``
-            (see the referenced Kraken documentation for more information)
-        :type oflags: str | List[str], optional
-        :param starttm: Unix timestamp or seconds defining the start time (default: ``"0"``)
+        :param oflags: Order flags like ``post``, ``fcib``, ``fciq``, ``nomp``,
+            ``viqc`` (see the referenced Kraken documentation for more
+            information)
+        :type oflags: str | list[str], optional
+        :param starttm: Unix timestamp or seconds defining the start time
+            (default: ``"0"``)
         :type starttm: str | int, optional
-        :param expiretim: Unix timestamp or time in seconds defining the expiration of
-            the order (default: ``"0"`` - i.e., no expiration)
+        :param expiretim: Unix timestamp or time in seconds defining the
+            expiration of the order (default: ``"0"`` - i.e., no expiration)
         :type expiretim: str
-        :param deadline: RFC3339 timestamp + {0..60} seconds that defines when the matching
-            engine should reject the order.
+        :param deadline: RFC3339 timestamp + {0..60} seconds that defines when
+            the matching engine should reject the order.
         :type deadline: str
         :param userref: User reference id for example to group orders
         :type userref: int
-        :param validate: Validate the order without placing on the market (default: ``False``)
+        :param validate: Validate the order without placing on the market
+            (default: ``False``)
         :type validate: bool, optional
-        :param close_ordertype:  Conditional close order type, one of: ``limit``, ``stop-loss``,
-            ``take-profit``, ``stop-loss-limit``, ``take-profit-limit``
+        :param close_ordertype:  Conditional close order type, one of:
+            ``limit``, ``stop-loss``, ``take-profit``, ``stop-loss-limit``,
+            ``take-profit-limit``
         :type close_ordertype: str, optional
         :param close_price: Conditional close price
         :type close_price: str | int | float, optional
         :param close_price2: Second conditional close price
         :type close_price2: str | int | float, optional
-        :param timeinforce: How long the order remains in the orderbook, one of: ``GTC``, ``IOC``,
-            ``GTD`` (see the referenced Kraken documentation for more information)
+        :param timeinforce: How long the order remains in the orderbook, one of:
+            ``GTC``, ``IOC``, ``GTD`` (see the referenced Kraken documentation
+            for more information)
         :type timeinforce: str, optional
+        :raises KrakenAuthenticationError: If the websocket is not connected or
+            the connection is not authenticated
         :raises ValueError: If input is not correct
         :rtype: None
 
-        Initialize your client as described in :class:`kraken.spot.KrakenSpotWSClient` to
-        run the following example:
+        Initialize your client as described in
+        :class:`kraken.spot.KrakenSpotWSClient` to run the following example:
 
         .. code-block:: python
             :linenos:
             :caption: Spot Websocket: Create an order
 
-            >>> await auth_bot.create_order(
+            >>> await client_auth.create_order(
             ...     ordertype="market",
             ...     pair="XBTUSD",
             ...     side="buy",
             ...     volume=0.001
             ... )
-            >>> await auth_bot.create_order(
+            >>> await client_auth.create_order(
             ...     ordertype="limit",
             ...     side="buy",
             ...     pair="XBTUSD",
             ...     volume=0.02,
             ...     price=23000,
             ...     expiretm=120,
             ...     oflags=["post", "fcib"]
             ... )
 
         """
-        if not self._priv_conn:
-            logging.warning("Websocket not connected!")
-            return
-        if not self._priv_conn.is_auth:
-            raise ValueError("Cannot create_order on public websocket client!")
+        if not self._priv_conn or not self._priv_conn.is_auth:
+            raise KrakenException.KrakenAuthenticationError(
+                "Can't place order - Authenticated websocket not connected!",
+            )
 
         payload: dict = {
             "event": "addOrder",
             "ordertype": str(ordertype),
             "type": str(side),
             "pair": str(pair),
             "volume": str(volume)
@@ -487,15 +515,16 @@
                 else Trade().truncate(amount=price, amount_type="price", pair=pair)
             )
         if defined(price2):
             payload["price2"] = str(price2)
         if defined(oflags):
             if not isinstance(oflags, str):
                 raise ValueError(
-                    "oflags must be a comma delimited list of order flags as str. Available flags: {viqc, fcib, fciq, nompp, post}"
+                    "oflags must be a comma delimited list of order flags as "
+                    "str. Available flags: {viqc, fcib, fciq, nompp, post}",
                 )
             payload["oflags"] = oflags
         if defined(starttm):
             payload["starttm"] = str(starttm)
         if defined(expiretm):
             payload["expiretm"] = str(expiretm)
         if defined(deadline):
@@ -509,81 +538,85 @@
         if defined(close_price):
             payload["close[price]"] = str(close_price)
         if defined(close_price2):
             payload["close[price2]"] = str(close_price2)
         if defined(timeinforce):
             payload["timeinforce"] = timeinforce
 
-        await self._priv_conn.send_message(msg=payload, private=True)
+        await self.send_message(message=payload, private=True)
 
     @ensure_string("oflags")
-    async def edit_order(
-        self: "KrakenSpotWSClient",
+    async def edit_order(  # noqa: PLR0913
+        self: KrakenSpotWSClient,
         orderid: str,
         reqid: Optional[Union[str, int]] = None,
         pair: Optional[str] = None,
         price: Optional[Union[str, int, float]] = None,
         price2: Optional[Union[str, int, float]] = None,
         truncate: bool = False,
         volume: Optional[Union[str, int, float]] = None,
         oflags: Optional[Union[str, List[str]]] = None,
         newuserref: Optional[Union[str, int]] = None,
         validate: bool = False,
     ) -> None:
         """
         Edit an open order that was placed on the Spot market.
 
-        Requires the ``Access WebSockets API`` and ``Create and modify orders`` API key permissions.
+        Requires the ``Access WebSockets API`` and ``Create and modify orders``
+        API key permissions.
 
         - https://docs.kraken.com/websockets/#message-editOrder
 
         :param orderId: The orderId of the order to edit
         :type orderId: str
         :param reqid: Filter by reqid
         :type reqid: str | int, optional
         :param pair: Filter by pair
         :type pair: str, optional
         :param price: Set a new price
         :type price: str | int | float, optional
         :param price2: Set a new second price
         :type price2: str | int | float, optional
         :param truncate: If enabled: round the ``price`` and ``volume`` to Kraken's
-            maximum allowed decimal places. See https://support.kraken.com/hc/en-us/articles/4521313131540
-            fore more information about decimals.
+            maximum allowed decimal places. See
+            https://support.kraken.com/hc/en-us/articles/4521313131540 fore more
+            information about decimals.
         :type truncate: bool, optional
         :param volume: Set a new volume
         :type volume: str | int | float, optional
         :param oflags: Set new oflags (overwrite old ones)
-        :type oflags: str | List[str], optional
+        :type oflags: str | list[str], optional
         :param newuserref: Set a new user reference id
         :type newuserref: str | int, optional
-        :param validate: Validate the input without applying the changes (default: ``False``)
+        :param validate: Validate the input without applying the changes
+            (default: ``False``)
         :type validate: bool, optional
+        :raises KrakenAuthenticationError: If the websocket is not connected or
+            the connection is not authenticated
         :raises ValueError: If input is not correct
         :rtype: None
 
-        Initialize your client as described in :class:`kraken.spot.KrakenSpotWSClient` to
-        run the following example:
+        Initialize your client as described in
+        :class:`kraken.spot.KrakenSpotWSClient` to run the following example:
 
         .. code-block:: python
             :linenos:
             :caption: Spot Websocket: Edit an order
 
-            >>> await auth_bot.edit_order(
+            >>> await client_auth.edit_order(
             ...     orderId="OBGFYP-XVQNL-P4GMWF",
             ...     volume=0.75,
             ...     pair="XBTUSD",
             ...     price=20000
             ... )
         """
-        if not self._priv_conn:
-            logging.warning("Websocket not connected!")
-            return
-        if not self._priv_conn.is_auth:
-            raise ValueError("Cannot edit_order on public websocket client!")
+        if not self._priv_conn or not self._priv_conn.is_auth:
+            raise KrakenException.KrakenAuthenticationError(
+                "Can't edit order - Authenticated websocket not connected!",
+            )
 
         payload: dict = {
             "event": "editOrder",
             "orderid": orderid,
             "validate": str(validate),
         }
         if defined(reqid):
@@ -605,102 +638,109 @@
                 else Trade().truncate(amount=volume, amount_type="volume", pair=pair)
             )
         if defined(oflags):
             payload["oflags"] = oflags
         if defined(newuserref):
             payload["newuserref"] = str(newuserref)
 
-        await self._priv_conn.send_message(msg=payload, private=True)
+        await self.send_message(message=payload, private=True)
 
-    async def cancel_order(self: "KrakenSpotWSClient", txid: List[str]) -> None:
+    async def cancel_order(self: KrakenSpotWSClient, txid: List[str]) -> None:
         """
         Cancel a specific order or a list of orders.
 
-        Requires the ``Access WebSockets API`` and ``Cancel/close orders`` API key permissions.
+        Requires the ``Access WebSockets API`` and ``Cancel/close orders`` API
+        key permissions.
 
         - https://docs.kraken.com/websockets/#message-cancelOrder
 
         :param txid: A single or multiple transaction ids as list
-        :type txid: List[str]
-        :raises ValueError: If the websocket is not connected or the connection is not authenticated
+        :type txid: list[str]
+        :raises KrakenAuthenticationError: If the websocket is not connected or
+            the connection is not authenticated
         :return: None
 
-        Initialize your client as described in :class:`kraken.spot.KrakenSpotWSClient` to
-        run the following example:
+        Initialize your client as described in
+        :class:`kraken.spot.KrakenSpotWSClient` to run the following example:
 
         .. code-block:: python
             :linenos:
             :caption: Spot Websocket: Cancel an order
 
-            >>> await auth_bot.cancel_order(txid=["OBGFYP-XVQNL-P4GMWF"])
+            >>> await client_auth.cancel_order(txid=["OBGFYP-XVQNL-P4GMWF"])
         """
-        if not self._priv_conn:
-            logging.warning("Websocket not connected!")
-            return
-        if not self._priv_conn.is_auth:
-            raise ValueError("Cannot cancel_order on public websocket client!")
-        await self._priv_conn.send_message(
-            msg={"event": "cancelOrder", "txid": txid}, private=True
+        if not self._priv_conn or not self._priv_conn.is_auth:
+            raise KrakenException.KrakenAuthenticationError(
+                "Can't cancel order - Authenticated websocket not connected!",
+            )
+        await self.send_message(
+            message={"event": "cancelOrder", "txid": txid},
+            private=True,
         )
 
-    async def cancel_all_orders(self: "KrakenSpotWSClient") -> None:
+    async def cancel_all_orders(self: KrakenSpotWSClient) -> None:
         """
         Cancel all open Spot orders.
 
-        Requires the ``Access WebSockets API`` and ``Cancel/close orders`` API key permissions.
+        Requires the ``Access WebSockets API`` and ``Cancel/close orders`` API
+        key permissions.
 
         - https://docs.kraken.com/websockets/#message-cancelAll
 
-        :raises ValueError: If the websocket is not connected or the connection is not authenticated
+        :raises KrakenAuthenticationError: If the websocket is not connected or
+            the connection is not authenticated
         :return: None
 
-        Initialize your client as described in :class:`kraken.spot.KrakenSpotWSClient` to
-        run the following example:
+        Initialize your client as described in
+        :class:`kraken.spot.KrakenSpotWSClient` to run the following example:
 
         .. code-block:: python
             :linenos:
             :caption: Spot Websocket: Cancel all Orders
 
-            >>> await auth_bot.cancel_all_orders()
+            >>> await client_auth.cancel_all_orders()
         """
-
-        if not self._priv_conn:
-            logging.warning("Websocket not connected!")
-            return
-        if not self._priv_conn.is_auth:
-            raise ValueError("Cannot use cancel_all_orders on public websocket client!")
-        await self._priv_conn.send_message(msg={"event": "cancelAll"}, private=True)
+        if not self._priv_conn or not self._priv_conn.is_auth:
+            raise KrakenException.KrakenAuthenticationError(
+                "Can't cancel all orders - Authenticated websocket not connected!",
+            )
+        await self.send_message(message={"event": "cancelAll"}, private=True)
 
     async def cancel_all_orders_after(
-        self: "KrakenSpotWSClient", timeout: int = 0
+        self: KrakenSpotWSClient,
+        timeout: int = 0,
     ) -> None:
         """
         Set a Death Man's Switch
 
-        Requires the ``Access WebSockets API`` and ``Cancel/close orders`` API key permissions.
+        Requires the ``Access WebSockets API`` and ``Cancel/close orders`` API
+        key permissions.
 
         - https://docs.kraken.com/websockets/#message-cancelAllOrdersAfter
 
-        :param timeout: Set the timeout in seconds to cancel the orders after, set to ``0`` to reset.
+        :param timeout: Set the timeout in seconds to cancel the orders after,
+            set to ``0`` to reset.
         :type timeout: int
-        :raises ValueError: If the websocket is not connected or the connection is not authenticated
+        :raises KrakenAuthenticationError: If the websocket is not connected or
+            the connection is not authenticated
         :return: None
 
-        Initialize your client as described in :class:`kraken.spot.KrakenSpotWSClient` to
-        run the following example:
+        Initialize your client as described in
+        :class:`kraken.spot.KrakenSpotWSClient` to run the following example:
 
         .. code-block:: python
             :linenos:
             :caption: Spot Websocket: Death Man's Switch
 
-            >>> await auth_bot.cancel_all_orders_after(timeout=60)
+            >>> await client_auth.cancel_all_orders_after(timeout=60)
         """
-        if not self._priv_conn:
-            logging.warning("Websocket not connected!")
-            return
-        if not self._priv_conn.is_auth:
-            raise ValueError(
-                "Cannot use cancel_all_orders_after on public websocket client!"
+        if not self._priv_conn or not self._priv_conn.is_auth:
+            raise KrakenException.KrakenAuthenticationError(
+                "Can't cancel all orders after - Authenticated websocket not connected!",
             )
-        await self._priv_conn.send_message(
-            msg={"event": "cancelAllOrdersAfter", "timeout": timeout}, private=True
+        await self.send_message(
+            message={"event": "cancelAllOrdersAfter", "timeout": timeout},
+            private=True,
         )
+
+
+__all__ = ["KrakenSpotWSClient"]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `python-kraken-sdk-1.5.0/python_kraken_sdk.egg-info/PKG-INFO` & `python-kraken-sdk-1.6.0/python_kraken_sdk.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-kraken-sdk
-Version: 1.5.0
+Version: 1.6.0
 Summary: Collection of REST and websocket clients to interact with the Kraken cryptocurrency exchange.
 Author-email: Benjamin Thomas Schwertfeger <contact@b-schwertfeger.de>
 License: GNU GENERAL PUBLIC LICENSE
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
         Everyone is permitted to copy and distribute verbatim copies
@@ -622,16 +622,16 @@
         an absolute waiver of all civil liability in connection with the
         Program, unless a warranty or assumption of liability accompanies a
         copy of the Program in return for a fee.
         
                              END OF TERMS AND CONDITIONS
         
             The python-kraken-sdk serves as a collection of REST and websocket
-            clients to interact with the Kraken cryptocurrency exchange to
-            access the Spot and Futures API.
+            clients to interact with the Kraken cryptocurrency exchange using it's Spot
+            and Futures APIs.
             Copyright (C) 2023 Benjamin Thomas Schwertfeger
         
             This program is free software: you can redistribute it and/or modify
             it under the terms of the GNU General Public License as published by
             the Free Software Foundation, either version 3 of the License, or
             (at your option) any later version.
         
@@ -666,276 +666,327 @@
 Classifier: Operating System :: Unix
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: examples
 License-File: LICENSE
 
-<h1 align="center">Futures and Spot Websocket and REST API Python SDK for the Kraken Cryptocurrency Exchange 🐙</h1>
+<h1 align="center">Futures and Spot - REST and Websocket API Python SDK for the Kraken Cryptocurrency Exchange 🐙</h1>
 
 <div align="center">
 
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/btschwertfeger/python-kraken-sdk)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-orange.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Generic badge](https://img.shields.io/badge/python-3.7_|_3.8_|_3.9_|_3.10_|_3.11-blue.svg)](https://shields.io/)
 [![Downloads](https://static.pepy.tech/personalized-badge/python-kraken-sdk?period=total&units=abbreviation&left_color=grey&right_color=orange&left_text=downloads)](https://pepy.tech/project/python-kraken-sdk)
 
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Typing](https://img.shields.io/badge/typing-mypy-informational)](https://mypy-lang.org/)
 [![CodeQL](https://github.com/btschwertfeger/python-kraken-sdk/actions/workflows/codeql.yaml/badge.svg?branch=master)](https://github.com/btschwertfeger/python-kraken-sdk/actions/workflows/codeql.yaml)
 [![CI/CD](https://github.com/btschwertfeger/python-kraken-sdk/actions/workflows/cicd.yaml/badge.svg?branch=master)](https://github.com/btschwertfeger/python-kraken-sdk/actions/workflows/cicd.yaml)
 [![codecov](https://codecov.io/gh/btschwertfeger/python-kraken-sdk/branch/master/badge.svg)](https://app.codecov.io/gh/btschwertfeger/python-kraken-sdk)
 
 ![release](https://shields.io/github/release-date/btschwertfeger/python-kraken-sdk)
 [![release](https://img.shields.io/pypi/v/python-kraken-sdk)](https://pypi.org/project/python-kraken-sdk/)
 [![DOI](https://zenodo.org/badge/510751854.svg)](https://zenodo.org/badge/latestdoi/510751854)
 [![Documentation Status stable](https://readthedocs.org/projects/python-kraken-sdk/badge/?version=stable)](https://python-kraken-sdk.readthedocs.io/en/stable)
 
 </div>
 
-> ⚠️ This is an unofficial collection of REST and websocket clients for Spot and Futures trading on the Kraken cryptocurrency exchange using Python. Payward Ltd. and Kraken are in no way associated with the authors of this module and documentation.
+> ⚠️ This is an unofficial collection of REST and websocket clients for Spot and
+> Futures trading on the Kraken cryptocurrency exchange using Python. Payward
+> Ltd. and Kraken are in no way associated with the authors of this module and
+> documentation.
 
 ---
 
 ## 📌 Disclaimer
 
-There is no guarantee that this software will work flawlessly at this or later times. Of course, no responsibility is taken for possible profits or losses. This software probably has some errors in it, so use it at your own risk. Also no one should be motivated or tempted to invest assets in speculative forms of investment. By using this software you release the authors from any liability regarding the use of this software.
+There is no guarantee that this software will work flawlessly at this or later
+times. Of course, no responsibility is taken for possible profits or losses.
+This software probably has some errors in it, so use it at your own risk. Also
+no one should be motivated or tempted to invest assets in speculative forms of
+investment. By using this software you release the authors from any liability
+regarding the use of this software.
 
 ---
 
 ## Features
 
-Clients:
+Available Clients:
 
 - Spot REST Clients
-- Spot Websocket Client
+- Spot Websocket Clients (Websocket API v1 and v2)
 - Spot Orderbook Client
 - Futures REST Clients
 - Futures Websocket Client
 
 General:
 
-- access both public and private endpoints
+- access both public and private, REST and websocket endpoints
 - responsive error handling and custom exceptions
 - extensive example scripts (see `/examples` and `/tests`)
 - tested using the [pytest](https://docs.pytest.org/en/7.3.x/) framework
 - releases are permanently archived at [Zenodo](https://zenodo.org/badge/latestdoi/510751854)
 
 Documentation:
 
-- Stable: [https://python-kraken-sdk.readthedocs.io/en/stable](https://python-kraken-sdk.readthedocs.io/en/stable)
-- Latest: [https://python-kraken-sdk.readthedocs.io/en/latest](https://python-kraken-sdk.readthedocs.io/en/latest)
+- [https://python-kraken-sdk.readthedocs.io/en/stable](https://python-kraken-sdk.readthedocs.io/en/stable)
+- [https://python-kraken-sdk.readthedocs.io/en/latest](https://python-kraken-sdk.readthedocs.io/en/latest)
 
 ---
 
 ## ❗️ Attention
 
-**ONLY** tagged releases are available at PyPI. So the content of the master may not match with the content of the latest release. - Please have a look at the release specific READMEs and changelogs.
+**ONLY** tagged releases are available at PyPI. So the content of the master may
+not match with the content of the latest release. - Please have a look at the
+release specific READMEs and changelogs.
 
 ---
 
 ## Table of Contents
 
 - [ Installation and setup ](#installation)
-- [ Spot Client Example Usage ](#spotusage)
+- [ Spot Clients ](#spotusage)
   - [REST API](#spotrest)
-  - [Websockets](#spotws)
-- [ Futures Client Example Usage ](#futuresusage)
+  - [Websocket API V2](#spotws)
+- [ Futures Clients ](#futuresusage)
   - [REST API](#futuresrest)
-  - [Websockets](#futuresws)
+  - [Websocket API](#futuresws)
 - [ Troubleshooting ](#trouble)
 - [ Contributions ](#contribution)
 - [ Notes ](#notes)
 - [ References ](#references)
 
 ---
 
 <a name="installation"></a>
 
 # 🛠 Installation and setup
 
-### 1. Install the Python module:
+### 1. Install the package into the desired environment
 
 ```bash
 python3 -m pip install python-kraken-sdk
 ```
 
-### 2. Register at Kraken and generate API Keys:
+### 2. Register at [Kraken](https://www.kraken.com) and generate API keys
 
 - Spot Trading: https://www.kraken.com/u/security/api
 - Futures Trading: https://futures.kraken.com/trade/settings/api (see _[help](https://docs.futures.kraken.com/#introduction-generate-api-keys)_)
 - Futures Sandbox: https://demo-futures.kraken.com/settings/api
 
 ### 3. Start using the provided example scripts
 
 ### 4. Error handling
 
-If any unexpected behavior occurs, please check <b style="color: yellow">your API permissions</b>, <b style="color: yellow">rate limits</b>, update the python-kraken-sdk, see the [Troubleshooting](#trouble) section, and if the error persists please open an issue.
+If any unexpected behavior occurs, please check <b style="color: yellow">your
+API permissions</b>, <b style="color: yellow">rate limits</b>, update the
+python-kraken-sdk, see the [Troubleshooting](#trouble) section, and if the error
+persists please open an issue.
 
 ---
 
 <a name="spotusage"></a>
 
-# 📍 Spot Client Example Usage
+# 📍 Spot Clients
 
-A template Spot trading bot using both websocket and REST clients can be found in `/examples/spot_trading_bot_template.py`.
+A template for Spot trading using both websocket and REST clients can be
+found in `examples/spot_trading_bot_template_v2.py`.
 
-For those who need a realtime order book - a script that demonstrates how to maintain a valid order book can be found here: `/examples/spot_orderbook.py`.
+For those who need a realtime order book - a script that demonstrates how to
+maintain a valid order book using the Orderbook client can be found in
+`examples/spot_orderbook.py`.
 
 <a name="spotrest"></a>
 
 ## Spot REST API
 
-... can be found in `/examples/spot_examples.py`
+The Kraken Spot REST API offers many endpoints for almost every use-case. The
+python-kraken-sdk aims to provide all of them - split in User, Market,
+Trade, Funding and Staking related clients.
+
+The following code block demonstrates how to use some of them. More examples
+can be found in `examples/spot_examples.py`.
 
 ```python
 from kraken.spot import User, Market, Trade, Funding, Staking
 
 def main():
     key = "kraken-public-key"
     secret = "kraken-secret-key"
 
     # ____USER________________________
     user = User(key=key, secret=secret)
     print(user.get_account_balance())
     print(user.get_open_orders())
-    # ...
+    # …
 
     # ____MARKET____
     market = Market()
     print(market.get_ticker(pair="BTCUSD"))
-    # ...
+    # …
 
     # ____TRADE_________________________
     trade = Trade(key=key, secret=secret)
     print(trade.create_order(
          ordertype="limit",
          side="buy",
          volume=1,
          pair="BTC/EUR",
          price=20000
     ))
-    # ...
+    # …
 
     # ____FUNDING___________________________
     funding = Funding(key=key, secret=secret)
     print(
         funding.withdraw_funds(
             asset="DOT", key="MyPolkadotWallet", amount=200
         )
     )
     print(funding.cancel_withdraw(asset="DOT", refid="<some id>"))
-    # ...
+    # …
 
     # ____STAKING___________________________
     staking = Staking(key=key, secret=secret)
     print(staking.list_stakeable_assets())
     print(
         staking.stake_asset(
             asset="DOT", amount=20, method="polkadot-staked"
         )
     )
-    # ...
+    # …
 
 if __name__ == "__main__":
     main()
 ```
 
 <a name="spotws"></a>
 
-## Websockets
+## Spot Websocket API V2
+
+Kraken offers two versions of their websocket API (V1 and V2). Since V2 is
+offers more possibilities, is way faster and easier to use, only those examples
+are shown below. For using the websocket API V1 please have a look into the
+`examples/spot_ws_examples_v1.py`.
 
-... can be found in `/examples/spot_ws_examples.py`
+The documentation for both API versions can be found here:
+
+- https://docs.kraken.com/websockets
+- https://docs.kraken.com/websockets-v2
+
+Note that authenticated Spot websocket clients can also un-/subscribe from/to
+public feeds.
+
+The example below can be found in an extended way in
+`examples/spot_ws_examples_v2.py`.
 
 ```python
-import time
 import asyncio
-from kraken.spot import KrakenSpotWSClient
+from kraken.spot import KrakenSpotWSClientV2
 
-async def main()
+async def main():
+    key = "spot-api-key"
+    secret = "spot-secret-key"
 
-    key = "kraken-public-key"
-    secret = "kraken-secret-key"
+    class Client(KrakenSpotWSClientV2):
+        """Can be used to create a custom trading strategy"""
 
-    class Bot(KrakenSpotWSClient):
-        async def on_message(self, msg):
-            if isinstance(msg, dict) and "event" in msg:
-                if msg["event"] in ("pong", "heartbeat"):
-                    return
-
-            print(msg)
-            # if condition:
-            #     await self.create_order(
-            #         ordertype="limit",
-            #         side="buy",
-            #         pair="BTC/EUR",
-            #         price=20000,
-            #         volume=1
+        async def on_message(self, message):
+            """Receives the websocket messages"""
+            if message.get("method") == "pong" \
+                or message.get("channel") == "heartbeat":
+                return
+
+            print(message)
+            # here we can access lots of methods, for example to create an order:
+            # if self.is_auth:  # only if the client is authenticated …
+            #     await self.send_message(
+            #         message={
+            #             "method": "add_order",
+            #             "params": {
+            #                 "limit_price": 1234.56,
+            #                 "order_type": "limit",
+            #                 "order_userref": 123456789,
+            #                 "order_qty": 1.0,
+            #                 "side": "buy",
+            #                 "symbol": "BTC/USD",
+            #                 "validate": True,
+            #             },
+            #         }
             #     )
-            # ... it is also possible to call regular Spot REST endpoints
-            # but using the WsClient's functions is more efficient
-            # because the requests will be sent via the ws connection
-
-    # ___Public_Websocket_Feeds__
-    bot = Bot() # only use the unauthenticated client if you don't need private feeds
-    print(bot.public_sub_names) # list public subscription names
-
-    await bot.subscribe(subscription={ "name": "ticker" }, pair=["XBT/EUR", "DOT/EUR"])
-    await bot.subscribe(subscription={ "name": "spread" }, pair=["XBT/EUR", "DOT/EUR"])
-    # await bot.subscribe(subscription={ "name": "book" }, pair=["BTC/EUR"])
-    # await bot.subscribe(subscription={ "name": "book", "depth": 25}, pair=["BTC/EUR"])
-    # await bot.subscribe(subscription={ "name": "ohlc" }, pair=["BTC/EUR"])
-    # await bot.subscribe(subscription={ "name": "ohlc", "interval": 15}, pair=["XBT/EUR", "DOT/EUR"])
-    # await bot.subscribe(subscription={ "name": "trade" }, pair=["BTC/EUR"])
-    # await bot.subscribe(subscription={ "name": "*" } , pair=["BTC/EUR"])
-
-    time.sleep(2) # wait because unsubscribing is faster than subscribing ...
-    await bot.unsubscribe(subscription={ "name": "ticker" }, pair=["XBT/EUR","DOT/EUR"])
-    await bot.unsubscribe(subscription={ "name": "spread" }, pair=["XBT/EUR"])
-    await bot.unsubscribe(subscription={ "name": "spread" }, pair=["DOT/EUR"])
-    # ...
-
-    # ___Authenticated_Websocket_________
-    # when using the authenticated client, you can also subscribe to public feeds
-    auth_bot = Bot(key=key, secret=secret)
-    print(auth_bot.private_sub_names) # list private subscription names
-    await auth_bot.subscribe(subscription={ "name": "ownTrades" })
-    await auth_bot.subscribe(subscription={ "name": "openOrders" })
-
-    time.sleep(2)
-    await auth_bot.unsubscribe(subscription={ "name": "ownTrades" })
-    await auth_bot.unsubscribe(subscription={ "name": "openOrders" })
+            # … it is also possible to call regular REST endpoints
+            # but using the websocket messages is more efficient.
+            # You can also un-/subscribe here using self.subscribe/self.unsubscribe.
 
-    while True:
+    # Public/unauthenticated websocket client
+    client = Client()  # only use this one if you don't need private feeds
+
+    await client.subscribe(
+        params={"channel": "ticker", "symbol": ["BTC/USD", "DOT/USD"]}
+    )
+    await client.subscribe(
+        params={"channel": "book", "depth": 25, "symbol": ["BTC/USD"]}
+    )
+    # wait because unsubscribing is faster than unsubscribing … (just for that example)
+    await asyncio.sleep(3)
+    # print(client.active_public_subscriptions) # to list active subscriptions
+    await client.unsubscribe(
+        params={"channel": "ticker", "symbol": ["BTC/USD", "DOT/USD"]}
+    )
+    # …
+
+    # Per default, the authenticated client starts two websocket connections,
+    # one for authenticated and one for public messages. If there is no need
+    # for a public connection, it can be disabled using the ``no_public``
+    # parameter.
+    client_auth = Client(key=key, secret=secret, no_public=True)
+    await client_auth.subscribe(params={"channel": "executions"})
+
+    while not client.exception_occur and not client_auth.exception_occur:
         await asyncio.sleep(6)
+    return
+
 
 if __name__ == "__main__":
     try:
         asyncio.run(main())
     except KeyboardInterrupt:
-        # do some exception handling ...
         pass
+        # The websocket client will send {'event': 'asyncio.CancelledError'}
+        # via on_message so you can handle the behavior/next actions
+        # individually within your strategy.
 ```
 
-Note: Authenticated Spot websocket clients can also un/subscribe from/to public feeds.
-
 ---
 
 <a name="futuresusage"></a>
 
-# 📍 Futures Client Example Usage
+# 📍 Futures Clients
 
-Kraken provides a sandbox environment at https://demo-futures.kraken.com for paper trading. When using this API keys you have to set the `sandbox` parameter to `True` when instantiating the respective client.
+Kraken provides a sandbox environment at https://demo-futures.kraken.com for
+Futures paper trading. When using these API keys you have to set the `sandbox`
+parameter to `True` when instantiating the respective client.
 
-A template Futures trading bot using both websocket and REST clients can be found in `/examples/futures_trading_bot_template.py`.
+A template for Futures trading using both websocket and REST clients can be
+found in `examples/futures_trading_bot_template.py`.
+
+The Kraken Futures API documentation can be found here:
+
+- https://docs.futures.kraken.com
+- https://support.kraken.com/hc/en-us/sections/360012894412-Futures-API
 
 <a name="futuresrest"></a>
 
 ## Futures REST API
 
-The following example can be found in `/examples/futures_examples.py`.
+As the Spot API, Kraken also offers a REST API for Futures. Examples on how to
+use the python-kraken-sdk fot Futures are shown in
+`examples/futures_examples.py` and listed in a shorter ways below.
 
 ```python
 from kraken.futures import Market, User, Trade, Funding
 
 def main():
 
     key = "futures-api-key"
@@ -943,24 +994,24 @@
 
     # ____USER________________________
     user = User(key=key, secret=secret) # optional: sandbox=True
     print(user.get_wallets())
     print(user.get_open_orders())
     print(user.get_open_positions())
     print(user.get_subaccounts())
-    # ...
+    # …
 
     # ____MARKET____
     market = Market()
     print(market.get_ohlc(tick_type="trade", symbol="PI_XBTUSD", resolution="5m"))
 
     priv_market = Market(key=key, secret=secret)
     print(priv_market.get_fee_schedules_vol())
     print(priv_market.get_execution_events())
-    # ...
+    # …
 
     # ____TRADE_________________________
     trade = Trade(key=key, secret=secret)
     print(trade.get_fills())
     print(trade.create_batch_order(
         batchorder_list = [{
             "order": "send",
@@ -994,118 +1045,137 @@
             orderType="lmt",
             side="buy",
             size=1,
             limitPrice=4,
             symbol="pf_bchusd"
         )
     )
-    # ...
+    # …
 
     # ____FUNDING___________________________
     funding = Funding(key=key, secret=secret)
-    # ...
+    # …
 
 if __name__ == "__main__":
     main()
 ```
 
 <a name="futuresws"></a>
 
-## Futures Websocket Client
+## Futures Websocket API
+
+Not only REST, also the websocket API for Kraken Futures is available. Examples
+are shown below and demonstrated in `examples/futures_ws_examples.py`.
 
-The following example can be found in `/examples/futures_ws_examples.py`.
+- https://docs.futures.kraken.com/#websocket-api
+
+Note: Authenticated Futures websocket clients can also un-/subscribe from/to
+public feeds.
 
 ```python
 import asyncio
 from kraken.futures import KrakenFuturesWSClient
 
 async def main():
 
     key = "futures-api-key"
     secret = "futures-secret-key"
 
-    # ___Custom_Trading_Bot________
-    class Bot(KrakenFuturesWSClient):
+    class Client(KrakenFuturesWSClient):
 
         async def on_message(self, event):
             print(event)
-            # >> apply your trading strategy here <<
-            # you can also combine this with the Futures REST clients
 
-    # ___Public_Websocket_Feeds____
-    bot = Bot()
-    # print(bot.get_available_public_subscription_feeds())
+    # Public/unauthenticated websocket connection
+    client = Client()
 
     products = ["PI_XBTUSD", "PF_ETHUSD"]
 
     # subscribe to a public websocket feed
-    await bot.subscribe(feed="ticker", products=products)
-    # await bot.subscribe(feed="book", products=products)
-    # ...
+    await client.subscribe(feed="ticker", products=products)
+    # await client.subscribe(feed="book", products=products)
+    # …
 
     # unsubscribe from a public websocket feed
-    # await bot.unsubscribe(feed="ticker", products=products)
+    # await client.unsubscribe(feed="ticker", products=products)
 
-    # ___Authenticated_Websocket_________
-    auth_bot = Bot(key=key, secret=secret)
-    # print(auth_bot.get_available_private_subscription_feeds())
+    # Private/authenticated websocket connection (+public)
+    client_auth = Client(key=key, secret=secret)
+    # print(client_auth.get_available_private_subscription_feeds())
 
     # subscribe to a private/authenticated websocket feed
-    await auth_bot.subscribe(feed="fills")
-    await auth_bot.subscribe(feed="open_positions")
-    await auth_bot.subscribe(feed="open_orders")
-    # ...
+    await client_auth.subscribe(feed="fills")
+    await client_auth.subscribe(feed="open_positions")
+    await client_auth.subscribe(feed="open_orders")
+    # …
 
     # unsubscribe from a private/authenticated websocket feed
-    await auth_bot.unsubscribe(feed="fills")
+    await client_auth.unsubscribe(feed="fills")
 
     while True:
         await asyncio.sleep(6)
 
 if __name__ == "__main__":
     try:
         asyncio.run(main())
     except KeyboardInterrupt:
-        # do some exception handling ...
+        # do some exception handling …
         pass
 ```
 
-Note: Authenticated Futures websocket clients can also un-/subscribe from/to public feeds.
-
 ---
 
 <a name="contribution"></a>
 
 # 🆕 Contributions
 
 … are welcome! - Please have a look at [CONTRIBUTION.md](./CONTRIBUTING.md).
 
 ---
 
 <a name="trouble"></a>
 
 # 🚨 Troubleshooting
 
-- Check if you downloaded and installed the **latest version** of the python-kraken-sdk.
-- Check the **permissions of your API keys** and the required permissions on the respective endpoints.
-- If you get some Cloudflare or **rate limit errors**, please check your Kraken Tier level and maybe apply for a higher rank if required.
-- **Use different API keys for different algorithms**, because the nonce calculation is based on timestamps and a sent nonce must always be the highest nonce ever sent of that API key. Having multiple algorithms using the same keys will result in invalid nonce errors.
+- Check if you downloaded and installed the **latest version** of the
+  python-kraken-sdk.
+- Check the **permissions of your API keys** and the required permissions on the
+  respective endpoints.
+- If you get some Cloudflare or **rate limit errors**, please check your Kraken
+  Tier level and maybe apply for a higher rank if required.
+- **Use different API keys for different algorithms**, because the nonce
+  calculation is based on timestamps and a sent nonce must always be the highest
+  nonce ever sent of that API key. Having multiple algorithms using the same
+  keys will result in invalid nonce errors.
 
 ---
 
 <a name="notes"></a>
 
 # 📝 Notes
 
-- Coding standards are not always followed to make arguments and function names as similar as possible to those in the Kraken API documentations.
+- The version scheme is `<Major>.<Minor>.<Service Level>` where:
+
+  - **Major** will affect everything and there will be breaking changes
+    in any case. This could be for example a change to Python 3.11+ only.
+
+  - **Minor** introduces features and enhancements which may bring breaking
+    changes in some cases. These breaking changes could be renaming or
+    addition of parameters, change in order of parameters or even renaming
+    a function.
+  - **Service Level** includes bug fixes, documentation or CI related changes.
+
+- Coding standards are not always followed to make arguments and function names
+  as similar as possible to those of the Kraken API documentations.
 
 <a name="references"></a>
 
 # 🔭 References
 
 - https://python-kraken-sdk.readthedocs.io/en/stable
 - https://docs.kraken.com/rest
 - https://docs.kraken.com/websockets
+- https://docs.kraken.com/websockets-v2
 - https://docs.futures.kraken.com
 - https://support.kraken.com/hc/en-us/sections/360012894412-Futures-API
 
 ---
```

### Comparing `python-kraken-sdk-1.5.0/python_kraken_sdk.egg-info/SOURCES.txt` & `python-kraken-sdk-1.6.0/python_kraken_sdk.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 .gitignore
 .pre-commit-config.yaml
-.pylintrc
 .readthedocs.yaml
 CHANGELOG.md
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 Makefile
@@ -44,31 +43,35 @@
 docs/make.bat
 docs/requirements.txt
 docs/src/introduction.rst
 docs/src/issues.rst
 docs/src/about/license.rst
 docs/src/base_api/base_api.rst
 docs/src/examples/futures_bot_template.rst
-docs/src/examples/spot_bot_template.rst
+docs/src/examples/futures_ws_examples.rst
+docs/src/examples/spot_bot_templates.rst
 docs/src/examples/spot_orderbook.rst
+docs/src/examples/spot_ws_examples.rst
 docs/src/examples/trading_bot_templates.rst
 docs/src/futures/rest.rst
 docs/src/futures/websockets.rst
 docs/src/getting_started/getting_started.rst
 docs/src/krakenexceptions/krakenexceptions.rst
 docs/src/spot/rest.rst
 docs/src/spot/websockets.rst
 examples/futures_examples.py
 examples/futures_trading_bot_template.py
 examples/futures_ws_examples.py
 examples/market_client_example.ipynb
 examples/spot_examples.py
 examples/spot_orderbook.py
-examples/spot_trading_bot_template.py
-examples/spot_ws_examples.py
+examples/spot_trading_bot_template_v1.py
+examples/spot_trading_bot_template_v2.py
+examples/spot_ws_examples_v1.py
+examples/spot_ws_examples_v2.py
 kraken/__init__.py
 kraken/_version.py
 kraken/base_api/__init__.py
 kraken/exceptions/__init__.py
 kraken/futures/__init__.py
 kraken/futures/funding.py
 kraken/futures/market.py
@@ -79,16 +82,18 @@
 kraken/spot/__init__.py
 kraken/spot/funding.py
 kraken/spot/market.py
 kraken/spot/orderbook.py
 kraken/spot/staking.py
 kraken/spot/trade.py
 kraken/spot/user.py
-kraken/spot/ws_client.py
+kraken/spot/websocket_v1.py
+kraken/spot/websocket_v2.py
 kraken/spot/websocket/__init__.py
+kraken/spot/websocket/connectors.py
 python_kraken_sdk.egg-info/PKG-INFO
 python_kraken_sdk.egg-info/SOURCES.txt
 python_kraken_sdk.egg-info/dependency_links.txt
 python_kraken_sdk.egg-info/requires.txt
 python_kraken_sdk.egg-info/top_level.txt
 tests/__init__.py
 tests/futures/__init__.py
@@ -106,9 +111,11 @@
 tests/spot/test_spot_base_api.py
 tests/spot/test_spot_funding.py
 tests/spot/test_spot_market.py
 tests/spot/test_spot_orderbook.py
 tests/spot/test_spot_staking.py
 tests/spot/test_spot_trade.py
 tests/spot/test_spot_user.py
-tests/spot/test_spot_websocket.py
+tests/spot/test_spot_websocket_internals.py
+tests/spot/test_spot_websocket_v1.py
+tests/spot/test_spot_websocket_v2.py
 tests/spot/fixture/orderbook.json
```

### Comparing `python-kraken-sdk-1.5.0/tests/futures/conftest.py` & `python-kraken-sdk-1.6.0/tests/futures/conftest.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,144 +4,141 @@
 # GitHub: https://github.com/btschwertfeger
 #
 
 import os
 
 import pytest
 
-from kraken.futures import Funding, KrakenFuturesWSClient, Market, Trade, User
+from kraken.futures import Funding, Market, Trade, User
 
+FUTURES_API_KEY: str = os.getenv("FUTURES_API_KEY")
+FUTURES_SECRET_KEY: str = os.getenv("FUTURES_SECRET_KEY")
+FUTURES_SANDBOX_KEY: str = os.getenv("FUTURES_SANDBOX_KEY")
+FUTURES_SANDBOX_SECRET_KEY: str = os.getenv("FUTURES_SANDBOX_SECRET")
 
-@pytest.fixture
+
+@pytest.fixture()
 def futures_api_key() -> str:
     """Returns the Futures API key"""
-    return os.getenv("FUTURES_API_KEY")
+    return FUTURES_API_KEY
 
 
-@pytest.fixture
+@pytest.fixture()
 def futures_secret_key() -> str:
     """Returns the Futures API secret key"""
-    return os.getenv("FUTURES_SECRET_KEY")
+    return FUTURES_SECRET_KEY
 
 
-@pytest.fixture
+@pytest.fixture()
 def futures_market() -> Market:
     """
     Fixture providing an unauthenticated Futures Market client
     """
     return Market()
 
 
-@pytest.fixture
+@pytest.fixture()
 def futures_auth_market() -> Market:
     """
     Fixture providing an authenticated Futures Market client.
     """
-    return Market(
-        key=os.getenv("FUTURES_API_KEY"), secret=os.getenv("FUTURES_SECRET_KEY")
-    )
+    return Market(key=FUTURES_API_KEY, secret=FUTURES_SECRET_KEY)
 
 
-@pytest.fixture
+@pytest.fixture()
 def futures_demo_market() -> Market:
     """
     Fixture providing an authenticated Futures Market client that
     uses the demo/sandbox environment.
     """
     return Market(
-        key=os.getenv("FUTURES_SANDBOX_KEY"),
-        secret=os.getenv("FUTURES_SANDBOX_SECRET"),
+        key=FUTURES_SANDBOX_KEY,
+        secret=FUTURES_SANDBOX_SECRET_KEY,
         sandbox=True,
     )
 
 
-@pytest.fixture
+@pytest.fixture()
 def futures_user() -> User:
     """
     Fixture providing an unauthenticated Futures User client.
     """
     return User()
 
 
-@pytest.fixture
+@pytest.fixture()
 def futures_auth_user() -> User:
     """
     Fixture providing an authenticated Futures User client.
     """
-    return User(
-        key=os.getenv("FUTURES_API_KEY"), secret=os.getenv("FUTURES_SECRET_KEY")
-    )
+    return User(key=FUTURES_API_KEY, secret=FUTURES_SECRET_KEY)
 
 
-@pytest.fixture
+@pytest.fixture()
 def futures_demo_user() -> User:
     """
     Fixture providing an authenticated Futures User client that
     uses the demo/sandbox environment.
     """
     return User(
-        key=os.getenv("FUTURES_SANDBOX_KEY"),
-        secret=os.getenv("FUTURES_SANDBOX_SECRET"),
+        key=FUTURES_SANDBOX_KEY,
+        secret=FUTURES_SANDBOX_SECRET_KEY,
         sandbox=True,
     )
 
 
-@pytest.fixture
+@pytest.fixture()
 def futures_trade() -> Trade:
     """
     Fixture providing an unauthenticated Futures Trade client.
     """
     return Trade()
 
 
-@pytest.fixture
+@pytest.fixture()
 def futures_auth_trade() -> Trade:
     """
     Fixture providing an authenticated Futures Trade client.
     """
-    return Trade(
-        key=os.getenv("FUTURES_API_KEY"), secret=os.getenv("FUTURES_SECRET_KEY")
-    )
+    return Trade(key=FUTURES_API_KEY, secret=FUTURES_SECRET_KEY)
 
 
-@pytest.fixture
+@pytest.fixture()
 def futures_demo_trade() -> Trade:
     """
     Fixture providing an authenticated Futures Trade client that
     uses the demo/sandbox environment.
     """
     return Trade(
-        key=os.getenv("FUTURES_SANDBOX_KEY"),
-        secret=os.getenv("FUTURES_SANDBOX_SECRET"),
+        key=FUTURES_SANDBOX_KEY,
+        secret=FUTURES_SANDBOX_SECRET_KEY,
         sandbox=True,
     )
 
 
-@pytest.fixture
+@pytest.fixture()
 def futures_funding() -> Funding:
     """
     Fixture providing an unauthenticated Futures Funding client.
     """
     return Funding()
 
 
-@pytest.fixture
+@pytest.fixture()
 def futures_auth_funding() -> Funding:
     """
     Fixture providing an authenticated Futures Funding client.
     """
-    return Funding(
-        key=os.getenv("FUTURES_API_KEY"), secret=os.getenv("FUTURES_SECRET_KEY")
-    )
+    return Funding(key=FUTURES_API_KEY, secret=FUTURES_SECRET_KEY)
 
 
-@pytest.fixture
+@pytest.fixture()
 def futures_demo_funding() -> Funding:
     """
     Fixture providing an authenticated Futures Funding client that
     uses the demo/sandbox environment.
     """
     return Funding(
-        key=os.getenv("FUTURES_SANDBOX_KEY"),
-        secret=os.getenv("FUTURES_SANDBOX_SECRET"),
+        key=FUTURES_SANDBOX_KEY,
+        secret=FUTURES_SANDBOX_SECRET_KEY,
         sandbox=True,
     )
```

### Comparing `python-kraken-sdk-1.5.0/tests/futures/helper.py` & `python-kraken-sdk-1.6.0/tests/futures/helper.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) 2023 Benjamin Thomas Schwertfeger
 # GitHub: https://github.com/btschwertfeger
 #
 
+from __future__ import annotations
+
 import logging
 from asyncio import sleep
 from time import time
 from typing import Any, Union
 
 from kraken.futures import KrakenFuturesWSClient
 
@@ -19,43 +21,45 @@
     return (
         isinstance(value, dict) and "result" in value and value["result"] == "success"
     )
 
 
 def is_not_error(value: Any) -> bool:
     """Returns true if result is not error"""
-    return isinstance(value, dict) and "error" not in value.keys()
+    return isinstance(value, dict) and "error" not in value
 
 
 async def async_wait(seconds: float = 1.0) -> None:
     """Function that realizes the wait for ``seconds``."""
     start: float = time()
     while time() - seconds < start:
         await sleep(0.2)
-    return
 
 
 class FuturesWebsocketClientTestWrapper(KrakenFuturesWSClient):
     """
     Class that creates an instance to test the KrakenFuturesWSClient.
 
     It writes the messages to the log and a file. The log is used
     within the tests, the log file is for local debugging.
     """
 
     LOG: logging.Logger = logging.getLogger(__name__)
 
     def __init__(
-        self: "FuturesWebsocketClientTestWrapper", key: str = "", secret: str = ""
+        self: "FuturesWebsocketClientTestWrapper",
+        key: str = "",
+        secret: str = "",
     ) -> None:
         super().__init__(key=key, secret=secret, callback=self.on_message)
         self.LOG.setLevel(logging.INFO)
 
     async def on_message(
-        self: "FuturesWebsocketClientTestWrapper", msg: Union[list, dict]
+        self: "FuturesWebsocketClientTestWrapper",
+        msg: Union[list, dict],
     ) -> None:
         """
         This is the callback function that must be implemented
         to handle custom websocket messages.
         """
         self.LOG.info(msg)  # the log is read within the tests
```

### Comparing `python-kraken-sdk-1.5.0/tests/futures/test_futures_base_api.py` & `python-kraken-sdk-1.6.0/tests/futures/test_futures_base_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from kraken.base_api import KrakenBaseFuturesAPI
 from kraken.exceptions import KrakenException
 from kraken.futures import Funding, Market, Trade, User
 
 from .helper import is_success
 
 
-@pytest.mark.futures
+@pytest.mark.futures()
 def test_KrakenBaseFuturesAPI_without_exception() -> None:
     """
     Checks first if the expected error will be raised and than
     creates a new KrakenBaseFuturesAPI instance that do not raise
     the custom Kraken exceptions. This new instance than executes
     the same request and the returned response gets evaluated.
     """
@@ -31,22 +31,20 @@
 
     result: dict = (
         KrakenBaseFuturesAPI(key="fake", secret="fake", use_custom_exceptions=False)  # type: ignore[union-attr]
         ._request(method="POST", uri="/derivatives/api/v3/sendorder", auth=True)
         .json()
     )
 
-    assert (
-        result.get("result") == "error"
-        and result.get("error") == "requiredArgumentMissing"
-    )
+    assert result.get("result") == "error"
+    assert result.get("error") == "requiredArgumentMissing"
 
 
-@pytest.mark.futures
-@pytest.mark.futures_auth
+@pytest.mark.futures()
+@pytest.mark.futures_auth()
 def test_futures_rest_contextmanager(
     futures_market: Market,
     futures_auth_funding: Funding,
     futures_demo_trade: Trade,
     futures_auth_user: User,
 ) -> None:
     """
```

### Comparing `python-kraken-sdk-1.5.0/tests/futures/test_futures_funding.py` & `python-kraken-sdk-1.6.0/tests/futures/test_futures_funding.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,67 +11,64 @@
 from kraken.futures import Funding
 
 from .helper import is_success
 
 # todo: Mocking? Or is this to dangerous?
 
 
-@pytest.mark.futures
-@pytest.mark.futures_auth
-@pytest.mark.futures_funding
+@pytest.mark.futures()
+@pytest.mark.futures_auth()
+@pytest.mark.futures_funding()
 def test_get_historical_funding_rates(futures_demo_funding: Funding) -> None:
     """
     Checks the ``get_historical_funding_rates`` function.
     """
     assert is_success(
-        futures_demo_funding.get_historical_funding_rates(symbol="PF_SOLUSD")
+        futures_demo_funding.get_historical_funding_rates(symbol="PF_SOLUSD"),
     )
 
 
-@pytest.mark.futures
-@pytest.mark.futures_auth
-@pytest.mark.futures_funding
+@pytest.mark.futures()
+@pytest.mark.futures_auth()
+@pytest.mark.futures_funding()
 @pytest.mark.skip(reason="CI does not have withdraw permission")
 def test_initiate_wallet_transfer(futures_demo_funding: Funding) -> None:
     """
     Checks the ``initiate_wallet_transfer`` function - skipped since
     a transfer in testing is not desired.
     """
     # accounts must exist..
     # print(futures_demo_funding.initiate_wallet_transfer(
     #     amount=200, fromAccount='Futures Wallet', toAccount='Spot Wallet', unit='XBT'
     # ))
-    pass
 
 
-@pytest.mark.futures
-@pytest.mark.futures_auth
-@pytest.mark.futures_funding
+@pytest.mark.futures()
+@pytest.mark.futures_auth()
+@pytest.mark.futures_funding()
 @pytest.mark.skip(reason="CI does not have withdraw permission")
 def test_initiate_subccount_transfer(futures_demo_funding: Funding) -> None:
     """
     Checks the ``initiate_subaccount_transfer`` function.
     """
-    # print(futures_demo_funding.initiate_subccount_transfer(
+    # print(futures_demo_funding.initiate_subaccount_transfer(
     #     amount=200,
     #     fromAccount='The wallet (cash or margin account) from which funds should be debited',
     #     fromUser='The user account (this or a sub account) from which funds should be debited',
     #     toAccount='The wallet (cash or margin account) to which funds should be credited',
     #     toUser='The user account (this or a sub account) to which funds should be credited',
     #     unit='XBT',
     # ))
-    pass
 
 
-@pytest.mark.futures
-@pytest.mark.futures_auth
-@pytest.mark.futures_funding
+@pytest.mark.futures()
+@pytest.mark.futures_auth()
+@pytest.mark.futures_funding()
 @pytest.mark.skip(reason="CI does not have withdraw permission")
 def test_initiate_withdrawal_to_spot_wallet(futures_demo_funding: Funding) -> None:
     """
     Checks the ``initiate_withdrawal_to_spot_wallet`` function.
     """
     # print(futures_demo_funding.initiate_withdrawal_to_spot_wallet(
     #     amount=200,
     #     currency='XBT',
     # ))
-    pass
```

### Comparing `python-kraken-sdk-1.5.0/tests/futures/test_futures_market.py` & `python-kraken-sdk-1.6.0/tests/futures/test_futures_market.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 import pytest
 
 from kraken.futures import Market
 
 from .helper import is_not_error, is_success
 
 
-@pytest.mark.futures
-@pytest.mark.futures_market
+@pytest.mark.futures()
+@pytest.mark.futures_market()
 def test_get_ohlc(futures_market: Market) -> None:
     """
     Checks the ``get_ohlc`` endpoint.
     """
     assert isinstance(
         futures_market.get_ohlc(
             tick_type="trade",
@@ -27,263 +27,265 @@
             from_="1668989233",
             to="1668999233",
         ),
         dict,
     )
 
 
-@pytest.mark.futures
-@pytest.mark.futures_market
+@pytest.mark.futures()
+@pytest.mark.futures_market()
 def test_get_ohlc_failing_wrong_tick_type(futures_market: Market) -> None:
     """
     Checks the ``get_ohlc`` function by passing an invalid tick type.
     """
-    with pytest.raises(ValueError):
+    with pytest.raises(
+        ValueError,
+        match=r"tick_type must be in \('spot', 'mark', 'trade'\)",
+    ):
         futures_market.get_ohlc(symbol="XBTUSDT", resolution="240", tick_type="fail")
 
 
-@pytest.mark.futures
-@pytest.mark.futures_market
+@pytest.mark.futures()
+@pytest.mark.futures_market()
 def test_get_ohlc_failing_wrong_resolution(futures_market: Market) -> None:
     """
     Checks the ``get_ohlc`` function by passing an invalid resolution.
     """
-    with pytest.raises(ValueError):
+    with pytest.raises(
+        ValueError,
+        match=r"resolution must be in \('1m', '5m', '15m', '30m', '1h', '4h', '12h', '1d', '1w'\)",
+    ):
         futures_market.get_ohlc(symbol="XBTUSDT", resolution="1234", tick_type="trade")
 
 
-@pytest.mark.futures
-@pytest.mark.futures_market
+@pytest.mark.futures()
+@pytest.mark.futures_market()
 def test_get_tick_types(futures_market: Market) -> None:
     assert isinstance(futures_market.get_tick_types(), list)
 
 
-@pytest.mark.futures
-@pytest.mark.futures_market
+@pytest.mark.futures()
+@pytest.mark.futures_market()
 def test_get_tradeable_products(futures_market: Market) -> None:
     """
     Checks the ``get_tradeable_products`` endpoint.
     """
     assert isinstance(futures_market.get_tradeable_products(tick_type="mark"), list)
 
 
-@pytest.mark.futures
-@pytest.mark.futures_market
+@pytest.mark.futures()
+@pytest.mark.futures_market()
 def test_get_resolutions(futures_market: Market) -> None:
     """
     Checks the ``get_resolutions`` endpoint.
     """
     assert isinstance(
         futures_market.get_resolutions(tick_type="trade", tradeable="PI_XBTUSD"),
         list,
     )
 
 
-@pytest.mark.futures
-@pytest.mark.futures_market
+@pytest.mark.futures()
+@pytest.mark.futures_market()
 def test_get_fee_schedules(futures_market: Market) -> None:
     """
     Checks the ``get_fee_schedules`` endpoint.
     """
     assert is_success(futures_market.get_fee_schedules())
 
 
-@pytest.mark.futures
-@pytest.mark.futures_auth
-@pytest.mark.futures_market
+@pytest.mark.futures()
+@pytest.mark.futures_auth()
+@pytest.mark.futures_market()
 def test_get_fee_schedules_vol(futures_auth_market: Market) -> None:
     """
     Checks the ``get_fee_schedules_vol`` endpoint.
     """
     assert is_success(futures_auth_market.get_fee_schedules_vol())
 
 
-@pytest.mark.futures
-@pytest.mark.futures_market
+@pytest.mark.futures()
+@pytest.mark.futures_market()
 def test_get_orderbook(futures_market: Market) -> None:
     """
     Checks the ``get_orderbook`` endpoint.
     """
     # assert type(market.get_orderbook()) == dict # raises 500-INTERNAL_SERVER_ERROR on Kraken,
     # but symbol is optional as described in the API documentation (Dec, 2022)
     assert is_success(futures_market.get_orderbook(symbol="PI_XBTUSD"))
 
 
-@pytest.mark.futures
-@pytest.mark.futures_market
+@pytest.mark.futures()
+@pytest.mark.futures_market()
 def test_get_tickers(futures_market: Market) -> None:
     """
     Checks the ``get_tickers`` endpoint.
     """
     assert is_success(futures_market.get_tickers())
 
 
-@pytest.mark.futures
-@pytest.mark.futures_market
+@pytest.mark.futures()
+@pytest.mark.futures_market()
 def test_get_instruments(futures_market: Market) -> None:
     """
     Checks the ``get_instruments`` endpoint.
     """
     assert is_success(futures_market.get_instruments())
 
 
-@pytest.mark.futures
-@pytest.mark.futures_market
+@pytest.mark.futures()
+@pytest.mark.futures_market()
 def test_get_instruments_status(futures_market: Market) -> None:
     """
     Checks the ``get_instruments_status`` endpoint.
     """
     assert is_success(futures_market.get_instruments_status())
     assert is_success(futures_market.get_instruments_status(instrument="PI_XBTUSD"))
 
 
-@pytest.mark.futures
-@pytest.mark.futures_market
+@pytest.mark.futures()
+@pytest.mark.futures_market()
 def test_get_trade_history(futures_market: Market) -> None:
     """
     Checks the ``get_trade_history`` endpoint.
     """
     assert is_success(futures_market.get_trade_history(symbol="PI_XBTUSD"))
 
 
-@pytest.mark.futures
-@pytest.mark.futures_market
+@pytest.mark.futures()
+@pytest.mark.futures_market()
 def test_get_historical_funding_rates(futures_market: Market) -> None:
     """
     Checks the ``get_historical_funding_rates`` endpoint.
     """
     assert is_success(futures_market.get_historical_funding_rates(symbol="PI_XBTUSD"))
 
 
-@pytest.mark.futures
-@pytest.mark.futures_auth
-@pytest.mark.futures_market
+@pytest.mark.futures()
+@pytest.mark.futures_auth()
+@pytest.mark.futures_market()
 def test_get_leverage_preference(futures_auth_market: Market) -> None:
     """
     Checks the ``get_leverage_preference`` endpoint.
     """
     assert is_not_error(futures_auth_market.get_leverage_preference())
 
 
-@pytest.mark.futures
-@pytest.mark.futures_auth
-@pytest.mark.futures_market
+@pytest.mark.futures()
+@pytest.mark.futures_auth()
+@pytest.mark.futures_market()
 @pytest.mark.skip(reason="CI does not have trade permission")
 def test_set_leverage_preference(futures_auth_market: Market) -> None:
     """
     Checks the ``set_leverage_preference`` endpoint.
     """
     old_leverage_preferences: dict = futures_auth_market.get_leverage_preference()
-    assert (
-        "result" in old_leverage_preferences.keys()
-        and old_leverage_preferences["result"] == "success"
-    )
+    assert "result" in old_leverage_preferences
+    assert old_leverage_preferences["result"] == "success"
     assert is_success(
-        futures_auth_market.set_leverage_preference(symbol="PF_XBTUSD", maxLeverage=2)
+        futures_auth_market.set_leverage_preference(symbol="PF_XBTUSD", maxLeverage=2),
     )
 
     new_leverage_preferences: dict = futures_auth_market.get_leverage_preference()
-    assert (
-        "result" in new_leverage_preferences.keys()
-        and new_leverage_preferences["result"] == "success"
-    )
-    assert (
-        "leveragePreferences" in new_leverage_preferences.keys()
-        and dict(symbol="PF_XBTUSD", maxLeverage=float(2.0))
-        in new_leverage_preferences["leveragePreferences"]
-    )
+    assert "result" in new_leverage_preferences
+    assert new_leverage_preferences["result"] == "success"
+    assert "leveragePreferences" in new_leverage_preferences
+    assert {"symbol": "PF_XBTUSD", "maxLeverage": 2.0} in new_leverage_preferences[
+        "leveragePreferences"
+    ]
 
-    if "leveragePreferences" in old_leverage_preferences.keys():
+    if "leveragePreferences" in old_leverage_preferences:
         for setting in old_leverage_preferences["leveragePreferences"]:
-            if "symbol" in setting.keys() and setting["symbol"] == "PF_XBTUSD":
+            if "symbol" in setting and setting["symbol"] == "PF_XBTUSD":
                 assert is_success(
-                    futures_auth_market.set_leverage_preference(symbol="PF_XBTUSD")
+                    futures_auth_market.set_leverage_preference(symbol="PF_XBTUSD"),
                 )
                 break
 
 
-@pytest.mark.futures
-@pytest.mark.futures_auth
-@pytest.mark.futures_market
+@pytest.mark.futures()
+@pytest.mark.futures_auth()
+@pytest.mark.futures_market()
 def test_get_pnl_preference(futures_auth_market: Market) -> None:
     """
     Checks the ``get_pnl_preference`` endpoint.
     """
     assert is_not_error(futures_auth_market.get_pnl_preference())
 
 
-@pytest.mark.futures
-@pytest.mark.futures_auth
-@pytest.mark.futures_market
+@pytest.mark.futures()
+@pytest.mark.futures_auth()
+@pytest.mark.futures_market()
 @pytest.mark.skip(reason="CI does not have trade permission")
 def test_set_pnl_preference(futures_auth_market: Market) -> None:
     """
     Checks the ``set_pnl_preference`` endpoint.
     """
     old_pnl_preference: dict = futures_auth_market.get_pnl_preference()
-    assert (
-        "result" in old_pnl_preference.keys()
-        and old_pnl_preference["result"] == "success"
-    )
+    assert "result" in old_pnl_preference
+    assert old_pnl_preference["result"] == "success"
     assert is_success(
-        futures_auth_market.set_pnl_preference(symbol="PF_XBTUSD", pnlPreference="BTC")
+        futures_auth_market.set_pnl_preference(symbol="PF_XBTUSD", pnlPreference="BTC"),
     )
 
     new_pnl_preference: dict = futures_auth_market.get_pnl_preference()
-    assert (
-        "result" in new_pnl_preference.keys()
-        and new_pnl_preference["result"] == "success"
-    )
-    assert (
-        "preferences" in new_pnl_preference.keys()
-        and dict(symbol="PF_XBTUSD", pnlCurrency="BTC")
-        in new_pnl_preference["preferences"]
-    )
+    assert "result" in new_pnl_preference
+    assert new_pnl_preference["result"] == "success"
+    assert "preferences" in new_pnl_preference
+    assert {"symbol": "PF_XBTUSD", "pnlCurrency": "BTC"} in new_pnl_preference[
+        "preferences"
+    ]
 
-    if "preferences" in old_pnl_preference.keys():
+    if "preferences" in old_pnl_preference:
         for setting in old_pnl_preference["preferences"]:
-            if "symbol" in setting.keys() and setting["symbol"] == "PF_XBTUSD":
+            if "symbol" in setting and setting["symbol"] == "PF_XBTUSD":
                 assert is_success(
                     futures_auth_market.set_pnl_preference(
-                        symbol="PF_XBTUSD", pnlPreference=setting["pnlCurrency"]
-                    )
+                        symbol="PF_XBTUSD",
+                        pnlPreference=setting["pnlCurrency"],
+                    ),
                 )
                 break
 
 
-@pytest.mark.futures
-@pytest.mark.futures_market
+@pytest.mark.futures()
+@pytest.mark.futures_market()
 def test_get_public_execution_events(futures_market: Market) -> None:
     """
     Checks the ``get_public_execution_events`` endpoint.
     """
     assert is_not_error(
         futures_market.get_public_execution_events(
-            tradeable="PF_SOLUSD", since=1668989233, before=1668999999
-        )
+            tradeable="PF_SOLUSD",
+            since=1668989233,
+            before=1668999999,
+        ),
     )
 
 
-@pytest.mark.futures
-@pytest.mark.futures_market
+@pytest.mark.futures()
+@pytest.mark.futures_market()
 def test_get_public_order_events(futures_market: Market) -> None:
     """
     Checks the ``public_order_events`` endpoint.
     """
     assert is_not_error(
         futures_market.get_public_order_events(
-            tradeable="PF_SOLUSD", since=1668989233, sort="asc"
-        )
+            tradeable="PF_SOLUSD",
+            since=1668989233,
+            sort="asc",
+        ),
     )
 
 
-@pytest.mark.futures
-@pytest.mark.futures_market
+@pytest.mark.futures()
+@pytest.mark.futures_market()
 def test_get_public_mark_price_events(futures_market: Market) -> None:
     """
     Checks the ``get_public_mark_price_events`` endpoint.
     """
     assert is_not_error(
         futures_market.get_public_mark_price_events(
-            tradeable="PF_SOLUSD", since=1668989233
-        )
+            tradeable="PF_SOLUSD",
+            since=1668989233,
+        ),
     )
```

### Comparing `python-kraken-sdk-1.5.0/tests/futures/test_futures_trade.py` & `python-kraken-sdk-1.6.0/tests/futures/test_futures_trade.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,120 +2,117 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) 2023 Benjamin Thomas Schwertfeger
 # GitHub: https://github.com/btschwertfeger
 #
 
 """Module that implements the unit tests for the Futures trade client"""
 
+from contextlib import suppress
 from time import sleep
 
 import pytest
 
 from kraken.exceptions import KrakenException
 
 from .helper import is_success
 
 
 @pytest.fixture(autouse=True)
-def run_before_and_after_tests(futures_demo_trade):
+def _run_before_and_after_tests(futures_demo_trade) -> None:
     """
     Fixture that ensures all orders are cancelled after test.
     """
     # Setup: fill with any logic you want
 
     yield  # this is where the testing happens
 
     # Teardown: fill with any logic you want
     futures_demo_trade.cancel_all_orders()
     sleep(0.25)
 
 
-@pytest.mark.futures
-@pytest.mark.futures_auth
-@pytest.mark.futures_trade
+@pytest.mark.futures()
+@pytest.mark.futures_auth()
+@pytest.mark.futures_trade()
 def test_get_fills(futures_demo_trade) -> None:
     """
     Checks the ``get_fills`` endpoint.
     """
     assert is_success(futures_demo_trade.get_fills())
     assert is_success(
-        futures_demo_trade.get_fills(lastFillTime="2020-07-21T12:41:52.790Z")
+        futures_demo_trade.get_fills(lastFillTime="2020-07-21T12:41:52.790Z"),
     )
 
 
-@pytest.mark.futures
-@pytest.mark.futures_auth
-@pytest.mark.futures_trade
+@pytest.mark.futures()
+@pytest.mark.futures_auth()
+@pytest.mark.futures_trade()
 def test_dead_mans_switch(futures_demo_trade) -> None:
     """
     Checks the ``dead_mans_switch`` endpoint.
     """
     assert is_success(futures_demo_trade.dead_mans_switch(timeout=60))
     assert is_success(
-        futures_demo_trade.dead_mans_switch(timeout=0)
+        futures_demo_trade.dead_mans_switch(timeout=0),
     )  # reset dead mans switch
 
 
-@pytest.mark.futures
-@pytest.mark.futures_auth
-@pytest.mark.futures_trade
+@pytest.mark.futures()
+@pytest.mark.futures_auth()
+@pytest.mark.futures_trade()
 def test_get_orders_status(futures_demo_trade) -> None:
     """
     Checks the ``get_orders_status`` endpoint.
     """
     assert is_success(
         futures_demo_trade.get_orders_status(
             orderIds=[
                 "d47e7fb4-aed0-4f3d-987b-9e3ca78ba74e",
                 "fc589be9-5095-48f0-b6f1-a2dfad6d9677",
-            ]
-        )
+            ],
+        ),
     )
     assert is_success(
         futures_demo_trade.get_orders_status(
             cliOrdIds=[
                 "2c611222-bfe6-42d1-9f55-77bddc01a313",
                 "fc589be9-5095-48f0-b6f1-a2dfad6d9677",
-            ]
-        )
+            ],
+        ),
     )
 
 
-@pytest.mark.futures
-@pytest.mark.futures_auth
-@pytest.mark.futures_trade
+@pytest.mark.futures()
+@pytest.mark.futures_auth()
+@pytest.mark.futures_trade()
 def test_create_order(futures_demo_trade) -> None:
     """
     Checks the ``create_order`` endpoint.
     """
-    try:
+    with suppress(KrakenException.KrakenInsufficientAvailableFundsError):
         futures_demo_trade.create_order(
             orderType="lmt",
             size=10,
             symbol="PI_XBTUSD",
             side="buy",
             limitPrice=1,
             stopPrice=10,
             reduceOnly=True,
         )
-    except KrakenException.KrakenInsufficientAvailableFundsError:
-        pass
 
-    try:
+    with suppress(KrakenException.KrakenInsufficientAvailableFundsError):
         futures_demo_trade.create_order(
             orderType="take_profit",
             size=10,
             side="buy",
             symbol="PI_XBTUSD",
             limitPrice=12000,
             triggerSignal="last",
             stopPrice=13000,
         )
-    except KrakenException.KrakenInsufficientAvailableFundsError:
-        pass
 
     # try:
     #     # does not work,  400 response "invalid order type"
     #     # but it is documented here: https://docs.futures.kraken.com/#http-api-trading-v3-api-order-management-send-order
     #     # Kraken needs to fix this
     #     futures_demo_trade.create_order(
     #         orderType="trailing_stop",
@@ -127,50 +124,56 @@
     #         trailingStopDeviationUnit="PERCENT",
     #         trailingStopMaxDeviation=10,
     #     )
     # except KrakenException.KrakenException.KrakenInsufficientAvailableFundsError:
     #     pass
 
 
-@pytest.mark.futures
-@pytest.mark.futures_auth
-@pytest.mark.futures_trade
+@pytest.mark.futures()
+@pytest.mark.futures_auth()
+@pytest.mark.futures_trade()
 def test_create_order_failing(futures_demo_trade) -> None:
     """
     Checks ``create_order`` endpoint to fail when using invalid
     parameters.
     """
-    with pytest.raises(ValueError):
+    with pytest.raises(
+        ValueError,
+        match=r"Invalid side. One of \[\('buy', 'sell'\)\] is required!",
+    ):
         futures_demo_trade.create_order(
             orderType="mkt",
             size=10,
             symbol="PI_XBTUSD",
             side="long",
         )
 
-    with pytest.raises(ValueError):
+    with pytest.raises(
+        ValueError,
+        match=r"Trigger signal must be in \[\('mark', 'spot', 'last'\)\]!",
+    ):
         futures_demo_trade.create_order(
             orderType="take-profit",
             size=10,
             side="buy",
             symbol="PI_XBTUSD",
             limitPrice=12000,
             triggerSignal="fail",
             stopPrice=13000,
         )
 
 
-@pytest.mark.futures
-@pytest.mark.futures_auth
-@pytest.mark.futures_trade
+@pytest.mark.futures()
+@pytest.mark.futures_auth()
+@pytest.mark.futures_trade()
 def test_create_batch_order(futures_demo_trade) -> None:
     """
     Checks the ``create_order_batch`` endpoint.
     """
-    try:
+    with suppress(KrakenException.KrakenInsufficientAvailableFundsError):
         assert is_success(
             futures_demo_trade.create_batch_order(
                 batchorder_list=[
                     {
                         "order": "send",
                         "order_tag": "1",
                         "orderType": "lmt",
@@ -195,76 +198,76 @@
                         "order_id": "e35d61dd-8a30-4d5f-a574-b5593ef0c050",
                     },
                     {
                         "order": "cancel",
                         "cliOrdId": "my_client_id",
                     },
                 ],
-            )
+            ),
         )
-    except KrakenException.KrakenInsufficientAvailableFundsError:
-        pass
 
 
-@pytest.mark.futures
-@pytest.mark.futures_auth
-@pytest.mark.futures_trade
+@pytest.mark.futures()
+@pytest.mark.futures_auth()
+@pytest.mark.futures_trade()
 def test_edit_order(futures_demo_trade) -> None:
     """
     Checks the ``edit_order`` endpoint.
     """
     # success, because kraken received the correct message, even if the id is invalid
     assert is_success(
-        futures_demo_trade.edit_order(orderId="my_another_client_id", limitPrice=3)
+        futures_demo_trade.edit_order(orderId="my_another_client_id", limitPrice=3),
     )
 
     assert is_success(
         futures_demo_trade.edit_order(
-            cliOrdId="myclientorderid", size=111.0, stopPrice=1000
-        )
+            cliOrdId="myclientorderid",
+            size=111.0,
+            stopPrice=1000,
+        ),
     )
 
 
-@pytest.mark.futures
-@pytest.mark.futures_auth
-@pytest.mark.futures_trade
+@pytest.mark.futures()
+@pytest.mark.futures_auth()
+@pytest.mark.futures_trade()
 def test_edit_order_failing(futures_demo_trade) -> None:
     """
     Checks if the ``edit_order`` endpoint fails when using invalid
     parameters.
     """
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match=r"Either orderId or cliOrdId must be set!"):
         futures_demo_trade.edit_order()
 
 
-@pytest.mark.futures
-@pytest.mark.futures_auth
-@pytest.mark.futures_trade
+@pytest.mark.futures()
+@pytest.mark.futures_auth()
+@pytest.mark.futures_trade()
 def test_cancel_order(futures_demo_trade) -> None:
     """
     Checks the ``cancel_order`` endpoint.
     """
     assert is_success(futures_demo_trade.cancel_order(cliOrdId="my_another_client_id"))
     assert is_success(futures_demo_trade.cancel_order(order_id="1234"))
 
 
-@pytest.mark.futures
-@pytest.mark.futures_auth
-@pytest.mark.futures_trade
+@pytest.mark.futures()
+@pytest.mark.futures_auth()
+@pytest.mark.futures_trade()
 def test_cancel_order_failing(futures_demo_trade) -> None:
     """
     Checks if the ``cancel_order`` endpoint is failing when
     passing invalid arguments.
     """
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match=r"Either order_id or cliOrdId must be set!"):
         futures_demo_trade.cancel_order()
 
 
-@pytest.mark.futures
-@pytest.mark.futures_auth
-@pytest.mark.futures_trade
+@pytest.mark.futures()
+@pytest.mark.futures_auth()
+@pytest.mark.futures_trade()
 def test_cancel_all_orders(futures_demo_trade) -> None:
     """
     Checks the ``cancel_all_orders`` endpoint.
     """
     assert is_success(futures_demo_trade.cancel_all_orders(symbol="pi_xbtusd"))
     assert is_success(futures_demo_trade.cancel_all_orders())
```

### Comparing `python-kraken-sdk-1.5.0/tests/futures/test_futures_user.py` & `python-kraken-sdk-1.6.0/tests/futures/test_futures_user.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,185 +5,199 @@
 #
 
 """Module that implements the unit tests for the Futures user client."""
 
 import os
 import random
 import tempfile
+from typing import TYPE_CHECKING
 
 import pytest
-import requests
 
 from kraken.futures import User
 
 from .helper import is_success
 
+if TYPE_CHECKING:
+    import requests
 
-@pytest.mark.futures
-@pytest.mark.futures_auth
-@pytest.mark.futures_user
+
+@pytest.mark.futures()
+@pytest.mark.futures_auth()
+@pytest.mark.futures_user()
 def test_get_wallets(futures_auth_user: User) -> None:
     """
     Checks the ``get_wallets`` endpoint.
     """
     assert is_success(futures_auth_user.get_wallets())
 
 
-@pytest.mark.futures
-@pytest.mark.futures_auth
-@pytest.mark.futures_user
+@pytest.mark.futures()
+@pytest.mark.futures_auth()
+@pytest.mark.futures_user()
 def test_get_subaccounts(futures_auth_user: User) -> None:
     """
     Checks the ``get_subaccounts`` endpoint.
     """
     assert is_success(futures_auth_user.get_subaccounts())
 
 
-@pytest.mark.futures
-@pytest.mark.futures_auth
-@pytest.mark.futures_user
+@pytest.mark.futures()
+@pytest.mark.futures_auth()
+@pytest.mark.futures_user()
 def test_get_unwindqueue(futures_auth_user: User) -> None:
     """
     Checks the ``get_unwindqueue`` endpoint.
     """
     assert is_success(futures_auth_user.get_unwind_queue())
 
 
-@pytest.mark.futures
-@pytest.mark.futures_auth
-@pytest.mark.futures_user
+@pytest.mark.futures()
+@pytest.mark.futures_auth()
+@pytest.mark.futures_user()
 def test_get_notifications(futures_auth_user: User) -> None:
     """
     Checks the ``get_notifications`` endpoint.
     """
     assert is_success(futures_auth_user.get_notifications())
 
 
-@pytest.mark.futures
-@pytest.mark.futures_auth
-@pytest.mark.futures_user
+@pytest.mark.futures()
+@pytest.mark.futures_auth()
+@pytest.mark.futures_user()
 def test_get_account_log(futures_auth_user: User) -> None:
     """
     Checks the ``get_account_log`` endpoint.
     """
     assert isinstance(futures_auth_user.get_account_log(), dict)
     assert isinstance(
-        futures_auth_user.get_account_log(info="futures liquidation"), dict
+        futures_auth_user.get_account_log(info="futures liquidation"),
+        dict,
     )
 
 
-@pytest.mark.futures
-@pytest.mark.futures_auth
-@pytest.mark.futures_user
+@pytest.mark.futures()
+@pytest.mark.futures_auth()
+@pytest.mark.futures_user()
 def test_get_account_log_csv(futures_auth_user: User) -> None:
     """
     Checks the ``get_account_log_csv`` endpoint.
     """
     response: requests.Response = futures_auth_user.get_account_log_csv()
     assert response.status_code in (200, "200")
 
-    with tempfile.TemporaryDirectory() as tmp_dir:
-        with open(
-            os.path.join(tmp_dir, f"account_log-{random.randint(0, 10000)}.csv"), "wb"
-        ) as file:
-            for chunk in response.iter_content(chunk_size=512):
-                if chunk:
-                    file.write(chunk)
+    with tempfile.TemporaryDirectory() as tmp_dir, open(
+        os.path.join(tmp_dir, f"account_log-{random.randint(0, 10000)}.csv"),
+        "wb",
+    ) as file:
+        for chunk in response.iter_content(chunk_size=512):
+            if chunk:
+                file.write(chunk)
 
 
-@pytest.mark.futures
-@pytest.mark.futures_auth
-@pytest.mark.futures_user
+@pytest.mark.futures()
+@pytest.mark.futures_auth()
+@pytest.mark.futures_user()
 def test_get_execution_events(futures_auth_user: User) -> None:
     """
     Checks the ``get_execution_events`` endpoint.
     """
     result: dict = futures_auth_user.get_execution_events(
-        tradeable="PF_SOLUSD", since=1668989233, before=1668999999, sort="asc"
+        tradeable="PF_SOLUSD",
+        since=1668989233,
+        before=1668999999,
+        sort="asc",
     )
 
     assert isinstance(result, dict)
-    assert "elements" in result.keys()
+    assert "elements" in result
 
 
-@pytest.mark.futures
-@pytest.mark.futures_auth
-@pytest.mark.futures_user
+@pytest.mark.futures()
+@pytest.mark.futures_auth()
+@pytest.mark.futures_user()
 def test_get_order_events(futures_auth_user: User) -> None:
     """
     Checks the ``get_order_events`` endpoint.
     """
     result: dict = futures_auth_user.get_order_events(
-        tradeable="PF_SOLUSD", since=1668989233, before=1668999999, sort="asc"
+        tradeable="PF_SOLUSD",
+        since=1668989233,
+        before=1668999999,
+        sort="asc",
     )
     assert isinstance(result, dict)
-    assert "elements" in result.keys()
+    assert "elements" in result
 
 
-@pytest.mark.futures
-@pytest.mark.futures_auth
-@pytest.mark.futures_user
+@pytest.mark.futures()
+@pytest.mark.futures_auth()
+@pytest.mark.futures_user()
 def test_get_open_orders(futures_auth_user: User) -> None:
     """
     Checks the ``get_open_orders`` endpoint.
     """
     assert is_success(futures_auth_user.get_open_orders())
 
 
-@pytest.mark.futures
-@pytest.mark.futures_auth
-@pytest.mark.futures_user
+@pytest.mark.futures()
+@pytest.mark.futures_auth()
+@pytest.mark.futures_user()
 def test_get_open_positions(futures_auth_user: User) -> None:
     """
     Checks the ``get_open_positions`` endpoint.
     """
     assert is_success(futures_auth_user.get_open_positions())
 
 
-@pytest.mark.futures
-@pytest.mark.futures_auth
-@pytest.mark.futures_user
+@pytest.mark.futures()
+@pytest.mark.futures_auth()
+@pytest.mark.futures_user()
 def test_get_trigger_events(futures_auth_user: User) -> None:
     """
     Checks the ``get_trigger_events`` endpoint.
     """
     result = futures_auth_user.get_trigger_events(
-        tradeable="PF_SOLUSD", since=1668989233, before=1668999999, sort="asc"
+        tradeable="PF_SOLUSD",
+        since=1668989233,
+        before=1668999999,
+        sort="asc",
     )
     assert isinstance(result, dict)
-    assert "elements" in result.keys()
+    assert "elements" in result
 
 
-@pytest.mark.futures
-@pytest.mark.futures_auth
-@pytest.mark.futures_user
+@pytest.mark.futures()
+@pytest.mark.futures_auth()
+@pytest.mark.futures_user()
 @pytest.mark.skip("Subaccount actions are only available for insitutional clients")
 def test_check_trading_enabled_on_subaccount(futures_auth_user: User) -> None:
     """
     Checks the ``check_trading_enabled_on_subaccount`` function.
 
     Until now, subaccounts are only available for institutional clients, so this
     execution raises an error. This test will work correctly (hopefully) when
     Kraken enables subaccounts for pro trader.
     """
     assert {
-        "tradingEnabled": False
+        "tradingEnabled": False,
     } == futures_auth_user.check_trading_enabled_on_subaccount(
-        subaccountUid="778387bh61b-f990-4128-16a7-f819abc8"
+        subaccountUid="778387bh61b-f990-4128-16a7-f819abc8",
     )
 
 
-@pytest.mark.futures
-@pytest.mark.futures_auth
-@pytest.mark.futures_user
+@pytest.mark.futures()
+@pytest.mark.futures_auth()
+@pytest.mark.futures_user()
 @pytest.mark.skip("Subaccount actions are only available for insitutional clients")
 def test_set_trading_on_subaccount(futures_auth_user: User) -> None:
     """
     Checks the ``set_trading_on_subaccount`` function.
 
     Until now, subaccounts are only available for institutional clients, so this
     execution raises an error. This test will work correctly (hopefully) when
     Kraken enables subaccounts for pro trader.
     """
     assert {"tradingEnabled": True} == futures_auth_user.set_trading_on_subaccount(
-        subaccountUid="778387bh61b-f990-4128-16a7-f819abc8", trading_enabled=True
+        subaccountUid="778387bh61b-f990-4128-16a7-f819abc8",
+        trading_enabled=True,
     )
```

### Comparing `python-kraken-sdk-1.5.0/tests/futures/test_futures_websocket.py` & `python-kraken-sdk-1.6.0/tests/futures/test_futures_websocket.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 from typing import Any, List
 
 import pytest
 
 from .helper import FuturesWebsocketClientTestWrapper, async_wait
 
 
-@pytest.mark.futures
-@pytest.mark.futures_websocket
-def test_create_public_bot(caplog: Any) -> None:
+@pytest.mark.futures()
+@pytest.mark.futures_websocket()
+def test_create_public_client(caplog: Any) -> None:
     """
     Checks if the unauthenticated websocket client
     can be instantiated.
     """
 
     async def instantiate_client() -> None:
         client: FuturesWebsocketClientTestWrapper = FuturesWebsocketClientTestWrapper()
@@ -31,39 +31,42 @@
         assert not client.is_auth
 
     asyncio.run(instantiate_client())
 
     assert "{'event': 'info', 'version': 1}" in caplog.text
 
 
-@pytest.mark.futures
-@pytest.mark.futures_auth
-@pytest.mark.futures_websocket
-def test_create_private_bot(
-    futures_api_key: str, futures_secret_key: str, caplog: Any
+@pytest.mark.futures()
+@pytest.mark.futures_auth()
+@pytest.mark.futures_websocket()
+def test_create_private_client(
+    futures_api_key: str,
+    futures_secret_key: str,
+    caplog: Any,
 ) -> None:
     """
     Checks if the authenticated websocket client
     can be instantiated.
     """
 
     async def instantiate_client() -> None:
         client: FuturesWebsocketClientTestWrapper = FuturesWebsocketClientTestWrapper(
-            key=futures_api_key, secret=futures_secret_key
+            key=futures_api_key,
+            secret=futures_secret_key,
         )
         assert client.is_auth
         await async_wait(5)
 
     asyncio.run(instantiate_client())
 
     assert "{'event': 'info', 'version': 1}" in caplog.text
 
 
-@pytest.mark.futures
-@pytest.mark.futures_websocket
+@pytest.mark.futures()
+@pytest.mark.futures_websocket()
 def test_get_available_public_subscriptions() -> None:
     """
     Checks the ``get_available_public_subscription_feeds`` function.
     """
 
     expected: List[str] = [
         "trade",
@@ -74,16 +77,16 @@
     ]
     assert all(
         feed in expected
         for feed in FuturesWebsocketClientTestWrapper.get_available_public_subscription_feeds()
     )
 
 
-@pytest.mark.futures
-@pytest.mark.futures_websocket
+@pytest.mark.futures()
+@pytest.mark.futures_websocket()
 def test_get_available_private_subscriptions() -> None:
     """
     Checks the ``get_available_private_subscription_feeds`` function.
     """
 
     expected: List[str] = [
         "fills",
@@ -98,27 +101,29 @@
     ]
     assert all(
         feed in expected
         for feed in FuturesWebsocketClientTestWrapper.get_available_private_subscription_feeds()
     )
 
 
-@pytest.mark.futures
-@pytest.mark.futures_websocket
+@pytest.mark.futures()
+@pytest.mark.futures_websocket()
 def test_subscribe_public(caplog: Any) -> None:
     """
     Checks if the client is able to subscribe to a public feed.
     """
 
     async def check_subscription() -> None:
         client: FuturesWebsocketClientTestWrapper = FuturesWebsocketClientTestWrapper()
         await async_wait(2)
 
-        with pytest.raises(ValueError):
-            # products must be List[str]
+        with pytest.raises(
+            TypeError,
+            match=r"Parameter products must be type of list\[str\] \(e.g. products=\[\"PI_XBTUSD\"\]\)",
+        ):
             await client.subscribe(feed="ticker", products="PI_XBTUSD")  # type: ignore[arg-type]
 
         await client.subscribe(feed="ticker", products=["PI_XBTUSD", "PF_SOLUSD"])
         await async_wait(seconds=2)
 
         subs: List[dict] = client.get_active_subscriptions()
         assert isinstance(subs, list)
@@ -134,63 +139,70 @@
     for expected in (
         "{'event': 'subscribed', 'feed': 'ticker', 'product_ids': ['PI_XBTUSD']}",
         "{'event': 'subscribed', 'feed': 'ticker', 'product_ids': ['PF_SOLUSD']}",
     ):
         assert expected in caplog.text
 
 
-@pytest.mark.futures
-@pytest.mark.futures_auth
-@pytest.mark.futures_websocket
+@pytest.mark.futures()
+@pytest.mark.futures_auth()
+@pytest.mark.futures_websocket()
 def test_subscribe_private(
-    futures_api_key: str, futures_secret_key: str, caplog: Any
+    futures_api_key: str,
+    futures_secret_key: str,
+    caplog: Any,
 ) -> None:
     """
     Checks if the authenticated websocket client is able to subscribe
     to private feeds.
     """
 
     async def submit_subscription() -> None:
         client: FuturesWebsocketClientTestWrapper = FuturesWebsocketClientTestWrapper(
-            key=futures_api_key, secret=futures_secret_key
+            key=futures_api_key,
+            secret=futures_secret_key,
         )
 
-        with pytest.raises(ValueError):
-            # private subscriptions does not use products
+        with pytest.raises(
+            ValueError,
+            match=r"There is no private feed that accepts products!",
+        ):
             await client.subscribe(feed="fills", products=["PI_XBTUSD"])
 
         await client.subscribe(feed="open_orders")
         await async_wait(2)
 
     asyncio.run(submit_subscription())
 
     for expected in (
         "{'event': 'subscribed', 'feed': 'open_orders'}",
         "{'feed': 'open_orders_snapshot', 'account':",
     ):
         assert expected in caplog.text
 
 
-@pytest.mark.futures
-@pytest.mark.futures_websocket
+@pytest.mark.futures()
+@pytest.mark.futures_websocket()
 def test_unsubscribe_public(caplog: Any) -> None:
     """
     Checks if the unauthenticated websocket client is able to unsubscribe
     from public feeds.
     """
 
     async def execute_unsubscribe() -> None:
         client: FuturesWebsocketClientTestWrapper = FuturesWebsocketClientTestWrapper()
         products: List[str] = ["PI_XBTUSD", "PF_SOLUSD"]
 
         await client.subscribe(feed="ticker", products=products)
         await async_wait(seconds=2)
 
-        with pytest.raises(ValueError):
-            # products must be type List[str]
+        with pytest.raises(
+            TypeError,
+            match=r"Parameter products must be type of list\[str\]",
+        ):
             await client.unsubscribe(feed="ticker", products="PI_XBTUSD")  # type: ignore[arg-type]
 
         await client.unsubscribe(feed="ticker", products=products)
         await async_wait(seconds=2)
 
     asyncio.run(execute_unsubscribe())
 
@@ -199,50 +211,55 @@
         "{'event': 'subscribed', 'feed': 'ticker', 'product_ids': ['PF_SOLUSD']}",
         "{'event': 'unsubscribed', 'feed': 'ticker', 'product_ids': ['PI_XBTUSD']}",
         "{'event': 'unsubscribed', 'feed': 'ticker', 'product_ids': ['PF_SOLUSD']}",
     ):
         assert expected in caplog.text
 
 
-@pytest.mark.futures
-@pytest.mark.futures_auth
-@pytest.mark.futures_websocket
+@pytest.mark.futures()
+@pytest.mark.futures_auth()
+@pytest.mark.futures_websocket()
 def test_unsubscribe_private(
-    futures_api_key: str, futures_secret_key: str, caplog: Any
+    futures_api_key: str,
+    futures_secret_key: str,
+    caplog: Any,
 ) -> None:
     """
     Checks if the authenticated websocket client is able to unsubscribe
     from private feeds.
     """
 
     async def execute_unsubscribe() -> None:
         client: FuturesWebsocketClientTestWrapper = FuturesWebsocketClientTestWrapper(
-            key=futures_api_key, secret=futures_secret_key
+            key=futures_api_key,
+            secret=futures_secret_key,
         )
         await client.subscribe(feed="open_orders")
 
         await async_wait(seconds=2)
-        with pytest.raises(ValueError):
-            # private un/-subscriptions does not accept a product
+        with pytest.raises(
+            ValueError,
+            match=r"There is no private feed that accepts products!",
+        ):
             await client.unsubscribe(feed="open_orders", products=["PI_XBTUSD"])
 
         await client.unsubscribe(feed="open_orders")
         await async_wait(seconds=2)
 
     asyncio.run(execute_unsubscribe())
 
     for expected in (
         "{'event': 'subscribed', 'feed': 'open_orders'}",
         "{'event': 'unsubscribed', 'feed': 'open_orders'}",
     ):
         assert expected in caplog.text
 
 
-@pytest.mark.futures
-@pytest.mark.futures_websocket
+@pytest.mark.futures()
+@pytest.mark.futures_websocket()
 def test_get_active_subscriptions(caplog: Any) -> None:
     """
     Checks the ``get_active_subscriptions`` function.
     """
 
     async def check_subscriptions() -> None:
         client: FuturesWebsocketClientTestWrapper = FuturesWebsocketClientTestWrapper()
```

### Comparing `python-kraken-sdk-1.5.0/tests/spot/helper.py` & `python-kraken-sdk-1.6.0/tests/spot/helper.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,106 +1,146 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) 2023 Benjamin Thomas Schwertfeger
 # GitHub: https://github.com/btschwertfeger
 #
 
+"""
+Module that implements the unit tests for the Kraken Spot Websocket API v1
+client.
+"""
+
+from __future__ import annotations
+
+import json
 import logging
 import os
 from asyncio import sleep
 from time import time
 from typing import Any, Union
 
-from kraken.spot import KrakenSpotWSClient, OrderbookClient
+from kraken.spot import KrakenSpotWSClient, KrakenSpotWSClientV2, OrderbookClient
 
 FIXTURE_DIR: str = os.path.join(os.path.dirname(__file__), "fixture")
 
 
 def is_not_error(value: Any) -> bool:
     """Returns True if 'error' as key not in dict."""
     return isinstance(value, dict) and "error" not in value
 
 
 async def async_wait(seconds: float = 1.0) -> None:
     """Function that waits for ``seconds`` - asynchron."""
     start: float = time()
     while time() - seconds < start:
         await sleep(0.2)
-    return
 
 
-class SpotWebsocketClientTestWrapper(KrakenSpotWSClient):
+class SpotWebsocketClientV1TestWrapper(KrakenSpotWSClient):
     """
     Class that creates an instance to test the KrakenSpotWSClient.
 
     It writes the messages to the log and a file. The log is used
     within the tests, the log file is for local debugging.
     """
 
     LOG: logging.Logger = logging.getLogger(__name__)
 
     def __init__(
-        self: "SpotWebsocketClientTestWrapper", key: str = "", secret: str = ""
+        self: SpotWebsocketClientV1TestWrapper,
+        key: str = "",
+        secret: str = "",
     ) -> None:
         super().__init__(key=key, secret=secret, callback=self.on_message)
         self.LOG.setLevel(logging.INFO)
-        fh = logging.FileHandler("spot_ws.log", mode="a")
+        fh = logging.FileHandler("spot_ws_v1.log", mode="a")
         fh.setLevel(logging.INFO)
         self.LOG.addHandler(fh)
 
     async def on_message(
-        self: "SpotWebsocketClientTestWrapper", msg: Union[list, dict]
+        self: SpotWebsocketClientV1TestWrapper,
+        message: Union[list, dict],
+    ) -> None:
+        """
+        This is the callback function that must be implemented
+        to handle custom websocket messages.
+        """
+        self.LOG.info(message)  # the log is read within the tests
+
+
+class SpotWebsocketClientV2TestWrapper(KrakenSpotWSClientV2):
+    """
+    Class that creates an instance to test the KrakenSpotWSClientV2.
+
+    It writes the messages to the log and a file. The log is used
+    within the tests, the log file is for local debugging.
+    """
+
+    LOG: logging.Logger = logging.getLogger(__name__)
+
+    def __init__(
+        self: SpotWebsocketClientV2TestWrapper,
+        key: str = "",
+        secret: str = "",
+        **kwargs: Any,
     ) -> None:
+        super().__init__(key=key, secret=secret, callback=self.on_message, **kwargs)
+        self.LOG.setLevel(logging.INFO)
+        fh = logging.FileHandler("spot_ws_v2.log", mode="a")
+        fh.setLevel(logging.INFO)
+        self.LOG.addHandler(fh)
+
+    async def on_message(self: SpotWebsocketClientV2TestWrapper, message: dict) -> None:
         """
         This is the callback function that must be implemented
         to handle custom websocket messages.
         """
-        self.LOG.info(msg)  # the log is read within the tests
+        self.LOG.info(json.dumps(message))  # the log is read within the tests
 
 
 class OrderbookClientWrapper(OrderbookClient):
     """
     This class is used for testing the Spot Orderbook client.
 
     It writes the messages to the log and a file. The log is used
     within the tests, the log file is for local debugging.
     """
 
     LOG: logging.Logger = logging.getLogger(__name__)
 
-    def __init__(self: "OrderbookClientWrapper") -> None:
+    def __init__(self: OrderbookClientWrapper) -> None:
         super().__init__()
         self.LOG.setLevel(logging.INFO)
 
-    async def on_message(
-        self: "OrderbookClientWrapper", msg: Union[list, dict]
-    ) -> None:
-        self.ensure_log(msg)
-        await super().on_message(msg=msg)
+    async def on_message(self: OrderbookClientWrapper, message: dict) -> None:
+        self.ensure_log(message)
+        await super().on_message(message=message)
 
     async def on_book_update(
-        self: "OrderbookClientWrapper", pair: str, message: list
+        self: OrderbookClientWrapper,
+        pair: str,
+        message: dict,
     ) -> None:
         """
         This is the callback function that must be implemented
         to handle custom websocket messages.
         """
         self.ensure_log((pair, message))
 
     @classmethod
     def ensure_log(cls, content: Any) -> None:
         """
         Ensures that the messages are logged.
         Into a file for debugging and general to the log
         to read the logs within the unit tests.
         """
-        cls.LOG.info(content)
+        cls.LOG.info(json.dumps(content))
 
         log: str = ""
         try:
             with open("spot_orderbook.log", "r", encoding="utf-8") as logfile:
                 log = logfile.read()
         except FileNotFoundError:
             pass
 
         with open("spot_orderbook.log", "w", encoding="utf-8") as logfile:
-            logfile.write(f"{log}\n{content}")
+            logfile.write(f"{log}\n{json.dumps(content)}")
```

### Comparing `python-kraken-sdk-1.5.0/tests/spot/test_spot_base_api.py` & `python-kraken-sdk-1.6.0/tests/spot/test_spot_base_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,37 +11,39 @@
 from kraken.base_api import KrakenBaseSpotAPI
 from kraken.exceptions import KrakenException
 from kraken.spot import Funding, Market, Staking, Trade, User
 
 from .helper import is_not_error
 
 
-@pytest.mark.spot
+@pytest.mark.spot()
 def test_KrakenBaseSpotAPI_without_exception() -> None:
     """
     Checks first if the expected error will be raised and than
     creates a new KrakenBaseSpotAPI instance that do not raise
     the custom Kraken exceptions. This new instance than executes
     the same request and the returned response gets evaluated.
     """
     with pytest.raises(KrakenException.KrakenInvalidAPIKeyError):
         KrakenBaseSpotAPI(
             key="fake",
             secret="fake",
         )._request(method="POST", uri="/private/AddOrder", auth=True)
 
     assert KrakenBaseSpotAPI(
-        key="fake", secret="fake", use_custom_exceptions=False
+        key="fake",
+        secret="fake",
+        use_custom_exceptions=False,
     )._request(method="POST", uri="/private/AddOrder", auth=True).json() == {
-        "error": ["EAPI:Invalid key"]
+        "error": ["EAPI:Invalid key"],
     }
 
 
-@pytest.mark.spot
-@pytest.mark.spot_auth
+@pytest.mark.spot()
+@pytest.mark.spot_auth()
 def test_spot_rest_contextmanager(
     spot_market: Market,
     spot_auth_funding: Funding,
     spot_auth_trade: Trade,
     spot_auth_user: User,
     spot_auth_staking: Staking,
 ) -> None:
@@ -57,10 +59,11 @@
 
     with spot_auth_user as user:
         assert is_not_error(user.get_account_balance())
 
     with spot_auth_staking as staking:
         assert isinstance(staking.get_pending_staking_transactions(), list)
 
-    with spot_auth_trade as trade:
-        with pytest.raises(KrakenException.KrakenPermissionDeniedError):
-            trade.cancel_order(txid="OB6JJR-7NZ5P-N5SKCB")
+    with spot_auth_trade as trade, pytest.raises(
+        KrakenException.KrakenPermissionDeniedError,
+    ):
+        trade.cancel_order(txid="OB6JJR-7NZ5P-N5SKCB")
```

### Comparing `python-kraken-sdk-1.5.0/tests/spot/test_spot_funding.py` & `python-kraken-sdk-1.6.0/tests/spot/test_spot_funding.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,120 +12,126 @@
 from kraken.spot import Funding
 
 from .helper import is_not_error
 
 # todo: Mock skipped tests - or is this to dangerous?
 
 
-@pytest.mark.spot
-@pytest.mark.spot_auth
-@pytest.mark.spot_funding
+@pytest.mark.spot()
+@pytest.mark.spot_auth()
+@pytest.mark.spot_funding()
 def test_get_deposit_methods(spot_auth_funding: Funding) -> None:
     """
     Checks if the response of the ``get_deposit_methods`` is of
     type list which mean that the request was successful.
     """
     assert isinstance(spot_auth_funding.get_deposit_methods(asset="XBT"), list)
 
 
-@pytest.mark.spot
-@pytest.mark.spot_auth
-@pytest.mark.spot_funding
+@pytest.mark.spot()
+@pytest.mark.spot_auth()
+@pytest.mark.spot_funding()
 def test_get_deposit_address(spot_auth_funding: Funding) -> None:
     """
     Checks the ``get_deposit_address`` function by performing a valid request
     and validating that the response is of type list.
     """
     assert isinstance(
         spot_auth_funding.get_deposit_address(asset="XBT", method="Bitcoin", new=False),
         list,
     )
 
 
-@pytest.mark.spot
-@pytest.mark.spot_auth
-@pytest.mark.spot_funding
+@pytest.mark.spot()
+@pytest.mark.spot_auth()
+@pytest.mark.spot_funding()
 def test_get_recent_deposits_status(spot_auth_funding: Funding) -> None:
     """
     Checks the ``get_recent_deposit_status`` endpoint by executing multiple
     request with different parameters and validating its return value.
     """
     assert isinstance(spot_auth_funding.get_recent_deposits_status(), list)
     assert isinstance(spot_auth_funding.get_recent_deposits_status(asset="XLM"), list)
     assert isinstance(
-        spot_auth_funding.get_recent_deposits_status(method="Stellar XLM"), list
+        spot_auth_funding.get_recent_deposits_status(method="Stellar XLM"),
+        list,
     )
     assert isinstance(
         spot_auth_funding.get_recent_deposits_status(asset="XLM", method="Stellar XLM"),
         list,
     )
 
 
-@pytest.mark.spot
-@pytest.mark.spot_auth
-@pytest.mark.spot_funding
+@pytest.mark.spot()
+@pytest.mark.spot_auth()
+@pytest.mark.spot_funding()
 @pytest.mark.skip(reason="CI does not have withdraw permission")
 def test_withdraw_funds(spot_auth_funding: Funding) -> None:
     """
     Checks the ``withdraw_funds`` endpoint by performing a withdraw.
 
     This test is disabled, because testing a withdraw cannot be done without
     a real withdraw which is not what should be done here. Also the
     API keys for testing are not allowed to withdraw or trade.
     """
     with pytest.raises(KrakenException.KrakenPermissionDeniedError):
         assert is_not_error(
             spot_auth_funding.withdraw_funds(
-                asset="XLM", key="enter-withdraw-key", amount=10000000
-            )
+                asset="XLM",
+                key="enter-withdraw-key",
+                amount=10000000,
+            ),
         )
 
 
-@pytest.mark.spot
-@pytest.mark.spot_auth
-@pytest.mark.spot_funding
+@pytest.mark.spot()
+@pytest.mark.spot_auth()
+@pytest.mark.spot_funding()
 @pytest.mark.skip(reason="CI does not have withdraw permission")
 def test_get_withdrawal_info(spot_auth_funding: Funding) -> None:
     """
     Checks the ``get_withdraw_info`` endpoint by requesting the data.
 
     This test is disabled, because the API keys for testing are not
     allowed to withdraw or trade or even get withdraw information.
     """
     with pytest.raises(KrakenException.KrakenPermissionDeniedError):
         assert is_not_error(
             spot_auth_funding.get_withdrawal_info(
-                asset="XLM", amount=10000000, key="enter-withdraw-key"
-            )
+                asset="XLM",
+                amount=10000000,
+                key="enter-withdraw-key",
+            ),
         )
 
 
-@pytest.mark.spot
-@pytest.mark.spot_auth
-@pytest.mark.spot_funding
+@pytest.mark.spot()
+@pytest.mark.spot_auth()
+@pytest.mark.spot_funding()
 @pytest.mark.skip(reason="CI does not have withdraw permission")
 def test_get_recent_withdraw_status(spot_auth_funding: Funding) -> None:
     """
     Checks the ``get_recent_withdraw_status`` endpoint using different arguments.
 
     This test is disabled, because testing a withdraw and receiving
     withdrawal information cannot be done without a real withdraw which is not what
     should be done here. Also the  API keys for testing are not allowed to withdraw
     or trade.
     """
     assert isinstance(spot_auth_funding.get_recent_withdraw_status(), list)
     assert isinstance(spot_auth_funding.get_recent_withdraw_status(asset="XLM"), list)
     assert isinstance(
-        spot_auth_funding.get_recent_withdraw_status(method="Stellar XLM"), list
+        spot_auth_funding.get_recent_withdraw_status(method="Stellar XLM"),
+        list,
     )
 
 
-@pytest.mark.spot
-@pytest.mark.spot_auth
-@pytest.mark.spot_funding
+@pytest.mark.spot()
+@pytest.mark.spot_auth()
+@pytest.mark.spot_funding()
 @pytest.mark.skip(reason="CI does not have withdraw permission")
 def test_wallet_transfer(spot_auth_funding: Funding) -> None:
     """
     Checks the ``get_recent_withdraw_status`` endpoint using different arguments.
     (only works if futures wallet exists)
 
     This test is disabled, because testing a withdraw and receiving
@@ -134,10 +140,13 @@
     or trade.
 
     This endpoint is broken, even the provided example on the kraken doc does not work.
     """
     with pytest.raises(KrakenException.KrakenInvalidArgumentsError):
         assert is_not_error(
             spot_auth_funding.wallet_transfer(
-                asset="XLM", from_="Futures Wallet", to_="Spot Wallet", amount=10000
-            )
+                asset="XLM",
+                from_="Futures Wallet",
+                to_="Spot Wallet",
+                amount=10000,
+            ),
         )
```

### Comparing `python-kraken-sdk-1.5.0/tests/spot/test_spot_market.py` & `python-kraken-sdk-1.6.0/tests/spot/test_spot_market.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,27 +11,27 @@
 import pytest
 
 from kraken.spot import Market
 
 from .helper import is_not_error
 
 
-@pytest.mark.spot
-@pytest.mark.spot_market
+@pytest.mark.spot()
+@pytest.mark.spot_market()
 def test_get_system_status(spot_market: Market) -> None:
     """
     Checks the ``get_system_status`` endpoint by performing a
     valid request and validating that the response does not
     contain the error key.
     """
     assert is_not_error(spot_market.get_system_status())
 
 
-@pytest.mark.spot
-@pytest.mark.spot_market
+@pytest.mark.spot()
+@pytest.mark.spot_market()
 def test_get_assets(spot_market: Market) -> None:
     """
     Checks the ``get_assets`` endpoint by performing multiple
     requests with different parameters and
     validating that the response does not contain the error key.
     """
     for params in (
@@ -41,16 +41,16 @@
         {"assets": ["XBT,USD"]},
         {"assets": ["XBT", "USD"], "aclass": "currency"},
     ):
         assert is_not_error(spot_market.get_assets(**params))
     sleep(3)
 
 
-@pytest.mark.spot
-@pytest.mark.spot_market
+@pytest.mark.spot()
+@pytest.mark.spot_market()
 def test_get_asset_pairs(spot_market: Market) -> None:
     """
     Checks the ``get_asset_pairs`` endpoint by performing multiple
     requests with different parameters and validating that the response
     does not contain the error key.
     """
     assert is_not_error(spot_market.get_asset_pairs())
@@ -58,74 +58,74 @@
     assert is_not_error(spot_market.get_asset_pairs(pair=["DOTEUR", "BTCUSD"]))
     for i in ("info", "leverage", "fees", "margin"):
         assert is_not_error(spot_market.get_asset_pairs(pair="DOTEUR", info=i))
         break  # there is no reason for requesting more - but this loop is just for info
     sleep(3)
 
 
-@pytest.mark.spot
-@pytest.mark.spot_market
+@pytest.mark.spot()
+@pytest.mark.spot_market()
 def test_get_ticker(spot_market: Market) -> None:
     """
     Checks the ``get_ticker`` endpoint by performing multiple
     requests with different paramaters and validating that the response
     does not contain the error key.
     """
     assert is_not_error(spot_market.get_ticker())
     assert is_not_error(spot_market.get_ticker(pair="XBTUSD"))
     assert is_not_error(spot_market.get_ticker(pair=["DOTUSD", "XBTUSD"]))
 
 
-@pytest.mark.spot
-@pytest.mark.spot_market
+@pytest.mark.spot()
+@pytest.mark.spot_market()
 def test_get_ohlc(spot_market: Market) -> None:
     """
     Checks the ``get_ohlc`` endpoint by performing multiple
     requests with different parameters and validating that the response
     does not contain the error key.
     """
     assert is_not_error(spot_market.get_ohlc(pair="XBTUSD"))
     assert is_not_error(
-        spot_market.get_ohlc(pair="XBTUSD", interval=240, since="1616663618")
+        spot_market.get_ohlc(pair="XBTUSD", interval=240, since="1616663618"),
     )  # interval in [1 5 15 30 60 240 1440 10080 21600]
 
 
-@pytest.mark.spot
-@pytest.mark.spot_market
+@pytest.mark.spot()
+@pytest.mark.spot_market()
 def test_get_order_book(spot_market: Market) -> None:
     """
     Checks the ``get_order_book`` endpoint by performing multiple
     requests with different parameters and validating that the response
     does not contain the error key.
     """
     assert is_not_error(spot_market.get_order_book(pair="XBTUSD"))
     assert is_not_error(
-        spot_market.get_order_book(pair="XBTUSD", count=2)
+        spot_market.get_order_book(pair="XBTUSD", count=2),
     )  # count in [1...500]
 
 
-@pytest.mark.spot
-@pytest.mark.spot_market
+@pytest.mark.spot()
+@pytest.mark.spot_market()
 def test_get_recent_trades(spot_market: Market) -> None:
     """
     Checks the ``get_recent_trades`` endpoint by performing multiple
     requests with different parameters and validating that the response
     does not contain the error key.
     """
     assert is_not_error(spot_market.get_recent_trades(pair="XBTUSD"))
     assert is_not_error(
-        spot_market.get_recent_trades(pair="XBTUSD", since="1616663618")
+        spot_market.get_recent_trades(pair="XBTUSD", since="1616663618", count=2),
     )
 
 
-@pytest.mark.spot
-@pytest.mark.spot_market
+@pytest.mark.spot()
+@pytest.mark.spot_market()
 def test_get_recent_spreads(spot_market: Market) -> None:
     """
     Checks the ``get_recent_spreads`` endpoint by performing multiple
     requests with different parameters and validating that the response
     does not contain the error key.
     """
     assert is_not_error(spot_market.get_recent_spreads(pair="XBTUSD"))
     assert is_not_error(
-        spot_market.get_recent_spreads(pair="XBTUSD", since="1616663618")
+        spot_market.get_recent_spreads(pair="XBTUSD", since="1616663618"),
     )
```

### Comparing `python-kraken-sdk-1.5.0/tests/spot/test_spot_orderbook.py` & `python-kraken-sdk-1.6.0/tests/spot/test_spot_orderbook.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,150 +4,155 @@
 # GitHub: https://github.com/btschwertfeger
 #
 
 """
 Module that implements the unit tests regarding the Spot Orderbook client.
 """
 
+from __future__ import annotations
+
 import asyncio
 import json
 import os
 from collections import OrderedDict
 from typing import Any, Optional
 from unittest import mock
 
 import pytest
 
 from kraken.spot import OrderbookClient
 
 from .helper import FIXTURE_DIR, OrderbookClientWrapper, async_wait
 
 
-@pytest.mark.spot
-@pytest.mark.spot_websocket
-@pytest.mark.spot_orderbook
+@pytest.mark.spot()
+@pytest.mark.spot_websocket()
+@pytest.mark.spot_orderbook()
 def test_create_public_bot(caplog: Any) -> None:
     """
     Checks if the websocket client can be instantiated.
     """
 
     async def create_bot() -> None:
         orderbook: OrderbookClientWrapper = OrderbookClientWrapper()
         await async_wait(seconds=4)
 
         assert orderbook.depth == 10
 
     asyncio.run(create_bot())
 
     for expected in (
-        "'connectionID",
-        "'event': 'systemStatus', 'status': 'online'",
-        "'event': 'pong', 'reqid':",
+        'channel": "status"',
+        '"api_version": "v2"',
+        '"system": "online", "version": "2.',
+        '"type": "update"',
     ):
         assert expected in caplog.text
-    assert "Kraken websockets at full capacity, try again later" not in caplog.text
 
 
-@pytest.mark.spot
-@pytest.mark.spot_websocket
-@pytest.mark.spot_orderbook
+@pytest.mark.spot()
+@pytest.mark.spot_websocket()
+@pytest.mark.spot_orderbook()
 def test_get_first() -> None:
     """
     Checks the ``get_first`` method.
     """
 
     assert (
         float(10)
         == OrderbookClientWrapper.get_first(("10", "5"))
         == OrderbookClientWrapper.get_first((10, 5))
     )
 
 
-@mock.patch("kraken.spot.orderbook.KrakenSpotWSClient", return_value=None)
-@pytest.mark.spot
-@pytest.mark.spot_orderbook
-def test_assing_msg_and_validate_checksum(mock_ws_client: mock.MagicMock) -> None:
+@mock.patch("kraken.spot.orderbook.KrakenSpotWSClientV2", return_value=None)
+@pytest.mark.spot()
+@pytest.mark.spot_orderbook()
+def test_passing_msg_and_validate_checksum(mock_ws_client: mock.MagicMock) -> None:
     """
     This function checks if the initial snapshot and the book updates are
     assigned correctly so that the checksum calculation can validate the
     assigned book updates and values.
     """
     with open(
-        os.path.join(FIXTURE_DIR, "orderbook.json"), "r", encoding="utf-8"
+        os.path.join(FIXTURE_DIR, "orderbook.json"),
+        "r",
+        encoding="utf-8",
     ) as json_file:
         orderbook: dict = json.load(json_file)
 
     async def assign() -> None:
         client: OrderbookClient = OrderbookClient(depth=10)
 
-        await client.on_message(msg=orderbook["init"])
-        assert client.get(pair="XBT/USD")["valid"]
+        await client.on_message(message=orderbook["init"])
+        assert client.get(pair="BTC/USD")["valid"]
 
         for update in orderbook["updates"]:
-            await client.on_message(msg=update)
-            assert client.get(pair="XBT/USD")["valid"]
+            await client.on_message(message=update)
+            assert client.get(pair="BTC/USD")["valid"]
 
     asyncio.run(assign())
 
 
-@pytest.mark.spot
-@pytest.mark.spot_websocket
-@pytest.mark.spot_orderbook
+@pytest.mark.spot()
+@pytest.mark.spot_websocket()
+@pytest.mark.spot_orderbook()
 def test_add_book(caplog: Any) -> None:
     """
     Checks if the orderbook client is able to add a book by subscribing.
     The logs are then checked for the expected results.
     """
 
     async def execute_add_book() -> None:
         orderbook: OrderbookClientWrapper = OrderbookClientWrapper()
 
-        await orderbook.add_book(pairs=["XBT/USD"])
+        await orderbook.add_book(pairs=["BTC/USD"])
         await async_wait(seconds=2)
 
-        book: Optional[dict] = orderbook.get(pair="XBT/USD")
+        book: Optional[dict] = orderbook.get(pair="BTC/USD")
         assert isinstance(book, dict)
 
-        assert all(key in book for key in ("ask", "bid", "valid")), book
+        assert all(
+            key in book
+            for key in ("ask", "bid", "valid", "price_decimals", "qty_decimals")
+        ), book
 
         assert isinstance(book["ask"], OrderedDict)
         assert isinstance(book["bid"], OrderedDict)
 
         for ask, bid in zip(book["ask"], book["bid"]):
             assert isinstance(ask, str)
             assert isinstance(bid, str)
 
     asyncio.run(execute_add_book())
 
     for expected in (
-        "'channelName': 'book-10', 'event': 'subscriptionStatus', 'pair': 'XBT/USD', 'reqid':",
-        "'status': 'subscribed', 'subscription': {'depth': 10, 'name': 'book'}}",
+        '{"method": "subscribe", "result": {"channel": "book", "depth": 10, "snapshot": true, "symbol": "BTC/USD"}, "success": true, "time_in": ',
+        '{"channel": "book", "type": "snapshot", "data": [{"symbol": "BTC/USD", "bids": ',
     ):
         assert expected in caplog.text
 
 
-@pytest.mark.spot
-@pytest.mark.spot_websocket
-@pytest.mark.spot_orderbook
+@pytest.mark.spot()
+@pytest.mark.spot_websocket()
+@pytest.mark.spot_orderbook()
 def test_remove_book(caplog: Any) -> None:
     """
     Checks if the orderbook client is able to add a book by subscribing to a book
     and unsubscribing right after + validating using the logs.
     """
 
     async def execute_remove_book() -> None:
         orderbook: OrderbookClientWrapper = OrderbookClientWrapper()
 
-        await orderbook.add_book(pairs=["XBT/USD"])
+        await orderbook.add_book(pairs=["BTC/USD"])
         await async_wait(seconds=2)
 
-        await orderbook.remove_book(pairs=["XBT/USD"])
+        await orderbook.remove_book(pairs=["BTC/USD"])
         await async_wait(seconds=2)
 
     asyncio.run(execute_remove_book())
 
-    for expected in (
-        "'channelName': 'book-10', 'event': 'subscriptionStatus', 'pair': 'XBT/USD', 'reqid':",
-        "'status': 'subscribed', 'subscription': {'depth': 10, 'name': 'book'}}",
-        "'status': 'unsubscribed', 'subscription': {'depth': 10, 'name': 'book'}}",
-    ):
-        assert expected in caplog.text
+    assert (
+        '{"method": "unsubscribe", "result": {"channel": "book", "depth": 10, "symbol": "BTC/USD"}, "success": true, "time_in":'
+        in caplog.text
+    )
```

### Comparing `python-kraken-sdk-1.5.0/tests/spot/test_spot_staking.py` & `python-kraken-sdk-1.6.0/tests/spot/test_spot_staking.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,93 +4,88 @@
 # GitHub: https://github.com/btschwertfeger
 #
 
 """Module that implements the unit tests for the Spot staking client."""
 
 import pytest
 
-from kraken.exceptions import KrakenException
+from kraken.exceptions import KrakenException  # noqa: F401
 from kraken.spot import Staking
 
-from .helper import is_not_error
+from .helper import is_not_error  # noqa: F401
 
 # todo: Mock skipped tests - or is this to dangerous?
 
 
-@pytest.mark.spot
-@pytest.mark.spot_auth
-@pytest.mark.spot_staking
+@pytest.mark.spot()
+@pytest.mark.spot_auth()
+@pytest.mark.spot_staking()
+@pytest.mark.skip(reason="CI does not have withdraw/stake permission")
 def test_list_stakeable_assets(spot_auth_staking: Staking) -> None:
     """
     Checks if the ``list_stakeable_assets`` endpoint returns the
     expected data type or raises the KrakenException.KrakenPermissionDeniedError.
 
     The error will be raised if some permissions of the API keys are not set.
     """
-    try:
-        assert isinstance(spot_auth_staking.list_stakeable_assets(), list)
-    except KrakenException.KrakenPermissionDeniedError:
-        pass
+    assert isinstance(spot_auth_staking.list_stakeable_assets(), list)
 
 
-@pytest.mark.spot
-@pytest.mark.spot_auth
-@pytest.mark.spot_staking
+@pytest.mark.spot()
+@pytest.mark.spot_auth()
+@pytest.mark.spot_staking()
 @pytest.mark.skip(reason="CI does not have withdraw/stake permission")
 def test_stake_asset(spot_auth_staking: Staking) -> None:
     """
     Checks the ``stake_asset`` endpoint by requesting a stake.
 
     This test is skipped since staking is not the desired result.
     """
-    try:
-        assert is_not_error(
-            spot_auth_staking.stake_asset(
-                asset="DOT", amount="4500000", method="polkadot-staked"
-            )
-        )
-    except KrakenException.KrakenInvalidAmountError:
-        pass
+    # assert is_not_error(
+    #     spot_auth_staking.stake_asset(
+    #         asset="DOT",
+    #         amount="4500000",
+    #         method="polkadot-staked",
+    #     ),
+    # )
 
 
-@pytest.mark.spot
-@pytest.mark.spot_auth
-@pytest.mark.spot_staking
+@pytest.mark.spot()
+@pytest.mark.spot_auth()
+@pytest.mark.spot_staking()
 @pytest.mark.skip(reason="CI does not have withdraw/stake permission")
 def test_unstake_asset(spot_auth_staking: Staking) -> None:
     """
     Checks if the ``unstake_asset`` endpoints returns a response that does
     not contain the error key.
 
     This test is skipped since unstaking is not wanted in the CI.
     """
-    try:
-        assert is_not_error(
-            spot_auth_staking.unstake_asset(asset="DOT", amount="4500000")
-        )
-    except KrakenException.KrakenInvalidAmountError:
-        pass
+    # with pytest.raises(KrakenException.KrakenPermissionDeniedError, "API key doesn't have permission to make this request."):
+    # assert is_not_error(
+    #     spot_auth_staking.unstake_asset(asset="DOT", amount="4500000"),
+    # )
 
 
-@pytest.mark.spot
-@pytest.mark.spot_auth
-@pytest.mark.spot_staking
+@pytest.mark.spot()
+@pytest.mark.spot_auth()
+@pytest.mark.spot_staking()
 @pytest.mark.skip(reason="CI does not have withdraw/stake permission")
 def test_get_pending_staking_transactions(spot_auth_staking: Staking) -> None:
     """
     Checks the ``get_pending_staking_transactions`` endpoint by validating
     that the response is of type list. This test is also skipped since
     the withdraw/stake permission is not set on the CI api keys.
     """
     assert isinstance(spot_auth_staking.get_pending_staking_transactions(), list)
 
 
-@pytest.mark.spot
-@pytest.mark.spot_auth
-@pytest.mark.spot_staking
+@pytest.mark.spot()
+@pytest.mark.spot_auth()
+@pytest.mark.spot_staking()
 @pytest.mark.skip(reason="CI does not have withdraw/stake permission")
 def test_list_staking_transactions(spot_auth_staking: Staking) -> None:
     """
     Checks the ``list_staking_transactions`` endpoint by performing a regular
     request. This test is skipped since the CI API keys do not have the
     withdraw/stake permission.
     """
```

### Comparing `python-kraken-sdk-1.5.0/tests/spot/test_spot_trade.py` & `python-kraken-sdk-1.6.0/tests/spot/test_spot_trade.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 
 from kraken.exceptions import KrakenException
 from kraken.spot import Trade
 
 # todo: Mock skipped tests - or is this to dangerous?
 
 
-@pytest.mark.spot
-@pytest.mark.spot_auth
-@pytest.mark.spot_trade
+@pytest.mark.spot()
+@pytest.mark.spot_auth()
+@pytest.mark.spot_trade()
 def test_create_order(spot_auth_trade: Trade) -> None:
     """
     This test checks the ``create_order`` function by performing
     calls to create an order - but in validate mode - so that
     no real order is placed. The KrakenException.KrakenPermissionDeniedError
     will be raised since the CI does not have trade permission.
     """
@@ -75,16 +75,19 @@
                 close_price="123",
                 close_price2="92",
                 validate=True,
             ),
             dict,
         )
 
-    with pytest.raises(KrakenException.KrakenPermissionDeniedError):
-        deadline = (datetime.now(timezone.utc) + timedelta(seconds=20)).isoformat()
+    deadline = (datetime.now(timezone.utc) + timedelta(seconds=20)).isoformat()
+    with pytest.raises(
+        KrakenException.KrakenPermissionDeniedError,
+        match=r"API key doesn't have permission to make this request.",
+    ):
         spot_auth_trade.create_order(
             ordertype="stop-loss-limit",
             pair="XBTUSD",
             side="buy",
             volume=0.001,
             price=25000,
             price2=27000,
@@ -92,39 +95,42 @@
             trigger="last",
             timeinforce="GTC",
             leverage=4,
             deadline=deadline,
         )
 
 
-@pytest.mark.spot
-@pytest.mark.spot_auth
-@pytest.mark.spot_trade
+@pytest.mark.spot()
+@pytest.mark.spot_auth()
+@pytest.mark.spot_trade()
 def test_failing_create_order(spot_auth_trade: Trade) -> None:
     """
     Test that checks if the ``create_order`` function raises a ValueError
     because of missing or invalid parameters.
     > stop-loss-limit (and take-profit-limit) require a second price ``price2``)
     """
-    with pytest.raises(ValueError):
+    with pytest.raises(
+        ValueError,
+        match=r"Ordertype stop-loss-limit requires a secondary price \(price2\)!",
+    ):
         spot_auth_trade.create_order(
             ordertype="stop-loss-limit",
             pair="XBTUSD",
             side="buy",
             volume=0.001,
             price=25000,
             timeinforce="GTC",
             leverage=4,
             validate=True,
         )
 
 
-@pytest.mark.spot
-@pytest.mark.spot_auth
-@pytest.mark.spot_trade
+@pytest.mark.spot()
+@pytest.mark.spot_auth()
+@pytest.mark.spot_trade()
 def test_create_order_batch(spot_auth_trade: Trade) -> None:
     """
     Checks the ``create_order_batch`` function by executing
     a batch order in validate mode. (Permission denied,
     since the CI does not have trade permissions)
     """
     with pytest.raises(KrakenException.KrakenPermissionDeniedError):
@@ -154,17 +160,17 @@
                 },
             ],
             pair="BTC/USD",
             validate=True,  # important
         )
 
 
-@pytest.mark.spot
-@pytest.mark.spot_auth
-@pytest.mark.spot_trade
+@pytest.mark.spot()
+@pytest.mark.spot_auth()
+@pytest.mark.spot_trade()
 def test_edit_order(spot_auth_trade: Trade) -> None:
     """
     Test the ``edit_order`` function by editing an order.
 
     KrakenException.KrakenPermissionDeniedError: since CI does not have
     trade permissions. If the request would be malformed, another
     exception could be observed.
@@ -180,83 +186,83 @@
             cancel_response=False,
             truncate=True,
             oflags=["post"],
             validate=True,
         )
 
 
-@pytest.mark.spot
-@pytest.mark.spot_auth
-@pytest.mark.spot_trade
+@pytest.mark.spot()
+@pytest.mark.spot_auth()
+@pytest.mark.spot_trade()
 def test_cancel_order(spot_auth_trade: Trade) -> None:
     """
     Checks the ``cancel_order`` function by canceling an order.
 
     A KrakenException.KrakenPermissionDeniedError is expected since CI keys are
     not allowed to trade/cancel/withdraw/stake.
     """
     with pytest.raises(KrakenException.KrakenPermissionDeniedError):
         spot_auth_trade.cancel_order(txid="OB6JJR-7NZ5P-N5SKCB")
 
 
-@pytest.mark.spot
-@pytest.mark.spot_auth
-@pytest.mark.spot_trade
+@pytest.mark.spot()
+@pytest.mark.spot_auth()
+@pytest.mark.spot_trade()
 @pytest.mark.skip(reason="CI does not have trade/cancel permission")
 def test_cancel_all_orders(spot_auth_trade: Trade) -> None:
     """
     Checks the ``cancel_all_orders`` endpoint by executing the function.
     A KrakenException.KrakenPermissionDeniedError will be raised since the CI API keys
     do not have cancel permission.
     """
     with pytest.raises(KrakenException.KrakenPermissionDeniedError):
         assert isinstance(spot_auth_trade.cancel_all_orders(), dict)
 
 
-@pytest.mark.spot
-@pytest.mark.spot_auth
-@pytest.mark.spot_trade
+@pytest.mark.spot()
+@pytest.mark.spot_auth()
+@pytest.mark.spot_trade()
 @pytest.mark.skip(reason="CI does not have trade/cancel permission")
 def test_cancel_all_orders_after_x(spot_auth_trade: Trade) -> None:
     """
     Checks the ``cancel_all_orders_after_x`` function by validating its response data
     type.
 
     THe KrakenException.KrakenPermissionDeniedError will be caught since the CI API keys are not
     allowed to cancel orders.
     """
     with pytest.raises(KrakenException.KrakenPermissionDeniedError):
         assert isinstance(spot_auth_trade.cancel_all_orders_after_x(timeout=0), dict)
 
 
-@pytest.mark.spot
-@pytest.mark.spot_auth
-@pytest.mark.spot_trade
+@pytest.mark.spot()
+@pytest.mark.spot_auth()
+@pytest.mark.spot_trade()
 def test_cancel_order_batch(spot_auth_trade: Trade) -> None:
     """
     Tests the ``cancel_order_batch`` function by cancelling dummy orders that
     do not exist anymore. Error will be raised since the CI do not have trade
     permissions.
     """
     with pytest.raises(KrakenException.KrakenPermissionDeniedError):
         assert isinstance(
             spot_auth_trade.cancel_order_batch(
                 orders=[
                     "O2JLFP-VYFIW-35ZAAE",
                     "O523KJ-DO4M2-KAT243",
                     "OCDIAL-YC66C-DOF7HS",
                     "OVFPZ2-DA2GV-VBFVVI",
-                ]
+                ],
             ),
             dict,
         )
 
 
-@pytest.mark.spot
-@pytest.mark.spot_trade
+@pytest.mark.spot()
+@pytest.mark.spot_trade()
 def test_truncate_price(spot_trade: Trade) -> None:
     """
     Checks if the truncate function returns the expected results by
     checking different inputs for price.
 
     NOTE: This test may break in the future since the lot_decimals, pair_decimals,
     ordermin and costmin attributes could change.
@@ -282,16 +288,16 @@
         assert (
             spot_trade.truncate(amount=price, amount_type="price", pair="DOTUSD")
             == expected
         )
     sleep(3)
 
 
-@pytest.mark.spot
-@pytest.mark.spot_trade
+@pytest.mark.spot()
+@pytest.mark.spot_trade()
 def test_truncate_volume(spot_trade: Trade) -> None:
     """
     Checks if the truncate function returns the expected results by
     checking different inputs for volume.
 
     NOTE: This test may break in the future since the lot_decimals, pair_decimals,
     ordermin and costmin attributes could change.
@@ -317,41 +323,41 @@
         assert (
             spot_trade.truncate(amount=volume, amount_type="volume", pair="DOTUSD")
             == expected
         )
     sleep(3)
 
 
-@pytest.mark.spot
-@pytest.mark.spot_trade
+@pytest.mark.spot()
+@pytest.mark.spot_trade()
 def test_truncate_fail_price_costmin(spot_trade: Trade) -> None:
     """
     Checks if the truncate function fails if the price is less than the costmin.
 
     NOTE: This test may break in the future since the lot_decimals, pair_decimals,
     ordermin and costmin attributes could change.
     """
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match=r"Price is less than the costmin: 0.5!"):
         spot_trade.truncate(amount=0.001, amount_type="price", pair="XBTUSD")
 
 
-@pytest.mark.spot
-@pytest.mark.spot_trade
+@pytest.mark.spot()
+@pytest.mark.spot_trade()
 def test_truncate_fail_volume_ordermin(spot_trade: Trade) -> None:
     """
     Checks if the truncate function fails if the volume is less than the ordermin.
 
     NOTE: This test may break in the future since the lot_decimals, pair_decimals,
     ordermin and costmin attributes could change.
     """
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match=r"Volume is less than the ordermin: 0.0001!"):
         spot_trade.truncate(amount=0.00001, amount_type="volume", pair="XBTUSD")
 
 
-@pytest.mark.spot
-@pytest.mark.spot_trade
+@pytest.mark.spot()
+@pytest.mark.spot_trade()
 def test_truncate_fail_invalid_amount_type(spot_trade: Trade) -> None:
     """
     Checks if the truncate function fails when no valid ``amount_type`` was specified.
     """
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match=r"Amount type must be 'volume' or 'price'!"):
         spot_trade.truncate(amount=1, amount_type="invalid", pair="XBTUSD")
```

### Comparing `python-kraken-sdk-1.5.0/tests/spot/test_spot_user.py` & `python-kraken-sdk-1.6.0/tests/spot/test_spot_user.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,52 +5,53 @@
 #
 
 """Module that implements the unit tests for the Spot user client."""
 
 import os
 import random
 import tempfile
+from contextlib import suppress
 from time import sleep, time
 from unittest import mock
 
 import pytest
 
 from kraken.exceptions import KrakenException
 from kraken.spot import User
 
 from .helper import is_not_error
 
 
-@pytest.mark.spot
-@pytest.mark.spot_auth
-@pytest.mark.spot_user
+@pytest.mark.spot()
+@pytest.mark.spot_auth()
+@pytest.mark.spot_user()
 def test_get_account_balance(spot_auth_user: User) -> None:
     """
     Checks the ``get_account_balance`` function by validating that
     the response do not contain the error key.
     """
     assert is_not_error(spot_auth_user.get_account_balance())
 
 
-@pytest.mark.spot
-@pytest.mark.spot_auth
-@pytest.mark.spot_user
+@pytest.mark.spot()
+@pytest.mark.spot_auth()
+@pytest.mark.spot_user()
 def test_get_balances(spot_auth_user: User) -> None:
     """
     Checks the ``get_balances`` function by validating that
     the response do not contain the error key.
     """
     result: dict = spot_auth_user.get_balances()
     assert isinstance(result, dict)
     assert is_not_error(result)
 
 
-@pytest.mark.spot
-@pytest.mark.spot_auth
-@pytest.mark.spot_user
+@pytest.mark.spot()
+@pytest.mark.spot_auth()
+@pytest.mark.spot_user()
 @mock.patch.object(
     User,
     "get_balances",
     return_value={
         "XXLM": {"balance": "0.00000000", "hold_trade": "0.00000000"},
         "ZEUR": {"balance": "500.0000", "hold_trade": "0.0000"},
         "XXBT": {"balance": "2.1031709100", "hold_trade": "0.1401000000"},
@@ -67,73 +68,76 @@
     assert result == {
         "currency": "XXBT",
         "balance": 2.1031709100,
         "available_balance": 1.96307091,
     }
 
 
-@pytest.mark.spot
-@pytest.mark.spot_auth
-@pytest.mark.spot_user
+@pytest.mark.spot()
+@pytest.mark.spot_auth()
+@pytest.mark.spot_user()
 def test_get_trade_balance(spot_auth_user: User) -> None:
     """
     Checks the ``get_trade_balances`` function by validating that
     the response do not contain the error key.
 
     (sleep since we don't want API rate limit error...)
     """
     sleep(3)
     assert is_not_error(spot_auth_user.get_trade_balance())
     assert is_not_error(spot_auth_user.get_trade_balance(asset="EUR"))
 
 
-@pytest.mark.spot
-@pytest.mark.spot_auth
-@pytest.mark.spot_user
+@pytest.mark.spot()
+@pytest.mark.spot_auth()
+@pytest.mark.spot_user()
 def test_get_open_orders(spot_auth_user: User) -> None:
     """
     Checks the ``get_open_orders`` function by validating that
     the response do not contain the error key.
     """
     assert is_not_error(spot_auth_user.get_open_orders(trades=True))
     assert is_not_error(spot_auth_user.get_open_orders(trades=False, userref="1234567"))
 
 
-@pytest.mark.spot
-@pytest.mark.spot_auth
-@pytest.mark.spot_user
+@pytest.mark.spot()
+@pytest.mark.spot_auth()
+@pytest.mark.spot_user()
 def test_get_closed_orders(spot_auth_user: User) -> None:
     """
     Checks the ``get_closed_orders`` function by validating that
     the responses do not contain the error key.
     """
     assert is_not_error(spot_auth_user.get_closed_orders())
     assert is_not_error(spot_auth_user.get_closed_orders(trades=True, userref="1234"))
     assert is_not_error(
-        spot_auth_user.get_closed_orders(trades=True, start="1668431675.4778206")
+        spot_auth_user.get_closed_orders(trades=True, start="1668431675.4778206"),
     )
     assert is_not_error(
         spot_auth_user.get_closed_orders(
-            trades=True, start="1668431675.4778206", end="1668455555.4778206", ofs=2
-        )
+            trades=True,
+            start="1668431675.4778206",
+            end="1668455555.4778206",
+            ofs=2,
+        ),
     )
     assert is_not_error(
         spot_auth_user.get_closed_orders(
             trades=True,
             start="1668431675.4778206",
             end="1668455555.4778206",
             ofs=1,
             closetime="open",
-        )
+        ),
     )
 
 
-@pytest.mark.spot
-@pytest.mark.spot_auth
-@pytest.mark.spot_user
+@pytest.mark.spot()
+@pytest.mark.spot_auth()
+@pytest.mark.spot_user()
 def test_get_trades_info(spot_auth_user: User) -> None:
     """
     Checks the ``get_trades_info`` function by validating that
     the responses do not contain the error key.
     """
     for params, method in zip(
         (
@@ -153,17 +157,17 @@
             assert is_not_error(method(**params))
         except KrakenException.KrakenInvalidOrderError:
             pass
         finally:
             sleep(2)
 
 
-@pytest.mark.spot
-@pytest.mark.spot_auth
-@pytest.mark.spot_user
+@pytest.mark.spot()
+@pytest.mark.spot_auth()
+@pytest.mark.spot_user()
 def test_get_orders_info(spot_auth_user: User) -> None:
     """
     Checks the ``get_orders_info`` function by validating that
     the responses do not contain the error key.
     """
     for params, method in zip(
         (
@@ -183,119 +187,127 @@
             assert is_not_error(method(**params))
         except KrakenException.KrakenInvalidOrderError:
             pass
         finally:
             sleep(2)
 
 
-@pytest.mark.spot
-@pytest.mark.spot_auth
-@pytest.mark.spot_user
+@pytest.mark.spot()
+@pytest.mark.spot_auth()
+@pytest.mark.spot_user()
 def test_get_trades_history(spot_auth_user: User) -> None:
     """
     Checks the ``get_trades_history`` function by validating that
     the responses do not contain the error key.
     """
     sleep(3)
     assert is_not_error(spot_auth_user.get_trades_history(type_="all", trades=True))
     assert is_not_error(
         spot_auth_user.get_trades_history(
             type_="closed position",
             start="1677717104",
             end="1677817104",
             ofs="1",
-        )
+        ),
     )
 
 
-@pytest.mark.spot
-@pytest.mark.spot_auth
-@pytest.mark.spot_user
+@pytest.mark.spot()
+@pytest.mark.spot_auth()
+@pytest.mark.spot_user()
 def test_get_open_positions(spot_auth_user: User) -> None:
     """
     Checks the ``get_open_positions`` function by validating that
     the responses do not contain the error key.
     """
     assert isinstance(spot_auth_user.get_open_positions(), list)
     assert isinstance(
-        spot_auth_user.get_open_positions(txid="OQQYNL-FXCFA-FBFVD7"), list
+        spot_auth_user.get_open_positions(txid="OQQYNL-FXCFA-FBFVD7"),
+        list,
     )
     assert isinstance(
         spot_auth_user.get_open_positions(txid="OQQYNL-FXCFA-FBFVD7", docalcs=True),
         list,
     )
 
 
-@pytest.mark.spot
-@pytest.mark.spot_auth
-@pytest.mark.spot_user
+@pytest.mark.spot()
+@pytest.mark.spot_auth()
+@pytest.mark.spot_user()
 def test_get_ledgers_info(spot_auth_user: User) -> None:
     """
     Checks the ``get_ledgers_info`` function by validating that
     the responses do not contain the error key.
     """
     assert is_not_error(spot_auth_user.get_ledgers_info())
     assert is_not_error(spot_auth_user.get_ledgers_info(type_="deposit"))
     assert is_not_error(
         spot_auth_user.get_ledgers_info(
-            asset="EUR", start="1668431675.4778206", end="1668455555.4778206", ofs=2
-        )
+            asset="EUR",
+            start="1668431675.4778206",
+            end="1668455555.4778206",
+            ofs=2,
+        ),
     )
     assert is_not_error(
         spot_auth_user.get_ledgers_info(
             asset=["EUR", "USD"],
-        )
+        ),
     )
     assert is_not_error(
         spot_auth_user.get_ledgers_info(
             asset="EUR,USD",
-        )
+        ),
     )
 
 
-@pytest.mark.spot
-@pytest.mark.spot_auth
-@pytest.mark.spot_user
+@pytest.mark.spot()
+@pytest.mark.spot_auth()
+@pytest.mark.spot_user()
 def test_get_ledgers(spot_auth_user: User) -> None:
     """
     Checks the ``get_ledgers`` function by validating that
     the responses do not contain the error key.
     """
     assert is_not_error(spot_auth_user.get_ledgers(id_="LNYQGU-SUR5U-UXTOWM"))
     assert is_not_error(
         spot_auth_user.get_ledgers(
-            id_=["LNYQGU-SUR5U-UXTOWM", "LTCMN2-5DZHX-6CPRC4"], trades=True
-        )
+            id_=["LNYQGU-SUR5U-UXTOWM", "LTCMN2-5DZHX-6CPRC4"],
+            trades=True,
+        ),
     )
 
 
-@pytest.mark.spot
-@pytest.mark.spot_auth
-@pytest.mark.spot_user
+@pytest.mark.spot()
+@pytest.mark.spot_auth()
+@pytest.mark.spot_user()
 def test_get_trade_volume(spot_auth_user: User) -> None:
     """
     Checks the ``get_trade_volume`` function by validating that
     the responses do not contain the error key.
     """
     assert is_not_error(spot_auth_user.get_trade_volume())
     assert is_not_error(spot_auth_user.get_trade_volume(pair="DOT/EUR", fee_info=False))
 
 
-@pytest.mark.spot
-@pytest.mark.spot_auth
-@pytest.mark.spot_user
+@pytest.mark.spot()
+@pytest.mark.spot_auth()
+@pytest.mark.spot_user()
 def test_request_save_export_report(spot_auth_user: User) -> None:
     """
     Checks the ``save_export_report`` function by requesting an
     report and saving them.
     """
-    with pytest.raises(ValueError):
-        # invalid report type
+    with pytest.raises(
+        ValueError,
+        match=r"`report` must be either \"trades\" or \"ledgers\"",
+    ):
         spot_auth_user.request_export_report(
-            report="invalid", description="this is an invalid report type"
+            report="invalid",
+            description="this is an invalid report type",
         )
 
     for report in ("trades", "ledgers"):
         if report == "trades":
             fields = [
                 "ordertxid",
                 "time",
@@ -325,65 +337,91 @@
             report=report,
             description=export_descr,
             fields=fields,
             format_="CSV",
             starttm="1662100592",
             endtm=int(1000 * time()),
         )
-        assert is_not_error(response) and "id" in response
+        assert is_not_error(response)
+        assert "id" in response
         sleep(2)
 
         status = spot_auth_user.get_export_report_status(report=report)
         assert isinstance(status, list)
         sleep(5)
 
         result = spot_auth_user.retrieve_export(id_=response["id"])
-        with tempfile.TemporaryDirectory() as tmp_dir:
-            with open(os.path.join(tmp_dir, f"{export_descr}.zip"), "wb") as file:
-                for chunk in result.iter_content(chunk_size=512):
-                    if chunk:
-                        file.write(chunk)
+        with tempfile.TemporaryDirectory() as tmp_dir, open(
+            os.path.join(tmp_dir, f"{export_descr}.zip"),
+            "wb",
+        ) as file:
+            for chunk in result.iter_content(chunk_size=512):
+                if chunk:
+                    file.write(chunk)
 
         status = spot_auth_user.get_export_report_status(report=report)
         assert isinstance(status, list)
         for response in status:
             assert "id" in response
-            try:
+            with suppress(Exception):
                 assert isinstance(
                     spot_auth_user.delete_export_report(
-                        id_=response["id"], type_="delete"
+                        id_=response["id"],
+                        type_="delete",
                     ),
                     dict,
                 )
-            except (
-                Exception
-            ):  # '200 - {"error":["WDatabase:No change"],"result":{"delete":true}}'
-                pass
             sleep(2)
 
 
-@pytest.mark.spot
-@pytest.mark.spot_auth
-@pytest.mark.spot_user
+@pytest.mark.spot()
+@pytest.mark.spot_auth()
+@pytest.mark.spot_user()
 def test_export_report_status_invalid(spot_auth_user: User) -> None:
     """
     Checks the ``export_report_status`` function by passing an invalid
     report type.
     """
-    try:
+    with pytest.raises(
+        ValueError,
+        match=r"report must be one of \"trades\", \"ledgers\"",
+    ):
         spot_auth_user.get_export_report_status(report="invalid")
-    except ValueError:
-        pass
 
 
-@pytest.mark.spot
-@pytest.mark.spot_auth
-@pytest.mark.spot_user
-def test_create_subaccount(spot_auth_user: User) -> None:
+@pytest.mark.spot()
+@pytest.mark.spot_auth()
+@pytest.mark.spot_user()
+def test_create_subaccount_failing(spot_auth_user: User) -> None:
     """
     Checks the ``create_subaccount`` function by creating one.
 
-    Creating subaccounts is only available for institutional clients (May 2023),
-    so a KrakenException.KrakenPermissionDeniedError will be raised.
+    Creating subaccounts is only available for institutional clients
+    (July 2023), so a KrakenException.KrakenPermissionDeniedError will be
+    raised.
+
+    todo: test this using a valid account
     """
     with pytest.raises(KrakenException.KrakenPermissionDeniedError):
         spot_auth_user.create_subaccount(email="abc@welt.de", username="tomtucker")
+
+
+@pytest.mark.spot()
+@pytest.mark.spot_auth()
+@pytest.mark.spot_user()
+def test_account_transfer_failing(spot_auth_user: User) -> None:
+    """
+    Checks the ``account_transfer`` function by creating one.
+
+    Transferring funds between subaccounts is only available for institutional
+    clients (July 2023), so a KrakenException.KrakenPermissionDeniedError will
+    be raised.
+
+    todo: test this using a valid account
+    """
+    with pytest.raises(KrakenException.KrakenAuthenticationFailedError):
+        spot_auth_user.account_transfer(
+            asset="XBT",
+            amount=1.0,
+            from_="ABCD 1234 EFGH 5678",
+            to_="JKIL 9012 MNOP 3456",
+        )
```

