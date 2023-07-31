# Comparing `tmp/optitrader-0.0.1.tar.gz` & `tmp/optitrader-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optitrader-0.0.1.tar", max compression
+gzip compressed data, was "optitrader-0.0.2.tar", max compression
```

## Comparing `optitrader-0.0.1.tar` & `optitrader-0.0.2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0     1073 2023-06-21 14:21:29.622704 optitrader-0.0.1/LICENSE
--rw-r--r--   0        0        0     8319 2023-07-31 22:29:17.217224 optitrader-0.0.1/README.md
--rw-r--r--   0        0        0     6611 2023-07-31 22:26:11.131030 optitrader-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      218 2023-07-31 22:16:21.858063 optitrader-0.0.1/src/optitrader/__init__.py
--rw-r--r--   0        0        0     2239 2023-07-31 22:25:43.134379 optitrader-0.0.1/src/optitrader/api.py
--rw-r--r--   0        0        0       87 2023-07-31 22:16:35.718200 optitrader-0.0.1/src/optitrader/app/1_🏠_Home.py
--rw-r--r--   0        0        0      177 2023-07-31 22:16:39.107123 optitrader-0.0.1/src/optitrader/app/__init__.py
--rw-r--r--   0        0        0      248 2023-07-31 22:25:56.769513 optitrader-0.0.1/src/optitrader/app/__pycache__/1_🏠_Home.cpython-310.pyc
--rw-r--r--   0        0        0      389 2023-07-31 22:16:25.132083 optitrader-0.0.1/src/optitrader/app/about.py
--rw-r--r--   0        0        0      518 2023-07-31 22:16:25.132046 optitrader-0.0.1/src/optitrader/app/account.py
--rw-r--r--   0        0        0     1187 2023-07-31 22:16:24.915829 optitrader-0.0.1/src/optitrader/app/backtester.py
--rw-r--r--   0        0        0     3575 2023-07-31 22:25:43.108796 optitrader-0.0.1/src/optitrader/app/explore.py
--rw-r--r--   0        0        0     1305 2023-07-31 22:25:43.071331 optitrader-0.0.1/src/optitrader/app/home.py
--rw-r--r--   0        0        0     1129 2023-07-31 22:16:22.689395 optitrader-0.0.1/src/optitrader/app/page.py
--rw-r--r--   0        0        0      105 2023-07-31 22:16:37.550338 optitrader-0.0.1/src/optitrader/app/pages/2_📈_Backtester.py
--rw-r--r--   0        0        0       96 2023-07-31 22:16:32.677118 optitrader-0.0.1/src/optitrader/app/pages/3_🗺️_Explore.py
--rw-r--r--   0        0        0       96 2023-07-31 22:16:35.747188 optitrader-0.0.1/src/optitrader/app/pages/4_💼_Account.py
--rw-r--r--   0        0        0       90 2023-07-31 22:16:25.026663 optitrader-0.0.1/src/optitrader/app/pages/5_👨🏻‍💻_About.py
--rw-r--r--   0        0        0       12 2023-07-31 19:38:53.710765 optitrader-0.0.1/src/optitrader/app/pages/__init__.py
--rw-r--r--   0        0        0      272 2023-07-31 22:25:57.146093 optitrader-0.0.1/src/optitrader/app/pages/__pycache__/2_📈_Backtester.cpython-310.pyc
--rw-r--r--   0        0        0      266 2023-07-31 22:25:57.157579 optitrader-0.0.1/src/optitrader/app/pages/__pycache__/3_🗺️_Explore.cpython-310.pyc
--rw-r--r--   0        0        0      263 2023-07-31 22:26:01.281761 optitrader-0.0.1/src/optitrader/app/pages/__pycache__/4_💼_Account.cpython-310.pyc
--rw-r--r--   0        0        0      268 2023-07-31 22:26:05.045788 optitrader-0.0.1/src/optitrader/app/pages/__pycache__/5_👨🏻‍💻_About.cpython-310.pyc
--rw-r--r--   0        0        0    24191 2023-07-31 22:29:19.781003 optitrader-0.0.1/src/optitrader/app/session_manager.py
--rw-r--r--   0        0        0    24190 2023-07-31 22:29:17.222694 optitrader-0.0.1/src/optitrader/app/session_manager.py.aeacae1dba05799ae3b187801467b414.tmp
--rw-r--r--   0        0        0     2621 2023-07-31 22:29:45.706649 optitrader-0.0.1/src/optitrader/backtester.py
--rw-r--r--   0        0        0      469 2023-07-31 22:16:21.845724 optitrader-0.0.1/src/optitrader/cli.py
--rw-r--r--   0        0        0     1542 2023-07-31 19:38:53.752242 optitrader-0.0.1/src/optitrader/config.py
--rw-r--r--   0        0        0      422 2023-07-31 22:16:38.897012 optitrader-0.0.1/src/optitrader/enums/__init__.py
--rw-r--r--   0        0        0      228 2023-07-31 22:16:29.794921 optitrader-0.0.1/src/optitrader/enums/backtester.py
--rw-r--r--   0        0        0      736 2023-07-31 19:38:53.803876 optitrader-0.0.1/src/optitrader/enums/iterable.py
--rw-r--r--   0        0        0     1712 2023-07-31 22:16:37.049303 optitrader-0.0.1/src/optitrader/enums/market.py
--rw-r--r--   0        0        0      860 2023-07-31 22:16:24.915822 optitrader-0.0.1/src/optitrader/enums/optimization.py
--rw-r--r--   0        0        0     6667 2023-07-31 22:28:44.554563 optitrader-0.0.1/src/optitrader/main.py
--rw-r--r--   0        0        0      231 2023-07-31 22:16:29.990535 optitrader-0.0.1/src/optitrader/market/__init__.py
--rw-r--r--   0        0        0     8461 2023-07-31 22:25:43.150556 optitrader-0.0.1/src/optitrader/market/alpaca_market_data.py
--rw-r--r--   0        0        0     8460 2023-07-31 22:16:38.373315 optitrader-0.0.1/src/optitrader/market/alpaca_market_data.py.9fafeb33ede105e202d2a274793d58ee.tmp
--rw-r--r--   0        0        0      768 2023-07-31 22:25:43.113539 optitrader-0.0.1/src/optitrader/market/base_data_provider.py
--rw-r--r--   0        0        0       12 2023-07-31 19:38:53.914363 optitrader-0.0.1/src/optitrader/market/db/__init__.py
--rw-r--r--   0        0        0     5339 2023-07-31 22:25:43.129931 optitrader-0.0.1/src/optitrader/market/db/database.py
--rw-r--r--   0        0        0     5338 2023-07-31 22:16:37.469729 optitrader-0.0.1/src/optitrader/market/db/database.py.7b38a0f9e78f0ef64524afe7b2c0c608.tmp
--rw-r--r--   0        0        0     1935 2023-07-31 19:38:53.949530 optitrader-0.0.1/src/optitrader/market/db/models.py
--rw-r--r--   0        0        0       12 2023-07-31 19:38:53.965858 optitrader-0.0.1/src/optitrader/market/db/scripts/__init__.py
--rw-r--r--   0        0        0      743 2023-07-31 22:16:40.153937 optitrader-0.0.1/src/optitrader/market/db/scripts/add_asset.py
--rw-r--r--   0        0        0     1311 2023-07-31 22:25:43.054031 optitrader-0.0.1/src/optitrader/market/db/scripts/create_assets_table.py
--rw-r--r--   0        0        0      733 2023-07-31 22:16:35.747150 optitrader-0.0.1/src/optitrader/market/db/scripts/update_number_of_shares.py
--rw-r--r--   0        0        0     2830 2023-07-31 22:25:43.025856 optitrader-0.0.1/src/optitrader/market/finnhub_market_data.py
--rw-r--r--   0        0        0     3473 2023-07-31 22:25:42.994845 optitrader-0.0.1/src/optitrader/market/investment_universe.py
--rw-r--r--   0        0        0    14240 2023-07-31 22:25:42.966510 optitrader-0.0.1/src/optitrader/market/market_data.py
--rw-r--r--   0        0        0    14239 2023-07-31 22:16:39.723467 optitrader-0.0.1/src/optitrader/market/market_data.py.185a99388c8a3ef51cc2541e94dbdc63.tmp
--rw-r--r--   0        0        0     3330 2023-07-31 22:25:42.927223 optitrader-0.0.1/src/optitrader/market/news.py
--rw-r--r--   0        0        0     4446 2023-07-31 22:25:42.888846 optitrader-0.0.1/src/optitrader/market/trading.py
--rw-r--r--   0        0        0     6381 2023-07-31 22:25:43.077120 optitrader-0.0.1/src/optitrader/market/yahoo_market_data.py
--rw-r--r--   0        0        0      270 2023-07-31 22:16:37.288605 optitrader-0.0.1/src/optitrader/models/__init__.py
--rw-r--r--   0        0        0     2112 2023-07-31 22:25:43.027353 optitrader-0.0.1/src/optitrader/models/asset.py
--rw-r--r--   0        0        0      243 2023-07-31 19:38:54.162170 optitrader-0.0.1/src/optitrader/models/base.py
--rw-r--r--   0        0        0     1962 2023-07-31 22:16:44.855769 optitrader-0.0.1/src/optitrader/models/optimization.py
--rw-r--r--   0        0        0     1962 2023-07-31 22:16:38.241893 optitrader-0.0.1/src/optitrader/models/optimization.py.0f97aab178a762049bd1442f7826f63f.tmp
--rw-r--r--   0        0        0       12 2023-07-31 19:38:54.193302 optitrader-0.0.1/src/optitrader/optimization/__init__.py
--rw-r--r--   0        0        0     7861 2023-07-31 22:25:42.975155 optitrader-0.0.1/src/optitrader/optimization/constraints.py
--rw-r--r--   0        0        0    12717 2023-07-31 22:25:42.953925 optitrader-0.0.1/src/optitrader/optimization/objectives.py
--rw-r--r--   0        0        0     6440 2023-07-31 22:25:42.902512 optitrader-0.0.1/src/optitrader/optimization/solver.py
--rw-r--r--   0        0        0     6510 2023-07-31 22:25:42.870039 optitrader-0.0.1/src/optitrader/portfolio.py
--rw-r--r--   0        0        0        0 2023-07-31 19:38:54.245739 optitrader-0.0.1/src/optitrader/py.typed
--rw-r--r--   0        0        0      203 2023-07-31 22:16:39.107081 optitrader-0.0.1/src/optitrader/utils/__init__.py
--rw-r--r--   0        0        0      953 2023-07-31 19:38:54.294727 optitrader-0.0.1/src/optitrader/utils/utils.py
--rw-r--r--   0        0        0     9610 1970-01-01 00:00:00.000000 optitrader-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-21 14:21:29.622704 optitrader-0.0.2/LICENSE
+-rw-r--r--   0        0        0     8319 2023-07-31 22:37:33.181726 optitrader-0.0.2/README.md
+-rw-r--r--   0        0        0     6611 2023-07-31 22:50:32.353355 optitrader-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      218 2023-07-31 22:31:29.394400 optitrader-0.0.2/src/optitrader/__init__.py
+-rw-r--r--   0        0        0     2239 2023-07-31 22:25:43.134379 optitrader-0.0.2/src/optitrader/api.py
+-rw-r--r--   0        0        0       87 2023-07-31 22:16:35.718200 optitrader-0.0.2/src/optitrader/app/1_🏠_Home.py
+-rw-r--r--   0        0        0      177 2023-07-31 22:16:39.107123 optitrader-0.0.2/src/optitrader/app/__init__.py
+-rw-r--r--   0        0        0      248 2023-07-31 22:25:56.769513 optitrader-0.0.2/src/optitrader/app/__pycache__/1_🏠_Home.cpython-310.pyc
+-rw-r--r--   0        0        0      389 2023-07-31 22:16:25.132083 optitrader-0.0.2/src/optitrader/app/about.py
+-rw-r--r--   0        0        0      518 2023-07-31 22:16:25.132046 optitrader-0.0.2/src/optitrader/app/account.py
+-rw-r--r--   0        0        0     1187 2023-07-31 22:16:24.915829 optitrader-0.0.2/src/optitrader/app/backtester.py
+-rw-r--r--   0        0        0     3575 2023-07-31 22:25:43.108796 optitrader-0.0.2/src/optitrader/app/explore.py
+-rw-r--r--   0        0        0     1305 2023-07-31 22:25:43.071331 optitrader-0.0.2/src/optitrader/app/home.py
+-rw-r--r--   0        0        0     1129 2023-07-31 22:16:22.689395 optitrader-0.0.2/src/optitrader/app/page.py
+-rw-r--r--   0        0        0      105 2023-07-31 22:16:37.550338 optitrader-0.0.2/src/optitrader/app/pages/2_📈_Backtester.py
+-rw-r--r--   0        0        0       96 2023-07-31 22:16:32.677118 optitrader-0.0.2/src/optitrader/app/pages/3_🗺️_Explore.py
+-rw-r--r--   0        0        0       96 2023-07-31 22:16:35.747188 optitrader-0.0.2/src/optitrader/app/pages/4_💼_Account.py
+-rw-r--r--   0        0        0       90 2023-07-31 22:16:25.026663 optitrader-0.0.2/src/optitrader/app/pages/5_👨🏻‍💻_About.py
+-rw-r--r--   0        0        0       12 2023-07-31 19:38:53.710765 optitrader-0.0.2/src/optitrader/app/pages/__init__.py
+-rw-r--r--   0        0        0      272 2023-07-31 22:25:57.146093 optitrader-0.0.2/src/optitrader/app/pages/__pycache__/2_📈_Backtester.cpython-310.pyc
+-rw-r--r--   0        0        0      266 2023-07-31 22:25:57.157579 optitrader-0.0.2/src/optitrader/app/pages/__pycache__/3_🗺️_Explore.cpython-310.pyc
+-rw-r--r--   0        0        0      263 2023-07-31 22:26:01.281761 optitrader-0.0.2/src/optitrader/app/pages/__pycache__/4_💼_Account.cpython-310.pyc
+-rw-r--r--   0        0        0      268 2023-07-31 22:26:05.045788 optitrader-0.0.2/src/optitrader/app/pages/__pycache__/5_👨🏻‍💻_About.cpython-310.pyc
+-rw-r--r--   0        0        0    24191 2023-07-31 22:36:35.174592 optitrader-0.0.2/src/optitrader/app/session_manager.py
+-rw-r--r--   0        0        0    24190 2023-07-31 22:36:33.537641 optitrader-0.0.2/src/optitrader/app/session_manager.py.aeacae1dba05799ae3b187801467b414.tmp
+-rw-r--r--   0        0        0     2621 2023-07-31 22:32:06.810228 optitrader-0.0.2/src/optitrader/backtester.py
+-rw-r--r--   0        0        0      469 2023-07-31 22:16:21.845724 optitrader-0.0.2/src/optitrader/cli.py
+-rw-r--r--   0        0        0     1542 2023-07-31 19:38:53.752242 optitrader-0.0.2/src/optitrader/config.py
+-rw-r--r--   0        0        0      422 2023-07-31 22:16:38.897012 optitrader-0.0.2/src/optitrader/enums/__init__.py
+-rw-r--r--   0        0        0      228 2023-07-31 22:16:29.794921 optitrader-0.0.2/src/optitrader/enums/backtester.py
+-rw-r--r--   0        0        0      736 2023-07-31 19:38:53.803876 optitrader-0.0.2/src/optitrader/enums/iterable.py
+-rw-r--r--   0        0        0     1712 2023-07-31 22:16:37.049303 optitrader-0.0.2/src/optitrader/enums/market.py
+-rw-r--r--   0        0        0      860 2023-07-31 22:16:24.915822 optitrader-0.0.2/src/optitrader/enums/optimization.py
+-rw-r--r--   0        0        0     6667 2023-07-31 22:28:44.554563 optitrader-0.0.2/src/optitrader/main.py
+-rw-r--r--   0        0        0      231 2023-07-31 22:16:29.990535 optitrader-0.0.2/src/optitrader/market/__init__.py
+-rw-r--r--   0        0        0     8461 2023-07-31 22:25:43.150556 optitrader-0.0.2/src/optitrader/market/alpaca_market_data.py
+-rw-r--r--   0        0        0     8460 2023-07-31 22:16:38.373315 optitrader-0.0.2/src/optitrader/market/alpaca_market_data.py.9fafeb33ede105e202d2a274793d58ee.tmp
+-rw-r--r--   0        0        0      768 2023-07-31 22:25:43.113539 optitrader-0.0.2/src/optitrader/market/base_data_provider.py
+-rw-r--r--   0        0        0       12 2023-07-31 19:38:53.914363 optitrader-0.0.2/src/optitrader/market/db/__init__.py
+-rw-r--r--   0        0        0     5339 2023-07-31 22:25:43.129931 optitrader-0.0.2/src/optitrader/market/db/database.py
+-rw-r--r--   0        0        0     5338 2023-07-31 22:16:37.469729 optitrader-0.0.2/src/optitrader/market/db/database.py.7b38a0f9e78f0ef64524afe7b2c0c608.tmp
+-rw-r--r--   0        0        0     1935 2023-07-31 19:38:53.949530 optitrader-0.0.2/src/optitrader/market/db/models.py
+-rw-r--r--   0        0        0       12 2023-07-31 19:38:53.965858 optitrader-0.0.2/src/optitrader/market/db/scripts/__init__.py
+-rw-r--r--   0        0        0      743 2023-07-31 22:16:40.153937 optitrader-0.0.2/src/optitrader/market/db/scripts/add_asset.py
+-rw-r--r--   0        0        0     1311 2023-07-31 22:25:43.054031 optitrader-0.0.2/src/optitrader/market/db/scripts/create_assets_table.py
+-rw-r--r--   0        0        0      733 2023-07-31 22:16:35.747150 optitrader-0.0.2/src/optitrader/market/db/scripts/update_number_of_shares.py
+-rw-r--r--   0        0        0     2830 2023-07-31 22:25:43.025856 optitrader-0.0.2/src/optitrader/market/finnhub_market_data.py
+-rw-r--r--   0        0        0     3473 2023-07-31 22:25:42.994845 optitrader-0.0.2/src/optitrader/market/investment_universe.py
+-rw-r--r--   0        0        0    14240 2023-07-31 22:25:42.966510 optitrader-0.0.2/src/optitrader/market/market_data.py
+-rw-r--r--   0        0        0    14239 2023-07-31 22:16:39.723467 optitrader-0.0.2/src/optitrader/market/market_data.py.185a99388c8a3ef51cc2541e94dbdc63.tmp
+-rw-r--r--   0        0        0     3330 2023-07-31 22:25:42.927223 optitrader-0.0.2/src/optitrader/market/news.py
+-rw-r--r--   0        0        0     4446 2023-07-31 22:25:42.888846 optitrader-0.0.2/src/optitrader/market/trading.py
+-rw-r--r--   0        0        0     6381 2023-07-31 22:25:43.077120 optitrader-0.0.2/src/optitrader/market/yahoo_market_data.py
+-rw-r--r--   0        0        0      270 2023-07-31 22:16:37.288605 optitrader-0.0.2/src/optitrader/models/__init__.py
+-rw-r--r--   0        0        0     2112 2023-07-31 22:25:43.027353 optitrader-0.0.2/src/optitrader/models/asset.py
+-rw-r--r--   0        0        0      243 2023-07-31 19:38:54.162170 optitrader-0.0.2/src/optitrader/models/base.py
+-rw-r--r--   0        0        0     1962 2023-07-31 22:16:44.855769 optitrader-0.0.2/src/optitrader/models/optimization.py
+-rw-r--r--   0        0        0     1962 2023-07-31 22:16:38.241893 optitrader-0.0.2/src/optitrader/models/optimization.py.0f97aab178a762049bd1442f7826f63f.tmp
+-rw-r--r--   0        0        0       12 2023-07-31 19:38:54.193302 optitrader-0.0.2/src/optitrader/optimization/__init__.py
+-rw-r--r--   0        0        0     7861 2023-07-31 22:25:42.975155 optitrader-0.0.2/src/optitrader/optimization/constraints.py
+-rw-r--r--   0        0        0    12717 2023-07-31 22:25:42.953925 optitrader-0.0.2/src/optitrader/optimization/objectives.py
+-rw-r--r--   0        0        0     6440 2023-07-31 22:25:42.902512 optitrader-0.0.2/src/optitrader/optimization/solver.py
+-rw-r--r--   0        0        0     6510 2023-07-31 22:25:42.870039 optitrader-0.0.2/src/optitrader/portfolio.py
+-rw-r--r--   0        0        0        0 2023-07-31 19:38:54.245739 optitrader-0.0.2/src/optitrader/py.typed
+-rw-r--r--   0        0        0      203 2023-07-31 22:16:39.107081 optitrader-0.0.2/src/optitrader/utils/__init__.py
+-rw-r--r--   0        0        0      953 2023-07-31 19:38:54.294727 optitrader-0.0.2/src/optitrader/utils/utils.py
+-rw-r--r--   0        0        0     9610 1970-01-01 00:00:00.000000 optitrader-0.0.2/PKG-INFO
```

### Comparing `optitrader-0.0.1/LICENSE` & `optitrader-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.1/README.md` & `optitrader-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 _Streamlit Dashboard_: to use this application from a Streamlit dashboard, run `optitrader dashboard`. This is equivalent to running `poe app` and open [localhost:8000](http://localhost:8000) in your browser.
 
 ## Example
 
 Once the package has been installed you can use it as follows:
 ```python
-from optitrader import optitrader
+from optitrader import Optitrader
 from optitrader.optimization.objectives import CVaRObjectiveFunction
 from optitrader.enums import UniverseName
 
 optimal_ptf = Optitrader(
         objectives=[CVaRObjectiveFunction()],
         universe_name=UniverseName.POPULAR_STOCKS,
     ).solve()
```

### Comparing `optitrader-0.0.1/pyproject.toml` & `optitrader-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]  # https://python-poetry.org/docs/pyproject/#poetry-and-pep-517
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]  # https://python-poetry.org/docs/pyproject/
 name = "optitrader"
-version = "0.0.1"
-description = "optitrader is an opne-source Python package for portfolio optimization. "
+version = "0.0.2"
+description = "Optitrader is an opne-source Python package for portfolio optimization. "
 authors = ["Alessio Castrica <castricaalessio@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/Ale-Cas/optitrader"
 
 [tool.commitizen]  # https://commitizen-tools.github.io/commitizen/config/
 bump_message = "bump(release): v$current_version → v$new_version"
 tag_format = "v$version"
```

### Comparing `optitrader-0.0.1/src/optitrader/api.py` & `optitrader-0.0.2/src/optitrader/api.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.1/src/optitrader/app/account.py` & `optitrader-0.0.2/src/optitrader/app/account.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.1/src/optitrader/app/backtester.py` & `optitrader-0.0.2/src/optitrader/app/backtester.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.1/src/optitrader/app/explore.py` & `optitrader-0.0.2/src/optitrader/app/explore.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.1/src/optitrader/app/home.py` & `optitrader-0.0.2/src/optitrader/app/home.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.1/src/optitrader/app/page.py` & `optitrader-0.0.2/src/optitrader/app/page.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.1/src/optitrader/app/session_manager.py` & `optitrader-0.0.2/src/optitrader/app/session_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from functools import partial
 
 import pandas as pd
 import plotly.express as px
 import streamlit as st
 from alpaca.trading import TradeAccount
 
-from optitrader import MarketData, Portfolio, optitrader
+from optitrader import MarketData, Optitrader, Portfolio
 from optitrader.backtester import Backtester, Portfolios
 from optitrader.enums import (
     ConstraintName,
     IterEnum,
     ObjectiveName,
     RebalanceFrequency,
     UniverseName,
@@ -398,15 +398,15 @@
                 label="Choose the rebalance frequency for the backtest.",
                 options=RebalanceFrequency,
                 is_value=False,
                 value=self.rebalance_frequency,
             )
         ]
 
-    def get_Optitrader(self) -> optitrader:
+    def get_optitrader(self) -> Optitrader:
         """Get the optitrader instance."""
         return Optitrader(
             objectives=self.obj_map.objectives,
             constraints=self.constr_map.constraints,
             universe_name=self.universe_name,
             market_data=self.market_data or MarketData(),
         )
@@ -433,15 +433,15 @@
                     with col2:
                         st.markdown(f"Weight: `{round(o.weight, 1)}`")
                     with col3:
                         st.markdown(f"Optimal value: `{round(o.value, 9)}`")
 
     def _run_optimization(self) -> None:
         """Run the optitrader solve."""
-        opt = self.get_Optitrader()
+        opt = self.get_optitrader()
         with st.spinner("Optimization in progress"):
             try:
                 opt_ptf = opt.solve(
                     start_date=self.start_date,
                     weights_tolerance=1e-3,
                 )
                 opt_ptf.set_market_data(opt.market_data)
@@ -462,15 +462,15 @@
                 )
             else:
                 self._run_optimization()
 
     def run_backtest(self) -> None:
         """Run the backtester."""
         if st.button(label="BACKTEST STRATEGY"):
-            opt = self.get_Optitrader()
+            opt = self.get_optitrader()
             with st.spinner("Backtest in progress"):
                 backtester = Backtester(
                     opt=opt,
                     start=self.start_date,
                     rebal_freq=self.rebalance_frequency,
                 )
                 self._ptfs = backtester.compute_portfolios()
```

### Comparing `optitrader-0.0.1/src/optitrader/app/session_manager.py.aeacae1dba05799ae3b187801467b414.tmp` & `optitrader-0.0.2/src/optitrader/app/session_manager.py.aeacae1dba05799ae3b187801467b414.tmp`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 from functools import partial
 
 import pandas as pd
 import plotly.express as px
 import streamlit as st
 from alpaca.trading import TradeAccount
-from optitrader import MarketData, Portfolio, optitrader
+from optitrader import MarketData, Portfolio, Optitrader
 from optitrader.backtester import Backtester, Portfolios
 from optitrader.enums import (
     ConstraintName,
     IterEnum,
     ObjectiveName,
     RebalanceFrequency,
     UniverseName,
@@ -397,15 +397,15 @@
                 label="Choose the rebalance frequency for the backtest.",
                 options=RebalanceFrequency,
                 is_value=False,
                 value=self.rebalance_frequency,
             )
         ]
 
-    def get_Optitrader(self) -> optitrader:
+    def get_optitrader(self) -> optitrader:
         """Get the optitrader instance."""
         return Optitrader(
             objectives=self.obj_map.objectives,
             constraints=self.constr_map.constraints,
             universe_name=self.universe_name,
             market_data=self.market_data or MarketData(),
         )
@@ -432,15 +432,15 @@
                     with col2:
                         st.markdown(f"Weight: `{round(o.weight, 1)}`")
                     with col3:
                         st.markdown(f"Optimal value: `{round(o.value, 9)}`")
 
     def _run_optimization(self) -> None:
         """Run the optitrader solve."""
-        opt = self.get_Optitrader()
+        opt = self.get_optitrader()
         with st.spinner("Optimization in progress"):
             try:
                 opt_ptf = opt.solve(
                     start_date=self.start_date,
                     weights_tolerance=1e-3,
                 )
                 opt_ptf.set_market_data(opt.market_data)
@@ -461,15 +461,15 @@
                 )
             else:
                 self._run_optimization()
 
     def run_backtest(self) -> None:
         """Run the backtester."""
         if st.button(label="BACKTEST STRATEGY"):
-            opt = self.get_Optitrader()
+            opt = self.get_optitrader()
             with st.spinner("Backtest in progress"):
                 backtester = Backtester(
                     opt=opt,
                     start=self.start_date,
                     rebal_freq=self.rebalance_frequency,
                 )
                 self._ptfs = backtester.compute_portfolios()
```

### Comparing `optitrader-0.0.1/src/optitrader/backtester.py` & `optitrader-0.0.2/src/optitrader/backtester.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Backtester implementation."""
 
 import pandas as pd
 import streamlit as st
 
-from optitrader import Portfolio, optitrader
+from optitrader import Optitrader, Portfolio
 from optitrader.enums import RebalanceFrequency
 from optitrader.utils import rearrange_columns_by_zeros
 
 
 class Portfolios:
     """Container of Portfolio objects."""
```

### Comparing `optitrader-0.0.1/src/optitrader/config.py` & `optitrader-0.0.2/src/optitrader/config.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.1/src/optitrader/enums/iterable.py` & `optitrader-0.0.2/src/optitrader/enums/iterable.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.1/src/optitrader/enums/market.py` & `optitrader-0.0.2/src/optitrader/enums/market.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.1/src/optitrader/enums/optimization.py` & `optitrader-0.0.2/src/optitrader/enums/optimization.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.1/src/optitrader/main.py` & `optitrader-0.0.2/src/optitrader/main.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.1/src/optitrader/market/alpaca_market_data.py` & `optitrader-0.0.2/src/optitrader/market/alpaca_market_data.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.1/src/optitrader/market/alpaca_market_data.py.9fafeb33ede105e202d2a274793d58ee.tmp` & `optitrader-0.0.2/src/optitrader/market/alpaca_market_data.py.9fafeb33ede105e202d2a274793d58ee.tmp`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.1/src/optitrader/market/base_data_provider.py` & `optitrader-0.0.2/src/optitrader/market/base_data_provider.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.1/src/optitrader/market/db/database.py` & `optitrader-0.0.2/src/optitrader/market/db/database.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.1/src/optitrader/market/db/database.py.7b38a0f9e78f0ef64524afe7b2c0c608.tmp` & `optitrader-0.0.2/src/optitrader/market/db/database.py.7b38a0f9e78f0ef64524afe7b2c0c608.tmp`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.1/src/optitrader/market/db/models.py` & `optitrader-0.0.2/src/optitrader/market/db/models.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.1/src/optitrader/market/db/scripts/add_asset.py` & `optitrader-0.0.2/src/optitrader/market/db/scripts/add_asset.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.1/src/optitrader/market/db/scripts/create_assets_table.py` & `optitrader-0.0.2/src/optitrader/market/db/scripts/create_assets_table.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.1/src/optitrader/market/db/scripts/update_number_of_shares.py` & `optitrader-0.0.2/src/optitrader/market/db/scripts/update_number_of_shares.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.1/src/optitrader/market/finnhub_market_data.py` & `optitrader-0.0.2/src/optitrader/market/finnhub_market_data.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.1/src/optitrader/market/investment_universe.py` & `optitrader-0.0.2/src/optitrader/market/investment_universe.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.1/src/optitrader/market/market_data.py` & `optitrader-0.0.2/src/optitrader/market/market_data.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.1/src/optitrader/market/market_data.py.185a99388c8a3ef51cc2541e94dbdc63.tmp` & `optitrader-0.0.2/src/optitrader/market/market_data.py.185a99388c8a3ef51cc2541e94dbdc63.tmp`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.1/src/optitrader/market/news.py` & `optitrader-0.0.2/src/optitrader/market/news.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.1/src/optitrader/market/trading.py` & `optitrader-0.0.2/src/optitrader/market/trading.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.1/src/optitrader/market/yahoo_market_data.py` & `optitrader-0.0.2/src/optitrader/market/yahoo_market_data.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.1/src/optitrader/models/asset.py` & `optitrader-0.0.2/src/optitrader/models/asset.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.1/src/optitrader/models/optimization.py` & `optitrader-0.0.2/src/optitrader/models/optimization.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.1/src/optitrader/models/optimization.py.0f97aab178a762049bd1442f7826f63f.tmp` & `optitrader-0.0.2/src/optitrader/models/optimization.py.0f97aab178a762049bd1442f7826f63f.tmp`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.1/src/optitrader/optimization/constraints.py` & `optitrader-0.0.2/src/optitrader/optimization/constraints.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.1/src/optitrader/optimization/objectives.py` & `optitrader-0.0.2/src/optitrader/optimization/objectives.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.1/src/optitrader/optimization/solver.py` & `optitrader-0.0.2/src/optitrader/optimization/solver.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.1/src/optitrader/portfolio.py` & `optitrader-0.0.2/src/optitrader/portfolio.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.1/src/optitrader/utils/utils.py` & `optitrader-0.0.2/src/optitrader/utils/utils.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.1/PKG-INFO` & `optitrader-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: optitrader
-Version: 0.0.1
-Summary: optitrader is an opne-source Python package for portfolio optimization. 
+Version: 0.0.2
+Summary: Optitrader is an opne-source Python package for portfolio optimization. 
 Home-page: https://github.com/Ale-Cas/optitrader
 Author: Alessio Castrica
 Author-email: castricaalessio@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -60,15 +60,15 @@
 
 _Streamlit Dashboard_: to use this application from a Streamlit dashboard, run `optitrader dashboard`. This is equivalent to running `poe app` and open [localhost:8000](http://localhost:8000) in your browser.
 
 ## Example
 
 Once the package has been installed you can use it as follows:
 ```python
-from optitrader import optitrader
+from optitrader import Optitrader
 from optitrader.optimization.objectives import CVaRObjectiveFunction
 from optitrader.enums import UniverseName
 
 optimal_ptf = Optitrader(
         objectives=[CVaRObjectiveFunction()],
         universe_name=UniverseName.POPULAR_STOCKS,
     ).solve()
```

