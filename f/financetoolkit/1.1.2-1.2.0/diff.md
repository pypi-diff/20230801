# Comparing `tmp/financetoolkit-1.1.2.tar.gz` & `tmp/financetoolkit-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "financetoolkit-1.1.2.tar", max compression
+gzip compressed data, was "financetoolkit-1.2.0.tar", max compression
```

## Comparing `financetoolkit-1.1.2.tar` & `financetoolkit-1.2.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0      126 2023-07-24 07:40:15.294645 financetoolkit-1.1.2/financetoolkit/__init__.py
--rw-r--r--   0        0        0        0 2023-07-24 07:40:15.295650 financetoolkit-1.1.2/financetoolkit/base/__init__.py
--rw-r--r--   0        0        0     3305 2023-07-24 07:40:15.296647 financetoolkit-1.1.2/financetoolkit/base/helpers.py
--rw-r--r--   0        0        0        0 2023-07-24 07:40:15.298642 financetoolkit-1.1.2/financetoolkit/base/models/__init__.py
--rw-r--r--   0        0        0    13677 2023-07-24 10:10:48.464634 financetoolkit-1.1.2/financetoolkit/base/models/fundamentals_model.py
--rw-r--r--   0        0        0     5548 2023-07-24 10:11:04.654704 financetoolkit-1.1.2/financetoolkit/base/models/historical_model.py
--rw-r--r--   0        0        0     1813 2023-07-24 07:40:15.304647 financetoolkit-1.1.2/financetoolkit/base/models/normalization/balance.csv
--rw-r--r--   0        0        0     1364 2023-07-24 07:40:15.305647 financetoolkit-1.1.2/financetoolkit/base/models/normalization/cash.csv
--rw-r--r--   0        0        0     1119 2023-07-24 07:40:15.306647 financetoolkit-1.1.2/financetoolkit/base/models/normalization/income.csv
--rw-r--r--   0        0        0     4267 2023-07-24 07:40:15.303656 financetoolkit-1.1.2/financetoolkit/base/models/normalization/README.md
--rw-r--r--   0        0        0     4126 2023-07-24 07:40:15.307643 financetoolkit-1.1.2/financetoolkit/base/models/normalization_model.py
--rw-r--r--   0        0        0     2751 2023-07-24 07:40:15.309645 financetoolkit-1.1.2/financetoolkit/base/models_controller.py
--rw-r--r--   0        0        0    53788 2023-07-24 07:40:15.310644 financetoolkit-1.1.2/financetoolkit/base/ratios_controller.py
--rw-r--r--   0        0        0    24679 2023-07-24 10:12:00.322591 financetoolkit-1.1.2/financetoolkit/base/toolkit_controller.py
--rw-r--r--   0        0        0        0 2023-07-24 07:40:15.313644 financetoolkit-1.1.2/financetoolkit/historical/__init__.py
--rw-r--r--   0        0        0     2804 2023-07-24 07:40:15.314643 financetoolkit-1.1.2/financetoolkit/historical/price.py
--rw-r--r--   0        0        0        0 2023-07-24 07:40:15.316652 financetoolkit-1.1.2/financetoolkit/models/__init__.py
--rw-r--r--   0        0        0     5436 2023-07-24 07:40:15.317645 financetoolkit-1.1.2/financetoolkit/models/dupont.py
--rw-r--r--   0        0        0        0 2023-07-24 07:40:15.319646 financetoolkit-1.1.2/financetoolkit/portfolio/__init__.py
--rw-r--r--   0        0        0     5958 2023-07-24 07:40:15.320645 financetoolkit-1.1.2/financetoolkit/portfolio/portfolio.py
--rw-r--r--   0        0        0        0 2023-07-24 07:40:15.321646 financetoolkit-1.1.2/financetoolkit/ratios/__init__.py
--rw-r--r--   0        0        0     9590 2023-07-24 07:40:15.323645 financetoolkit-1.1.2/financetoolkit/ratios/efficiency.py
--rw-r--r--   0        0        0     5236 2023-07-24 07:40:15.324648 financetoolkit-1.1.2/financetoolkit/ratios/liquidity.py
--rw-r--r--   0        0        0    12600 2023-07-24 07:40:15.326647 financetoolkit-1.1.2/financetoolkit/ratios/profitability.py
--rw-r--r--   0        0        0     7090 2023-07-24 07:40:15.327648 financetoolkit-1.1.2/financetoolkit/ratios/solvency.py
--rw-r--r--   0        0        0    15285 2023-07-24 07:40:15.328647 financetoolkit-1.1.2/financetoolkit/ratios/valuation.py
--rw-r--r--   0        0        0     1069 2023-07-24 07:40:15.153513 financetoolkit-1.1.2/LICENSE.txt
--rw-r--r--   0        0        0     2028 2023-07-24 10:14:25.119555 financetoolkit-1.1.2/pyproject.toml
--rw-r--r--   0        0        0    15047 2023-07-24 07:40:15.154509 financetoolkit-1.1.2/README.md
--rw-r--r--   0        0        0    15896 1970-01-01 00:00:00.000000 financetoolkit-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0      126 2023-07-24 07:40:15.294645 financetoolkit-1.2.0/financetoolkit/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-24 07:40:15.295650 financetoolkit-1.2.0/financetoolkit/base/__init__.py
+-rw-r--r--   0        0        0     3305 2023-08-01 09:24:28.644299 financetoolkit-1.2.0/financetoolkit/base/helpers.py
+-rw-r--r--   0        0        0        0 2023-07-24 07:40:15.298642 financetoolkit-1.2.0/financetoolkit/base/models/__init__.py
+-rw-r--r--   0        0        0    16066 2023-08-01 13:35:49.252118 financetoolkit-1.2.0/financetoolkit/base/models/fundamentals_model.py
+-rw-r--r--   0        0        0     5548 2023-07-27 13:42:17.475661 financetoolkit-1.2.0/financetoolkit/base/models/historical_model.py
+-rw-r--r--   0        0        0     1795 2023-07-27 13:42:17.479661 financetoolkit-1.2.0/financetoolkit/base/models/normalization/balance.csv
+-rw-r--r--   0        0        0     1364 2023-07-24 07:40:15.305647 financetoolkit-1.2.0/financetoolkit/base/models/normalization/cash.csv
+-rw-r--r--   0        0        0     1119 2023-07-24 07:40:15.306647 financetoolkit-1.2.0/financetoolkit/base/models/normalization/income.csv
+-rw-r--r--   0        0        0     4267 2023-07-24 07:40:15.303656 financetoolkit-1.2.0/financetoolkit/base/models/normalization/README.md
+-rw-r--r--   0        0        0      205 2023-07-27 14:01:00.024982 financetoolkit-1.2.0/financetoolkit/base/models/normalization/statistics.csv
+-rw-r--r--   0        0        0     4151 2023-07-27 14:25:28.576247 financetoolkit-1.2.0/financetoolkit/base/models/normalization_model.py
+-rw-r--r--   0        0        0     2751 2023-07-24 07:40:15.309645 financetoolkit-1.2.0/financetoolkit/base/models_controller.py
+-rw-r--r--   0        0        0    56374 2023-08-01 13:30:29.416521 financetoolkit-1.2.0/financetoolkit/base/ratios_controller.py
+-rw-r--r--   0        0        0    27469 2023-08-01 12:39:21.124629 financetoolkit-1.2.0/financetoolkit/base/toolkit_controller.py
+-rw-r--r--   0        0        0        0 2023-07-24 07:40:15.313644 financetoolkit-1.2.0/financetoolkit/historical/__init__.py
+-rw-r--r--   0        0        0     2804 2023-07-24 07:40:15.314643 financetoolkit-1.2.0/financetoolkit/historical/price.py
+-rw-r--r--   0        0        0        0 2023-07-24 07:40:15.316652 financetoolkit-1.2.0/financetoolkit/models/__init__.py
+-rw-r--r--   0        0        0     5436 2023-07-24 07:40:15.317645 financetoolkit-1.2.0/financetoolkit/models/dupont.py
+-rw-r--r--   0        0        0        0 2023-07-24 07:40:15.319646 financetoolkit-1.2.0/financetoolkit/portfolio/__init__.py
+-rw-r--r--   0        0        0     5958 2023-07-24 07:40:15.320645 financetoolkit-1.2.0/financetoolkit/portfolio/portfolio.py
+-rw-r--r--   0        0        0        0 2023-07-24 07:40:15.321646 financetoolkit-1.2.0/financetoolkit/ratios/__init__.py
+-rw-r--r--   0        0        0     9590 2023-07-24 07:40:15.323645 financetoolkit-1.2.0/financetoolkit/ratios/efficiency.py
+-rw-r--r--   0        0        0     5236 2023-07-24 07:40:15.324648 financetoolkit-1.2.0/financetoolkit/ratios/liquidity.py
+-rw-r--r--   0        0        0    12600 2023-07-24 07:40:15.326647 financetoolkit-1.2.0/financetoolkit/ratios/profitability.py
+-rw-r--r--   0        0        0     7090 2023-07-24 07:40:15.327648 financetoolkit-1.2.0/financetoolkit/ratios/solvency.py
+-rw-r--r--   0        0        0    15285 2023-07-24 07:40:15.328647 financetoolkit-1.2.0/financetoolkit/ratios/valuation.py
+-rw-r--r--   0        0        0     1069 2023-07-24 07:40:15.153513 financetoolkit-1.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     2053 2023-08-01 13:56:29.197391 financetoolkit-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0    17895 2023-08-01 13:30:29.370518 financetoolkit-1.2.0/README.md
+-rw-r--r--   0        0        0    18786 1970-01-01 00:00:00.000000 financetoolkit-1.2.0/PKG-INFO
```

### Comparing `financetoolkit-1.1.2/financetoolkit/base/helpers.py` & `financetoolkit-1.2.0/financetoolkit/base/helpers.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.1.2/financetoolkit/base/models/fundamentals_model.py` & `financetoolkit-1.2.0/financetoolkit/base/models/fundamentals_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     statement: str = "",
     api_key: str = "",
     quarter: bool = False,
     start_date: str | None = None,
     end_date: str | None = None,
     limit: int = 100,
     statement_format: pd.DataFrame = pd.DataFrame(),
+    statistics_format: pd.DataFrame = pd.DataFrame(),
 ):
     """
     Retrieves financial statements (balance, income, or cash flow statements) for one or multiple companies,
     and returns a DataFrame containing the data.
 
     Args:
         tickers (List[str]): List of company tickers.
@@ -78,71 +79,106 @@
             response = requests.get(
                 f"https://financialmodelingprep.com/api/v3/{location}/"
                 f"{ticker}?period={period}&apikey={api_key}&limit={limit}",
                 timeout=60,
             )
             response.raise_for_status()
             financial_statement = pd.read_json(response.text)
+
         except requests.exceptions.HTTPError:
-            print(f"{response.json()['Error Message']} (ticker: {ticker})")
-            invalid_tickers.append(ticker)
-            continue
+            if (
+                "not available under your current subscription"
+                in response.json()["Error Message"]
+            ):
+                print(
+                    f"The requested data for {ticker} is part of the Premium Subscription from "
+                    "FinancialModelingPrep. If you wish to access this data, consider upgrading "
+                    "your plan.\nYou can get 15% off by using the following affiliate link which "
+                    "also supports the project: https://site.financialmodelingprep.com/developer/docs/pricing/jeroen/"
+                )
+            break
 
         try:
             financial_statement = financial_statement.drop("symbol", axis=1)
         except KeyError:
             print(f"No financial statement data found for {ticker}")
             invalid_tickers.append(ticker)
             continue
 
         if quarter:
             financial_statement["date"] = pd.to_datetime(
                 financial_statement["date"]
-            ).dt.to_period("M")
+            ).dt.to_period("Q")
         else:
             financial_statement["date"] = pd.to_datetime(
-                financial_statement["date"]
-            ).dt.year
+                financial_statement["calendarYear"].astype(str)
+            ).dt.to_period("Y")
 
         financial_statement = financial_statement.set_index("date").T
 
+        if financial_statement.columns.duplicated().any():
+            # This happens in the rare case that a company has two financial statements for the same period.
+            # Browsing through the data has shown that these financial statements are also equal therefore
+            # one of the columns can be dropped.
+            financial_statement = financial_statement.loc[
+                :, ~financial_statement.columns.duplicated()
+            ]
+
         financial_statement_dict[ticker] = financial_statement
 
     if financial_statement_dict:
         financial_statement_total = pd.concat(financial_statement_dict, axis=0)
 
+        financial_statement_statistics = convert_financial_statements(
+            financial_statement_total, statistics_format, True
+        )
+
         financial_statement_total = convert_financial_statements(
             financial_statement_total, statement_format, True
         )
 
         try:
             financial_statement_total = financial_statement_total.astype(np.float64)
         except ValueError as error:
             print(
                 f"Not able to convert DataFrame to float64 due to {error}. This could result in"
                 "issues when values are zero and is predominently relevant for "
                 "ratio calculations."
             )
 
+        financial_statement_statistics = financial_statement_statistics.sort_index(
+            axis=1
+        ).truncate(before=start_date, after=end_date, axis=1)
+
         financial_statement_total = financial_statement_total.sort_index(
             axis=1
         ).truncate(before=start_date, after=end_date, axis=1)
 
         if quarter:
+            financial_statement_statistics.columns = pd.PeriodIndex(
+                financial_statement_statistics.columns, freq="Q"
+            )
             financial_statement_total.columns = pd.PeriodIndex(
-                financial_statement_total.columns, freq="M"
+                financial_statement_total.columns, freq="Q"
             )
         else:
+            financial_statement_statistics.columns = pd.PeriodIndex(
+                financial_statement_statistics.columns, freq="Y"
+            )
             financial_statement_total.columns = pd.PeriodIndex(
                 financial_statement_total.columns, freq="Y"
             )
 
-        return financial_statement_total, invalid_tickers
+        return (
+            financial_statement_total,
+            financial_statement_statistics,
+            invalid_tickers,
+        )
 
-    return pd.DataFrame(), invalid_tickers
+    return pd.DataFrame(), pd.DataFrame(), invalid_tickers
 
 
 def get_profile(tickers: list[str] | str, api_key: str):
     """
     Description
     ----
     Gives information about the profile of a company which includes
@@ -170,15 +206,15 @@
     invalid_tickers = []
     for ticker in ticker_list:
         try:
             profile_dataframe[ticker] = pd.read_json(
                 f"https://financialmodelingprep.com/api/v3/profile/{ticker}?apikey={api_key}"
             ).T
         except ValueError:
-            print(f"No historical data found for {ticker}")
+            print(f"No profile data found for {ticker}")
             invalid_tickers.append(ticker)
         except Exception as error:
             raise ValueError(error) from error
 
     return profile_dataframe, invalid_tickers
 
 
@@ -211,15 +247,15 @@
     invalid_tickers = []
     for ticker in ticker_list:
         try:
             quote_dataframe[ticker] = pd.read_json(
                 f"https://financialmodelingprep.com/api/v3/quote/{ticker}?apikey={api_key}"
             ).T
         except ValueError:
-            print(f"No historical data found for {ticker}")
+            print(f"No quote data found for {ticker}")
             invalid_tickers.append(ticker)
         except Exception as error:
             raise ValueError(error) from error
 
     return quote_dataframe, invalid_tickers
 
 
@@ -267,24 +303,32 @@
                 f"https://financialmodelingprep.com/api/v3/enterprise-values/{ticker}"
                 f"?period={period}&limit={limit}&apikey={api_key}",
                 timeout=60,
             )
             response.raise_for_status()
             enterprise_values = pd.read_json(response.text)
         except requests.exceptions.HTTPError:
-            print(f"{response.json()['Error Message']} (ticker: {ticker})")
-            invalid_tickers.append(ticker)
-            continue
+            if (
+                "not available under your current subscription"
+                in response.json()["Error Message"]
+            ):
+                print(
+                    f"The requested data for {ticker} is part of the Premium Subscription from "
+                    "FinancialModelingPrep. If you wish to access this data, consider upgrading "
+                    "your plan.\nYou can get 15% off by using the following affiliate link which "
+                    "also supports the project: https://site.financialmodelingprep.com/developer/docs/pricing/jeroen/"
+                )
+            break
 
         try:
             enterprise_values = enterprise_values.drop("symbol", axis=1).sort_values(
                 by="date", ascending=True
             )
         except KeyError:
-            print(f"No historical data found for {ticker}.")
+            print(f"No enterprise data found for {ticker}.")
             invalid_tickers.append(ticker)
             continue
 
         if quarter:
             enterprise_values["date"] = pd.PeriodIndex(
                 enterprise_values["date"], freq="M"
             )
@@ -347,20 +391,28 @@
     invalid_tickers = []
     for ticker in ticker_list:
         try:
             ratings = pd.read_json(
                 f"https://financialmodelingprep.com/api/v3/historical-rating/{ticker}?limit={limit}&apikey={api_key}"
             )
         except ValueError:
-            print(f"No historical data found for {ticker}")
+            print(f"No rating data found for {ticker}")
             invalid_tickers.append(ticker)
         except Exception as error:
             raise ValueError(error) from error
 
-        ratings = ratings.drop("symbol", axis=1).sort_values(by="date", ascending=True)
+        try:
+            ratings = ratings.drop("symbol", axis=1).sort_values(
+                by="date", ascending=True
+            )
+        except KeyError:
+            print(f"No rating data found for {ticker}")
+            invalid_tickers.append(ticker)
+            continue
+
         ratings = ratings.set_index("date")
 
         ratings = ratings.rename(
             columns={
                 "rating": "Rating",
                 "ratingScore": "Rating Score",
                 "ratingRecommendation": "Rating Recommendation",
```

### Comparing `financetoolkit-1.1.2/financetoolkit/base/models/historical_model.py` & `financetoolkit-1.2.0/financetoolkit/base/models/historical_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,11 +134,11 @@
     dates = pd.to_datetime(daily_historical_data.Date).dt.to_period("Q")
     quarterly_historical_data = daily_historical_data.groupby(dates).transform("last")
     quarterly_historical_data["Date"] = quarterly_historical_data["Date"].str[:7]
     quarterly_historical_data = quarterly_historical_data.drop_duplicates().set_index(
         "Date"
     )
     quarterly_historical_data.index = pd.PeriodIndex(
-        quarterly_historical_data.index, freq="M"
+        quarterly_historical_data.index, freq="Q"
     )
 
     return quarterly_historical_data
```

### Comparing `financetoolkit-1.1.2/financetoolkit/base/models/normalization/balance.csv` & `financetoolkit-1.2.0/financetoolkit/base/models/normalization/balance.csv`

 * *Files 3% similar despite different names*

```diff
@@ -33,13 +33,12 @@
 totalInvestments,Total Investments
 totalLiabilities,Total Liabilities
 preferredStock,Preferred Stock
 commonStock,Common Stock
 retainedEarnings,Retained Earnings
 accumulatedOtherComprehensiveIncomeLoss,Accumulated Other Comprehensive Income
 othertotalStockholdersEquity,Other Total Shareholder Equity
-,Minority Interest
 totalStockholdersEquity,Total Shareholder Equity
 totalEquity,Total Equity
 totalLiabilitiesAndStockholdersEquity,Total Liabilities and Shareholder Equity
 minorityInterest,Minority Interest
-totalLiabilitiesAndTotalEquity,Total Liabilities and Equity
+totalLiabilitiesAndTotalEquity,Total Liabilities and Equity
```

### Comparing `financetoolkit-1.1.2/financetoolkit/base/models/normalization/cash.csv` & `financetoolkit-1.2.0/financetoolkit/base/models/normalization/cash.csv`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.1.2/financetoolkit/base/models/normalization/income.csv` & `financetoolkit-1.2.0/financetoolkit/base/models/normalization/income.csv`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.1.2/financetoolkit/base/models/normalization/README.md` & `financetoolkit-1.2.0/financetoolkit/base/models/normalization/README.md`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.1.2/financetoolkit/base/models/normalization_model.py` & `financetoolkit-1.2.0/financetoolkit/base/models/normalization_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 
     Args:
         statement (string): the type of statement you wish to read (balance, income, or cash).
         format_location (string): the location to read the file from.
     Returns:
         A pandas Series containing the line items for the desired statement.
     """
-    if statement not in ["balance", "income", "cash"]:
+    if statement not in ["balance", "income", "cash", "statistics"]:
         raise ValueError(
-            "Please provide a valid statement type (balance, income, or cash)."
+            "Please provide a valid statement type (balance, income, cash or statistics)."
         )
 
     if format_location:
         file_location = f"{format_location}/{statement}.csv"
     else:
         file_location = pkg_resources.resource_stream(
             __name__, f"normalization/{statement}.csv"
```

### Comparing `financetoolkit-1.1.2/financetoolkit/base/models_controller.py` & `financetoolkit-1.2.0/financetoolkit/base/models_controller.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.1.2/financetoolkit/base/ratios_controller.py` & `financetoolkit-1.2.0/financetoolkit/base/ratios_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 """Ratios Module"""
 __docformat__ = "numpy"
 
+import operator
+import re
+
 import pandas as pd
 
 from financetoolkit.base.helpers import handle_errors
 from financetoolkit.ratios import (
     efficiency,
     liquidity,
     profitability,
@@ -23,20 +26,23 @@
     def __init__(
         self,
         tickers: str | list[str],
         historical: pd.DataFrame,
         balance: pd.DataFrame,
         income: pd.DataFrame,
         cash: pd.DataFrame,
+        custom_ratios: dict | None = None,
     ):
         self._tickers = tickers
         self._historical_data: pd.DataFrame = historical
         self._balance_sheet_statement: pd.DataFrame = balance
         self._income_statement: pd.DataFrame = income
         self._cash_flow_statement: pd.DataFrame = cash
+        self._custom_ratios: dict | None = custom_ratios
+        self._custom_ratios_df: pd.DataFrame = pd.DataFrame()
 
         # Initialization of Fundamentals Variables
         self._all_ratios: pd.DataFrame = pd.DataFrame()
         self._efficiency_ratios: pd.DataFrame = pd.DataFrame()
         self._liquidity_ratios: pd.DataFrame = pd.DataFrame()
         self._profitability_ratios: pd.DataFrame = pd.DataFrame()
         self._solvency_ratios: pd.DataFrame = pd.DataFrame()
@@ -206,17 +212,14 @@
         """
         if self._solvency_ratios.empty:
             solvency_ratios: dict = {}
 
             solvency_ratios["Debt-to-Assets Ratio"] = self.get_debt_to_assets_ratio()
             solvency_ratios["Debt-to-Equity Ratio"] = self.get_debt_to_equity_ratio()
             solvency_ratios[
-                "Interest Coverage Ratio"
-            ] = self.get_interest_coverage_ratio()
-            solvency_ratios[
                 "Debt Service Coverage Ratio"
             ] = self.get_debt_service_coverage_ratio()
             solvency_ratios["Equity Multiplier"] = self.get_equity_multiplier()
             solvency_ratios["Free Cash Flow Yield"] = self.get_free_cash_flow_yield(
                 diluted=diluted
             )
             solvency_ratios[
@@ -322,14 +325,85 @@
             )
 
         if len(self._tickers) == 1:
             return self._valuation_ratios.loc[self._tickers[0]]
 
         return self._valuation_ratios
 
+    # @handle_errors
+    def collect_custom_ratios(self, overwrite: bool = False):
+        """
+        Calculates all Custom Ratios based on the data provided.
+        """
+        if not self._custom_ratios:
+            print(
+                "Please define custom ratios through the Toolkit initialization. "
+                "See https://github.com/JerBouma/FinanceToolkit how to do this."
+            )
+
+        if self._custom_ratios and (self._custom_ratios_df.empty or overwrite):
+            if self._all_ratios.empty:
+                self._all_ratios = self.collect_all_ratios()
+
+            custom_ratios_df = pd.DataFrame(
+                index=pd.MultiIndex.from_product(
+                    [self._tickers, self._custom_ratios.keys()]
+                ),
+                columns=self._balance_sheet_statement.columns,
+            )
+
+            total_financials = pd.concat(
+                [
+                    self._balance_sheet_statement,
+                    self._income_statement,
+                    self._cash_flow_statement,
+                    self._all_ratios,
+                    custom_ratios_df,
+                ],
+                axis=0,
+            )
+
+            total_financials = total_financials[
+                ~total_financials.index.duplicated(keep="first")
+            ]
+
+            operations = {
+                "+": operator.add,
+                "-": operator.sub,
+                "*": operator.mul,
+                "/": operator.truediv,
+                "^": operator.pow,
+            }
+
+            for name, formula in self._custom_ratios.items():
+                operator_use = re.findall("[+\\-*^/]", formula)[0]
+
+                split_1, split_2 = formula.split(operator_use)
+                calculation = operations[operator_use]
+
+                result_dataframe = calculation(
+                    total_financials.loc[:, split_1.strip(), :],
+                    total_financials.loc[:, split_2.strip(), :],
+                )
+
+                for company in self._tickers:
+                    total_financials.loc[company, name, :] = result_dataframe.loc[
+                        company
+                    ].to_numpy()
+
+            self._custom_ratios_df = total_financials.loc[
+                :, list(self._custom_ratios.keys()), :
+            ]
+            self._custom_ratios_df = self._custom_ratios_df.sort_index(axis=0)
+
+        if len(self._tickers) == 1:
+            return self._custom_ratios_df.loc[self._tickers[0]]
+
+        return self._custom_ratios_df
+
     @handle_errors
     def get_asset_turnover_ratio(self):
         """
         Calculate the asset turnover ratio, an efficiency ratio that measures how
         efficiently a company uses its assets to generate sales.
         """
         return efficiency.get_asset_turnover_ratio(
@@ -869,14 +943,15 @@
 
     @handle_errors
     def get_free_cash_flow_yield(self, diluted: bool = True):
         """
         Calculates the free cash flow yield ratio, which measures the free cash flow
         relative to the market capitalization of the company.
         """
+
         years = self._balance_sheet_statement.columns
         begin, end = str(years[0]), str(years[-1])
 
         share_prices = self._historical_data.loc[begin:end, "Adj Close"].T  # type: ignore
 
         average_shares = (
             self._income_statement.loc[:, "Weighted Average Shares Diluted", :]
```

### Comparing `financetoolkit-1.1.2/financetoolkit/base/toolkit_controller.py` & `financetoolkit-1.2.0/financetoolkit/base/toolkit_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,14 +44,15 @@
         self,
         tickers: list | str,
         api_key: str = "",
         historical: pd.DataFrame = pd.DataFrame(),
         balance: pd.DataFrame = pd.DataFrame(),
         income: pd.DataFrame = pd.DataFrame(),
         cash: pd.DataFrame = pd.DataFrame(),
+        custom_ratios: dict | None = None,
         start_date: str | None = None,
         end_date: str | None = None,
         quarterly: bool = False,
         format_location: str = "",
         reverse_dates: bool = False,
         remove_invalid_tickers: bool = True,
     ):
@@ -126,14 +127,18 @@
         self._income_statement_generic: pd.DataFrame = _read_normalization_file(
             "income", format_location
         )
         self._cash_flow_statement_generic: pd.DataFrame = _read_normalization_file(
             "cash", format_location
         )
 
+        self._statistics_statement_generic: pd.DataFrame = _read_normalization_file(
+            "statistics", format_location
+        )
+
         # Initialization of Financial Statements
         self._balance_sheet_statement: pd.DataFrame = (
             _convert_financial_statements(
                 balance, self._balance_sheet_statement_generic, reverse_dates
             )
             if not balance.empty
             else pd.DataFrame()
@@ -148,14 +153,16 @@
         self._cash_flow_statement: pd.DataFrame = (
             _convert_financial_statements(
                 cash, self._cash_flow_statement_generic, reverse_dates
             )
             if not cash.empty
             else pd.DataFrame()
         )
+        self._statistics_statement: pd.DataFrame = pd.DataFrame()
+        self._custom_ratios: dict | None = custom_ratios
 
     @property
     def ratios(self) -> Ratios:
         """
         Gives access to financial ratios.
         """
         empty_data: list = []
@@ -223,14 +230,15 @@
             self._tickers,
             self._quarterly_historical_data
             if self._quarterly
             else self._yearly_historical_data,
             self._balance_sheet_statement,
             self._income_statement,
             self._cash_flow_statement,
+            self._custom_ratios,
         )
 
     @property
     def models(self) -> Models:
         """
         Gives access to financial models.
         """
@@ -409,15 +417,16 @@
         """
         Returns a pandas dataframe containing the historical data for the specified tickers.
 
         Args:
             start (str): The start date for the historical data. Defaults to None.
             end (str): The end date for the historical data. Defaults to None.
             period (str): The interval at which the historical data should be
-            returned - daily, weekly, monthly, or yearly. Defaults to "daily".
+            returned - daily, weekly, monthly, quarterly, or yearly.
+            Defaults to "daily".
 
         Raises:
             ValueError: If an invalid value is specified for period.
 
         Returns:
             pandas.DataFrame: The historical data for the specified tickers.
         """
@@ -550,36 +559,39 @@
         overwrite: bool = False,
     ):
         """
         Retrieves the balance sheet statement financial data for the company(s) from the specified source.
 
         Args:
             limit (int): Defines the maximum years or quarters to obtain.
+            overwrite (bool): Defines whether to overwrite the existing data.
 
         Returns:
             pd.DataFrame: A pandas DataFrame with the retrieved balance sheet statement data.
         """
         if not self._api_key and self._balance_sheet_statement.empty:
             raise ValueError(
                 "Please define an API key from FinancialModelingPrep to use this functionality."
             )
 
         if self._balance_sheet_statement.empty or overwrite:
             (
                 self._balance_sheet_statement,
+                self._statistics_statement,
                 self._invalid_tickers,
             ) = _get_financial_statements(
                 self._tickers,
                 "balance",
                 self._api_key,
                 self._quarterly,
                 self._start_date,
                 self._end_date,
                 limit,
                 self._balance_sheet_statement_generic,
+                self._statistics_statement_generic,
             )
 
         if self._remove_invalid_tickers:
             self._tickers = [
                 ticker
                 for ticker in self._tickers
                 if ticker not in self._invalid_tickers
@@ -596,33 +608,39 @@
         overwrite: bool = False,
     ):
         """
         Retrieves the income statement financial data for the company(s) from the specified source.
 
         Args:
             limit (int): Defines the maximum years or quarters to obtain.
+            overwrite (bool): Defines whether to overwrite the existing data.
 
         Returns:
             pd.DataFrame: A pandas DataFrame with the retrieved income statement data.
         """
         if not self._api_key and self._income_statement.empty:
             raise ValueError(
                 "Please define an API key from FinancialModelingPrep to use this functionality."
             )
 
         if self._income_statement.empty or overwrite:
-            self._income_statement, self._invalid_tickers = _get_financial_statements(
+            (
+                self._income_statement,
+                self._statistics_statement,
+                self._invalid_tickers,
+            ) = _get_financial_statements(
                 self._tickers,
                 "income",
                 self._api_key,
                 self._quarterly,
                 self._start_date,
                 self._end_date,
                 limit,
                 self._income_statement_generic,
+                self._statistics_statement_generic,
             )
 
         if self._remove_invalid_tickers:
             self._tickers = [
                 ticker
                 for ticker in self._tickers
                 if ticker not in self._invalid_tickers
@@ -639,50 +657,105 @@
         overwrite: bool = False,
     ):
         """
         Retrieves the cash flow statement financial data for the company(s) from the specified source.
 
         Args:
             limit (int): Defines the maximum years or quarters to obtain.
+            overwrite (bool): Defines whether to overwrite the existing data.
 
         Returns:
             pd.DataFrame: A pandas DataFrame with the retrieved cash flow statement data.
         """
         if not self._api_key and self._cash_flow_statement.empty:
             raise ValueError(
                 "Please define an API key from FinancialModelingPrep to use this functionality."
             )
 
         if self._cash_flow_statement.empty or overwrite:
             (
                 self._cash_flow_statement,
+                self._statistics_statement,
                 self._invalid_tickers,
             ) = _get_financial_statements(
                 self._tickers,
                 "cashflow",
                 self._api_key,
                 self._quarterly,
                 self._start_date,
                 self._end_date,
                 limit,
                 self._cash_flow_statement_generic,
+                self._statistics_statement_generic,
             )
 
         if self._remove_invalid_tickers:
             self._tickers = [
                 ticker
                 for ticker in self._tickers
                 if ticker not in self._invalid_tickers
             ]
 
         if len(self._tickers) == 1:
             return self._cash_flow_statement.loc[self._tickers[0]]
 
         return self._cash_flow_statement
 
+    def get_statistics_statement(
+        self,
+        limit: int = 100,
+        overwrite: bool = False,
+    ):
+        """
+        Retrieves the balance, cash and income statistics for the company(s) from the specified source.
+
+        Note that this also obtains the balance sheet statement at the same time given that it's the same
+        API call. This is done to reduce the number of API calls to FinancialModelingPrep.
+
+        Args:
+            limit (int): Defines the maximum years or quarters to obtain.
+            overwrite (bool): Defines whether to overwrite the existing data.
+
+        Returns:
+            pd.DataFrame: A pandas DataFrame with the retrieved statistics statement data.
+        """
+        if not self._api_key and self._statistics_statement.empty:
+            raise ValueError(
+                "Please define an API key from FinancialModelingPrep to use this functionality."
+            )
+
+        if self._statistics_statement.empty or overwrite:
+            (
+                self._balance_sheet_statement,
+                self._statistics_statement,
+                self._invalid_tickers,
+            ) = _get_financial_statements(
+                self._tickers,
+                "balance",
+                self._api_key,
+                self._quarterly,
+                self._start_date,
+                self._end_date,
+                limit,
+                self._balance_sheet_statement_generic,
+                self._statistics_statement_generic,
+            )
+
+        if self._remove_invalid_tickers:
+            self._tickers = [
+                ticker
+                for ticker in self._tickers
+                if ticker not in self._invalid_tickers
+            ]
+
+        if len(self._tickers) == 1:
+            return self._statistics_statement.loc[self._tickers[0]]
+
+        return self._statistics_statement
+
     def get_normalization_files(self, path: str = ""):
         """
         Copies the normalization files to a folder based on path. By default, this is the path
         of the 'Downloads' folder.
 
         Args:
             path (str, optional): The path where to save the files to.
```

### Comparing `financetoolkit-1.1.2/financetoolkit/historical/price.py` & `financetoolkit-1.2.0/financetoolkit/historical/price.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.1.2/financetoolkit/models/dupont.py` & `financetoolkit-1.2.0/financetoolkit/models/dupont.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.1.2/financetoolkit/portfolio/portfolio.py` & `financetoolkit-1.2.0/financetoolkit/portfolio/portfolio.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.1.2/financetoolkit/ratios/efficiency.py` & `financetoolkit-1.2.0/financetoolkit/ratios/efficiency.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.1.2/financetoolkit/ratios/liquidity.py` & `financetoolkit-1.2.0/financetoolkit/ratios/liquidity.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.1.2/financetoolkit/ratios/profitability.py` & `financetoolkit-1.2.0/financetoolkit/ratios/profitability.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.1.2/financetoolkit/ratios/solvency.py` & `financetoolkit-1.2.0/financetoolkit/ratios/solvency.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.1.2/financetoolkit/ratios/valuation.py` & `financetoolkit-1.2.0/financetoolkit/ratios/valuation.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.1.2/LICENSE.txt` & `financetoolkit-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.1.2/pyproject.toml` & `financetoolkit-1.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "financetoolkit"
-version = "1.1.2"
+version = "1.2.0"
 description = "Transparent and Efficient Financial Analysis"
 license = "MIT"
 authors = ["Jeroen Bouma"]
 packages = [
     { include = "financetoolkit" },
 ]
 include = ['normalization/*.csv']
@@ -21,14 +21,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 
 [tool.poetry.dependencies]
 pandas = "^2.0.0"
 python = "^3.10"
+requests = "^2.31.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^6.2.2"
 pylint = "2.17.0"
 codespell = "^2.2.4"
 black = "^23.1.0"
 bandit = "^1.7.0"
@@ -60,14 +61,14 @@
 [tool.isort]
 profile = "black"
 line_length = 122
 skip_gitignore = true
 combine_as_imports = true
 
 [tool.codespell]
-ignore-words-list = 'zar,profund,basf,applicatio,ser,mone,vie,wew,ist,tre,ue,nd,fo,nWe,nwe,0t,Ot,ot,juNI'
+ignore-words-list = 'zar,profund,basf,applicatio,ser,mone,vie,wew,ist,tre,ue,nd,fo,nwe,0t,Ot,ot,juni,acn,hve'
 skip = '*.json,./.git,pyproject.toml,poetry.lock'
 
 [tool.pytest.ini_options]
 filterwarnings = [
     "ignore::pytest.PytestAssertRewriteWarning:",
 ]
```

### Comparing `financetoolkit-1.1.2/README.md` & `financetoolkit-1.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -13,929 +13,1107 @@
 000000c0: 6f6e 6174 652d 6272 6967 6874 6772 6565  onate-brightgree
 000000d0: 6e3f 6c6f 676f 3d62 7579 6d65 6163 6f66  n?logo=buymeacof
 000000e0: 6665 6529 5d28 6874 7470 733a 2f2f 7777  fee)](https://ww
 000000f0: 772e 6275 796d 6561 636f 6666 6565 2e63  w.buymeacoffee.c
 00000100: 6f6d 2f6a 6572 626f 756d 6129 0a5b 215b  om/jerbouma).[![
 00000110: 5765 6273 6974 655d 2868 7474 7073 3a2f  Website](https:/
 00000120: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000130: 6261 6467 652f 5765 6273 6974 652d 4c65  badge/Website-Le
-00000140: 6172 6e25 3230 6d6f 7265 2532 3061 626f  arn%20more%20abo
-00000150: 7574 2532 306d 6525 3230 6865 7265 2d62  ut%20me%20here-b
-00000160: 7269 6768 7467 7265 656e 3f6c 6f67 6f3d  rightgreen?logo=
-00000170: 5265 6164 4d65 295d 2868 7474 7073 3a2f  ReadMe)](https:/
-00000180: 2f6a 6572 6f65 6e62 6f75 6d61 2e63 6f6d  /jeroenbouma.com
-00000190: 2f29 0a5b 215b 5375 7070 6f72 7465 6420  /).[![Supported 
-000001a0: 5079 7468 6f6e 2056 6572 7369 6f6e 735d  Python Versions]
-000001b0: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-000001c0: 656c 6473 2e69 6f2f 7079 7069 2f70 7976  elds.io/pypi/pyv
-000001d0: 6572 7369 6f6e 732f 6669 6e61 6e63 6574  ersions/financet
-000001e0: 6f6f 6c6b 6974 295d 2868 7474 7073 3a2f  oolkit)](https:/
-000001f0: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
-00000200: 742f 4669 6e61 6e63 6554 6f6f 6c6b 6974  t/FinanceToolkit
-00000210: 2f29 0a5b 215b 5059 5049 2056 6572 7369  /).[![PYPI Versi
-00000220: 6f6e 5d28 6874 7470 733a 2f2f 696d 672e  on](https://img.
-00000230: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
-00000240: 762f 4669 6e61 6e63 6554 6f6f 6c6b 6974  v/FinanceToolkit
-00000250: 295d 2868 7474 7073 3a2f 2f70 7970 692e  )](https://pypi.
-00000260: 6f72 672f 7072 6f6a 6563 742f 4669 6e61  org/project/Fina
-00000270: 6e63 6554 6f6f 6c6b 6974 2f29 0a5b 215b  nceToolkit/).[![
-00000280: 5059 5049 2044 6f77 6e6c 6f61 6473 5d28  PYPI Downloads](
-00000290: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-000002a0: 6c64 732e 696f 2f70 7970 692f 646d 2f46  lds.io/pypi/dm/F
+00000130: 6261 6467 652f 5265 6164 5f4d 6f72 652d  badge/Read_More-
+00000140: 7765 6273 6974 653f 6c6f 676f 3d72 6561  website?logo=rea
+00000150: 646d 6526 6c61 6265 6c3d 5765 6273 6974  dme&label=Websit
+00000160: 6529 5d28 6874 7470 733a 2f2f 6a65 726f  e)](https://jero
+00000170: 656e 626f 756d 612e 636f 6d2f 290a 5b21  enbouma.com/).[!
+00000180: 5b44 6973 636f 7264 5d28 6874 7470 733a  [Discord](https:
+00000190: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000001a0: 2f62 6164 6765 2f43 6861 742d 6865 6c6c  /badge/Chat-hell
+000001b0: 6f3f 6c6f 676f 3d64 6973 636f 7264 266c  o?logo=discord&l
+000001c0: 6162 656c 3d44 6973 636f 7264 295d 2868  abel=Discord)](h
+000001d0: 7474 7073 3a2f 2f64 6973 636f 7264 6170  ttps://discordap
+000001e0: 702e 636f 6d2f 7573 6572 732f 3534 3738  p.com/users/5478
+000001f0: 3836 3938 3134 3638 3738 3236 3133 290a  86981468782613).
+00000200: 5b21 5b53 7570 706f 7274 6564 2050 7974  [![Supported Pyt
+00000210: 686f 6e20 5665 7273 696f 6e73 5d28 6874  hon Versions](ht
+00000220: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000230: 732e 696f 2f70 7970 692f 7079 7665 7273  s.io/pypi/pyvers
+00000240: 696f 6e73 2f66 696e 616e 6365 746f 6f6c  ions/financetool
+00000250: 6b69 7429 5d28 6874 7470 733a 2f2f 7079  kit)](https://py
+00000260: 7069 2e6f 7267 2f70 726f 6a65 6374 2f46  pi.org/project/F
+00000270: 696e 616e 6365 546f 6f6c 6b69 742f 290a  inanceToolkit/).
+00000280: 5b21 5b50 5950 4920 5665 7273 696f 6e5d  [![PYPI Version]
+00000290: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+000002a0: 656c 6473 2e69 6f2f 7079 7069 2f76 2f46  elds.io/pypi/v/F
 000002b0: 696e 616e 6365 546f 6f6c 6b69 7429 5d28  inanceToolkit)](
 000002c0: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
 000002d0: 2f70 726f 6a65 6374 2f46 696e 616e 6365  /project/Finance
-000002e0: 546f 6f6c 6b69 742f 290a 0a57 6869 6c65  Toolkit/)..While
-000002f0: 2062 726f 7773 696e 6720 6120 7661 7269   browsing a vari
-00000300: 6574 7920 6f66 2077 6562 7369 7465 732c  ety of websites,
-00000310: 2049 206b 6570 7420 6669 6e64 696e 6720   I kept finding 
-00000320: 7468 6174 2074 6865 2073 616d 6520 6669  that the same fi
-00000330: 6e61 6e63 6961 6c20 6d65 7472 6963 2063  nancial metric c
-00000340: 616e 2067 7265 6174 6c79 2076 6172 7920  an greatly vary 
-00000350: 7065 7220 736f 7572 6365 2061 6e64 2073  per source and s
-00000360: 6f20 646f 2074 6865 2066 696e 616e 6369  o do the financi
-00000370: 616c 2073 7461 7465 6d65 6e74 7320 7265  al statements re
-00000380: 706f 7274 6564 2077 6869 6c65 206c 6974  ported while lit
-00000390: 746c 6520 696e 666f 726d 6174 696f 6e20  tle information 
-000003a0: 6973 2067 6976 656e 2068 6f77 2074 6865  is given how the
-000003b0: 206d 6574 7269 6320 7761 7320 6361 6c63   metric was calc
-000003c0: 756c 6174 6564 2e0a 0a46 6f72 2065 7861  ulated...For exa
-000003d0: 6d70 6c65 2c20 4d69 6372 6f73 6f66 7427  mple, Microsoft'
-000003e0: 7320 5072 6963 652d 746f 2d45 6172 6e69  s Price-to-Earni
-000003f0: 6e67 7320 2850 4529 2072 6174 696f 206f  ngs (PE) ratio o
-00000400: 6e20 7468 6520 3674 6820 6f66 204d 6179  n the 6th of May
-00000410: 2c20 3230 3233 2069 7320 7265 706f 7274  , 2023 is report
-00000420: 6564 2074 6f20 6265 2032 382e 3933 2028  ed to be 28.93 (
-00000430: 5374 6f63 6b6f 7065 6469 6129 2c20 3332  Stockopedia), 32
-00000440: 2e30 3520 284d 6f72 6e69 6e67 7374 6172  .05 (Morningstar
-00000450: 292c 2033 322e 3636 2028 4d61 6372 6f74  ), 32.66 (Macrot
-00000460: 7265 6e64 7329 2c20 3333 2e30 3920 2846  rends), 33.09 (F
-00000470: 696e 616e 6365 2043 6861 7274 7329 2c20  inance Charts), 
-00000480: 3333 2e36 3620 2859 2043 6861 7274 7329  33.66 (Y Charts)
-00000490: 2c20 3333 2e36 3720 2857 616c 6c20 5374  , 33.67 (Wall St
-000004a0: 7265 6574 204a 6f75 726e 616c 292c 2033  reet Journal), 3
-000004b0: 332e 3830 2028 5961 686f 6f20 4669 6e61  3.80 (Yahoo Fina
-000004c0: 6e63 6529 2061 6e64 2033 342e 3420 2843  nce) and 34.4 (C
-000004d0: 6f6d 7061 6e69 6573 204d 6172 6b65 7420  ompanies Market 
-000004e0: 4361 7029 2e20 416c 6c20 6f66 2074 6865  Cap). All of the
-000004f0: 7365 2063 616c 6375 6c61 7469 6f6e 7320  se calculations 
-00000500: 6172 6520 636f 7272 6563 742c 2068 6f77  are correct, how
-00000510: 6576 6572 2074 6865 206d 6574 686f 6420  ever the method 
-00000520: 6170 706c 6965 6420 7661 7269 6573 206c  applied varies l
-00000530: 6561 6469 6e67 2074 6f20 6469 6666 6572  eading to differ
-00000540: 656e 7420 7265 7375 6c74 732e 2054 6865  ent results. The
-00000550: 7265 666f 7265 2c20 636f 6c6c 6563 7469  refore, collecti
-00000560: 6e67 2064 6174 6120 6672 6f6d 206d 756c  ng data from mul
-00000570: 7469 706c 6520 736f 7572 6365 7320 6361  tiple sources ca
-00000580: 6e20 6c65 6164 2074 6f20 7772 6f6e 6720  n lead to wrong 
-00000590: 696e 7465 7270 7265 7461 7469 6f6e 206f  interpretation o
-000005a0: 6620 7468 6520 7265 7375 6c74 7320 6769  f the results gi
-000005b0: 7665 6e20 7468 6174 206f 6e65 2073 6f75  ven that one sou
-000005c0: 7263 6520 636f 756c 6420 6265 2061 7070  rce could be app
-000005d0: 6c79 696e 6720 6120 6469 6666 6572 656e  lying a differen
-000005e0: 7420 6361 6c63 756c 6174 696f 6e20 6d65  t calculation me
-000005f0: 7468 6f64 2074 6861 6e20 616e 6f74 6865  thod than anothe
-00000600: 722e 2041 6e64 2074 6861 7420 6973 2c20  r. And that is, 
-00000610: 6966 2069 7420 6973 2065 7665 6e20 6672  if it is even fr
-00000620: 6565 6c79 2061 7661 696c 6162 6c65 2e20  eely available. 
-00000630: 4f66 7465 6e20 7468 6520 6361 6c63 756c  Often the calcul
-00000640: 6174 696f 6e20 6973 2068 6964 6465 6e20  ation is hidden 
-00000650: 6265 6869 6e64 2061 2070 6169 6420 7375  behind a paid su
-00000660: 6273 6372 6970 7469 6f6e 2e0a 0a2a 2a54  bscription...**T
-00000670: 6869 7320 6973 2077 6879 2049 2064 6573  his is why I des
-00000680: 6967 6e65 6420 7468 6520 4669 6e61 6e63  igned the Financ
-00000690: 6554 6f6f 6c6b 6974 2a2a 2c20 7468 6973  eToolkit**, this
-000006a0: 2069 7320 616e 206f 7065 6e2d 736f 7572   is an open-sour
-000006b0: 6365 2074 6f6f 6c6b 6974 2069 6e20 7768  ce toolkit in wh
-000006c0: 6963 6820 616c 6c20 7265 6c65 7661 6e74  ich all relevant
-000006d0: 2066 696e 616e 6369 616c 2072 6174 696f   financial ratio
-000006e0: 7320 2835 302b 292c 2069 6e64 6963 6174  s (50+), indicat
-000006f0: 6f72 7320 616e 6420 7065 7266 6f72 6d61  ors and performa
-00000700: 6e63 6520 6d65 6173 7572 656d 656e 7473  nce measurements
-00000710: 2061 7265 2077 7269 7474 656e 2064 6f77   are written dow
-00000720: 6e20 696e 2074 6865 206d 6f73 7420 7369  n in the most si
-00000730: 6d70 6c69 7374 6963 2077 6179 2061 6c6c  mplistic way all
-00000740: 6f77 696e 6720 666f 7220 636f 6d70 6c65  owing for comple
-00000750: 7465 2074 7261 6e73 7061 7265 6e63 7920  te transparency 
-00000760: 6f66 2074 6865 2063 616c 6375 6c61 7469  of the calculati
-00000770: 6f6e 206d 6574 686f 642e 2054 6869 7320  on method. This 
-00000780: 616c 6c6f 7773 2079 6f75 2074 6f20 6e6f  allows you to no
-00000790: 7420 6861 7665 2074 6f20 7265 6c79 206f  t have to rely o
-000007a0: 6e20 6d65 7472 6963 7320 6672 6f6d 206f  n metrics from o
-000007b0: 7468 6572 2070 726f 7669 6465 7273 2061  ther providers a
-000007c0: 6e64 2c20 6769 7665 6e20 6120 6669 6e61  nd, given a fina
-000007d0: 6e63 6961 6c20 7374 6174 656d 656e 742c  ncial statement,
-000007e0: 2061 6c6c 6f77 2066 6f72 2065 6666 6963   allow for effic
-000007f0: 6965 6e74 206d 616e 7561 6c20 6361 6c63  ient manual calc
-00000800: 756c 6174 696f 6e73 2e20 5468 6973 206c  ulations. This l
-00000810: 6561 6473 2074 6f20 6f6e 6520 756e 6966  eads to one unif
-00000820: 6f72 6d20 6d65 7468 6f64 206f 6620 6361  orm method of ca
-00000830: 6c63 756c 6174 696f 6e20 6265 696e 6720  lculation being 
-00000840: 6170 706c 6965 6420 7468 6174 2069 7320  applied that is 
-00000850: 6176 6169 6c61 626c 6520 616e 6420 756e  available and un
-00000860: 6465 7273 746f 6f64 2062 7920 6576 6572  derstood by ever
-00000870: 796f 6e65 2e0a 0a54 6865 2046 696e 616e  yone...The Finan
-00000880: 6365 2054 6f6f 6c6b 6974 2069 7320 636f  ce Toolkit is co
-00000890: 6d70 6c69 6d65 6e74 6564 2076 6572 7920  mplimented very 
-000008a0: 7765 6c6c 2077 6974 6820 7468 6520 5b46  well with the [F
-000008b0: 696e 616e 6365 2044 6174 6162 6173 6520  inance Database 
-000008c0: f09f 8c8e 5d28 6874 7470 733a 2f2f 6769  ....](https://gi
-000008d0: 7468 7562 2e63 6f6d 2f4a 6572 426f 756d  thub.com/JerBoum
-000008e0: 612f 4669 6e61 6e63 6544 6174 6162 6173  a/FinanceDatabas
-000008f0: 6529 2c20 6120 6461 7461 6261 7365 2074  e), a database t
-00000900: 6861 7420 6665 6174 7572 6573 2033 3030  hat features 300
-00000910: 2e30 3030 2b20 7379 6d62 6f6c 7320 636f  .000+ symbols co
-00000920: 6e74 6169 6e69 6e67 2045 7175 6974 6965  ntaining Equitie
-00000930: 732c 2045 5446 732c 2046 756e 6473 2c20  s, ETFs, Funds, 
-00000940: 496e 6469 6365 732c 2043 7572 7265 6e63  Indices, Currenc
-00000950: 6965 732c 2043 7279 7074 6f63 7572 7265  ies, Cryptocurre
-00000960: 6e63 6965 7320 616e 6420 4d6f 6e65 7920  ncies and Money 
-00000970: 4d61 726b 6574 732e 2042 7920 7574 696c  Markets. By util
-00000980: 6973 696e 6720 626f 7468 2c20 6974 2069  ising both, it i
-00000990: 7320 706f 7373 6962 6c65 2074 6f20 646f  s possible to do
-000009a0: 2061 2066 756c 6c79 2d66 6c65 6467 6564   a fully-fledged
-000009b0: 2063 6f6d 7065 7469 7469 7665 2061 6e61   competitive ana
-000009c0: 6c79 7369 7320 7769 7468 2074 6865 2074  lysis with the t
-000009d0: 6963 6b65 7273 2066 6f75 6e64 2066 726f  ickers found fro
-000009e0: 6d20 7468 6520 4669 6e61 6e63 6544 6174  m the FinanceDat
-000009f0: 6162 6173 6520 696e 7075 7474 6564 2069  abase inputted i
-00000a00: 6e74 6f20 7468 6520 4669 6e61 6e63 6554  nto the FinanceT
-00000a10: 6f6f 6c6b 6974 2e0a 0a3c 7020 616c 6967  oolkit...<p alig
-00000a20: 6e3d 2263 656e 7465 7222 3e0a 2020 2020  n="center">.    
-00000a30: 3c69 6d67 2073 7263 3d22 6578 616d 706c  <img src="exampl
-00000a40: 6573 2f46 696e 616e 6365 2054 6f6f 6c6b  es/Finance Toolk
-00000a50: 6974 202d 2035 2e20 5669 6465 6f20 4465  it - 5. Video De
-00000a60: 6d6f 2e67 6966 2220 616c 743d 2246 696e  mo.gif" alt="Fin
-00000a70: 616e 6365 2054 6f6f 6c6b 6974 2049 6c6c  ance Toolkit Ill
-00000a80: 7573 7472 6174 696f 6e22 2077 6964 7468  ustration" width
-00000a90: 3d22 3130 3025 2220 6f6e 6572 726f 723d  ="100%" onerror=
-00000aa0: 2774 6869 732e 7374 796c 652e 6469 7370  'this.style.disp
-00000ab0: 6c61 7920 3d20 226e 6f6e 6522 272f 3e0a  lay = "none"'/>.
-00000ac0: 3c2f 703e 0a0a 2d2d 2d0a 0a23 2054 6162  </p>..---..# Tab
-00000ad0: 6c65 206f 6620 436f 6e74 656e 7473 0a0a  le of Contents..
-00000ae0: 312e 205b 496e 7374 616c 6c61 7469 6f6e  1. [Installation
-00000af0: 5d28 2369 6e73 7461 6c6c 6174 696f 6e29  ](#installation)
-00000b00: 0a32 2e20 5b42 6173 6963 2055 7361 6765  .2. [Basic Usage
-00000b10: 5d28 2362 6173 6963 2d75 7361 6765 290a  ](#basic-usage).
-00000b20: 2020 2020 312e 205b 5573 696e 6720 7468      1. [Using th
-00000b30: 6520 4669 6e61 6e63 6520 546f 6f6c 6b69  e Finance Toolki
-00000b40: 745d 2823 7573 696e 672d 7468 652d 6669  t](#using-the-fi
-00000b50: 6e61 6e63 652d 746f 6f6c 6b69 7429 0a20  nance-toolkit). 
-00000b60: 2020 2032 2e20 5b57 6f72 6b69 6e67 2077     2. [Working w
-00000b70: 6974 6820 6f74 6865 7220 4461 7461 7365  ith other Datase
-00000b80: 7473 5d28 2377 6f72 6b69 6e67 2d77 6974  ts](#working-wit
-00000b90: 682d 6f74 6865 722d 6461 7461 7365 7473  h-other-datasets
-00000ba0: 290a 2020 2020 332e 205b 4361 6c6c 696e  ).    3. [Callin
-00000bb0: 6720 4675 6e63 7469 6f6e 7320 4469 7265  g Functions Dire
-00000bc0: 6374 6c79 5d28 2363 616c 6c69 6e67 2d66  ctly](#calling-f
-00000bd0: 756e 6374 696f 6e73 2d64 6972 6563 746c  unctions-directl
-00000be0: 7929 0a33 2e20 5b43 6f6e 7461 6374 5d28  y).3. [Contact](
-00000bf0: 2363 6f6e 7461 6374 290a 0a23 2049 6e73  #contact)..# Ins
-00000c00: 7461 6c6c 6174 696f 6e0a 0a54 6f20 696e  tallation..To in
-00000c10: 7374 616c 6c20 7468 6520 4669 6e61 6e63  stall the Financ
-00000c20: 6554 6f6f 6c6b 6974 2069 7420 7369 6d70  eToolkit it simp
-00000c30: 6c79 2072 6571 7569 7265 7320 7468 6520  ly requires the 
-00000c40: 666f 6c6c 6f77 696e 673a 0a0a 6060 600a  following:..```.
-00000c50: 7069 7020 696e 7374 616c 6c20 6669 6e61  pip install fina
-00000c60: 6e63 6574 6f6f 6c6b 6974 0a60 6060 600a  ncetoolkit.````.
-00000c70: 0a54 6865 6e20 7769 7468 696e 2050 7974  .Then within Pyt
-00000c80: 686f 6e20 7573 653a 0a0a 6060 6070 7974  hon use:..```pyt
-00000c90: 686f 6e0a 6672 6f6d 2066 696e 616e 6365  hon.from finance
-00000ca0: 746f 6f6c 6b69 7420 696d 706f 7274 2054  toolkit import T
-00000cb0: 6f6f 6c6b 6974 0a60 6060 0a54 6f20 6265  oolkit.```.To be
-00000cc0: 2061 626c 6520 746f 2067 6574 2073 7461   able to get sta
-00000cd0: 7274 6564 2c20 796f 7520 6e65 6564 2074  rted, you need t
-00000ce0: 6f20 6f62 7461 696e 2061 6e20 4150 4920  o obtain an API 
-00000cf0: 4b65 7920 6672 6f6d 2046 696e 616e 6369  Key from Financi
-00000d00: 616c 4d6f 6465 6c69 6e67 5072 6570 2e20  alModelingPrep. 
-00000d10: 5573 6520 7468 6520 666f 6c6c 6f77 696e  Use the followin
-00000d20: 6720 696e 7374 7275 6374 696f 6e73 2074  g instructions t
-00000d30: 6f20 6f62 7461 696e 2061 205f 6672 6565  o obtain a _free
-00000d40: 5f20 4150 4920 4b65 792e 204e 6f74 6520  _ API Key. Note 
-00000d50: 7468 6174 2074 6865 7365 206b 6579 7320  that these keys 
-00000d60: 6172 6520 6c69 6d69 7465 6420 746f 2032  are limited to 2
-00000d70: 3530 2072 6571 7565 7374 7320 7065 7220  50 requests per 
-00000d80: 6461 7920 6275 7420 7468 6520 7072 656d  day but the prem
-00000d90: 6975 6d20 706c 616e 7320 6172 6520 6b65  ium plans are ke
-00000da0: 7074 2061 7420 6120 6c6f 7720 636f 7374  pt at a low cost
-00000db0: 2069 6e20 6361 7365 2079 6f75 2064 6f20   in case you do 
-00000dc0: 7275 6e20 6f75 7420 6f66 2074 6865 206c  run out of the l
-00000dd0: 696d 6974 206f 7220 6861 7665 2061 206e  imit or have a n
-00000de0: 6565 6420 666f 7220 6163 6365 7373 2074  eed for access t
-00000df0: 6f20 6d6f 7265 2064 6174 612e 202a 2a49  o more data. **I
-00000e00: 7420 6973 2070 6f73 7369 626c 6520 746f  t is possible to
-00000e10: 2075 7365 2079 6f75 7220 6f77 6e20 7365   use your own se
-00000e20: 7420 6f66 2066 696e 616e 6369 616c 2073  t of financial s
-00000e30: 7461 7465 6d65 6e74 7320 616e 6420 6e6f  tatements and no
-00000e40: 7420 7265 6c79 206f 6e20 4669 6e61 6e63  t rely on Financ
-00000e50: 6961 6c4d 6f64 656c 696e 6750 7265 702c  ialModelingPrep,
-00000e60: 2070 6c65 6173 6520 6861 7665 2061 206c   please have a l
-00000e70: 6f6f 6b20 5b68 6572 655d 2823 776f 726b  ook [here](#work
-00000e80: 696e 672d 7769 7468 2d6f 7468 6572 2d64  ing-with-other-d
-00000e90: 6174 6173 6574 7329 2e2a 2a0a 0a31 2e20  atasets).**..1. 
-00000ea0: 476f 2074 6f20 5b46 696e 616e 6369 616c  Go to [Financial
-00000eb0: 4d6f 6465 6c6c 696e 6750 7265 7027 7320  ModellingPrep's 
-00000ec0: 4150 495d 2868 7474 7073 3a2f 2f66 696e  API](https://fin
-00000ed0: 616e 6369 616c 6d6f 6465 6c69 6e67 7072  ancialmodelingpr
-00000ee0: 6570 2e63 6f6d 2f64 6576 656c 6f70 6572  ep.com/developer
-00000ef0: 2f64 6f63 732f 290a 322e 2055 6e64 6572  /docs/).2. Under
-00000f00: 2022 4765 7420 796f 7572 2046 7265 6520   "Get your Free 
-00000f10: 4150 4920 4b65 7920 546f 6461 7921 2220  API Key Today!" 
-00000f20: 636c 6963 6b20 6f6e 2022 4765 7420 6d79  click on "Get my
-00000f30: 2041 5049 204b 4559 2068 6572 6522 0a33   API KEY here".3
-00000f40: 2e20 5369 676e 2d75 7020 746f 2074 6865  . Sign-up to the
-00000f50: 2077 6562 7369 7465 2061 6e64 2073 656c   website and sel
-00000f60: 6563 7420 7468 6520 4672 6565 2050 6c61  ect the Free Pla
-00000f70: 6e0a 342e 204f 6274 6169 6e20 7468 6520  n.4. Obtain the 
-00000f80: 4150 4920 4b65 7920 6173 2066 6f75 6e64  API Key as found
-00000f90: 205b 6865 7265 5d28 6874 7470 733a 2f2f   [here](https://
-00000fa0: 6669 6e61 6e63 6961 6c6d 6f64 656c 696e  financialmodelin
-00000fb0: 6770 7265 702e 636f 6d2f 6465 7665 6c6f  gprep.com/develo
-00000fc0: 7065 722f 646f 6373 2f29 0a35 2e20 5374  per/docs/).5. St
-00000fd0: 6172 7420 7573 696e 6720 7468 6973 2070  art using this p
-00000fe0: 6163 6b61 6765 2e0a 0a4e 6f74 6520 7468  ackage...Note th
-00000ff0: 6174 2049 2061 6d20 696e 206e 6f20 7761  at I am in no wa
-00001000: 7920 6166 6669 6c69 6174 6564 2046 696e  y affiliated Fin
-00001010: 616e 6369 616c 4d6f 6465 6c69 6e67 7072  ancialModelingpr
-00001020: 6570 2061 6e64 206e 6576 6572 2077 696c  ep and never wil
-00001030: 6c20 6265 2e20 4920 6861 7665 2063 686f  l be. I have cho
-00001040: 7365 6e20 7468 6569 7220 736f 7572 6365  sen their source
-00001050: 2061 7320 4920 6669 6e64 2069 7420 746f   as I find it to
-00001060: 2062 6520 7468 6520 6d6f 7374 2074 7261   be the most tra
-00001070: 6e73 7061 7265 6e74 2061 6e64 2072 656c  nsparent and rel
-00001080: 6961 626c 652e 2057 6865 6e20 796f 7520  iable. When you 
-00001090: 6e6f 7469 6365 2074 6861 7420 6461 7461  notice that data
-000010a0: 2069 7320 696e 6163 6375 7261 7465 206f   is inaccurate o
-000010b0: 7220 6861 7665 2061 6e79 206f 7468 6572  r have any other
-000010c0: 2069 7373 7565 2072 656c 6174 6564 2074   issue related t
-000010d0: 6f20 7468 6520 6461 7461 2c20 6e6f 7465  o the data, note
-000010e0: 2074 6861 7420 4920 7369 6d70 6c79 2070   that I simply p
-000010f0: 726f 7669 6465 2074 6865 206d 6561 6e73  rovide the means
-00001100: 2074 6f20 6163 6365 7373 2074 6869 7320   to access this 
-00001110: 6461 7461 2061 6e64 2049 2061 6d20 6e6f  data and I am no
-00001120: 7420 7265 7370 6f6e 7369 626c 6520 666f  t responsible fo
-00001130: 7220 7468 6520 6163 6375 7261 6379 206f  r the accuracy o
-00001140: 6620 7468 6520 6461 7461 2069 7473 656c  f the data itsel
-00001150: 662e 2046 6f72 2074 6869 732c 2075 7365  f. For this, use
-00001160: 205b 7468 6569 7220 636f 6e74 6163 7420   [their contact 
-00001170: 666f 726d 5d28 6874 7470 733a 2f2f 7369  form](https://si
-00001180: 7465 2e66 696e 616e 6369 616c 6d6f 6465  te.financialmode
-00001190: 6c69 6e67 7072 6570 2e63 6f6d 2f63 6f6e  lingprep.com/con
-000011a0: 7461 6374 2920 6f72 2070 726f 7669 6465  tact) or provide
-000011b0: 2074 6865 2064 6174 6120 796f 7572 7365   the data yourse
-000011c0: 6c66 2e20 0a0a 2320 4261 7369 6320 5573  lf. ..# Basic Us
-000011d0: 6167 650a 0a54 6869 7320 7365 6374 696f  age..This sectio
-000011e0: 6e20 6578 706c 6169 6e73 2069 6e20 6465  n explains in de
-000011f0: 7461 696c 2068 6f77 2074 6865 2046 696e  tail how the Fin
-00001200: 616e 6365 2054 6f6f 6c6b 6974 2063 616e  ance Toolkit can
-00001210: 2075 7469 6c69 7469 7365 6420 6566 6665   utilitised effe
-00001220: 6374 6976 656c 792e 2041 6c73 6f20 7365  ctively. Also se
-00001230: 6520 7468 6520 4a75 7079 7465 7220 4e6f  e the Jupyter No
-00001240: 7465 626f 6f6b 2069 6e20 7768 6963 6820  tebook in which 
-00001250: 796f 7520 6361 6e20 7275 6e20 7468 6520  you can run the 
-00001260: 6578 616d 706c 6573 2061 6c73 6f20 6465  examples also de
-00001270: 6d6f 6e73 7472 6174 6564 2068 6572 652e  monstrated here.
-00001280: 0a0a 5f5f 5f20 0a0a 3c62 3e3c 6469 7620  ..___ ..<b><div 
-00001290: 616c 6967 6e3d 2263 656e 7465 7222 3e46  align="center">F
-000012a0: 696e 6420 6120 7661 7269 6574 7920 6f66  ind a variety of
-000012b0: 2048 6f77 2d54 6f20 4775 6964 6573 2066   How-To Guides f
-000012c0: 6f72 2074 6865 2046 696e 616e 6365 546f  or the FinanceTo
-000012d0: 6f6c 6b69 7420 3c61 2068 7265 663d 2268  olkit <a href="h
-000012e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000012f0: 6d2f 4a65 7242 6f75 6d61 2f46 696e 616e  m/JerBouma/Finan
-00001300: 6365 546f 6f6c 6b69 742f 7472 6565 2f6d  ceToolkit/tree/m
-00001310: 6169 6e2f 6578 616d 706c 6573 223e 6865  ain/examples">he
-00001320: 7265 3c2f 613e 2e3c 2f64 6976 3e3c 2f62  re</a>.</div></b
-00001330: 3e0a 5f5f 5f0a 0a57 6974 6869 6e20 7468  >.___..Within th
-00001340: 6973 2070 6163 6b61 6765 2074 6865 2066  is package the f
-00001350: 6f6c 6c6f 7769 6e67 2074 6869 6e67 7320  ollowing things 
-00001360: 6172 6520 696e 636c 7564 6564 3a0a 0a2d  are included:..-
-00001370: 2043 6f6d 7061 6e79 2070 726f 6669 6c65   Company profile
-00001380: 7320 2860 7072 6f66 696c 6560 292c 2069  s (`profile`), i
-00001390: 6e63 6c75 6469 6e67 2063 6f75 6e74 7279  ncluding country
-000013a0: 2c20 7365 6374 6f72 2c20 4953 494e 2061  , sector, ISIN a
-000013b0: 6e64 2067 656e 6572 616c 2063 6861 7261  nd general chara
-000013c0: 6374 6572 6973 7469 6373 2028 6672 6f6d  cteristics (from
-000013d0: 2046 696e 616e 6369 616c 4d6f 6465 6c69   FinancialModeli
-000013e0: 6e67 5072 6570 290a 2d20 436f 6d70 616e  ngPrep).- Compan
-000013f0: 7920 7175 6f74 6573 2028 6071 756f 7465  y quotes (`quote
-00001400: 6029 2c20 696e 636c 7564 696e 6720 3532  `), including 52
-00001410: 2077 6565 6b20 6869 6768 7320 616e 6420   week highs and 
-00001420: 6c6f 7773 2c20 766f 6c75 6d65 206d 6574  lows, volume met
-00001430: 7269 6373 2061 6e64 2063 7572 7265 6e74  rics and current
-00001440: 2073 6861 7265 7320 6f75 7473 7461 6e64   shares outstand
-00001450: 696e 6720 2866 726f 6d20 4669 6e61 6e63  ing (from Financ
-00001460: 6961 6c4d 6f64 656c 696e 6750 7265 7029  ialModelingPrep)
-00001470: 0a2d 204d 6172 6b65 7420 6361 7020 616e  .- Market cap an
-00001480: 6420 656e 7465 7270 7269 7365 2076 616c  d enterprise val
-00001490: 7565 7320 2860 656e 7465 7270 7269 7365  ues (`enterprise
-000014a0: 6029 2c20 696e 636c 7564 696e 6720 6576  `), including ev
-000014b0: 6572 7920 696e 7465 726d 6564 6961 7465  ery intermediate
-000014c0: 2073 7465 7020 2866 726f 6d20 4669 6e61   step (from Fina
-000014d0: 6e63 6961 6c4d 6f64 656c 696e 6750 7265  ncialModelingPre
-000014e0: 7029 0a2d 2043 6f6d 7061 6e79 2072 6174  p).- Company rat
-000014f0: 696e 6773 2028 6072 6174 696e 6760 292c  ings (`rating`),
-00001500: 2062 6173 6564 206f 6e20 6b65 7920 696e   based on key in
-00001510: 6469 6361 746f 7273 206c 696b 6520 5045  dicators like PE
-00001520: 2061 6e64 2044 4520 7261 7469 6f73 2028   and DE ratios (
-00001530: 6672 6f6d 2046 696e 616e 6369 616c 4d6f  from FinancialMo
-00001540: 6465 6c69 6e67 5072 6570 290a 2d20 4869  delingPrep).- Hi
-00001550: 7374 6f72 6963 616c 206d 6172 6b65 7420  storical market 
-00001560: 6461 7461 2028 6068 6973 746f 7269 6361  data (`historica
-00001570: 6c5f 6461 7461 6029 2c20 7768 6963 6820  l_data`), which 
-00001580: 6361 6e20 6265 2072 6574 7269 6576 6564  can be retrieved
-00001590: 206f 6e20 6120 6461 696c 792c 2077 6565   on a daily, wee
-000015a0: 6b6c 792c 206d 6f6e 7468 6c79 2061 6e64  kly, monthly and
-000015b0: 2079 6561 726c 7920 6261 7369 7320 2866   yearly basis (f
-000015c0: 726f 6d20 5961 686f 6f20 4669 6e61 6e63  rom Yahoo Financ
-000015d0: 6529 0a2d 2042 616c 616e 6365 2053 6865  e).- Balance She
-000015e0: 6574 2053 7461 7465 6d65 6e74 7320 2860  et Statements (`
-000015f0: 6261 6c61 6e63 655f 7368 6565 745f 7374  balance_sheet_st
-00001600: 6174 656d 656e 7460 292c 2049 6e63 6f6d  atement`), Incom
-00001610: 6520 5374 6174 656d 656e 7473 2028 6069  e Statements (`i
-00001620: 6e63 6f6d 655f 7374 6174 656d 656e 7460  ncome_statement`
-00001630: 2920 616e 6420 4361 7368 2046 6c6f 7720  ) and Cash Flow 
-00001640: 5374 6174 656d 656e 7473 2028 6063 6173  Statements (`cas
-00001650: 685f 666c 6f77 5f73 7461 7465 6d65 6e74  h_flow_statement
-00001660: 6029 2c20 6f62 7461 696e 6162 6c65 2066  `), obtainable f
-00001670: 726f 6d20 4669 6e61 6e63 6961 6c4d 6f64  rom FinancialMod
-00001680: 656c 696e 6750 7265 7020 6f72 2074 6865  elingPrep or the
-00001690: 2073 6f75 7263 6520 6f66 2079 6f75 7220   source of your 
-000016a0: 6368 6f6f 7369 6e67 2074 6872 6f75 6768  choosing through
-000016b0: 2063 7573 746f 6d20 696e 7075 742e 2054   custom input. T
-000016c0: 6865 7365 2066 756e 6374 696f 6e73 2061  hese functions a
-000016d0: 7265 2061 6363 6f6d 7061 6e69 6564 2077  re accompanied w
-000016e0: 6974 6820 6120 6e6f 726d 616c 697a 6174  ith a normalizat
-000016f0: 696f 6e20 6675 6e63 7469 6f6e 2073 6f20  ion function so 
-00001700: 7468 6174 2066 6f72 2061 6e79 2073 6f75  that for any sou
-00001710: 7263 652c 2074 6865 2073 616d 6520 7261  rce, the same ra
-00001720: 7469 6f20 616e 616c 7973 6973 2063 616e  tio analysis can
-00001730: 2062 6520 7065 7266 6f72 6d65 642e 2050   be performed. P
-00001740: 6c65 6173 6520 7365 6520 7468 6973 204a  lease see this J
-00001750: 7570 7974 6572 204e 6f74 6562 6f6f 6b20  upyter Notebook 
-00001760: 7468 6174 2065 7870 6c61 696e 7320 686f  that explains ho
-00001770: 7720 746f 2075 7365 2061 2063 7573 746f  w to use a custo
-00001780: 6d20 736f 7572 6365 2e0a 2d20 4566 6669  m source..- Effi
-00001790: 6369 656e 6379 2072 6174 696f 7320 2860  ciency ratios (`
-000017a0: 6566 6669 6369 656e 6379 5f72 6174 696f  efficiency_ratio
-000017b0: 7360 292c 206c 6971 7569 6469 7479 2072  s`), liquidity r
-000017c0: 6174 696f 7320 2860 6c69 7175 6964 6974  atios (`liquidit
-000017d0: 795f 7261 7469 6f73 6029 2c20 7072 6f66  y_ratios`), prof
-000017e0: 6974 6162 696c 6974 7920 7261 7469 6f73  itability ratios
-000017f0: 2028 6070 726f 6669 7461 6269 6c69 7479   (`profitability
-00001800: 5f72 6174 696f 7360 292c 2073 6f6c 7665  _ratios`), solve
-00001810: 6e63 7920 7261 7469 6f73 2028 6073 6f6c  ncy ratios (`sol
-00001820: 7665 6e63 795f 7261 7469 6f73 6029 2061  vency_ratios`) a
-00001830: 6e64 2076 616c 7561 7469 6f6e 2072 6174  nd valuation rat
-00001840: 696f 7320 2860 7661 6c75 6174 696f 6e5f  ios (`valuation_
-00001850: 7261 7469 6f73 6029 2066 756e 6374 696f  ratios`) functio
-00001860: 6e61 6c69 7479 2074 6861 7420 6175 746f  nality that auto
-00001870: 6d61 7469 6361 6c6c 7920 6361 6c63 756c  matically calcul
-00001880: 6174 6573 2074 6865 206d 6f73 7420 696d  ates the most im
-00001890: 706f 7274 616e 7420 7261 7469 6f73 2062  portant ratios b
-000018a0: 6173 6564 206f 6e20 7468 6520 696e 7075  ased on the inpu
-000018b0: 7474 6564 2062 616c 616e 6365 2073 6865  tted balance she
-000018c0: 6574 2c20 696e 636f 6d65 2061 6e64 2063  et, income and c
-000018d0: 6173 6820 666c 6f77 2073 7461 7465 6d65  ash flow stateme
-000018e0: 6e74 732e 0a2d 204d 6f64 656c 7320 2860  nts..- Models (`
-000018f0: 6d6f 6465 6c73 6029 206c 696b 6520 4455  models`) like DU
-00001900: 504f 4e54 2061 6e61 6c79 7369 7320 7468  PONT analysis th
-00001910: 6174 2063 616e 2062 6520 7573 6564 2074  at can be used t
-00001920: 6f20 7065 7266 6f72 6d20 696e 2d64 6570  o perform in-dep
-00001930: 7468 2066 696e 616e 6369 616c 2061 6e61  th financial ana
-00001940: 6c79 7369 7320 7468 726f 7567 6820 6120  lysis through a 
-00001950: 7369 6e67 6c65 2066 756e 6374 696f 6e2e  single function.
-00001960: 0a0a 5468 6520 6465 7065 6e64 656e 6369  ..The dependenci
-00001970: 6573 206f 6620 7468 6520 7061 636b 6167  es of the packag
-00001980: 6520 6172 6520 6f6e 2070 7572 706f 7365  e are on purpose
-00001990: 202a 7665 7279 2073 6c69 6d2a 2073 6f20   *very slim* so 
-000019a0: 7468 6174 2069 7420 7769 6c6c 2077 6f72  that it will wor
-000019b0: 6b20 7765 6c6c 2077 6974 6820 616e 7920  k well with any 
-000019c0: 636f 6d62 696e 6174 696f 6e20 6f66 2070  combination of p
-000019d0: 6163 6b61 6765 7320 616e 6420 6e6f 7420  ackages and not 
-000019e0: 7265 7375 6c74 2069 6e20 636f 6e66 6c69  result in confli
-000019f0: 6374 732e 2049 2776 6520 616c 736f 2062  cts. I've also b
-00001a00: 6565 6e20 6361 7265 6675 6c20 7769 7468  een careful with
-00001a10: 206d 7920 7365 6c65 6374 696f 6e20 696e   my selection in
-00001a20: 2077 6869 6368 2049 206c 6561 7665 206f   which I leave o
-00001a30: 7574 2066 756e 6374 696f 6e61 6c69 7479  ut functionality
-00001a40: 206c 696b 6520 7465 6368 6e69 6361 6c20   like technical 
-00001a50: 616e 616c 7973 6973 2069 6e20 7768 6963  analysis in whic
-00001a60: 6820 5b74 612d 6c69 625d 2868 7474 7073  h [ta-lib](https
-00001a70: 3a2f 2f74 612d 6c69 622e 6f72 672f 2920  ://ta-lib.org/) 
-00001a80: 646f 6573 2061 6e20 6578 6365 6c6c 656e  does an excellen
-00001a90: 7420 6a6f 6220 6173 2077 656c 6c20 6173  t job as well as
-00001aa0: 2070 6f72 7466 6f6c 696f 2061 7474 7269   portfolio attri
-00001ab0: 6275 7469 6f6e 2061 6e64 206f 7074 696d  bution and optim
-00001ac0: 6973 6174 696f 6e20 696e 2077 6869 6368  isation in which
-00001ad0: 205b 5269 736b 666f 6c69 6f2d 6c69 625d   [Riskfolio-lib]
-00001ae0: 2868 7474 7073 3a2f 2f72 6973 6b66 6f6c  (https://riskfol
-00001af0: 696f 2d6c 6962 2e72 6561 6474 6865 646f  io-lib.readthedo
-00001b00: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
-00001b10: 696e 6465 782e 6874 6d6c 2920 7368 696e  index.html) shin
-00001b20: 6573 2061 6e64 206c 6173 746c 7920 616c  es and lastly al
-00001b30: 6c6f 7720 666f 7220 616e 7920 736f 7572  low for any sour
-00001b40: 6365 2074 6f20 6265 2069 6e63 6f72 706f  ce to be incorpo
-00001b50: 7261 7465 6420 746f 2061 6c6c 6f77 2066  rated to allow f
-00001b60: 6f72 2074 6865 2069 6e63 6f72 706f 7261  or the incorpora
-00001b70: 7469 6f6e 206f 6620 6461 7461 2073 6f75  tion of data sou
-00001b80: 7263 6573 2066 726f 6d20 5b4f 7065 6e42  rces from [OpenB
-00001b90: 425d 2868 7474 7073 3a2f 2f6f 7065 6e62  B](https://openb
-00001ba0: 622e 636f 2f29 2e0a 0a23 2320 5573 696e  b.co/)...## Usin
-00001bb0: 6720 7468 6520 4669 6e61 6e63 6520 546f  g the Finance To
-00001bc0: 6f6c 6b69 740a 0a41 2062 6173 6963 2065  olkit..A basic e
-00001bd0: 7861 6d70 6c65 206f 6620 686f 7720 746f  xample of how to
-00001be0: 2069 6e69 7469 616c 6973 6520 7468 6520   initialise the 
-00001bf0: 4669 6e61 6e63 6520 546f 6f6c 6b69 7420  Finance Toolkit 
-00001c00: 6973 2073 686f 776e 2062 656c 6f77 2c20  is shown below, 
-00001c10: 616c 736f 2073 6565 205b 7468 6973 206e  also see [this n
-00001c20: 6f74 6562 6f6f 6b5d 2868 7474 7073 3a2f  otebook](https:/
-00001c30: 2f67 6974 6875 622e 636f 6d2f 4a65 7242  /github.com/JerB
-00001c40: 6f75 6d61 2f46 696e 616e 6365 546f 6f6c  ouma/FinanceTool
-00001c50: 6b69 742f 626c 6f62 2f6d 6169 6e2f 6578  kit/blob/main/ex
-00001c60: 616d 706c 6573 2f46 696e 616e 6365 2532  amples/Finance%2
-00001c70: 3054 6f6f 6c6b 6974 2532 302d 2532 3031  0Toolkit%20-%201
-00001c80: 2e25 3230 4765 7474 696e 6725 3230 5374  .%20Getting%20St
-00001c90: 6172 7465 642e 6970 796e 6229 2066 6f72  arted.ipynb) for
-00001ca0: 2061 2064 6574 6169 6c65 6420 4765 7474   a detailed Gett
-00001cb0: 696e 6720 5374 6172 7465 6420 6775 6964  ing Started guid
-00001cc0: 6520 6173 2077 656c 6c20 6173 205b 7468  e as well as [th
-00001cd0: 6973 206e 6f74 6562 6f6f 6b5d 2868 7474  is notebook](htt
-00001ce0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001cf0: 4a65 7242 6f75 6d61 2f46 696e 616e 6365  JerBouma/Finance
-00001d00: 546f 6f6c 6b69 742f 626c 6f62 2f6d 6169  Toolkit/blob/mai
-00001d10: 6e2f 6578 616d 706c 6573 2f46 696e 616e  n/examples/Finan
-00001d20: 6365 2532 3054 6f6f 6c6b 6974 2532 302d  ce%20Toolkit%20-
-00001d30: 2532 3032 2e25 3230 436f 6d62 696e 696e  %202.%20Combinin
-00001d40: 6725 3230 7468 6525 3230 4669 6e61 6e63  g%20the%20Financ
-00001d50: 6525 3230 546f 6f6c 6b69 7425 3230 7769  e%20Toolkit%20wi
-00001d60: 7468 2532 3074 6865 2532 3046 696e 616e  th%20the%20Finan
-00001d70: 6365 2532 3044 6174 6162 6173 652e 6970  ce%20Database.ip
-00001d80: 796e 6229 2074 6861 7420 696e 636c 7564  ynb) that includ
-00001d90: 6573 2074 6865 205b 4669 6e61 6e63 6520  es the [Finance 
-00001da0: 4461 7461 6261 7365 20f0 9f8c 8e5d 2868  Database ....](h
-00001db0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001dc0: 6d2f 4a65 7242 6f75 6d61 2f46 696e 616e  m/JerBouma/Finan
-00001dd0: 6365 4461 7461 6261 7365 2920 616e 6420  ceDatabase) and 
-00001de0: 6120 7072 6f70 6572 2066 696e 616e 6369  a proper financi
-00001df0: 616c 2061 6e61 6c79 7369 732e 0a0a 6060  al analysis...``
-00001e00: 6060 7079 7468 6f6e 0a66 726f 6d20 6669  ``python.from fi
-00001e10: 6e61 6e63 6574 6f6f 6c6b 6974 2069 6d70  nancetoolkit imp
-00001e20: 6f72 7420 546f 6f6c 6b69 740a 0a63 6f6d  ort Toolkit..com
-00001e30: 7061 6e69 6573 203d 2054 6f6f 6c6b 6974  panies = Toolkit
-00001e40: 285b 2741 4150 4c27 2c20 274d 5346 5427  (['AAPL', 'MSFT'
-00001e50: 5d2c 2061 7069 5f6b 6579 3d22 464d 505f  ], api_key="FMP_
-00001e60: 4b45 5922 290a 0a23 2061 6e20 456e 7465  KEY")..# an Ente
-00001e70: 7270 7269 7365 2065 7861 6d70 6c65 0a65  rprise example.e
-00001e80: 6e74 6572 7072 6973 6520 3d20 636f 6d70  nterprise = comp
-00001e90: 616e 6965 732e 6765 745f 656e 7465 7270  anies.get_enterp
-00001ea0: 7269 7365 2829 0a0a 2320 6120 4869 7374  rise()..# a Hist
-00001eb0: 6f72 6963 616c 2065 7861 6d70 6c65 0a68  orical example.h
-00001ec0: 6973 746f 7269 6361 6c5f 6461 7461 203d  istorical_data =
-00001ed0: 2063 6f6d 7061 6e69 6573 2e67 6574 5f68   companies.get_h
-00001ee0: 6973 746f 7269 6361 6c5f 6461 7461 2873  istorical_data(s
-00001ef0: 7461 7274 3d27 3230 3030 2d30 312d 3031  tart='2000-01-01
-00001f00: 272c 2065 6e64 3d27 3230 3230 2d30 312d  ', end='2020-01-
-00001f10: 3031 2729 0a0a 2320 6120 4669 6e61 6e63  01')..# a Financ
-00001f20: 6961 6c20 5374 6174 656d 656e 7420 6578  ial Statement ex
-00001f30: 616d 706c 650a 6261 6c61 6e63 655f 7368  ample.balance_sh
-00001f40: 6565 745f 7374 6174 656d 656e 7420 3d20  eet_statement = 
-00001f50: 636f 6d70 616e 6965 732e 6765 745f 6261  companies.get_ba
-00001f60: 6c61 6e63 655f 7368 6565 745f 7374 6174  lance_sheet_stat
-00001f70: 656d 656e 7428 290a 0a23 2061 2052 6174  ement()..# a Rat
-00001f80: 696f 7320 6578 616d 706c 650a 7072 6f66  ios example.prof
-00001f90: 6974 6162 696c 6974 795f 7261 7469 6f73  itability_ratios
-00001fa0: 203d 2063 6f6d 7061 6e69 6573 2e72 6174   = companies.rat
-00001fb0: 696f 732e 636f 6c6c 6563 745f 7072 6f66  ios.collect_prof
-00001fc0: 6974 6162 696c 6974 795f 7261 7469 6f73  itability_ratios
-00001fd0: 2829 0a0a 2320 5368 6f77 2074 6865 2070  ()..# Show the p
-00001fe0: 726f 6669 7461 6269 6c69 7479 2072 6174  rofitability rat
-00001ff0: 696f 7320 666f 7220 4170 706c 650a 7072  ios for Apple.pr
-00002000: 6f66 6974 6162 696c 6974 795f 7261 7469  ofitability_rati
-00002010: 6f73 2e6c 6f63 5b27 4141 504c 275d 0a60  os.loc['AAPL'].`
-00002020: 6060 600a 0a54 6869 7320 7265 7475 726e  ```..This return
-00002030: 7320 7468 6520 666f 6c6c 6f77 696e 6720  s the following 
-00002040: 6f75 7470 7574 2066 6f72 2060 7072 6f66  output for `prof
-00002050: 6974 6162 696c 6974 795f 7261 7469 6f73  itability_ratios
-00002060: 2e6c 6f63 5b27 4141 504c 5d60 2e20 4f6d  .loc['AAPL]`. Om
-00002070: 6974 7469 6e67 2060 2e6c 6f63 5b27 4141  itting `.loc['AA
-00002080: 504c 275d 6020 7769 6c6c 2072 6574 7572  PL']` will retur
-00002090: 6e20 7468 6520 7265 7375 6c74 2066 6f72  n the result for
-000020a0: 2062 6f74 6820 4141 504c 2061 6e64 204d   both AAPL and M
-000020b0: 5346 542e 0a0a 0a7c 2020 2020 2020 2020  SFT....|        
-000020c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020e0: 2020 2020 207c 2020 2020 2032 3031 3820       |     2018 
-000020f0: 7c20 2020 2020 3230 3139 207c 2020 2020  |     2019 |    
-00002100: 2032 3032 3020 7c20 2020 2020 3230 3231   2020 |     2021
-00002110: 207c 2020 2020 2032 3032 3220 7c0a 7c3a   |     2022 |.|:
+000002e0: 546f 6f6c 6b69 742f 290a 5b21 5b50 5950  Toolkit/).[![PYP
+000002f0: 4920 446f 776e 6c6f 6164 735d 2868 7474  I Downloads](htt
+00000300: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000310: 2e69 6f2f 7079 7069 2f64 6d2f 4669 6e61  .io/pypi/dm/Fina
+00000320: 6e63 6554 6f6f 6c6b 6974 295d 2868 7474  nceToolkit)](htt
+00000330: 7073 3a2f 2f70 7970 692e 6f72 672f 7072  ps://pypi.org/pr
+00000340: 6f6a 6563 742f 4669 6e61 6e63 6554 6f6f  oject/FinanceToo
+00000350: 6c6b 6974 2f29 0a0a 5768 696c 6520 6272  lkit/)..While br
+00000360: 6f77 7369 6e67 2061 2076 6172 6965 7479  owsing a variety
+00000370: 206f 6620 7765 6273 6974 6573 2c20 4920   of websites, I 
+00000380: 6b65 7074 2066 696e 6469 6e67 2074 6861  kept finding tha
+00000390: 7420 7468 6520 7361 6d65 2066 696e 616e  t the same finan
+000003a0: 6369 616c 206d 6574 7269 6320 6361 6e20  cial metric can 
+000003b0: 6772 6561 746c 7920 7661 7279 2070 6572  greatly vary per
+000003c0: 2073 6f75 7263 6520 616e 6420 736f 2064   source and so d
+000003d0: 6f20 7468 6520 6669 6e61 6e63 6961 6c20  o the financial 
+000003e0: 7374 6174 656d 656e 7473 2072 6570 6f72  statements repor
+000003f0: 7465 6420 7768 696c 6520 6c69 7474 6c65  ted while little
+00000400: 2069 6e66 6f72 6d61 7469 6f6e 2069 7320   information is 
+00000410: 6769 7665 6e20 686f 7720 7468 6520 6d65  given how the me
+00000420: 7472 6963 2077 6173 2063 616c 6375 6c61  tric was calcula
+00000430: 7465 642e 0a0a 466f 7220 6578 616d 706c  ted...For exampl
+00000440: 652c 204d 6963 726f 736f 6674 2773 2050  e, Microsoft's P
+00000450: 7269 6365 2d74 6f2d 4561 726e 696e 6773  rice-to-Earnings
+00000460: 2028 5045 2920 7261 7469 6f20 6f6e 2074   (PE) ratio on t
+00000470: 6865 2036 7468 206f 6620 4d61 792c 2032  he 6th of May, 2
+00000480: 3032 3320 6973 2072 6570 6f72 7465 6420  023 is reported 
+00000490: 746f 2062 6520 3238 2e39 3320 2853 746f  to be 28.93 (Sto
+000004a0: 636b 6f70 6564 6961 292c 2033 322e 3035  ckopedia), 32.05
+000004b0: 2028 4d6f 726e 696e 6773 7461 7229 2c20   (Morningstar), 
+000004c0: 3332 2e36 3620 284d 6163 726f 7472 656e  32.66 (Macrotren
+000004d0: 6473 292c 2033 332e 3039 2028 4669 6e61  ds), 33.09 (Fina
+000004e0: 6e63 6520 4368 6172 7473 292c 2033 332e  nce Charts), 33.
+000004f0: 3636 2028 5920 4368 6172 7473 292c 2033  66 (Y Charts), 3
+00000500: 332e 3637 2028 5761 6c6c 2053 7472 6565  3.67 (Wall Stree
+00000510: 7420 4a6f 7572 6e61 6c29 2c20 3333 2e38  t Journal), 33.8
+00000520: 3020 2859 6168 6f6f 2046 696e 616e 6365  0 (Yahoo Finance
+00000530: 2920 616e 6420 3334 2e34 2028 436f 6d70  ) and 34.4 (Comp
+00000540: 616e 6965 7320 4d61 726b 6574 2043 6170  anies Market Cap
+00000550: 292e 2041 6c6c 206f 6620 7468 6573 6520  ). All of these 
+00000560: 6361 6c63 756c 6174 696f 6e73 2061 7265  calculations are
+00000570: 2063 6f72 7265 6374 2c20 686f 7765 7665   correct, howeve
+00000580: 7220 7468 6520 6d65 7468 6f64 2061 7070  r the method app
+00000590: 6c69 6564 2076 6172 6965 7320 6c65 6164  lied varies lead
+000005a0: 696e 6720 746f 2064 6966 6665 7265 6e74  ing to different
+000005b0: 2072 6573 756c 7473 2e20 5468 6572 6566   results. Theref
+000005c0: 6f72 652c 2063 6f6c 6c65 6374 696e 6720  ore, collecting 
+000005d0: 6461 7461 2066 726f 6d20 6d75 6c74 6970  data from multip
+000005e0: 6c65 2073 6f75 7263 6573 2063 616e 206c  le sources can l
+000005f0: 6561 6420 746f 2077 726f 6e67 2069 6e74  ead to wrong int
+00000600: 6572 7072 6574 6174 696f 6e20 6f66 2074  erpretation of t
+00000610: 6865 2072 6573 756c 7473 2067 6976 656e  he results given
+00000620: 2074 6861 7420 6f6e 6520 736f 7572 6365   that one source
+00000630: 2063 6f75 6c64 2062 6520 6170 706c 7969   could be applyi
+00000640: 6e67 2061 2064 6966 6665 7265 6e74 2063  ng a different c
+00000650: 616c 6375 6c61 7469 6f6e 206d 6574 686f  alculation metho
+00000660: 6420 7468 616e 2061 6e6f 7468 6572 2e20  d than another. 
+00000670: 416e 6420 7468 6174 2069 732c 2069 6620  And that is, if 
+00000680: 6974 2069 7320 6576 656e 2066 7265 656c  it is even freel
+00000690: 7920 6176 6169 6c61 626c 652e 204f 6674  y available. Oft
+000006a0: 656e 2074 6865 2063 616c 6375 6c61 7469  en the calculati
+000006b0: 6f6e 2069 7320 6869 6464 656e 2062 6568  on is hidden beh
+000006c0: 696e 6420 6120 7061 6964 2073 7562 7363  ind a paid subsc
+000006d0: 7269 7074 696f 6e2e 0a0a 2a2a 5468 6973  ription...**This
+000006e0: 2069 7320 7768 7920 4920 6465 7369 676e   is why I design
+000006f0: 6564 2074 6865 2046 696e 616e 6365 546f  ed the FinanceTo
+00000700: 6f6c 6b69 742a 2a2c 2074 6869 7320 6973  olkit**, this is
+00000710: 2061 6e20 6f70 656e 2d73 6f75 7263 6520   an open-source 
+00000720: 746f 6f6c 6b69 7420 696e 2077 6869 6368  toolkit in which
+00000730: 2061 6c6c 2072 656c 6576 616e 7420 6669   all relevant fi
+00000740: 6e61 6e63 6961 6c20 7261 7469 6f73 2028  nancial ratios (
+00000750: 3530 2b29 2c20 696e 6469 6361 746f 7273  50+), indicators
+00000760: 2061 6e64 2070 6572 666f 726d 616e 6365   and performance
+00000770: 206d 6561 7375 7265 6d65 6e74 7320 6172   measurements ar
+00000780: 6520 7772 6974 7465 6e20 646f 776e 2069  e written down i
+00000790: 6e20 7468 6520 6d6f 7374 2073 696d 706c  n the most simpl
+000007a0: 6973 7469 6320 7761 7920 616c 6c6f 7769  istic way allowi
+000007b0: 6e67 2066 6f72 2063 6f6d 706c 6574 6520  ng for complete 
+000007c0: 7472 616e 7370 6172 656e 6379 206f 6620  transparency of 
+000007d0: 7468 6520 6361 6c63 756c 6174 696f 6e20  the calculation 
+000007e0: 6d65 7468 6f64 2e20 5468 6973 2061 6c6c  method. This all
+000007f0: 6f77 7320 796f 7520 746f 206e 6f74 2068  ows you to not h
+00000800: 6176 6520 746f 2072 656c 7920 6f6e 206d  ave to rely on m
+00000810: 6574 7269 6373 2066 726f 6d20 6f74 6865  etrics from othe
+00000820: 7220 7072 6f76 6964 6572 7320 616e 642c  r providers and,
+00000830: 2067 6976 656e 2061 2066 696e 616e 6369   given a financi
+00000840: 616c 2073 7461 7465 6d65 6e74 2c20 616c  al statement, al
+00000850: 6c6f 7720 666f 7220 6566 6669 6369 656e  low for efficien
+00000860: 7420 6d61 6e75 616c 2063 616c 6375 6c61  t manual calcula
+00000870: 7469 6f6e 732e 2054 6869 7320 6c65 6164  tions. This lead
+00000880: 7320 746f 206f 6e65 2075 6e69 666f 726d  s to one uniform
+00000890: 206d 6574 686f 6420 6f66 2063 616c 6375   method of calcu
+000008a0: 6c61 7469 6f6e 2062 6569 6e67 2061 7070  lation being app
+000008b0: 6c69 6564 2074 6861 7420 6973 2061 7661  lied that is ava
+000008c0: 696c 6162 6c65 2061 6e64 2075 6e64 6572  ilable and under
+000008d0: 7374 6f6f 6420 6279 2065 7665 7279 6f6e  stood by everyon
+000008e0: 652e 0a0a 5468 6520 4669 6e61 6e63 6520  e...The Finance 
+000008f0: 546f 6f6c 6b69 7420 6973 2063 6f6d 706c  Toolkit is compl
+00000900: 696d 656e 7465 6420 7665 7279 2077 656c  imented very wel
+00000910: 6c20 7769 7468 2074 6865 205b 4669 6e61  l with the [Fina
+00000920: 6e63 6520 4461 7461 6261 7365 20f0 9f8c  nce Database ...
+00000930: 8e5d 2868 7474 7073 3a2f 2f67 6974 6875  .](https://githu
+00000940: 622e 636f 6d2f 4a65 7242 6f75 6d61 2f46  b.com/JerBouma/F
+00000950: 696e 616e 6365 4461 7461 6261 7365 292c  inanceDatabase),
+00000960: 2061 2064 6174 6162 6173 6520 7468 6174   a database that
+00000970: 2066 6561 7475 7265 7320 3330 302e 3030   features 300.00
+00000980: 302b 2073 796d 626f 6c73 2063 6f6e 7461  0+ symbols conta
+00000990: 696e 696e 6720 4571 7569 7469 6573 2c20  ining Equities, 
+000009a0: 4554 4673 2c20 4675 6e64 732c 2049 6e64  ETFs, Funds, Ind
+000009b0: 6963 6573 2c20 4375 7272 656e 6369 6573  ices, Currencies
+000009c0: 2c20 4372 7970 746f 6375 7272 656e 6369  , Cryptocurrenci
+000009d0: 6573 2061 6e64 204d 6f6e 6579 204d 6172  es and Money Mar
+000009e0: 6b65 7473 2e20 4279 2075 7469 6c69 7369  kets. By utilisi
+000009f0: 6e67 2062 6f74 682c 2069 7420 6973 2070  ng both, it is p
+00000a00: 6f73 7369 626c 6520 746f 2064 6f20 6120  ossible to do a 
+00000a10: 6675 6c6c 792d 666c 6564 6765 6420 636f  fully-fledged co
+00000a20: 6d70 6574 6974 6976 6520 616e 616c 7973  mpetitive analys
+00000a30: 6973 2077 6974 6820 7468 6520 7469 636b  is with the tick
+00000a40: 6572 7320 666f 756e 6420 6672 6f6d 2074  ers found from t
+00000a50: 6865 2046 696e 616e 6365 4461 7461 6261  he FinanceDataba
+00000a60: 7365 2069 6e70 7574 7465 6420 696e 746f  se inputted into
+00000a70: 2074 6865 2046 696e 616e 6365 546f 6f6c   the FinanceTool
+00000a80: 6b69 742e 0a0a 3c70 2061 6c69 676e 3d22  kit...<p align="
+00000a90: 6365 6e74 6572 223e 0a20 2020 203c 696d  center">.    <im
+00000aa0: 6720 7372 633d 2265 7861 6d70 6c65 732f  g src="examples/
+00000ab0: 4669 6e61 6e63 6520 546f 6f6c 6b69 7420  Finance Toolkit 
+00000ac0: 2d20 362e 2056 6964 656f 2044 656d 6f2e  - 6. Video Demo.
+00000ad0: 6769 6622 2061 6c74 3d22 4669 6e61 6e63  gif" alt="Financ
+00000ae0: 6520 546f 6f6c 6b69 7420 496c 6c75 7374  e Toolkit Illust
+00000af0: 7261 7469 6f6e 2220 7769 6474 683d 2231  ration" width="1
+00000b00: 3030 2522 206f 6e65 7272 6f72 3d22 7468  00%" onerror="th
+00000b10: 6973 2e73 7479 6c65 2e64 6973 706c 6179  is.style.display
+00000b20: 203d 2027 6e6f 6e65 2722 2f3e 0a3c 2f70   = 'none'"/>.</p
+00000b30: 3e0a 0a2d 2d2d 0a0a 2320 5461 626c 6520  >..---..# Table 
+00000b40: 6f66 2043 6f6e 7465 6e74 730a 0a31 2e20  of Contents..1. 
+00000b50: 5b49 6e73 7461 6c6c 6174 696f 6e5d 2823  [Installation](#
+00000b60: 696e 7374 616c 6c61 7469 6f6e 290a 322e  installation).2.
+00000b70: 205b 4261 7369 6320 5573 6167 655d 2823   [Basic Usage](#
+00000b80: 6261 7369 632d 7573 6167 6529 0a20 2020  basic-usage).   
+00000b90: 2031 2e20 5b55 7369 6e67 2074 6865 2046   1. [Using the F
+00000ba0: 696e 616e 6365 2054 6f6f 6c6b 6974 5d28  inance Toolkit](
+00000bb0: 2375 7369 6e67 2d74 6865 2d66 696e 616e  #using-the-finan
+00000bc0: 6365 2d74 6f6f 6c6b 6974 290a 2020 2020  ce-toolkit).    
+00000bd0: 322e 205b 4465 6669 6e69 6e67 2043 7573  2. [Defining Cus
+00000be0: 746f 6d20 5261 7469 6f73 5d28 2364 6566  tom Ratios](#def
+00000bf0: 696e 696e 672d 6375 7374 6f6d 2d72 6174  ining-custom-rat
+00000c00: 696f 7329 0a20 2020 2033 2e20 5b43 616c  ios).    3. [Cal
+00000c10: 6c69 6e67 2046 756e 6374 696f 6e73 2044  ling Functions D
+00000c20: 6972 6563 746c 795d 2823 6361 6c6c 696e  irectly](#callin
+00000c30: 672d 6675 6e63 7469 6f6e 732d 6469 7265  g-functions-dire
+00000c40: 6374 6c79 290a 2020 2020 342e 205b 576f  ctly).    4. [Wo
+00000c50: 726b 696e 6720 7769 7468 206f 7468 6572  rking with other
+00000c60: 2044 6174 6173 6574 735d 2823 776f 726b   Datasets](#work
+00000c70: 696e 672d 7769 7468 2d6f 7468 6572 2d64  ing-with-other-d
+00000c80: 6174 6173 6574 7329 0a33 2e20 5b43 6f6e  atasets).3. [Con
+00000c90: 7461 6374 5d28 2363 6f6e 7461 6374 290a  tact](#contact).
+00000ca0: 0a23 2049 6e73 7461 6c6c 6174 696f 6e0a  .# Installation.
+00000cb0: 0a54 6f20 696e 7374 616c 6c20 7468 6520  .To install the 
+00000cc0: 4669 6e61 6e63 6554 6f6f 6c6b 6974 2069  FinanceToolkit i
+00000cd0: 7420 7369 6d70 6c79 2072 6571 7569 7265  t simply require
+00000ce0: 7320 7468 6520 666f 6c6c 6f77 696e 673a  s the following:
+00000cf0: 0a0a 6060 600a 7069 7020 696e 7374 616c  ..```.pip instal
+00000d00: 6c20 6669 6e61 6e63 6574 6f6f 6c6b 6974  l financetoolkit
+00000d10: 0a60 6060 600a 0a54 6865 6e20 7769 7468  .````..Then with
+00000d20: 696e 2050 7974 686f 6e20 7573 653a 0a0a  in Python use:..
+00000d30: 6060 6070 7974 686f 6e0a 6672 6f6d 2066  ```python.from f
+00000d40: 696e 616e 6365 746f 6f6c 6b69 7420 696d  inancetoolkit im
+00000d50: 706f 7274 2054 6f6f 6c6b 6974 0a60 6060  port Toolkit.```
+00000d60: 0a54 6f20 6265 2061 626c 6520 746f 2067  .To be able to g
+00000d70: 6574 2073 7461 7274 6564 2c20 796f 7520  et started, you 
+00000d80: 6e65 6564 2074 6f20 6f62 7461 696e 2061  need to obtain a
+00000d90: 6e20 4150 4920 4b65 7920 6672 6f6d 2046  n API Key from F
+00000da0: 696e 616e 6369 616c 4d6f 6465 6c69 6e67  inancialModeling
+00000db0: 5072 6570 2e20 5468 6973 2069 7320 7573  Prep. This is us
+00000dc0: 6564 2074 6f20 6761 696e 2061 6363 6573  ed to gain acces
+00000dd0: 7320 746f 2033 302b 2079 6561 7273 206f  s to 30+ years o
+00000de0: 6620 6669 6e61 6e63 6961 6c20 7374 6174  f financial stat
+00000df0: 656d 656e 7420 626f 7468 2061 6e6e 7561  ement both annua
+00000e00: 6c6c 7920 616e 6420 7175 6172 7465 726c  lly and quarterl
+00000e10: 792e 204e 6f74 6520 7468 6174 2074 6865  y. Note that the
+00000e20: 2046 7265 6520 706c 616e 2069 7320 6c69   Free plan is li
+00000e30: 6d69 7465 6420 746f 2032 3530 2072 6571  mited to 250 req
+00000e40: 7565 7374 7320 6561 6368 2064 6179 2c20  uests each day, 
+00000e50: 3520 7965 6172 7320 6f66 2064 6174 6120  5 years of data 
+00000e60: 616e 6420 6f6e 6c79 2066 6561 7475 7265  and only feature
+00000e70: 7320 636f 6d70 616e 6965 7320 6c69 7374  s companies list
+00000e80: 6564 206f 6e20 5553 2065 7863 6861 6e67  ed on US exchang
+00000e90: 6573 2e0a 0a5f 5f5f 200a 0a3c 623e 3c64  es...___ ..<b><d
+00000ea0: 6976 2061 6c69 676e 3d22 6365 6e74 6572  iv align="center
+00000eb0: 223e 4f62 7461 696e 2061 6e20 4150 4920  ">Obtain an API 
+00000ec0: 4b65 7920 6672 6f6d 2046 696e 616e 6369  Key from Financi
+00000ed0: 616c 4d6f 6465 6c69 6e67 5072 6570 203c  alModelingPrep <
+00000ee0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000ef0: 7369 7465 2e66 696e 616e 6369 616c 6d6f  site.financialmo
+00000f00: 6465 6c69 6e67 7072 6570 2e63 6f6d 2f64  delingprep.com/d
+00000f10: 6576 656c 6f70 6572 2f64 6f63 732f 7072  eveloper/docs/pr
+00000f20: 6963 696e 672f 6a65 726f 656e 2f22 3e68  icing/jeroen/">h
+00000f30: 6572 653c 2f61 3e2e 3c2f 6469 763e 3c2f  ere</a>.</div></
+00000f40: 623e 0a5f 5f5f 0a0a 5468 726f 7567 6820  b>.___..Through 
+00000f50: 7468 6520 6c69 6e6b 2079 6f75 2061 7265  the link you are
+00000f60: 2061 626c 6520 746f 2073 7562 7363 7269   able to subscri
+00000f70: 6265 2066 6f72 2074 6865 2066 7265 6520  be for the free 
+00000f80: 706c 616e 2061 6e64 2061 6c73 6f20 7072  plan and also pr
+00000f90: 656d 6975 6d20 706c 616e 7320 6174 2061  emium plans at a
+00000fa0: 202a 3135 2520 6469 7363 6f75 6e74 2a2e   *15% discount*.
+00000fb0: 2054 6869 7320 6973 2061 6e20 6166 6669   This is an affi
+00000fc0: 6c69 6174 6520 6c69 6e6b 2061 6e64 2074  liate link and t
+00000fd0: 6875 7320 7375 7070 6f72 7473 2074 6865  hus supports the
+00000fe0: 2070 726f 6a65 6374 2061 7420 7468 6520   project at the 
+00000ff0: 7361 6d65 2074 696d 652e 2049 2068 6176  same time. I hav
+00001000: 6520 6368 6f73 656e 2046 696e 616e 6369  e chosen Financi
+00001010: 616c 4d6f 6465 6c69 6e67 5072 6570 2061  alModelingPrep a
+00001020: 7320 6120 736f 7572 6365 2061 7320 4920  s a source as I 
+00001030: 6669 6e64 2069 7420 746f 2062 6520 7468  find it to be th
+00001040: 6520 6d6f 7374 2074 7261 6e73 7061 7265  e most transpare
+00001050: 6e74 2c20 7265 6c69 6162 6c65 2061 6e64  nt, reliable and
+00001060: 2061 7420 616e 2061 6666 6f72 6461 626c   at an affordabl
+00001070: 6520 7072 6963 652e 2057 6865 6e20 796f  e price. When yo
+00001080: 7520 6e6f 7469 6365 2074 6861 7420 6461  u notice that da
+00001090: 7461 2069 7320 696e 6163 6375 7261 7465  ta is inaccurate
+000010a0: 206f 7220 6861 7665 2061 6e79 206f 7468   or have any oth
+000010b0: 6572 2069 7373 7565 2072 656c 6174 6564  er issue related
+000010c0: 2074 6f20 7468 6520 6461 7461 2c20 6e6f   to the data, no
+000010d0: 7465 2074 6861 7420 4920 7369 6d70 6c79  te that I simply
+000010e0: 2070 726f 7669 6465 2074 6865 206d 6561   provide the mea
+000010f0: 6e73 2074 6f20 6163 6365 7373 2074 6869  ns to access thi
+00001100: 7320 6461 7461 2061 6e64 2049 2061 6d20  s data and I am 
+00001110: 6e6f 7420 7265 7370 6f6e 7369 626c 6520  not responsible 
+00001120: 666f 7220 7468 6520 6163 6375 7261 6379  for the accuracy
+00001130: 206f 6620 7468 6520 6461 7461 2069 7473   of the data its
+00001140: 656c 662e 2046 6f72 2074 6869 732c 2075  elf. For this, u
+00001150: 7365 205b 7468 6569 7220 636f 6e74 6163  se [their contac
+00001160: 7420 666f 726d 5d28 6874 7470 733a 2f2f  t form](https://
+00001170: 7369 7465 2e66 696e 616e 6369 616c 6d6f  site.financialmo
+00001180: 6465 6c69 6e67 7072 6570 2e63 6f6d 2f63  delingprep.com/c
+00001190: 6f6e 7461 6374 2920 6f72 2070 726f 7669  ontact) or provi
+000011a0: 6465 2074 6865 2064 6174 6120 796f 7572  de the data your
+000011b0: 7365 6c66 2e20 0a0a 2320 4261 7369 6320  self. ..# Basic 
+000011c0: 5573 6167 650a 0a54 6869 7320 7365 6374  Usage..This sect
+000011d0: 696f 6e20 6578 706c 6169 6e73 2069 6e20  ion explains in 
+000011e0: 6465 7461 696c 2068 6f77 2074 6865 2046  detail how the F
+000011f0: 696e 616e 6365 2054 6f6f 6c6b 6974 2063  inance Toolkit c
+00001200: 616e 2075 7469 6c69 7469 7365 6420 6566  an utilitised ef
+00001210: 6665 6374 6976 656c 792e 2041 6c73 6f20  fectively. Also 
+00001220: 7365 6520 7468 6520 4a75 7079 7465 7220  see the Jupyter 
+00001230: 4e6f 7465 626f 6f6b 2069 6e20 7768 6963  Notebook in whic
+00001240: 6820 796f 7520 6361 6e20 7275 6e20 7468  h you can run th
+00001250: 6520 6578 616d 706c 6573 2061 6c73 6f20  e examples also 
+00001260: 6465 6d6f 6e73 7472 6174 6564 2068 6572  demonstrated her
+00001270: 652e 0a0a 5f5f 5f20 0a0a 3c62 3e3c 6469  e...___ ..<b><di
+00001280: 7620 616c 6967 6e3d 2263 656e 7465 7222  v align="center"
+00001290: 3e46 696e 6420 6120 7661 7269 6574 7920  >Find a variety 
+000012a0: 6f66 2048 6f77 2d54 6f20 4775 6964 6573  of How-To Guides
+000012b0: 2066 6f72 2074 6865 2046 696e 616e 6365   for the Finance
+000012c0: 546f 6f6c 6b69 7420 3c61 2068 7265 663d  Toolkit <a href=
+000012d0: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+000012e0: 636f 6d2f 4a65 7242 6f75 6d61 2f46 696e  com/JerBouma/Fin
+000012f0: 616e 6365 546f 6f6c 6b69 742f 7472 6565  anceToolkit/tree
+00001300: 2f6d 6169 6e2f 6578 616d 706c 6573 223e  /main/examples">
+00001310: 6865 7265 3c2f 613e 2e3c 2f64 6976 3e3c  here</a>.</div><
+00001320: 2f62 3e0a 5f5f 5f0a 0a57 6974 6869 6e20  /b>.___..Within 
+00001330: 7468 6973 2070 6163 6b61 6765 2074 6865  this package the
+00001340: 2066 6f6c 6c6f 7769 6e67 2074 6869 6e67   following thing
+00001350: 7320 6172 6520 696e 636c 7564 6564 3a0a  s are included:.
+00001360: 0a2d 2043 6f6d 7061 6e79 2070 726f 6669  .- Company profi
+00001370: 6c65 7320 2860 7072 6f66 696c 6560 292c  les (`profile`),
+00001380: 2069 6e63 6c75 6469 6e67 2063 6f75 6e74   including count
+00001390: 7279 2c20 7365 6374 6f72 2c20 4953 494e  ry, sector, ISIN
+000013a0: 2061 6e64 2067 656e 6572 616c 2063 6861   and general cha
+000013b0: 7261 6374 6572 6973 7469 6373 2028 6672  racteristics (fr
+000013c0: 6f6d 2046 696e 616e 6369 616c 4d6f 6465  om FinancialMode
+000013d0: 6c69 6e67 5072 6570 290a 2d20 436f 6d70  lingPrep).- Comp
+000013e0: 616e 7920 7175 6f74 6573 2028 6071 756f  any quotes (`quo
+000013f0: 7465 6029 2c20 696e 636c 7564 696e 6720  te`), including 
+00001400: 3532 2077 6565 6b20 6869 6768 7320 616e  52 week highs an
+00001410: 6420 6c6f 7773 2c20 766f 6c75 6d65 206d  d lows, volume m
+00001420: 6574 7269 6373 2061 6e64 2063 7572 7265  etrics and curre
+00001430: 6e74 2073 6861 7265 7320 6f75 7473 7461  nt shares outsta
+00001440: 6e64 696e 6720 2866 726f 6d20 4669 6e61  nding (from Fina
+00001450: 6e63 6961 6c4d 6f64 656c 696e 6750 7265  ncialModelingPre
+00001460: 7029 0a2d 204d 6172 6b65 7420 6361 7020  p).- Market cap 
+00001470: 616e 6420 656e 7465 7270 7269 7365 2076  and enterprise v
+00001480: 616c 7565 7320 2860 656e 7465 7270 7269  alues (`enterpri
+00001490: 7365 6029 2c20 696e 636c 7564 696e 6720  se`), including 
+000014a0: 6576 6572 7920 696e 7465 726d 6564 6961  every intermedia
+000014b0: 7465 2073 7465 7020 2866 726f 6d20 4669  te step (from Fi
+000014c0: 6e61 6e63 6961 6c4d 6f64 656c 696e 6750  nancialModelingP
+000014d0: 7265 7029 0a2d 2043 6f6d 7061 6e79 2072  rep).- Company r
+000014e0: 6174 696e 6773 2028 6072 6174 696e 6760  atings (`rating`
+000014f0: 292c 2062 6173 6564 206f 6e20 6b65 7920  ), based on key 
+00001500: 696e 6469 6361 746f 7273 206c 696b 6520  indicators like 
+00001510: 5045 2061 6e64 2044 4520 7261 7469 6f73  PE and DE ratios
+00001520: 2028 6672 6f6d 2046 696e 616e 6369 616c   (from Financial
+00001530: 4d6f 6465 6c69 6e67 5072 6570 290a 2d20  ModelingPrep).- 
+00001540: 4869 7374 6f72 6963 616c 206d 6172 6b65  Historical marke
+00001550: 7420 6461 7461 2028 6068 6973 746f 7269  t data (`histori
+00001560: 6361 6c5f 6461 7461 6029 2c20 7768 6963  cal_data`), whic
+00001570: 6820 6361 6e20 6265 2072 6574 7269 6576  h can be retriev
+00001580: 6564 206f 6e20 6120 6461 696c 792c 2077  ed on a daily, w
+00001590: 6565 6b6c 792c 206d 6f6e 7468 6c79 2061  eekly, monthly a
+000015a0: 6e64 2079 6561 726c 7920 6261 7369 7320  nd yearly basis 
+000015b0: 2866 726f 6d20 5961 686f 6f20 4669 6e61  (from Yahoo Fina
+000015c0: 6e63 6529 0a2d 2042 616c 616e 6365 2053  nce).- Balance S
+000015d0: 6865 6574 2053 7461 7465 6d65 6e74 7320  heet Statements 
+000015e0: 2860 6261 6c61 6e63 655f 7368 6565 745f  (`balance_sheet_
+000015f0: 7374 6174 656d 656e 7460 292c 2049 6e63  statement`), Inc
+00001600: 6f6d 6520 5374 6174 656d 656e 7473 2028  ome Statements (
+00001610: 6069 6e63 6f6d 655f 7374 6174 656d 656e  `income_statemen
+00001620: 7460 292c 2043 6173 6820 466c 6f77 2053  t`), Cash Flow S
+00001630: 7461 7465 6d65 6e74 7320 2860 6361 7368  tatements (`cash
+00001640: 5f66 6c6f 775f 7374 6174 656d 656e 7460  _flow_statement`
+00001650: 2920 616e 6420 5374 6174 6973 7469 6373  ) and Statistics
+00001660: 2053 7461 7465 6d65 6e74 2028 6073 7461   Statement (`sta
+00001670: 7469 7374 6963 735f 7374 6174 656d 656e  tistics_statemen
+00001680: 7460 292c 206f 6274 6169 6e61 626c 6520  t`), obtainable 
+00001690: 6672 6f6d 2046 696e 616e 6369 616c 4d6f  from FinancialMo
+000016a0: 6465 6c69 6e67 5072 6570 206f 7220 7468  delingPrep or th
+000016b0: 6520 736f 7572 6365 206f 6620 796f 7572  e source of your
+000016c0: 2063 686f 6f73 696e 6720 7468 726f 7567   choosing throug
+000016d0: 6820 6375 7374 6f6d 2069 6e70 7574 2e20  h custom input. 
+000016e0: 5468 6573 6520 6675 6e63 7469 6f6e 7320  These functions 
+000016f0: 6172 6520 6163 636f 6d70 616e 6965 6420  are accompanied 
+00001700: 7769 7468 2061 206e 6f72 6d61 6c69 7a61  with a normaliza
+00001710: 7469 6f6e 2066 756e 6374 696f 6e20 736f  tion function so
+00001720: 2074 6861 7420 666f 7220 616e 7920 736f   that for any so
+00001730: 7572 6365 2c20 7468 6520 7361 6d65 2072  urce, the same r
+00001740: 6174 696f 2061 6e61 6c79 7369 7320 6361  atio analysis ca
+00001750: 6e20 6265 2070 6572 666f 726d 6564 2e20  n be performed. 
+00001760: 506c 6561 7365 2073 6565 2074 6869 7320  Please see this 
+00001770: 4a75 7079 7465 7220 4e6f 7465 626f 6f6b  Jupyter Notebook
+00001780: 2074 6861 7420 6578 706c 6169 6e73 2068   that explains h
+00001790: 6f77 2074 6f20 7573 6520 6120 6375 7374  ow to use a cust
+000017a0: 6f6d 2073 6f75 7263 652e 0a2d 2045 6666  om source..- Eff
+000017b0: 6963 6965 6e63 7920 7261 7469 6f73 2028  iciency ratios (
+000017c0: 6065 6666 6963 6965 6e63 795f 7261 7469  `efficiency_rati
+000017d0: 6f73 6029 2c20 6c69 7175 6964 6974 7920  os`), liquidity 
+000017e0: 7261 7469 6f73 2028 606c 6971 7569 6469  ratios (`liquidi
+000017f0: 7479 5f72 6174 696f 7360 292c 2070 726f  ty_ratios`), pro
+00001800: 6669 7461 6269 6c69 7479 2072 6174 696f  fitability ratio
+00001810: 7320 2860 7072 6f66 6974 6162 696c 6974  s (`profitabilit
+00001820: 795f 7261 7469 6f73 6029 2c20 736f 6c76  y_ratios`), solv
+00001830: 656e 6379 2072 6174 696f 7320 2860 736f  ency ratios (`so
+00001840: 6c76 656e 6379 5f72 6174 696f 7360 2920  lvency_ratios`) 
+00001850: 616e 6420 7661 6c75 6174 696f 6e20 7261  and valuation ra
+00001860: 7469 6f73 2028 6076 616c 7561 7469 6f6e  tios (`valuation
+00001870: 5f72 6174 696f 7360 2920 6675 6e63 7469  _ratios`) functi
+00001880: 6f6e 616c 6974 7920 7468 6174 2061 7574  onality that aut
+00001890: 6f6d 6174 6963 616c 6c79 2063 616c 6375  omatically calcu
+000018a0: 6c61 7465 7320 7468 6520 6d6f 7374 2069  lates the most i
+000018b0: 6d70 6f72 7461 6e74 2072 6174 696f 7320  mportant ratios 
+000018c0: 6261 7365 6420 6f6e 2074 6865 2069 6e70  based on the inp
+000018d0: 7574 7465 6420 6261 6c61 6e63 6520 7368  utted balance sh
+000018e0: 6565 742c 2069 6e63 6f6d 6520 616e 6420  eet, income and 
+000018f0: 6361 7368 2066 6c6f 7720 7374 6174 656d  cash flow statem
+00001900: 656e 7473 2e20 4e65 7874 2074 6f20 7468  ents. Next to th
+00001910: 6174 2c20 6974 2069 7320 616c 736f 2070  at, it is also p
+00001920: 6f73 7369 626c 6520 746f 2069 6e70 7574  ossible to input
+00001930: 2079 6f75 7220 6f77 6e20 6375 7374 6f6d   your own custom
+00001940: 2072 6174 696f 7320 2860 6375 7374 6f6d   ratios (`custom
+00001950: 5f72 6174 696f 7360 292e 0a2d 204d 6f64  _ratios`)..- Mod
+00001960: 656c 7320 2860 6d6f 6465 6c73 6029 206c  els (`models`) l
+00001970: 696b 6520 4455 504f 4e54 2061 6e61 6c79  ike DUPONT analy
+00001980: 7369 7320 7468 6174 2063 616e 2062 6520  sis that can be 
+00001990: 7573 6564 2074 6f20 7065 7266 6f72 6d20  used to perform 
+000019a0: 696e 2d64 6570 7468 2066 696e 616e 6369  in-depth financi
+000019b0: 616c 2061 6e61 6c79 7369 7320 7468 726f  al analysis thro
+000019c0: 7567 6820 6120 7369 6e67 6c65 2066 756e  ugh a single fun
+000019d0: 6374 696f 6e2e 0a0a 5468 6520 6465 7065  ction...The depe
+000019e0: 6e64 656e 6369 6573 206f 6620 7468 6520  ndencies of the 
+000019f0: 7061 636b 6167 6520 6172 6520 6f6e 2070  package are on p
+00001a00: 7572 706f 7365 202a 7665 7279 2073 6c69  urpose *very sli
+00001a10: 6d2a 2073 6f20 7468 6174 2069 7420 7769  m* so that it wi
+00001a20: 6c6c 2077 6f72 6b20 7765 6c6c 2077 6974  ll work well wit
+00001a30: 6820 616e 7920 636f 6d62 696e 6174 696f  h any combinatio
+00001a40: 6e20 6f66 2070 6163 6b61 6765 7320 616e  n of packages an
+00001a50: 6420 6e6f 7420 7265 7375 6c74 2069 6e20  d not result in 
+00001a60: 636f 6e66 6c69 6374 732e 2049 2776 6520  conflicts. I've 
+00001a70: 616c 736f 2062 6565 6e20 6361 7265 6675  also been carefu
+00001a80: 6c20 7769 7468 206d 7920 7365 6c65 6374  l with my select
+00001a90: 696f 6e20 696e 2077 6869 6368 2049 206c  ion in which I l
+00001aa0: 6561 7665 206f 7574 2066 756e 6374 696f  eave out functio
+00001ab0: 6e61 6c69 7479 206c 696b 6520 7465 6368  nality like tech
+00001ac0: 6e69 6361 6c20 616e 616c 7973 6973 2069  nical analysis i
+00001ad0: 6e20 7768 6963 6820 5b74 612d 6c69 625d  n which [ta-lib]
+00001ae0: 2868 7474 7073 3a2f 2f74 612d 6c69 622e  (https://ta-lib.
+00001af0: 6f72 672f 2920 646f 6573 2061 6e20 6578  org/) does an ex
+00001b00: 6365 6c6c 656e 7420 6a6f 6220 6173 2077  cellent job as w
+00001b10: 656c 6c20 6173 2070 6f72 7466 6f6c 696f  ell as portfolio
+00001b20: 2061 7474 7269 6275 7469 6f6e 2061 6e64   attribution and
+00001b30: 206f 7074 696d 6973 6174 696f 6e20 696e   optimisation in
+00001b40: 2077 6869 6368 205b 5269 736b 666f 6c69   which [Riskfoli
+00001b50: 6f2d 6c69 625d 2868 7474 7073 3a2f 2f72  o-lib](https://r
+00001b60: 6973 6b66 6f6c 696f 2d6c 6962 2e72 6561  iskfolio-lib.rea
+00001b70: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
+00001b80: 6174 6573 742f 696e 6465 782e 6874 6d6c  atest/index.html
+00001b90: 2920 7368 696e 6573 2e0a 0a23 2320 5573  ) shines...## Us
+00001ba0: 696e 6720 7468 6520 4669 6e61 6e63 6520  ing the Finance 
+00001bb0: 546f 6f6c 6b69 740a 0a41 2062 6173 6963  Toolkit..A basic
+00001bc0: 2065 7861 6d70 6c65 206f 6620 686f 7720   example of how 
+00001bd0: 746f 2069 6e69 7469 616c 6973 6520 7468  to initialise th
+00001be0: 6520 4669 6e61 6e63 6520 546f 6f6c 6b69  e Finance Toolki
+00001bf0: 7420 6973 2073 686f 776e 2062 656c 6f77  t is shown below
+00001c00: 2c20 616c 736f 2073 6565 205b 7468 6973  , also see [this
+00001c10: 206e 6f74 6562 6f6f 6b5d 2868 7474 7073   notebook](https
+00001c20: 3a2f 2f67 6974 6875 622e 636f 6d2f 4a65  ://github.com/Je
+00001c30: 7242 6f75 6d61 2f46 696e 616e 6365 546f  rBouma/FinanceTo
+00001c40: 6f6c 6b69 742f 626c 6f62 2f6d 6169 6e2f  olkit/blob/main/
+00001c50: 6578 616d 706c 6573 2f46 696e 616e 6365  examples/Finance
+00001c60: 2532 3054 6f6f 6c6b 6974 2532 302d 2532  %20Toolkit%20-%2
+00001c70: 3031 2e25 3230 4765 7474 696e 6725 3230  01.%20Getting%20
+00001c80: 5374 6172 7465 642e 6970 796e 6229 2066  Started.ipynb) f
+00001c90: 6f72 2061 2064 6574 6169 6c65 6420 4765  or a detailed Ge
+00001ca0: 7474 696e 6720 5374 6172 7465 6420 6775  tting Started gu
+00001cb0: 6964 6520 6173 2077 656c 6c20 6173 205b  ide as well as [
+00001cc0: 7468 6973 206e 6f74 6562 6f6f 6b5d 2868  this notebook](h
+00001cd0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001ce0: 6d2f 4a65 7242 6f75 6d61 2f46 696e 616e  m/JerBouma/Finan
+00001cf0: 6365 546f 6f6c 6b69 742f 626c 6f62 2f6d  ceToolkit/blob/m
+00001d00: 6169 6e2f 6578 616d 706c 6573 2f46 696e  ain/examples/Fin
+00001d10: 616e 6365 2532 3054 6f6f 6c6b 6974 2532  ance%20Toolkit%2
+00001d20: 302d 2532 3032 2e25 3230 436f 6d62 696e  0-%202.%20Combin
+00001d30: 696e 6725 3230 7468 6525 3230 4669 6e61  ing%20the%20Fina
+00001d40: 6e63 6525 3230 546f 6f6c 6b69 7425 3230  nce%20Toolkit%20
+00001d50: 7769 7468 2532 3074 6865 2532 3046 696e  with%20the%20Fin
+00001d60: 616e 6365 2532 3044 6174 6162 6173 652e  ance%20Database.
+00001d70: 6970 796e 6229 2074 6861 7420 696e 636c  ipynb) that incl
+00001d80: 7564 6573 2074 6865 205b 4669 6e61 6e63  udes the [Financ
+00001d90: 6520 4461 7461 6261 7365 20f0 9f8c 8e5d  e Database ....]
+00001da0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00001db0: 636f 6d2f 4a65 7242 6f75 6d61 2f46 696e  com/JerBouma/Fin
+00001dc0: 616e 6365 4461 7461 6261 7365 2920 616e  anceDatabase) an
+00001dd0: 6420 6120 7072 6f70 6572 2066 696e 616e  d a proper finan
+00001de0: 6369 616c 2061 6e61 6c79 7369 732e 0a0a  cial analysis...
+00001df0: 6060 6060 7079 7468 6f6e 0a66 726f 6d20  ````python.from 
+00001e00: 6669 6e61 6e63 6574 6f6f 6c6b 6974 2069  financetoolkit i
+00001e10: 6d70 6f72 7420 546f 6f6c 6b69 740a 0a63  mport Toolkit..c
+00001e20: 6f6d 7061 6e69 6573 203d 2054 6f6f 6c6b  ompanies = Toolk
+00001e30: 6974 285b 2741 4150 4c27 2c20 274d 5346  it(['AAPL', 'MSF
+00001e40: 5427 5d2c 2061 7069 5f6b 6579 3d22 464d  T'], api_key="FM
+00001e50: 505f 4b45 5922 2c20 7374 6172 745f 6461  P_KEY", start_da
+00001e60: 7465 3d27 3230 3137 2d31 322d 3331 2729  te='2017-12-31')
+00001e70: 0a0a 2320 616e 2045 6e74 6572 7072 6973  ..# an Enterpris
+00001e80: 6520 6578 616d 706c 650a 656e 7465 7270  e example.enterp
+00001e90: 7269 7365 203d 2063 6f6d 7061 6e69 6573  rise = companies
+00001ea0: 2e67 6574 5f65 6e74 6572 7072 6973 6528  .get_enterprise(
+00001eb0: 290a 0a23 2061 2048 6973 746f 7269 6361  )..# a Historica
+00001ec0: 6c20 6578 616d 706c 650a 6869 7374 6f72  l example.histor
+00001ed0: 6963 616c 5f64 6174 6120 3d20 636f 6d70  ical_data = comp
+00001ee0: 616e 6965 732e 6765 745f 6869 7374 6f72  anies.get_histor
+00001ef0: 6963 616c 5f64 6174 6128 290a 0a23 2061  ical_data()..# a
+00001f00: 2046 696e 616e 6369 616c 2053 7461 7465   Financial State
+00001f10: 6d65 6e74 2065 7861 6d70 6c65 0a62 616c  ment example.bal
+00001f20: 616e 6365 5f73 6865 6574 5f73 7461 7465  ance_sheet_state
+00001f30: 6d65 6e74 203d 2063 6f6d 7061 6e69 6573  ment = companies
+00001f40: 2e67 6574 5f62 616c 616e 6365 5f73 6865  .get_balance_she
+00001f50: 6574 5f73 7461 7465 6d65 6e74 2829 0a0a  et_statement()..
+00001f60: 2320 6120 5261 7469 6f73 2065 7861 6d70  # a Ratios examp
+00001f70: 6c65 0a70 726f 6669 7461 6269 6c69 7479  le.profitability
+00001f80: 5f72 6174 696f 7320 3d20 636f 6d70 616e  _ratios = compan
+00001f90: 6965 732e 7261 7469 6f73 2e63 6f6c 6c65  ies.ratios.colle
+00001fa0: 6374 5f70 726f 6669 7461 6269 6c69 7479  ct_profitability
+00001fb0: 5f72 6174 696f 7328 290a 0a23 2053 686f  _ratios()..# Sho
+00001fc0: 7720 7468 6520 7072 6f66 6974 6162 696c  w the profitabil
+00001fd0: 6974 7920 7261 7469 6f73 2066 6f72 2041  ity ratios for A
+00001fe0: 7070 6c65 0a70 726f 6669 7461 6269 6c69  pple.profitabili
+00001ff0: 7479 5f72 6174 696f 732e 6c6f 635b 2741  ty_ratios.loc['A
+00002000: 4150 4c27 5d0a 6060 6060 0a0a 5468 6973  APL'].````..This
+00002010: 2072 6574 7572 6e73 2074 6865 2066 6f6c   returns the fol
+00002020: 6c6f 7769 6e67 206f 7574 7075 7420 666f  lowing output fo
+00002030: 7220 6070 726f 6669 7461 6269 6c69 7479  r `profitability
+00002040: 5f72 6174 696f 732e 6c6f 635b 2741 4150  _ratios.loc['AAP
+00002050: 4c5d 602e 204f 6d69 7474 696e 6720 602e  L]`. Omitting `.
+00002060: 6c6f 635b 2741 4150 4c27 5d60 2077 696c  loc['AAPL']` wil
+00002070: 6c20 7265 7475 726e 2074 6865 2072 6573  l return the res
+00002080: 756c 7420 666f 7220 626f 7468 2041 4150  ult for both AAP
+00002090: 4c20 616e 6420 4d53 4654 2e0a 0a0a 7c20  L and MSFT....| 
+000020a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000020b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000020c0: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
+000020d0: 2020 3230 3138 207c 2020 2020 2032 3031    2018 |     201
+000020e0: 3920 7c20 2020 2020 3230 3230 207c 2020  9 |     2020 |  
+000020f0: 2020 2032 3032 3120 7c20 2020 2020 3230     2021 |     20
+00002100: 3232 207c 0a7c 3a2d 2d2d 2d2d 2d2d 2d2d  22 |.|:---------
+00002110: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00002120: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002130: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002140: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d  ------------|---
-00002150: 2d2d 2d2d 2d2d 3a7c 2d2d 2d2d 2d2d 2d2d  ------:|--------
-00002160: 2d3a 7c2d 2d2d 2d2d 2d2d 2d2d 3a7c 2d2d  -:|---------:|--
-00002170: 2d2d 2d2d 2d2d 2d3a 7c2d 2d2d 2d2d 2d2d  -------:|-------
-00002180: 2d2d 3a7c 0a7c 2047 726f 7373 204d 6172  --:|.| Gross Mar
-00002190: 6769 6e20 2020 2020 2020 2020 2020 2020  gin             
-000021a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000021b0: 2020 207c 2030 2e33 3833 3433 3720 7c20     | 0.383437 | 
-000021c0: 302e 3337 3831 3738 207c 2030 2e33 3832  0.378178 | 0.382
-000021d0: 3333 3220 7c20 302e 3431 3737 3934 207c  332 | 0.417794 |
-000021e0: 2030 2e34 3333 3039 3620 7c0a 7c20 4f70   0.433096 |.| Op
-000021f0: 6572 6174 696e 6720 4d61 7267 696e 2020  erating Margin  
-00002200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002210: 2020 2020 2020 2020 2020 7c20 302e 3236            | 0.26
-00002220: 3639 3420 207c 2030 2e32 3435 3732 2020  694  | 0.24572  
-00002230: 7c20 302e 3234 3134 3733 207c 2030 2e32  | 0.241473 | 0.2
-00002240: 3937 3832 3420 7c20 302e 3330 3238 3837  97824 | 0.302887
-00002250: 207c 0a7c 204e 6574 2050 726f 6669 7420   |.| Net Profit 
-00002260: 4d61 7267 696e 2020 2020 2020 2020 2020  Margin          
-00002270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002280: 207c 2030 2e32 3234 3134 3220 7c20 302e   | 0.224142 | 0.
-00002290: 3231 3233 3831 207c 2030 2e32 3039 3133  212381 | 0.20913
-000022a0: 3620 7c20 302e 3235 3838 3138 207c 2030  6 | 0.258818 | 0
-000022b0: 2e32 3533 3039 3620 7c0a 7c20 496e 7465  .253096 |.| Inte
-000022c0: 7265 7374 2042 7572 6465 6e20 5261 7469  rest Burden Rati
-000022d0: 6f20 2020 2020 2020 2020 2020 2020 2020  o               
-000022e0: 2020 2020 2020 2020 7c20 312e 3032 3832          | 1.0282
-000022f0: 3820 207c 2031 2e30 3238 3237 2020 7c20  8  | 1.02827  | 
-00002300: 312e 3031 3231 3120 207c 2031 2e30 3032  1.01211  | 1.002
-00002310: 3337 2020 7c20 302e 3939 3732 3034 207c  37  | 0.997204 |
-00002320: 0a7c 2049 6e63 6f6d 6520 4265 666f 7265  .| Income Before
-00002330: 2054 6178 2050 726f 6669 7420 4d61 7267   Tax Profit Marg
-00002340: 696e 2020 2020 2020 2020 2020 2020 207c  in             |
-00002350: 2030 2e32 3734 3438 3920 7c20 302e 3235   0.274489 | 0.25
-00002360: 3236 3636 207c 2030 2e32 3434 3339 3820  2666 | 0.244398 
-00002370: 7c20 302e 3239 3835 3239 207c 2030 2e33  | 0.298529 | 0.3
-00002380: 3032 3034 2020 7c0a 7c20 4566 6665 6374  0204  |.| Effect
-00002390: 6976 6520 5461 7820 5261 7465 2020 2020  ive Tax Rate    
-000023a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023b0: 2020 2020 2020 7c20 302e 3138 3334 3232        | 0.183422
-000023c0: 207c 2030 2e31 3539 3433 3820 7c20 302e   | 0.159438 | 0.
-000023d0: 3134 3432 3832 207c 2030 2e31 3333 3032  144282 | 0.13302
-000023e0: 3320 7c20 302e 3136 3230 3435 207c 0a7c  3 | 0.162045 |.|
-000023f0: 2052 6574 7572 6e20 6f6e 2041 7373 6574   Return on Asset
-00002400: 7320 2852 4f41 2920 2020 2020 2020 2020  s (ROA)         
-00002410: 2020 2020 2020 2020 2020 2020 207c 2030               | 0
-00002420: 2e31 3632 3737 3520 7c20 302e 3136 3332  .162775 | 0.1632
-00002430: 3320 207c 2030 2e31 3737 3235 3620 7c20  3  | 0.177256 | 
-00002440: 302e 3236 3937 3432 207c 2030 2e32 3832  0.269742 | 0.282
-00002450: 3932 3420 7c0a 7c20 5265 7475 726e 206f  924 |.| Return o
-00002460: 6e20 4571 7569 7479 2028 524f 4529 2020  n Equity (ROE)  
-00002470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002480: 2020 2020 7c20 302e 3535 3536 3031 207c      | 0.555601 |
-00002490: 2030 2e36 3130 3634 3520 7c20 302e 3837   0.610645 | 0.87
-000024a0: 3836 3634 207c 2031 2e35 3030 3731 2020  8664 | 1.50071  
-000024b0: 7c20 312e 3936 3935 3920 207c 0a7c 2052  | 1.96959  |.| R
-000024c0: 6574 7572 6e20 6f6e 2049 6e76 6573 7465  eturn on Investe
-000024d0: 6420 4361 7069 7461 6c20 2852 4f49 4329  d Capital (ROIC)
-000024e0: 2020 2020 2020 2020 2020 207c 2030 2e32             | 0.2
-000024f0: 3639 3835 3820 7c20 302e 3239 3337 3231  69858 | 0.293721
-00002500: 207c 2030 2e33 3434 3132 3620 7c20 302e   | 0.344126 | 0.
-00002510: 3530 3338 3532 207c 2030 2e35 3632 3634  503852 | 0.56264
-00002520: 3520 7c0a 7c20 5265 7475 726e 206f 6e20  5 |.| Return on 
-00002530: 4361 7069 7461 6c20 456d 706c 6f79 6564  Capital Employed
-00002540: 2028 524f 4345 2920 2020 2020 2020 2020   (ROCE)         
-00002550: 2020 7c20 302e 3330 3539 3638 207c 2030    | 0.305968 | 0
-00002560: 2e32 3937 3733 3920 7c20 302e 3332 3032  .297739 | 0.3202
-00002570: 3037 207c 2030 2e34 3935 3937 3220 7c20  07 | 0.495972 | 
-00002580: 302e 3631 3339 3337 207c 0a7c 2052 6574  0.613937 |.| Ret
-00002590: 7572 6e20 6f6e 2054 616e 6769 626c 6520  urn on Tangible 
-000025a0: 4173 7365 7473 2020 2020 2020 2020 2020  Assets          
-000025b0: 2020 2020 2020 2020 207c 2030 2e35 3535           | 0.555
-000025c0: 3630 3120 7c20 302e 3631 3036 3435 207c  601 | 0.610645 |
-000025d0: 2030 2e38 3738 3636 3420 7c20 312e 3530   0.878664 | 1.50
-000025e0: 3037 3120 207c 2031 2e39 3639 3539 2020  071  | 1.96959  
-000025f0: 7c0a 7c20 496e 636f 6d65 2051 7561 6c69  |.| Income Quali
-00002600: 7479 2052 6174 696f 2020 2020 2020 2020  ty Ratio        
-00002610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002620: 7c20 312e 3330 3037 3320 207c 2031 2e32  | 1.30073  | 1.2
-00002630: 3535 3831 2020 7c20 312e 3430 3532 2020  5581  | 1.4052  
-00002640: 207c 2031 2e30 3938 3834 2020 7c20 312e   | 1.09884  | 1.
-00002650: 3232 3339 3220 207c 0a7c 204e 6574 2049  22392  |.| Net I
-00002660: 6e63 6f6d 6520 7065 7220 4542 5420 2020  ncome per EBT   
-00002670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002680: 2020 2020 2020 207c 2030 2e38 3136 3537         | 0.81657
-00002690: 3820 7c20 302e 3834 3035 3632 207c 2030  8 | 0.840562 | 0
-000026a0: 2e38 3535 3731 3820 7c20 302e 3836 3639  .855718 | 0.8669
-000026b0: 3737 207c 2030 2e38 3337 3935 3520 7c0a  77 | 0.837955 |.
-000026c0: 7c20 4672 6565 2043 6173 6820 466c 6f77  | Free Cash Flow
-000026d0: 2074 6f20 4f70 6572 6174 696e 6720 4361   to Operating Ca
-000026e0: 7368 2046 6c6f 7720 5261 7469 6f20 7c20  sh Flow Ratio | 
-000026f0: 302e 3832 3830 3733 207c 2030 2e38 3438  0.828073 | 0.848
-00002700: 3735 3620 7c20 302e 3930 3934 3031 207c  756 | 0.909401 |
-00002710: 2030 2e38 3933 3435 3220 7c20 302e 3931   0.893452 | 0.91
-00002720: 3233 3338 207c 0a7c 2045 4254 2074 6f20  2338 |.| EBT to 
-00002730: 4542 4954 2052 6174 696f 2020 2020 2020  EBIT Ratio      
-00002740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002750: 2020 2020 207c 2030 2e39 3537 3434 3820       | 0.957448 
-00002760: 7c20 302e 3934 3834 3038 207c 2030 2e39  | 0.948408 | 0.9
-00002770: 3538 3933 3620 7c20 302e 3937 3633 3533  58936 | 0.976353
-00002780: 207c 2030 2e39 3735 3938 3220 7c0a 7c20   | 0.975982 |.| 
-00002790: 4542 4954 2074 6f20 5265 7665 6e75 6520  EBIT to Revenue 
-000027a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027b0: 2020 2020 2020 2020 2020 2020 7c20 302e              | 0.
-000027c0: 3238 3636 3838 207c 2030 2e32 3636 3431  286688 | 0.26641
-000027d0: 2020 7c20 302e 3235 3438 3634 207c 2030    | 0.254864 | 0
-000027e0: 2e33 3035 3735 3920 7c20 302e 3330 3934  .305759 | 0.3094
-000027f0: 3733 207c 0a0a 2323 2057 6f72 6b69 6e67  73 |..## Working
-00002800: 2077 6974 6820 6f74 6865 7220 4461 7461   with other Data
-00002810: 7365 7473 0a0a 5468 6520 4669 6e61 6e63  sets..The Financ
-00002820: 6520 546f 6f6c 6b69 7420 7368 696e 6573  e Toolkit shines
-00002830: 2069 6e20 6974 7320 6162 696c 6974 7920   in its ability 
-00002840: 746f 206c 6576 6572 6167 6520 6375 7374  to leverage cust
-00002850: 6f6d 2064 6174 6173 6574 7320 6672 6f6d  om datasets from
-00002860: 2061 6e79 2064 6174 6120 7072 6f76 6964   any data provid
-00002870: 6572 2061 7320 7765 6c6c 2e20 5468 6973  er as well. This
-00002880: 206d 616b 6573 2069 7420 706f 7373 6962   makes it possib
-00002890: 6c65 2074 6f20 776f 726b 2077 6974 6820  le to work with 
-000028a0: 796f 7572 2070 7265 6665 7272 6564 2064  your preferred d
-000028b0: 6174 6120 616e 6420 6e6f 7420 6265 206c  ata and not be l
-000028c0: 696d 6974 6564 2074 6f20 7468 6520 6461  imited to the da
-000028d0: 7461 2073 6f75 7263 6520 7468 6520 4669  ta source the Fi
-000028e0: 6e61 6e63 6520 546f 6f6c 6b69 7420 6375  nance Toolkit cu
-000028f0: 7272 656e 746c 7920 7072 6f76 6964 6573  rrently provides
-00002900: 2e20 4120 6465 7461 696c 6564 2065 7861  . A detailed exa
-00002910: 6d70 6c65 2063 616e 2062 6520 666f 756e  mple can be foun
-00002920: 6420 5b68 6572 655d 2868 7474 7073 3a2f  d [here](https:/
-00002930: 2f67 6974 6875 622e 636f 6d2f 4a65 7242  /github.com/JerB
-00002940: 6f75 6d61 2f46 696e 616e 6365 546f 6f6c  ouma/FinanceTool
-00002950: 6b69 742f 626c 6f62 2f6d 6169 6e2f 6578  kit/blob/main/ex
-00002960: 616d 706c 6573 2f46 696e 616e 6365 2532  amples/Finance%2
-00002970: 3054 6f6f 6c6b 6974 2532 302d 2532 3033  0Toolkit%20-%203
-00002980: 2e25 3230 5573 696e 6725 3230 4578 7465  .%20Using%20Exte
-00002990: 726e 616c 2532 3044 6174 6173 6574 7325  rnal%20Datasets%
-000029a0: 3230 284f 7065 6e42 4229 2e69 7079 6e62  20(OpenBB).ipynb
-000029b0: 2920 6275 7420 746f 2067 6574 2073 7461  ) but to get sta
-000029c0: 7274 6564 2073 6565 2074 6865 2063 6f64  rted see the cod
-000029d0: 6520 6265 6c6f 772e 0a0a 6060 6070 7974  e below...```pyt
-000029e0: 686f 6e0a 6672 6f6d 2066 696e 616e 6365  hon.from finance
-000029f0: 746f 6f6c 6b69 7420 696d 706f 7274 2054  toolkit import T
-00002a00: 6f6f 6c6b 6974 0a0a 2320 496e 6974 6961  oolkit..# Initia
-00002a10: 6c69 7a65 2074 6865 2046 696e 616e 6365  lize the Finance
-00002a20: 2054 6f6f 6c6b 6974 0a63 6f6d 7061 6e69   Toolkit.compani
-00002a30: 6573 203d 2054 6f6f 6c6b 6974 285b 2741  es = Toolkit(['A
-00002a40: 4150 4c27 2c20 274d 5346 5427 5d29 0a0a  APL', 'MSFT'])..
-00002a50: 2320 436f 7079 2074 6865 206e 6f72 6d61  # Copy the norma
-00002a60: 6c69 7a61 7469 6f6e 2066 696c 6573 0a63  lization files.c
-00002a70: 6f6d 7061 6e69 6573 2e67 6574 5f6e 6f72  ompanies.get_nor
-00002a80: 6d61 6c69 7a61 7469 6f6e 5f66 696c 6573  malization_files
-00002a90: 2829 0a60 6060 0a54 6869 7320 636f 7069  ().```.This copi
-00002aa0: 6573 206f 7665 7220 7468 7265 6520 6669  es over three fi
-00002ab0: 6c65 732c 2060 6261 6c61 6e63 652e 6373  les, `balance.cs
-00002ac0: 7660 2c20 6069 6e63 6f6d 652e 6373 7660  v`, `income.csv`
-00002ad0: 2061 6e64 2060 6361 7368 2e63 7376 6020   and `cash.csv` 
-00002ae0: 7768 6963 6820 7769 6c6c 2063 6f6e 7461  which will conta
-00002af0: 696e 2061 2073 7472 7563 7475 7265 206c  in a structure l
-00002b00: 696b 6520 7468 6520 666f 6c6c 6f77 696e  ike the followin
-00002b10: 673a 0a0a 215b 4e6f 726d 616c 697a 6174  g:..![Normalizat
-00002b20: 696f 6e20 466f 726d 6174 5d28 6874 7470  ion Format](http
-00002b30: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4a  s://github.com/J
-00002b40: 6572 426f 756d 612f 4669 6e61 6e63 6554  erBouma/FinanceT
-00002b50: 6f6f 6c6b 6974 2f61 7373 6574 732f 3436  oolkit/assets/46
-00002b60: 3335 3533 3634 2f65 6134 6562 6638 372d  355364/ea4ebf87-
-00002b70: 3161 3237 2d34 6334 302d 6131 6662 2d34  1a27-4c40-a1fb-4
-00002b80: 3064 3065 6230 3633 3462 6329 0a0a 4279  0d0eb0634bc)..By
-00002b90: 2072 6570 6c61 6369 6e67 2074 6865 2066   replacing the f
-00002ba0: 6972 7374 2063 6f6c 756d 6e20 7769 7468  irst column with
-00002bb0: 2074 6865 206e 616d 6573 2066 726f 6d20   the names from 
-00002bc0: 796f 7572 2064 6174 6173 6574 2028 652e  your dataset (e.
-00002bd0: 672e 2072 6570 6c61 6365 2060 6361 7368  g. replace `cash
-00002be0: 416e 6443 6173 6845 7175 6976 616c 656e  AndCashEquivalen
-00002bf0: 7473 6020 7769 7468 2060 4361 7368 6020  ts` with `Cash` 
-00002c00: 6966 2074 6869 7320 6973 2068 6f77 2069  if this is how i
-00002c10: 7420 6973 2063 616c 6c65 6420 696e 2079  t is called in y
-00002c20: 6f75 7220 6461 7461 7365 7429 2c20 6974  our dataset), it
-00002c30: 2077 696c 6c20 6175 746f 6d61 7469 6361   will automatica
-00002c40: 6c6c 7920 6e6f 726d 616c 697a 6520 7468  lly normalize th
-00002c50: 6520 6461 7461 7365 7420 7768 656e 2079  e dataset when y
-00002c60: 6f75 2069 6e69 7469 616c 697a 6520 7468  ou initialize th
-00002c70: 6520 4669 6e61 6e63 6520 546f 6f6c 6b69  e Finance Toolki
-00002c80: 742e 204e 6f74 6520 7468 6174 2074 6865  t. Note that the
-00002c90: 2044 6174 6146 7261 6d65 206e 6565 6473   DataFrame needs
-00002ca0: 2074 6f20 6265 2061 206d 756c 7469 2d69   to be a multi-i
-00002cb0: 6e64 6578 2069 6e20 6361 7365 2079 6f75  ndex in case you
-00002cc0: 2075 7365 206d 756c 7469 706c 6520 7469   use multiple ti
-00002cd0: 636b 6572 7320 7374 7275 6374 7572 6564  ckers structured
-00002ce0: 2061 7320 6054 6963 6b65 7220 7820 4669   as `Ticker x Fi
-00002cf0: 6e61 6e63 6961 6c20 5374 6174 656d 656e  nancial Statemen
-00002d00: 7420 4974 656d 2078 2050 6572 696f 6473  t Item x Periods
-00002d10: 602e 0a0a 4173 2061 6e20 6578 616d 706c  `...As an exampl
-00002d20: 653a 0a0a 215b 4461 7461 7365 7420 4578  e:..![Dataset Ex
-00002d30: 616d 706c 655d 2868 7474 7073 3a2f 2f67  ample](https://g
-00002d40: 6974 6875 622e 636f 6d2f 4a65 7242 6f75  ithub.com/JerBou
-00002d50: 6d61 2f46 696e 616e 6365 546f 6f6c 6b69  ma/FinanceToolki
-00002d60: 742f 6173 7365 7473 2f34 3633 3535 3336  t/assets/4635536
-00002d70: 342f 6665 3065 3364 6230 2d33 6538 382d  4/fe0e3db0-3e88-
-00002d80: 3431 6432 2d61 3335 352d 3566 3638 3131  41d2-a355-5f6811
-00002d90: 3066 6463 6633 290a 0a49 6620 796f 7520  0fdcf3)..If you 
-00002da0: 6861 7665 2069 6e64 6976 6964 7561 6c20  have individual 
-00002db0: 4461 7461 4672 616d 6573 2066 6f72 2065  DataFrames for e
-00002dc0: 6163 6820 636f 6d70 616e 792c 2079 6f75  ach company, you
-00002dd0: 2063 616e 2064 6f20 7468 6520 666f 6c6c   can do the foll
-00002de0: 6f77 696e 6720 7768 6963 6820 7769 6c6c  owing which will
-00002df0: 2072 6574 7572 6e20 7468 6520 4461 7461   return the Data
-00002e00: 4672 616d 6520 7374 7275 6374 7572 6520  Frame structure 
-00002e10: 7468 6174 2069 7320 7265 7175 6972 6564  that is required
-00002e20: 3a0a 0a60 6060 7079 7468 6f6e 0a66 726f  :..```python.fro
-00002e30: 6d20 6669 6e61 6e63 6574 6f6f 6c6b 6974  m financetoolkit
-00002e40: 2e62 6173 6520 696d 706f 7274 2068 656c  .base import hel
-00002e50: 7065 7273 0a0a 6261 6c61 6e63 655f 6772  pers..balance_gr
-00002e60: 6f75 7065 6420 3d20 6865 6c70 6572 732e  ouped = helpers.
-00002e70: 636f 6d62 696e 655f 6461 7461 6672 616d  combine_datafram
-00002e80: 6573 287b 2741 4150 4c27 3a20 6261 6c61  es({'AAPL': bala
-00002e90: 6e63 655f 6170 706c 652c 2027 4d53 4654  nce_apple, 'MSFT
-00002ea0: 273a 2062 616c 616e 6365 5f6d 7366 747d  ': balance_msft}
-00002eb0: 290a 6060 600a 0a4f 6e63 6520 616c 6c20  ).```..Once all 
-00002ec0: 6f66 2074 6869 7320 6973 2073 6574 2d75  of this is set-u
-00002ed0: 7020 796f 7520 6361 6e20 6665 6564 2074  p you can feed t
-00002ee0: 6869 7320 696e 666f 726d 6174 696f 6e20  his information 
-00002ef0: 746f 2074 6865 2054 6f6f 6c6b 6974 2061  to the Toolkit a
-00002f00: 6e64 2075 7365 2074 6865 2054 6f6f 6c6b  nd use the Toolk
-00002f10: 6974 2061 7320 6e6f 726d 616c 6c79 2e0a  it as normally..
-00002f20: 0a60 6060 7079 7468 6f6e 0a0a 2320 496e  .```python..# In
-00002f30: 6974 6961 6c69 7a65 2074 6865 2054 6f6f  itialize the Too
-00002f40: 6c6b 6974 0a63 6f6d 7061 6e69 6573 203d  lkit.companies =
-00002f50: 2054 6f6f 6c6b 6974 280a 2020 2020 7469   Toolkit(.    ti
-00002f60: 636b 6572 733d 5b27 4141 504c 272c 2027  ckers=['AAPL', '
-00002f70: 4d53 4654 275d 2c0a 2020 2020 6261 6c61  MSFT'],.    bala
-00002f80: 6e63 653d 6261 6c61 6e63 655f 6772 6f75  nce=balance_grou
-00002f90: 7065 642c 0a20 2020 2069 6e63 6f6d 653d  ped,.    income=
-00002fa0: 696e 636f 6d65 5f67 726f 7570 6564 2c0a  income_grouped,.
-00002fb0: 2020 2020 6361 7368 3d63 6173 685f 6772      cash=cash_gr
-00002fc0: 6f75 7065 642c 0a20 2020 2066 6f72 6d61  ouped,.    forma
-00002fd0: 745f 6c6f 6361 7469 6f6e 3d22 464f 4c44  t_location="FOLD
-00002fe0: 4552 5f50 4154 4822 2c0a 2020 2020 7265  ER_PATH",.    re
-00002ff0: 7665 7273 655f 6461 7465 733d 4661 6c73  verse_dates=Fals
-00003000: 6529 2023 2050 7574 2074 6869 7320 746f  e) # Put this to
-00003010: 2054 7275 6520 696e 2063 6173 6520 6461   True in case da
-00003020: 7465 7320 6172 6520 6465 7363 656e 6469  tes are descendi
-00003030: 6e67 0a0a 2320 5265 7475 726e 2061 6c6c  ng..# Return all
-00003040: 2052 6174 696f 730a 636f 6d70 616e 6965   Ratios.companie
-00003050: 732e 7261 7469 6f73 2e63 6f6c 6c65 6374  s.ratios.collect
-00003060: 5f61 6c6c 5f72 6174 696f 7328 290a 6060  _all_ratios().``
-00003070: 600a 0a54 6869 7320 7769 6c6c 2072 6574  `..This will ret
-00003080: 7572 6e20 616c 6c20 6669 6e61 6e63 6961  urn all financia
-00003090: 6c20 7261 7469 6f73 2074 6861 7420 6361  l ratios that ca
-000030a0: 6e20 6265 2063 6f6c 6c65 6374 6564 2062  n be collected b
-000030b0: 6173 6564 206f 6e20 7468 6520 7072 6f76  ased on the prov
-000030c0: 6964 6564 2064 6174 6120 616e 6420 7468  ided data and th
-000030d0: 6520 666f 726d 6174 2e0a 0a21 5b4f 7574  e format...![Out
-000030e0: 7075 7420 6f66 2052 6573 756c 745d 2868  put of Result](h
-000030f0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00003100: 6d2f 4a65 7242 6f75 6d61 2f46 696e 616e  m/JerBouma/Finan
-00003110: 6365 546f 6f6c 6b69 742f 6173 7365 7473  ceToolkit/assets
-00003120: 2f34 3633 3535 3336 342f 3261 3939 3534  /46355364/2a9954
-00003130: 3330 2d62 3864 382d 3432 3336 2d38 3932  30-b8d8-4236-892
-00003140: 632d 6564 6234 3730 3432 6436 6166 290a  c-edb47042d6af).
-00003150: 0a23 2320 4361 6c6c 696e 6720 4675 6e63  .## Calling Func
-00003160: 7469 6f6e 7320 4469 7265 6374 6c79 0a0a  tions Directly..
-00003170: 4974 2061 6c73 6f20 706f 7373 6962 6c65  It also possible
-00003180: 2074 6f20 6361 6c6c 2061 6e79 2072 6174   to call any rat
-00003190: 696f 206f 7220 6d6f 6465 6c20 6469 7265  io or model dire
-000031a0: 6374 6c79 2061 7320 7368 6f77 6e20 6265  ctly as shown be
-000031b0: 6c6f 772e 2054 6869 7320 616c 6c6f 7773  low. This allows
-000031c0: 2061 6363 6573 7320 746f 2035 302b 2072   access to 50+ r
-000031d0: 6174 696f 7320 7769 7468 2063 7573 746f  atios with custo
-000031e0: 6d20 6461 7461 2e20 416c 736f 2073 6565  m data. Also see
-000031f0: 205b 7468 6973 206e 6f74 6562 6f6f 6b5d   [this notebook]
-00003200: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00003210: 636f 6d2f 4a65 7242 6f75 6d61 2f46 696e  com/JerBouma/Fin
-00003220: 616e 6365 546f 6f6c 6b69 742f 626c 6f62  anceToolkit/blob
-00003230: 2f6d 6169 6e2f 6578 616d 706c 6573 2f46  /main/examples/F
-00003240: 696e 616e 6365 2532 3054 6f6f 6c6b 6974  inance%20Toolkit
-00003250: 2532 302d 2532 3034 2e25 3230 4361 6c6c  %20-%204.%20Call
-00003260: 696e 6725 3230 4675 6e63 7469 6f6e 7325  ing%20Functions%
-00003270: 3230 4469 7265 6374 6c79 2e69 7079 6e62  20Directly.ipynb
-00003280: 292e 0a0a 6060 6070 7974 686f 6e0a 696d  )...```python.im
-00003290: 706f 7274 2070 616e 6461 7320 6173 2070  port pandas as p
-000032a0: 640a 696d 706f 7274 206e 756d 7079 2061  d.import numpy a
-000032b0: 7320 6e70 0a0a 6672 6f6d 2066 696e 616e  s np..from finan
-000032c0: 6365 746f 6f6c 6b69 742e 6d6f 6465 6c73  cetoolkit.models
-000032d0: 2069 6d70 6f72 7420 6475 706f 6e74 0a0a   import dupont..
-000032e0: 7965 6172 7320 3d20 5b32 3031 382c 2032  years = [2018, 2
-000032f0: 3031 392c 2032 3032 302c 2032 3032 312c  019, 2020, 2021,
-00003300: 2032 3032 325d 0a0a 6475 706f 6e74 2e67   2022]..dupont.g
-00003310: 6574 5f64 7570 6f6e 745f 616e 616c 7973  et_dupont_analys
-00003320: 6973 280a 2020 2020 6e65 745f 696e 636f  is(.    net_inco
-00003330: 6d65 3d70 642e 5365 7269 6573 280a 2020  me=pd.Series(.  
-00003340: 2020 2020 2020 5b35 3935 3331 3030 3030        [595310000
-00003350: 3030 2c20 3535 3235 3630 3030 3030 302c  00, 55256000000,
-00003360: 2035 3734 3131 3030 3030 3030 2c20 3934   57411000000, 94
-00003370: 3638 3030 3030 3030 302c 2039 3938 3033  680000000, 99803
-00003380: 3030 3030 3030 5d2c 2069 6e64 6578 3d79  000000], index=y
-00003390: 6561 7273 0a20 2020 2029 2c0a 2020 2020  ears.    ),.    
-000033a0: 746f 7461 6c5f 7265 7665 6e75 653d 7064  total_revenue=pd
-000033b0: 2e53 6572 6965 7328 0a20 2020 2020 2020  .Series(.       
-000033c0: 205b 3236 3535 3935 3030 3030 3030 2c20   [265595000000, 
-000033d0: 3236 3031 3734 3030 3030 3030 2c20 3237  260174000000, 27
-000033e0: 3435 3135 3030 3030 3030 2c20 3336 3538  4515000000, 3658
-000033f0: 3137 3030 3030 3030 2c20 3339 3433 3238  17000000, 394328
-00003400: 3030 3030 3030 5d2c 0a20 2020 2020 2020  000000],.       
-00003410: 2069 6e64 6578 3d79 6561 7273 2c0a 2020   index=years,.  
-00003420: 2020 292c 0a20 2020 2074 6f74 616c 5f61    ),.    total_a
-00003430: 7373 6574 735f 6265 6769 6e3d 7064 2e53  ssets_begin=pd.S
-00003440: 6572 6965 7328 0a20 2020 2020 2020 205b  eries(.        [
-00003450: 6e70 2e6e 616e 2c20 3336 3537 3235 3030  np.nan, 36572500
-00003460: 3030 3030 2c20 3333 3835 3136 3030 3030  0000, 3385160000
-00003470: 3030 2c20 3332 3338 3838 3030 3030 3030  00, 323888000000
-00003480: 2c20 3335 3130 3032 3030 3030 3030 5d2c  , 351002000000],
-00003490: 0a20 2020 2020 2020 2069 6e64 6578 3d79  .        index=y
-000034a0: 6561 7273 2c0a 2020 2020 292c 0a20 2020  ears,.    ),.   
-000034b0: 2074 6f74 616c 5f61 7373 6574 735f 656e   total_assets_en
-000034c0: 643d 7064 2e53 6572 6965 7328 0a20 2020  d=pd.Series(.   
-000034d0: 2020 2020 205b 3336 3537 3235 3030 3030       [3657250000
-000034e0: 3030 2c20 3333 3835 3136 3030 3030 3030  00, 338516000000
-000034f0: 2c20 3332 3338 3838 3030 3030 3030 2c20  , 323888000000, 
-00003500: 3335 3130 3032 3030 3030 3030 2c20 3335  351002000000, 35
-00003510: 3237 3535 3030 3030 3030 5d2c 0a20 2020  2755000000],.   
-00003520: 2020 2020 2069 6e64 6578 3d79 6561 7273       index=years
-00003530: 2c0a 2020 2020 292c 0a20 2020 2074 6f74  ,.    ),.    tot
-00003540: 616c 5f65 7175 6974 795f 6265 6769 6e3d  al_equity_begin=
-00003550: 7064 2e53 6572 6965 7328 0a20 2020 2020  pd.Series(.     
-00003560: 2020 205b 6e70 2e6e 616e 2c20 3130 3731     [np.nan, 1071
-00003570: 3437 3030 3030 3030 2c20 3930 3438 3830  47000000, 904880
-00003580: 3030 3030 302c 2036 3533 3339 3030 3030  00000, 653390000
-00003590: 3030 2c20 3633 3039 3030 3030 3030 305d  00, 63090000000]
-000035a0: 2c20 696e 6465 783d 7965 6172 730a 2020  , index=years.  
-000035b0: 2020 292c 0a20 2020 2074 6f74 616c 5f65    ),.    total_e
-000035c0: 7175 6974 795f 656e 643d 7064 2e53 6572  quity_end=pd.Ser
-000035d0: 6965 7328 0a20 2020 2020 2020 205b 3130  ies(.        [10
-000035e0: 3731 3437 3030 3030 3030 2c20 3930 3438  7147000000, 9048
-000035f0: 3830 3030 3030 302c 2036 3533 3339 3030  8000000, 6533900
-00003600: 3030 3030 2c20 3633 3039 3030 3030 3030  0000, 6309000000
-00003610: 302c 2035 3036 3732 3030 3030 3030 5d2c  0, 50672000000],
-00003620: 2069 6e64 6578 3d79 6561 7273 0a20 2020   index=years.   
-00003630: 2029 2c0a 290a 6060 600a 0a54 6869 7320   ),.).```..This 
-00003640: 7265 7475 726e 7320 7468 6520 666f 6c6c  returns the foll
-00003650: 6f77 696e 6720 7461 626c 6520 7768 6963  owing table whic
-00003660: 6820 636c 6f73 656c 7920 7265 7365 6d62  h closely resemb
-00003670: 6c65 7320 6120 7072 6f70 6572 2044 7570  les a proper Dup
-00003680: 6f6e 7420 616e 616c 7973 6973 2066 6f72  ont analysis for
-00003690: 2041 7070 6c65 2061 7420 7468 6569 7220   Apple at their 
-000036a0: 6769 7665 6e20 7265 706f 7274 696e 6720  given reporting 
-000036b0: 6461 7465 7320 696e 204f 6374 6f62 6572  dates in October
-000036c0: 3a0a 0a7c 2020 2020 2020 2020 2020 2020  :..|            
-000036d0: 2020 2020 2020 207c 2020 2020 2020 2032         |       2
-000036e0: 3031 3820 7c20 2020 2020 3230 3139 207c  018 |     2019 |
-000036f0: 2020 2020 2032 3032 3020 7c20 2020 2020       2020 |     
-00003700: 3230 3231 207c 2020 2020 2032 3032 3220  2021 |     2022 
-00003710: 7c0a 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |.|:------------
-00003720: 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d  ------|---------
-00003730: 2d2d 3a7c 2d2d 2d2d 2d2d 2d2d 2d3a 7c2d  --:|---------:|-
-00003740: 2d2d 2d2d 2d2d 2d2d 3a7c 2d2d 2d2d 2d2d  --------:|------
-00003750: 2d2d 2d3a 7c2d 2d2d 2d2d 2d2d 2d2d 3a7c  ---:|---------:|
-00003760: 0a7c 204e 6574 2050 726f 6669 7420 4d61  .| Net Profit Ma
-00003770: 7267 696e 207c 2020 2030 2e32 3234 3134  rgin |   0.22414
-00003780: 3220 7c20 302e 3231 3233 3831 207c 2030  2 | 0.212381 | 0
-00003790: 2e32 3039 3133 3620 7c20 302e 3235 3838  .209136 | 0.2588
-000037a0: 3138 207c 2030 2e32 3533 3039 3620 7c0a  18 | 0.253096 |.
-000037b0: 7c20 4173 7365 7420 5475 726e 6f76 6572  | Asset Turnover
-000037c0: 2020 2020 7c20 6e61 6e20 2020 2020 2020      | nan       
-000037d0: 207c 2030 2e37 3338 3837 3820 7c20 302e   | 0.738878 | 0.
-000037e0: 3832 3838 3435 207c 2031 2e30 3834 3038  828845 | 1.08408
-000037f0: 2020 7c20 312e 3132 3036 3420 207c 0a7c    | 1.12064  |.|
-00003800: 2045 7175 6974 7920 4d75 6c74 6970 6c69   Equity Multipli
-00003810: 6572 207c 206e 616e 2020 2020 2020 2020  er | nan        
-00003820: 7c20 332e 3536 3333 3420 207c 2034 2e32  | 3.56334  | 4.2
-00003830: 3530 3839 2020 7c20 352e 3235 3439 3720  5089  | 5.25497 
-00003840: 207c 2036 2e31 3836 3232 2020 7c0a 7c20   | 6.18622  |.| 
-00003850: 5265 7475 726e 206f 6e20 4571 7569 7479  Return on Equity
-00003860: 2020 7c20 6e61 6e20 2020 2020 2020 207c    | nan        |
-00003870: 2030 2e35 3539 3137 3220 7c20 302e 3733   0.559172 | 0.73
-00003880: 3638 3536 207c 2031 2e34 3734 3433 2020  6856 | 1.47443  
-00003890: 7c20 312e 3735 3435 3920 207c 0a0a 2320  | 1.75459  |..# 
-000038a0: 436f 6e74 6163 740a 4966 2079 6f75 2068  Contact.If you h
-000038b0: 6176 6520 616e 7920 7175 6573 7469 6f6e  ave any question
-000038c0: 7320 6162 6f75 7420 7468 6520 4669 6e61  s about the Fina
-000038d0: 6e63 6554 6f6f 6c6b 6974 206f 7220 776f  nceToolkit or wo
-000038e0: 756c 6420 6c69 6b65 2074 6f20 7368 6172  uld like to shar
-000038f0: 6520 7769 7468 206d 6520 7768 6174 2079  e with me what y
-00003900: 6f75 2068 6176 6520 6265 656e 2077 6f72  ou have been wor
-00003910: 6b69 6e67 206f 6e2c 2066 6565 6c20 6672  king on, feel fr
-00003920: 6565 2074 6f20 7265 6163 6820 6f75 7420  ee to reach out 
-00003930: 746f 206d 6520 7669 613a 0a0a 2d20 2a2a  to me via:..- **
-00003940: 4c69 6e6b 6564 496e 3a2a 2a20 6874 7470  LinkedIn:** http
-00003950: 733a 2f2f 7777 772e 6c69 6e6b 6564 696e  s://www.linkedin
-00003960: 2e63 6f6d 2f69 6e2f 626f 756d 616a 6572  .com/in/boumajer
-00003970: 6f65 6e2f 0a2d 2020 2a2a 456d 6169 6c3a  oen/.-  **Email:
-00003980: 2a2a 206a 6572 2e62 6f75 6d61 4067 6d61  ** jer.bouma@gma
-00003990: 696c 2e63 6f6d 0a0a 4966 2079 6f75 2764  il.com..If you'd
-000039a0: 206c 696b 6520 746f 2073 7570 706f 7274   like to support
-000039b0: 206d 7920 6566 666f 7274 732c 2065 6974   my efforts, eit
-000039c0: 6865 7220 6865 6c70 206d 6520 6f75 7420  her help me out 
-000039d0: 6279 2063 6f6e 7472 6962 7574 696e 6720  by contributing 
-000039e0: 746f 2074 6865 2070 6163 6b61 6765 206f  to the package o
-000039f0: 7220 5b42 7579 206d 6520 6120 436f 6666  r [Buy me a Coff
-00003a00: 6565 5d28 6874 7470 733a 2f2f 7777 772e  ee](https://www.
-00003a10: 6275 796d 6561 636f 6666 6565 2e63 6f6d  buymeacoffee.com
-00003a20: 2f6a 6572 626f 756d 6129 2e0a 0a5b 215b  /jerbouma)...[![
-00003a30: 5374 6172 2048 6973 746f 7279 2043 6861  Star History Cha
-00003a40: 7274 5d28 6874 7470 733a 2f2f 6170 692e  rt](https://api.
-00003a50: 7374 6172 2d68 6973 746f 7279 2e63 6f6d  star-history.com
-00003a60: 2f73 7667 3f72 6570 6f73 3d4a 6572 426f  /svg?repos=JerBo
-00003a70: 756d 612f 4669 6e61 6e63 6554 6f6f 6c6b  uma/FinanceToolk
-00003a80: 6974 2674 7970 653d 4461 7465 295d 2868  it&type=Date)](h
-00003a90: 7474 7073 3a2f 2f73 7461 722d 6869 7374  ttps://star-hist
-00003aa0: 6f72 792e 636f 6d2f 234a 6572 426f 756d  ory.com/#JerBoum
-00003ab0: 612f 4669 6e61 6e63 6554 6f6f 6c6b 6974  a/FinanceToolkit
-00003ac0: 2644 6174 6529 0a                        &Date).
+00002130: 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d 2d3a 7c2d  ---|---------:|-
+00002140: 2d2d 2d2d 2d2d 2d2d 3a7c 2d2d 2d2d 2d2d  --------:|------
+00002150: 2d2d 2d3a 7c2d 2d2d 2d2d 2d2d 2d2d 3a7c  ---:|---------:|
+00002160: 2d2d 2d2d 2d2d 2d2d 2d3a 7c0a 7c20 4772  ---------:|.| Gr
+00002170: 6f73 7320 4d61 7267 696e 2020 2020 2020  oss Margin      
+00002180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002190: 2020 2020 2020 2020 2020 7c20 302e 3338            | 0.38
+000021a0: 3334 3337 207c 2030 2e33 3738 3137 3820  3437 | 0.378178 
+000021b0: 7c20 302e 3338 3233 3332 207c 2030 2e34  | 0.382332 | 0.4
+000021c0: 3137 3739 3420 7c20 302e 3433 3330 3936  17794 | 0.433096
+000021d0: 207c 0a7c 204f 7065 7261 7469 6e67 204d   |.| Operating M
+000021e0: 6172 6769 6e20 2020 2020 2020 2020 2020  argin           
+000021f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002200: 207c 2030 2e32 3636 3934 2020 7c20 302e   | 0.26694  | 0.
+00002210: 3234 3537 3220 207c 2030 2e32 3431 3437  24572  | 0.24147
+00002220: 3320 7c20 302e 3239 3738 3234 207c 2030  3 | 0.297824 | 0
+00002230: 2e33 3032 3838 3720 7c0a 7c20 4e65 7420  .302887 |.| Net 
+00002240: 5072 6f66 6974 204d 6172 6769 6e20 2020  Profit Margin   
+00002250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002260: 2020 2020 2020 2020 7c20 302e 3232 3431          | 0.2241
+00002270: 3432 207c 2030 2e32 3132 3338 3120 7c20  42 | 0.212381 | 
+00002280: 302e 3230 3931 3336 207c 2030 2e32 3538  0.209136 | 0.258
+00002290: 3831 3820 7c20 302e 3235 3330 3936 207c  818 | 0.253096 |
+000022a0: 0a7c 2049 6e74 6572 6573 7420 4275 7264  .| Interest Burd
+000022b0: 656e 2052 6174 696f 2020 2020 2020 2020  en Ratio        
+000022c0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+000022d0: 2031 2e30 3238 3238 2020 7c20 312e 3032   1.02828  | 1.02
+000022e0: 3832 3720 207c 2031 2e30 3132 3131 2020  827  | 1.01211  
+000022f0: 7c20 312e 3030 3233 3720 207c 2030 2e39  | 1.00237  | 0.9
+00002300: 3937 3230 3420 7c0a 7c20 496e 636f 6d65  97204 |.| Income
+00002310: 2042 6566 6f72 6520 5461 7820 5072 6f66   Before Tax Prof
+00002320: 6974 204d 6172 6769 6e20 2020 2020 2020  it Margin       
+00002330: 2020 2020 2020 7c20 302e 3237 3434 3839        | 0.274489
+00002340: 207c 2030 2e32 3532 3636 3620 7c20 302e   | 0.252666 | 0.
+00002350: 3234 3433 3938 207c 2030 2e32 3938 3532  244398 | 0.29852
+00002360: 3920 7c20 302e 3330 3230 3420 207c 0a7c  9 | 0.30204  |.|
+00002370: 2045 6666 6563 7469 7665 2054 6178 2052   Effective Tax R
+00002380: 6174 6520 2020 2020 2020 2020 2020 2020  ate             
+00002390: 2020 2020 2020 2020 2020 2020 207c 2030               | 0
+000023a0: 2e31 3833 3432 3220 7c20 302e 3135 3934  .183422 | 0.1594
+000023b0: 3338 207c 2030 2e31 3434 3238 3220 7c20  38 | 0.144282 | 
+000023c0: 302e 3133 3330 3233 207c 2030 2e31 3632  0.133023 | 0.162
+000023d0: 3034 3520 7c0a 7c20 5265 7475 726e 206f  045 |.| Return o
+000023e0: 6e20 4173 7365 7473 2028 524f 4129 2020  n Assets (ROA)  
+000023f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002400: 2020 2020 7c20 302e 3136 3237 3735 207c      | 0.162775 |
+00002410: 2030 2e31 3633 3233 2020 7c20 302e 3137   0.16323  | 0.17
+00002420: 3732 3536 207c 2030 2e32 3639 3734 3220  7256 | 0.269742 
+00002430: 7c20 302e 3238 3239 3234 207c 0a7c 2052  | 0.282924 |.| R
+00002440: 6574 7572 6e20 6f6e 2045 7175 6974 7920  eturn on Equity 
+00002450: 2852 4f45 2920 2020 2020 2020 2020 2020  (ROE)           
+00002460: 2020 2020 2020 2020 2020 207c 2030 2e35             | 0.5
+00002470: 3535 3630 3120 7c20 302e 3631 3036 3435  55601 | 0.610645
+00002480: 207c 2030 2e38 3738 3636 3420 7c20 312e   | 0.878664 | 1.
+00002490: 3530 3037 3120 207c 2031 2e39 3639 3539  50071  | 1.96959
+000024a0: 2020 7c0a 7c20 5265 7475 726e 206f 6e20    |.| Return on 
+000024b0: 496e 7665 7374 6564 2043 6170 6974 616c  Invested Capital
+000024c0: 2028 524f 4943 2920 2020 2020 2020 2020   (ROIC)         
+000024d0: 2020 7c20 302e 3236 3938 3538 207c 2030    | 0.269858 | 0
+000024e0: 2e32 3933 3732 3120 7c20 302e 3334 3431  .293721 | 0.3441
+000024f0: 3236 207c 2030 2e35 3033 3835 3220 7c20  26 | 0.503852 | 
+00002500: 302e 3536 3236 3435 207c 0a7c 2052 6574  0.562645 |.| Ret
+00002510: 7572 6e20 6f6e 2043 6170 6974 616c 2045  urn on Capital E
+00002520: 6d70 6c6f 7965 6420 2852 4f43 4529 2020  mployed (ROCE)  
+00002530: 2020 2020 2020 2020 207c 2030 2e33 3035           | 0.305
+00002540: 3936 3820 7c20 302e 3239 3737 3339 207c  968 | 0.297739 |
+00002550: 2030 2e33 3230 3230 3720 7c20 302e 3439   0.320207 | 0.49
+00002560: 3539 3732 207c 2030 2e36 3133 3933 3720  5972 | 0.613937 
+00002570: 7c0a 7c20 5265 7475 726e 206f 6e20 5461  |.| Return on Ta
+00002580: 6e67 6962 6c65 2041 7373 6574 7320 2020  ngible Assets   
+00002590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025a0: 7c20 302e 3535 3536 3031 207c 2030 2e36  | 0.555601 | 0.6
+000025b0: 3130 3634 3520 7c20 302e 3837 3836 3634  10645 | 0.878664
+000025c0: 207c 2031 2e35 3030 3731 2020 7c20 312e   | 1.50071  | 1.
+000025d0: 3936 3935 3920 207c 0a7c 2049 6e63 6f6d  96959  |.| Incom
+000025e0: 6520 5175 616c 6974 7920 5261 7469 6f20  e Quality Ratio 
+000025f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002600: 2020 2020 2020 207c 2031 2e33 3030 3733         | 1.30073
+00002610: 2020 7c20 312e 3235 3538 3120 207c 2031    | 1.25581  | 1
+00002620: 2e34 3035 3220 2020 7c20 312e 3039 3838  .4052   | 1.0988
+00002630: 3420 207c 2031 2e32 3233 3932 2020 7c0a  4  | 1.22392  |.
+00002640: 7c20 4e65 7420 496e 636f 6d65 2070 6572  | Net Income per
+00002650: 2045 4254 2020 2020 2020 2020 2020 2020   EBT            
+00002660: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00002670: 302e 3831 3635 3738 207c 2030 2e38 3430  0.816578 | 0.840
+00002680: 3536 3220 7c20 302e 3835 3537 3138 207c  562 | 0.855718 |
+00002690: 2030 2e38 3636 3937 3720 7c20 302e 3833   0.866977 | 0.83
+000026a0: 3739 3535 207c 0a7c 2046 7265 6520 4361  7955 |.| Free Ca
+000026b0: 7368 2046 6c6f 7720 746f 204f 7065 7261  sh Flow to Opera
+000026c0: 7469 6e67 2043 6173 6820 466c 6f77 2052  ting Cash Flow R
+000026d0: 6174 696f 207c 2030 2e38 3238 3037 3320  atio | 0.828073 
+000026e0: 7c20 302e 3834 3837 3536 207c 2030 2e39  | 0.848756 | 0.9
+000026f0: 3039 3430 3120 7c20 302e 3839 3334 3532  09401 | 0.893452
+00002700: 207c 2030 2e39 3132 3333 3820 7c0a 7c20   | 0.912338 |.| 
+00002710: 4542 5420 746f 2045 4249 5420 5261 7469  EBT to EBIT Rati
+00002720: 6f20 2020 2020 2020 2020 2020 2020 2020  o               
+00002730: 2020 2020 2020 2020 2020 2020 7c20 302e              | 0.
+00002740: 3935 3734 3438 207c 2030 2e39 3438 3430  957448 | 0.94840
+00002750: 3820 7c20 302e 3935 3839 3336 207c 2030  8 | 0.958936 | 0
+00002760: 2e39 3736 3335 3320 7c20 302e 3937 3539  .976353 | 0.9759
+00002770: 3832 207c 0a7c 2045 4249 5420 746f 2052  82 |.| EBIT to R
+00002780: 6576 656e 7565 2020 2020 2020 2020 2020  evenue          
+00002790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000027a0: 2020 207c 2030 2e32 3836 3638 3820 7c20     | 0.286688 | 
+000027b0: 302e 3236 3634 3120 207c 2030 2e32 3534  0.26641  | 0.254
+000027c0: 3836 3420 7c20 302e 3330 3537 3539 207c  864 | 0.305759 |
+000027d0: 2030 2e33 3039 3437 3320 7c0a 0a23 2320   0.309473 |..## 
+000027e0: 4465 6669 6e69 6e67 2043 7573 746f 6d20  Defining Custom 
+000027f0: 5261 7469 6f73 0a0a 5468 6520 4669 6e61  Ratios..The Fina
+00002800: 6e63 6520 546f 6f6c 6b69 7420 6861 7320  nce Toolkit has 
+00002810: 616e 2061 6275 6e64 616e 6365 206f 6620  an abundance of 
+00002820: 6669 6e61 6e63 6961 6c20 7261 7469 6f73  financial ratios
+00002830: 2c20 686f 7765 7665 7220 6974 2063 6f75  , however it cou
+00002840: 6c64 2062 6520 7468 6174 2079 6f75 2061  ld be that you a
+00002850: 7265 206c 6f6f 6b69 6e67 2066 6f72 2061  re looking for a
+00002860: 2073 7065 6369 6669 6320 7261 7469 6f20   specific ratio 
+00002870: 7468 6174 2069 7320 6375 7272 656e 746c  that is currentl
+00002880: 7920 6e6f 7420 7072 6f76 6964 6564 2e20  y not provided. 
+00002890: 4669 7273 7420 616e 6420 666f 7265 6d6f  First and foremo
+000028a0: 7374 2c20 4920 656e 636f 7572 6167 6520  st, I encourage 
+000028b0: 746f 205b 6372 6561 7465 2061 2050 756c  to [create a Pul
+000028c0: 6c20 5265 7175 6573 745d 2868 7474 7073  l Request](https
+000028d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 4a65  ://github.com/Je
+000028e0: 7242 6f75 6d61 2f46 696e 616e 6365 546f  rBouma/FinanceTo
+000028f0: 6f6c 6b69 742f 7075 6c6c 7329 2074 6f20  olkit/pulls) to 
+00002900: 6164 6420 7468 6573 6520 7261 7469 6f73  add these ratios
+00002910: 2069 6e20 6275 7420 7468 6572 6520 6973   in but there is
+00002920: 2061 6c73 6f20 616e 206f 7074 696f 6e20   also an option 
+00002930: 746f 2061 6464 2063 7573 746f 6d20 7261  to add custom ra
+00002940: 7469 6f73 2061 7320 666f 6c6c 6f77 732e  tios as follows.
+00002950: 2054 6869 7320 6665 6174 7572 6520 7761   This feature wa
+00002960: 7320 6465 7369 676e 6564 2062 7920 5b73  s designed by [s
+00002970: 776f 7264 3133 345d 2868 7474 7073 3a2f  word134](https:/
+00002980: 2f67 6974 6875 622e 636f 6d2f 7377 6f72  /github.com/swor
+00002990: 6431 3334 292e 2046 696e 6420 6120 4e6f  d134). Find a No
+000029a0: 7465 626f 6f6b 2065 7861 6d70 6c65 205b  tebook example [
+000029b0: 6865 7265 5d28 6874 7470 733a 2f2f 6769  here](https://gi
+000029c0: 7468 7562 2e63 6f6d 2f4a 6572 426f 756d  thub.com/JerBoum
+000029d0: 612f 4669 6e61 6e63 6554 6f6f 6c6b 6974  a/FinanceToolkit
+000029e0: 2f62 6c6f 622f 6d61 696e 2f65 7861 6d70  /blob/main/examp
+000029f0: 6c65 732f 4669 6e61 6e63 6525 3230 546f  les/Finance%20To
+00002a00: 6f6c 6b69 7425 3230 2d25 3230 332e 2532  olkit%20-%203.%2
+00002a10: 3044 6566 696e 696e 6725 3230 4375 7374  0Defining%20Cust
+00002a20: 6f6d 2532 3052 6174 696f 732e 6970 796e  om%20Ratios.ipyn
+00002a30: 6229 2e0a 0a44 6566 696e 6520 686f 7720  b)...Define how 
+00002a40: 6561 6368 2063 7573 746f 6d20 7261 7469  each custom rati
+00002a50: 6f20 6e65 6564 7320 746f 2062 6520 6361  o needs to be ca
+00002a60: 6c63 756c 6174 6564 2e20 5468 6973 2066  lculated. This f
+00002a70: 6f6c 6c6f 7773 2074 6865 2073 7472 7563  ollows the struc
+00002a80: 7475 7265 2060 4e61 6d65 206f 6620 5261  ture `Name of Ra
+00002a90: 7469 6f60 3a20 6046 696e 616e 6369 616c  tio`: `Financial
+00002aa0: 2053 7461 7465 6d65 6e74 2049 7465 6d20   Statement Item 
+00002ab0: 2a20 4669 6e61 6e63 6961 6c20 5374 6174  * Financial Stat
+00002ac0: 656d 656e 7420 4974 656d 602e 204e 6f74  ement Item`. Not
+00002ad0: 6520 7468 6174 2079 6f75 2061 6468 6572  e that you adher
+00002ae0: 6520 746f 2074 6865 206e 6f72 6d61 6c69  e to the normali
+00002af0: 7a61 7469 6f6e 2066 696c 6573 206e 616d  zation files nam
+00002b00: 696e 672e 2054 6869 7320 6361 6e20 6265  ing. This can be
+00002b10: 2076 6965 7765 6420 7265 6c61 7469 7665   viewed relative
+00002b20: 6c79 2065 6173 7920 6279 2069 6e69 7469  ly easy by initi
+00002b30: 616c 697a 696e 6720 7468 6520 546f 6f6c  alizing the Tool
+00002b40: 6b69 7420 616e 6420 7275 6e6e 696e 6720  kit and running 
+00002b50: 666f 7220 6578 616d 706c 6520 6067 6574  for example `get
+00002b60: 5f62 616c 616e 6365 5f73 6865 6574 5f73  _balance_sheet_s
+00002b70: 7461 7465 6d65 6e74 602e 0a0a 6060 6070  tatement`...```p
+00002b80: 7974 686f 6e0a 6375 7374 6f6d 5f72 6174  ython.custom_rat
+00002b90: 696f 7320 3d20 7b0a 2020 2020 2757 4320  ios = {.    'WC 
+00002ba0: 2f20 4e65 7420 496e 636f 6d65 273a 2027  / Net Income': '
+00002bb0: 576f 726b 696e 6720 4361 7069 7461 6c20  Working Capital 
+00002bc0: 2f20 4e65 7420 496e 636f 6d65 272c 0a20  / Net Income',. 
+00002bd0: 2020 2027 4e65 7420 496e 636f 6d65 202f     'Net Income /
+00002be0: 2054 6f74 616c 2041 7373 6574 7327 3a20   Total Assets': 
+00002bf0: 274e 6574 2049 6e63 6f6d 6520 2f20 546f  'Net Income / To
+00002c00: 7461 6c20 4173 7365 7473 272c 0a20 2020  tal Assets',.   
+00002c10: 2027 4375 7272 656e 7420 4173 7365 7473   'Current Assets
+00002c20: 2049 6e76 656e 746f 7279 273a 2027 546f   Inventory': 'To
+00002c30: 7461 6c20 4375 7272 656e 7420 4173 7365  tal Current Asse
+00002c40: 7473 202d 2049 6e76 656e 746f 7279 272c  ts - Inventory',
+00002c50: 0a20 2020 2027 5175 6963 6b20 5261 7469  .    'Quick Rati
+00002c60: 6f20 4375 7272 656e 7427 3a20 2743 7572  o Current': 'Cur
+00002c70: 7265 6e74 2041 7373 6574 7320 496e 7665  rent Assets Inve
+00002c80: 6e74 6f72 7920 2f20 546f 7461 6c20 4375  ntory / Total Cu
+00002c90: 7272 656e 7420 4c69 6162 696c 6974 6965  rrent Liabilitie
+00002ca0: 7327 2c0a 2020 2020 2751 7569 636b 2052  s',.    'Quick R
+00002cb0: 6174 696f 2054 6f74 616c 273a 2027 4375  atio Total': 'Cu
+00002cc0: 7272 656e 7420 4173 7365 7473 2049 6e76  rrent Assets Inv
+00002cd0: 656e 746f 7279 202f 2054 6f74 616c 204c  entory / Total L
+00002ce0: 6961 6269 6c69 7469 6573 270a 7d0a 6060  iabilities'.}.``
+00002cf0: 600a 0a49 6e69 7469 616c 697a 696e 6720  `..Initializing 
+00002d00: 7468 6520 4669 6e61 6e63 6520 546f 6f6c  the Finance Tool
+00002d10: 6b69 742e 204d 616b 6520 7375 7265 2074  kit. Make sure t
+00002d20: 6f20 7365 7420 7468 6520 7061 7261 6d65  o set the parame
+00002d30: 7465 7220 6063 7573 746f 6d5f 7261 7469  ter `custom_rati
+00002d40: 6f73 6020 7769 7468 2074 6865 2061 626f  os` with the abo
+00002d50: 7665 2064 6963 7469 6f6e 6172 792e 204e  ve dictionary. N
+00002d60: 6f74 6520 7468 6174 2060 7175 6172 7465  ote that `quarte
+00002d70: 726c 793d 5472 7565 6020 646f 6573 6e27  rly=True` doesn'
+00002d80: 7420 776f 726b 2077 6974 686f 7574 2061  t work without a
+00002d90: 2050 7265 6d69 756d 2070 6c61 6e2e 0a0a   Premium plan...
+00002da0: 6060 6070 7974 686f 6e0a 6672 6f6d 2066  ```python.from f
+00002db0: 696e 616e 6365 746f 6f6c 6b69 7420 696d  inancetoolkit im
+00002dc0: 706f 7274 2054 6f6f 6c6b 6974 0a0a 2320  port Toolkit..# 
+00002dd0: 496e 6974 6961 6c69 7a65 2074 6865 2046  Initialize the F
+00002de0: 696e 616e 6365 2054 6f6f 6c6b 6974 0a63  inance Toolkit.c
+00002df0: 6f6d 7061 6e69 6573 203d 2054 6f6f 6c6b  ompanies = Toolk
+00002e00: 6974 280a 2020 2020 5b22 4141 504c 222c  it(.    ["AAPL",
+00002e10: 2022 4d53 4654 222c 2022 474f 4f47 4c22   "MSFT", "GOOGL"
+00002e20: 2c20 2241 4d5a 4e22 5d2c 2061 7069 5f6b  , "AMZN"], api_k
+00002e30: 6579 3d41 5049 5f4b 4559 2c20 7374 6172  ey=API_KEY, star
+00002e40: 745f 6461 7465 3d22 3230 3232 2d30 382d  t_date="2022-08-
+00002e50: 3130 222c 0a20 2020 2063 7573 746f 6d5f  10",.    custom_
+00002e60: 7261 7469 6f73 3d63 7573 746f 6d5f 7261  ratios=custom_ra
+00002e70: 7469 6f73 2c20 7175 6172 7465 726c 793d  tios, quarterly=
+00002e80: 5472 7565 0a29 0a60 6060 0a0a 4279 2074  True.).```..By t
+00002e90: 6865 6e20 7275 6e6e 696e 6720 6072 6174  hen running `rat
+00002ea0: 696f 732e 636f 6c6c 6563 745f 6375 7374  ios.collect_cust
+00002eb0: 6f6d 5f72 6174 696f 7360 2069 7420 6175  om_ratios` it au
+00002ec0: 746f 6d61 7469 6361 6c6c 7920 6361 6c63  tomatically calc
+00002ed0: 756c 6174 6573 2074 6865 2067 6976 656e  ulates the given
+00002ee0: 2072 6174 696f 732e 204e 6f74 6520 7468   ratios. Note th
+00002ef0: 6520 7261 7469 6f73 2027 5175 6963 6b20  e ratios 'Quick 
+00002f00: 5261 7469 6f20 4375 7272 656e 7427 2061  Ratio Current' a
+00002f10: 6e64 2027 5175 6963 6b20 5261 7469 6f20  nd 'Quick Ratio 
+00002f20: 546f 7461 6c27 2077 6869 6368 2072 656c  Total' which rel
+00002f30: 7920 6f6e 2061 6e20 6561 726c 6965 7220  y on an earlier 
+00002f40: 6465 6669 6e65 6420 7261 7469 6f20 2827  defined ratio ('
+00002f50: 4375 7272 656e 7420 4173 7365 7473 2049  Current Assets I
+00002f60: 6e76 656e 746f 7279 2729 2e20 5468 6973  nventory'). This
+00002f70: 2069 7320 616e 2065 7861 6d70 6c65 206f   is an example o
+00002f80: 6620 686f 7720 796f 7520 6361 6e20 6372  f how you can cr
+00002f90: 6561 7465 2061 2063 7573 746f 6d20 7261  eate a custom ra
+00002fa0: 7469 6f20 6261 7365 6420 6f6e 2061 6e6f  tio based on ano
+00002fb0: 7468 6572 2063 7573 746f 6d20 7261 7469  ther custom rati
+00002fc0: 6f2e 0a0a 4265 6c6f 7720 796f 7520 6361  o...Below you ca
+00002fd0: 6e20 6669 6e64 2074 6865 2063 7573 746f  n find the custo
+00002fe0: 6d20 7261 7469 6f73 2066 726f 6d20 474f  m ratios from GO
+00002ff0: 4f47 4c20 7768 6963 6820 6861 7320 6265  OGL which has be
+00003000: 656e 2073 656c 6563 7465 6420 7769 7468  en selected with
+00003010: 2060 2e6c 6f63 5b27 474f 4f47 4c5d 602e   `.loc['GOOGL]`.
+00003020: 2054 6865 204e 6f74 6562 6f6f 6b20 6173   The Notebook as
+00003030: 2066 6f75 6e64 205b 6865 7265 5d28 6874   found [here](ht
+00003040: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00003050: 2f4a 6572 426f 756d 612f 4669 6e61 6e63  /JerBouma/Financ
+00003060: 6554 6f6f 6c6b 6974 2f62 6c6f 622f 6d61  eToolkit/blob/ma
+00003070: 696e 2f65 7861 6d70 6c65 732f 4669 6e61  in/examples/Fina
+00003080: 6e63 6525 3230 546f 6f6c 6b69 7425 3230  nce%20Toolkit%20
+00003090: 2d25 3230 332e 2532 3044 6566 696e 696e  -%203.%20Definin
+000030a0: 6725 3230 4375 7374 6f6d 2532 3052 6174  g%20Custom%20Rat
+000030b0: 696f 732e 6970 796e 6229 2073 686f 7773  ios.ipynb) shows
+000030c0: 2074 6865 2066 756c 6c20 6f75 7470 7574   the full output
+000030d0: 2e0a 0a7c 2020 2020 2020 2020 2020 2020  ...|            
+000030e0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+000030f0: 2020 2020 2020 3230 3232 5133 207c 2020        2022Q3 |  
+00003100: 2020 2020 3230 3232 5134 207c 2020 2020      2022Q4 |    
+00003110: 2032 3032 3351 3120 7c20 2020 2020 2032   2023Q1 |      2
+00003120: 3032 3351 3220 7c0a 7c3a 2d2d 2d2d 2d2d  023Q2 |.|:------
+00003130: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003140: 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----|-----------
+00003150: 2d3a 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a  -:|------------:
+00003160: 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 3a7c 2d2d  |-----------:|--
+00003170: 2d2d 2d2d 2d2d 2d2d 2d2d 3a7c 0a7c 2043  ----------:|.| C
+00003180: 7572 7265 6e74 2041 7373 6574 7320 496e  urrent Assets In
+00003190: 7665 6e74 6f72 7920 207c 2031 2e36 3239  ventory  | 1.629
+000031a0: 3533 652b 3131 207c 2031 2e36 3231 3235  53e+11 | 1.62125
+000031b0: 652b 3131 207c 2031 2e35 3936 3765 2b31  e+11 | 1.5967e+1
+000031c0: 3120 7c20 312e 3636 3535 3765 2b31 3120  1 | 1.66557e+11 
+000031d0: 7c0a 7c20 4e65 7420 496e 636f 6d65 202f  |.| Net Income /
+000031e0: 2054 6f74 616c 2041 7373 6574 7320 7c20   Total Assets | 
+000031f0: 302e 3033 3838 3237 3120 2020 7c20 302e  0.0388271   | 0.
+00003200: 3033 3732 3939 2020 2020 7c20 302e 3034  037299    | 0.04
+00003210: 3037 3334 3420 207c 2030 2e30 3437 3935  07344  | 0.04795
+00003220: 3237 2020 207c 0a7c 2051 7569 636b 2052  27   |.| Quick R
+00003230: 6174 696f 2043 7572 7265 6e74 2020 2020  atio Current    
+00003240: 2020 207c 2032 2e34 3639 3737 2020 2020     | 2.46977    
+00003250: 207c 2032 2e33 3339 3437 2020 2020 207c   | 2.33947     |
+00003260: 2032 2e33 3138 3936 2020 2020 7c20 322e   2.31896    | 2.
+00003270: 3134 3333 3420 2020 2020 7c0a 7c20 5175  14334     |.| Qu
+00003280: 6963 6b20 5261 7469 6f20 546f 7461 6c20  ick Ratio Total 
+00003290: 2020 2020 2020 2020 7c20 312e 3535 3734          | 1.5574
+000032a0: 3420 2020 2020 7c20 312e 3438 3537 3520  4     | 1.48575 
+000032b0: 2020 2020 7c20 312e 3437 3033 2020 2020      | 1.4703    
+000032c0: 207c 2031 2e34 3337 3034 2020 2020 207c   | 1.43704     |
+000032d0: 0a7c 2057 4320 2f20 4e65 7420 496e 636f  .| WC / Net Inco
+000032e0: 6d65 2020 2020 2020 2020 2020 207c 2037  me           | 7
+000032f0: 2e31 3938 3432 2020 2020 207c 2037 2e30  .19842     | 7.0
+00003300: 3039 3332 2020 2020 207c 2036 2e31 3837  0932     | 6.187
+00003310: 3720 2020 2020 7c20 342e 3935 3835 3720  7     | 4.95857 
+00003320: 2020 2020 7c0a 0a23 2320 4361 6c6c 696e      |..## Callin
+00003330: 6720 4675 6e63 7469 6f6e 7320 4469 7265  g Functions Dire
+00003340: 6374 6c79 0a0a 4974 2061 6c73 6f20 706f  ctly..It also po
+00003350: 7373 6962 6c65 2074 6f20 6361 6c6c 2061  ssible to call a
+00003360: 6e79 2072 6174 696f 206f 7220 6d6f 6465  ny ratio or mode
+00003370: 6c20 6469 7265 6374 6c79 2061 7320 7368  l directly as sh
+00003380: 6f77 6e20 6265 6c6f 772e 2054 6869 7320  own below. This 
+00003390: 616c 6c6f 7773 2061 6363 6573 7320 746f  allows access to
+000033a0: 2035 302b 2072 6174 696f 7320 7769 7468   50+ ratios with
+000033b0: 2063 7573 746f 6d20 6461 7461 2e20 416c   custom data. Al
+000033c0: 736f 2073 6565 205b 7468 6973 206e 6f74  so see [this not
+000033d0: 6562 6f6f 6b5d 2868 7474 7073 3a2f 2f67  ebook](https://g
+000033e0: 6974 6875 622e 636f 6d2f 4a65 7242 6f75  ithub.com/JerBou
+000033f0: 6d61 2f46 696e 616e 6365 546f 6f6c 6b69  ma/FinanceToolki
+00003400: 742f 626c 6f62 2f6d 6169 6e2f 6578 616d  t/blob/main/exam
+00003410: 706c 6573 2f46 696e 616e 6365 2532 3054  ples/Finance%20T
+00003420: 6f6f 6c6b 6974 2532 302d 2532 3034 2e25  oolkit%20-%204.%
+00003430: 3230 4361 6c6c 696e 6725 3230 4675 6e63  20Calling%20Func
+00003440: 7469 6f6e 7325 3230 4469 7265 6374 6c79  tions%20Directly
+00003450: 2e69 7079 6e62 292e 0a0a 6060 6070 7974  .ipynb)...```pyt
+00003460: 686f 6e0a 696d 706f 7274 2070 616e 6461  hon.import panda
+00003470: 7320 6173 2070 640a 696d 706f 7274 206e  s as pd.import n
+00003480: 756d 7079 2061 7320 6e70 0a0a 6672 6f6d  umpy as np..from
+00003490: 2066 696e 616e 6365 746f 6f6c 6b69 742e   financetoolkit.
+000034a0: 6d6f 6465 6c73 2069 6d70 6f72 7420 6475  models import du
+000034b0: 706f 6e74 0a0a 7965 6172 7320 3d20 5b32  pont..years = [2
+000034c0: 3031 382c 2032 3031 392c 2032 3032 302c  018, 2019, 2020,
+000034d0: 2032 3032 312c 2032 3032 325d 0a0a 6475   2021, 2022]..du
+000034e0: 706f 6e74 2e67 6574 5f64 7570 6f6e 745f  pont.get_dupont_
+000034f0: 616e 616c 7973 6973 280a 2020 2020 6e65  analysis(.    ne
+00003500: 745f 696e 636f 6d65 3d70 642e 5365 7269  t_income=pd.Seri
+00003510: 6573 280a 2020 2020 2020 2020 5b35 3935  es(.        [595
+00003520: 3331 3030 3030 3030 2c20 3535 3235 3630  31000000, 552560
+00003530: 3030 3030 302c 2035 3734 3131 3030 3030  00000, 574110000
+00003540: 3030 2c20 3934 3638 3030 3030 3030 302c  00, 94680000000,
+00003550: 2039 3938 3033 3030 3030 3030 5d2c 2069   99803000000], i
+00003560: 6e64 6578 3d79 6561 7273 0a20 2020 2029  ndex=years.    )
+00003570: 2c0a 2020 2020 746f 7461 6c5f 7265 7665  ,.    total_reve
+00003580: 6e75 653d 7064 2e53 6572 6965 7328 0a20  nue=pd.Series(. 
+00003590: 2020 2020 2020 205b 3236 3535 3935 3030         [26559500
+000035a0: 3030 3030 2c20 3236 3031 3734 3030 3030  0000, 2601740000
+000035b0: 3030 2c20 3237 3435 3135 3030 3030 3030  00, 274515000000
+000035c0: 2c20 3336 3538 3137 3030 3030 3030 2c20  , 365817000000, 
+000035d0: 3339 3433 3238 3030 3030 3030 5d2c 0a20  394328000000],. 
+000035e0: 2020 2020 2020 2069 6e64 6578 3d79 6561         index=yea
+000035f0: 7273 2c0a 2020 2020 292c 0a20 2020 2074  rs,.    ),.    t
+00003600: 6f74 616c 5f61 7373 6574 735f 6265 6769  otal_assets_begi
+00003610: 6e3d 7064 2e53 6572 6965 7328 0a20 2020  n=pd.Series(.   
+00003620: 2020 2020 205b 6e70 2e6e 616e 2c20 3336       [np.nan, 36
+00003630: 3537 3235 3030 3030 3030 2c20 3333 3835  5725000000, 3385
+00003640: 3136 3030 3030 3030 2c20 3332 3338 3838  16000000, 323888
+00003650: 3030 3030 3030 2c20 3335 3130 3032 3030  000000, 35100200
+00003660: 3030 3030 5d2c 0a20 2020 2020 2020 2069  0000],.        i
+00003670: 6e64 6578 3d79 6561 7273 2c0a 2020 2020  ndex=years,.    
+00003680: 292c 0a20 2020 2074 6f74 616c 5f61 7373  ),.    total_ass
+00003690: 6574 735f 656e 643d 7064 2e53 6572 6965  ets_end=pd.Serie
+000036a0: 7328 0a20 2020 2020 2020 205b 3336 3537  s(.        [3657
+000036b0: 3235 3030 3030 3030 2c20 3333 3835 3136  25000000, 338516
+000036c0: 3030 3030 3030 2c20 3332 3338 3838 3030  000000, 32388800
+000036d0: 3030 3030 2c20 3335 3130 3032 3030 3030  0000, 3510020000
+000036e0: 3030 2c20 3335 3237 3535 3030 3030 3030  00, 352755000000
+000036f0: 5d2c 0a20 2020 2020 2020 2069 6e64 6578  ],.        index
+00003700: 3d79 6561 7273 2c0a 2020 2020 292c 0a20  =years,.    ),. 
+00003710: 2020 2074 6f74 616c 5f65 7175 6974 795f     total_equity_
+00003720: 6265 6769 6e3d 7064 2e53 6572 6965 7328  begin=pd.Series(
+00003730: 0a20 2020 2020 2020 205b 6e70 2e6e 616e  .        [np.nan
+00003740: 2c20 3130 3731 3437 3030 3030 3030 2c20  , 107147000000, 
+00003750: 3930 3438 3830 3030 3030 302c 2036 3533  90488000000, 653
+00003760: 3339 3030 3030 3030 2c20 3633 3039 3030  39000000, 630900
+00003770: 3030 3030 305d 2c20 696e 6465 783d 7965  00000], index=ye
+00003780: 6172 730a 2020 2020 292c 0a20 2020 2074  ars.    ),.    t
+00003790: 6f74 616c 5f65 7175 6974 795f 656e 643d  otal_equity_end=
+000037a0: 7064 2e53 6572 6965 7328 0a20 2020 2020  pd.Series(.     
+000037b0: 2020 205b 3130 3731 3437 3030 3030 3030     [107147000000
+000037c0: 2c20 3930 3438 3830 3030 3030 302c 2036  , 90488000000, 6
+000037d0: 3533 3339 3030 3030 3030 2c20 3633 3039  5339000000, 6309
+000037e0: 3030 3030 3030 302c 2035 3036 3732 3030  0000000, 5067200
+000037f0: 3030 3030 5d2c 2069 6e64 6578 3d79 6561  0000], index=yea
+00003800: 7273 0a20 2020 2029 2c0a 290a 6060 600a  rs.    ),.).```.
+00003810: 0a54 6869 7320 7265 7475 726e 7320 7468  .This returns th
+00003820: 6520 666f 6c6c 6f77 696e 6720 7461 626c  e following tabl
+00003830: 6520 7768 6963 6820 636c 6f73 656c 7920  e which closely 
+00003840: 7265 7365 6d62 6c65 7320 6120 7072 6f70  resembles a prop
+00003850: 6572 2044 7570 6f6e 7420 616e 616c 7973  er Dupont analys
+00003860: 6973 2066 6f72 2041 7070 6c65 2061 7420  is for Apple at 
+00003870: 7468 6569 7220 6769 7665 6e20 7265 706f  their given repo
+00003880: 7274 696e 6720 6461 7465 7320 696e 204f  rting dates in O
+00003890: 6374 6f62 6572 3a0a 0a7c 2020 2020 2020  ctober:..|      
+000038a0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+000038b0: 2020 2020 2032 3031 3820 7c20 2020 2020       2018 |     
+000038c0: 3230 3139 207c 2020 2020 2032 3032 3020  2019 |     2020 
+000038d0: 7c20 2020 2020 3230 3231 207c 2020 2020  |     2021 |    
+000038e0: 2032 3032 3220 7c0a 7c3a 2d2d 2d2d 2d2d   2022 |.|:------
+000038f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d  ------------|---
+00003900: 2d2d 2d2d 2d2d 2d2d 3a7c 2d2d 2d2d 2d2d  --------:|------
+00003910: 2d2d 2d3a 7c2d 2d2d 2d2d 2d2d 2d2d 3a7c  ---:|---------:|
+00003920: 2d2d 2d2d 2d2d 2d2d 2d3a 7c2d 2d2d 2d2d  ---------:|-----
+00003930: 2d2d 2d2d 3a7c 0a7c 204e 6574 2050 726f  ----:|.| Net Pro
+00003940: 6669 7420 4d61 7267 696e 207c 2020 2030  fit Margin |   0
+00003950: 2e32 3234 3134 3220 7c20 302e 3231 3233  .224142 | 0.2123
+00003960: 3831 207c 2030 2e32 3039 3133 3620 7c20  81 | 0.209136 | 
+00003970: 302e 3235 3838 3138 207c 2030 2e32 3533  0.258818 | 0.253
+00003980: 3039 3620 7c0a 7c20 4173 7365 7420 5475  096 |.| Asset Tu
+00003990: 726e 6f76 6572 2020 2020 7c20 6e61 6e20  rnover    | nan 
+000039a0: 2020 2020 2020 207c 2030 2e37 3338 3837         | 0.73887
+000039b0: 3820 7c20 302e 3832 3838 3435 207c 2031  8 | 0.828845 | 1
+000039c0: 2e30 3834 3038 2020 7c20 312e 3132 3036  .08408  | 1.1206
+000039d0: 3420 207c 0a7c 2045 7175 6974 7920 4d75  4  |.| Equity Mu
+000039e0: 6c74 6970 6c69 6572 207c 206e 616e 2020  ltiplier | nan  
+000039f0: 2020 2020 2020 7c20 332e 3536 3333 3420        | 3.56334 
+00003a00: 207c 2034 2e32 3530 3839 2020 7c20 352e   | 4.25089  | 5.
+00003a10: 3235 3439 3720 207c 2036 2e31 3836 3232  25497  | 6.18622
+00003a20: 2020 7c0a 7c20 5265 7475 726e 206f 6e20    |.| Return on 
+00003a30: 4571 7569 7479 2020 7c20 6e61 6e20 2020  Equity  | nan   
+00003a40: 2020 2020 207c 2030 2e35 3539 3137 3220       | 0.559172 
+00003a50: 7c20 302e 3733 3638 3536 207c 2031 2e34  | 0.736856 | 1.4
+00003a60: 3734 3433 2020 7c20 312e 3735 3435 3920  7443  | 1.75459 
+00003a70: 207c 0a0a 2323 2057 6f72 6b69 6e67 2077   |..## Working w
+00003a80: 6974 6820 6f74 6865 7220 4461 7461 7365  ith other Datase
+00003a90: 7473 0a0a 5468 6520 4669 6e61 6e63 6520  ts..The Finance 
+00003aa0: 546f 6f6c 6b69 7420 6861 7320 7468 6520  Toolkit has the 
+00003ab0: 6162 696c 6974 7920 746f 206c 6576 6572  ability to lever
+00003ac0: 6167 6520 6375 7374 6f6d 2064 6174 6173  age custom datas
+00003ad0: 6574 7320 6672 6f6d 2061 6e79 2064 6174  ets from any dat
+00003ae0: 6120 7072 6f76 6964 6572 2061 7320 7765  a provider as we
+00003af0: 6c6c 2e20 5468 6973 206d 616b 6573 2069  ll. This makes i
+00003b00: 7420 706f 7373 6962 6c65 2074 6f20 776f  t possible to wo
+00003b10: 726b 2077 6974 6820 796f 7572 2070 7265  rk with your pre
+00003b20: 6665 7272 6564 2064 6174 6120 616e 6420  ferred data and 
+00003b30: 6e6f 7420 6265 206c 696d 6974 6564 2074  not be limited t
+00003b40: 6f20 7468 6520 6461 7461 2073 6f75 7263  o the data sourc
+00003b50: 6520 7468 6520 4669 6e61 6e63 6520 546f  e the Finance To
+00003b60: 6f6c 6b69 7420 6375 7272 656e 746c 7920  olkit currently 
+00003b70: 7072 6f76 6964 6573 2e20 4120 6465 7461  provides. A deta
+00003b80: 696c 6564 2065 7861 6d70 6c65 2063 616e  iled example can
+00003b90: 2062 6520 666f 756e 6420 5b68 6572 655d   be found [here]
+00003ba0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00003bb0: 636f 6d2f 4a65 7242 6f75 6d61 2f46 696e  com/JerBouma/Fin
+00003bc0: 616e 6365 546f 6f6c 6b69 742f 626c 6f62  anceToolkit/blob
+00003bd0: 2f6d 6169 6e2f 6578 616d 706c 6573 2f46  /main/examples/F
+00003be0: 696e 616e 6365 2532 3054 6f6f 6c6b 6974  inance%20Toolkit
+00003bf0: 2532 302d 2532 3035 2e25 3230 5573 696e  %20-%205.%20Usin
+00003c00: 6725 3230 4578 7465 726e 616c 2532 3044  g%20External%20D
+00003c10: 6174 6173 6574 732e 6970 796e 6229 2062  atasets.ipynb) b
+00003c20: 7574 2074 6f20 6765 7420 7374 6172 7465  ut to get starte
+00003c30: 6420 7365 6520 7468 6520 636f 6465 2062  d see the code b
+00003c40: 656c 6f77 2e0a 0a60 6060 7079 7468 6f6e  elow...```python
+00003c50: 0a66 726f 6d20 6669 6e61 6e63 6574 6f6f  .from financetoo
+00003c60: 6c6b 6974 2069 6d70 6f72 7420 546f 6f6c  lkit import Tool
+00003c70: 6b69 740a 0a23 2049 6e69 7469 616c 697a  kit..# Initializ
+00003c80: 6520 7468 6520 4669 6e61 6e63 6520 546f  e the Finance To
+00003c90: 6f6c 6b69 740a 636f 6d70 616e 6965 7320  olkit.companies 
+00003ca0: 3d20 546f 6f6c 6b69 7428 5b27 4141 504c  = Toolkit(['AAPL
+00003cb0: 272c 2027 4d53 4654 275d 290a 0a23 2043  ', 'MSFT'])..# C
+00003cc0: 6f70 7920 7468 6520 6e6f 726d 616c 697a  opy the normaliz
+00003cd0: 6174 696f 6e20 6669 6c65 730a 636f 6d70  ation files.comp
+00003ce0: 616e 6965 732e 6765 745f 6e6f 726d 616c  anies.get_normal
+00003cf0: 697a 6174 696f 6e5f 6669 6c65 7328 290a  ization_files().
+00003d00: 6060 600a 5468 6973 2063 6f70 6965 7320  ```.This copies 
+00003d10: 6f76 6572 2074 6872 6565 2066 696c 6573  over three files
+00003d20: 2c20 6062 616c 616e 6365 2e63 7376 602c  , `balance.csv`,
+00003d30: 2060 696e 636f 6d65 2e63 7376 6020 616e   `income.csv` an
+00003d40: 6420 6063 6173 682e 6373 7660 2077 6869  d `cash.csv` whi
+00003d50: 6368 2077 696c 6c20 636f 6e74 6169 6e20  ch will contain 
+00003d60: 6120 7374 7275 6374 7572 6520 6c69 6b65  a structure like
+00003d70: 2074 6865 2066 6f6c 6c6f 7769 6e67 3a0a   the following:.
+00003d80: 0a21 5b4e 6f72 6d61 6c69 7a61 7469 6f6e  .![Normalization
+00003d90: 2046 6f72 6d61 745d 2868 7474 7073 3a2f   Format](https:/
+00003da0: 2f67 6974 6875 622e 636f 6d2f 4a65 7242  /github.com/JerB
+00003db0: 6f75 6d61 2f46 696e 616e 6365 546f 6f6c  ouma/FinanceTool
+00003dc0: 6b69 742f 6173 7365 7473 2f34 3633 3535  kit/assets/46355
+00003dd0: 3336 342f 6561 3465 6266 3837 2d31 6132  364/ea4ebf87-1a2
+00003de0: 372d 3463 3430 2d61 3166 622d 3430 6430  7-4c40-a1fb-40d0
+00003df0: 6562 3036 3334 6263 290a 0a42 7920 7265  eb0634bc)..By re
+00003e00: 706c 6163 696e 6720 7468 6520 6669 7273  placing the firs
+00003e10: 7420 636f 6c75 6d6e 2077 6974 6820 7468  t column with th
+00003e20: 6520 6e61 6d65 7320 6672 6f6d 2079 6f75  e names from you
+00003e30: 7220 6461 7461 7365 7420 2865 2e67 2e20  r dataset (e.g. 
+00003e40: 7265 706c 6163 6520 6063 6173 6841 6e64  replace `cashAnd
+00003e50: 4361 7368 4571 7569 7661 6c65 6e74 7360  CashEquivalents`
+00003e60: 2077 6974 6820 6043 6173 6860 2069 6620   with `Cash` if 
+00003e70: 7468 6973 2069 7320 686f 7720 6974 2069  this is how it i
+00003e80: 7320 6361 6c6c 6564 2069 6e20 796f 7572  s called in your
+00003e90: 2064 6174 6173 6574 292c 2069 7420 7769   dataset), it wi
+00003ea0: 6c6c 2061 7574 6f6d 6174 6963 616c 6c79  ll automatically
+00003eb0: 206e 6f72 6d61 6c69 7a65 2074 6865 2064   normalize the d
+00003ec0: 6174 6173 6574 2077 6865 6e20 796f 7520  ataset when you 
+00003ed0: 696e 6974 6961 6c69 7a65 2074 6865 2046  initialize the F
+00003ee0: 696e 616e 6365 2054 6f6f 6c6b 6974 2e20  inance Toolkit. 
+00003ef0: 4e6f 7465 2074 6861 7420 7468 6520 4461  Note that the Da
+00003f00: 7461 4672 616d 6520 6e65 6564 7320 746f  taFrame needs to
+00003f10: 2062 6520 6120 6d75 6c74 692d 696e 6465   be a multi-inde
+00003f20: 7820 696e 2063 6173 6520 796f 7520 7573  x in case you us
+00003f30: 6520 6d75 6c74 6970 6c65 2074 6963 6b65  e multiple ticke
+00003f40: 7273 2073 7472 7563 7475 7265 6420 6173  rs structured as
+00003f50: 2060 5469 636b 6572 2078 2046 696e 616e   `Ticker x Finan
+00003f60: 6369 616c 2053 7461 7465 6d65 6e74 2049  cial Statement I
+00003f70: 7465 6d20 7820 5065 7269 6f64 7360 2e0a  tem x Periods`..
+00003f80: 0a41 7320 616e 2065 7861 6d70 6c65 3a0a  .As an example:.
+00003f90: 0a21 5b44 6174 6173 6574 2045 7861 6d70  .![Dataset Examp
+00003fa0: 6c65 5d28 6874 7470 733a 2f2f 6769 7468  le](https://gith
+00003fb0: 7562 2e63 6f6d 2f4a 6572 426f 756d 612f  ub.com/JerBouma/
+00003fc0: 4669 6e61 6e63 6554 6f6f 6c6b 6974 2f61  FinanceToolkit/a
+00003fd0: 7373 6574 732f 3436 3335 3533 3634 2f66  ssets/46355364/f
+00003fe0: 6530 6533 6462 302d 3365 3838 2d34 3164  e0e3db0-3e88-41d
+00003ff0: 322d 6133 3535 2d35 6636 3831 3130 6664  2-a355-5f68110fd
+00004000: 6366 3329 0a0a 4966 2079 6f75 2068 6176  cf3)..If you hav
+00004010: 6520 696e 6469 7669 6475 616c 2044 6174  e individual Dat
+00004020: 6146 7261 6d65 7320 666f 7220 6561 6368  aFrames for each
+00004030: 2063 6f6d 7061 6e79 2c20 796f 7520 6361   company, you ca
+00004040: 6e20 646f 2074 6865 2066 6f6c 6c6f 7769  n do the followi
+00004050: 6e67 2077 6869 6368 2077 696c 6c20 7265  ng which will re
+00004060: 7475 726e 2074 6865 2044 6174 6146 7261  turn the DataFra
+00004070: 6d65 2073 7472 7563 7475 7265 2074 6861  me structure tha
+00004080: 7420 6973 2072 6571 7569 7265 643a 0a0a  t is required:..
+00004090: 6060 6070 7974 686f 6e0a 6672 6f6d 2066  ```python.from f
+000040a0: 696e 616e 6365 746f 6f6c 6b69 742e 6261  inancetoolkit.ba
+000040b0: 7365 2069 6d70 6f72 7420 6865 6c70 6572  se import helper
+000040c0: 730a 0a62 616c 616e 6365 5f67 726f 7570  s..balance_group
+000040d0: 6564 203d 2068 656c 7065 7273 2e63 6f6d  ed = helpers.com
+000040e0: 6269 6e65 5f64 6174 6166 7261 6d65 7328  bine_dataframes(
+000040f0: 7b27 4141 504c 273a 2062 616c 616e 6365  {'AAPL': balance
+00004100: 5f61 7070 6c65 2c20 274d 5346 5427 3a20  _apple, 'MSFT': 
+00004110: 6261 6c61 6e63 655f 6d73 6674 7d29 0a60  balance_msft}).`
+00004120: 6060 0a0a 4f6e 6365 2061 6c6c 206f 6620  ``..Once all of 
+00004130: 7468 6973 2069 7320 7365 742d 7570 2079  this is set-up y
+00004140: 6f75 2063 616e 2066 6565 6420 7468 6973  ou can feed this
+00004150: 2069 6e66 6f72 6d61 7469 6f6e 2074 6f20   information to 
+00004160: 7468 6520 546f 6f6c 6b69 7420 616e 6420  the Toolkit and 
+00004170: 7573 6520 7468 6520 546f 6f6c 6b69 7420  use the Toolkit 
+00004180: 6173 206e 6f72 6d61 6c6c 792e 0a0a 6060  as normally...``
+00004190: 6070 7974 686f 6e0a 0a23 2049 6e69 7469  `python..# Initi
+000041a0: 616c 697a 6520 7468 6520 546f 6f6c 6b69  alize the Toolki
+000041b0: 740a 636f 6d70 616e 6965 7320 3d20 546f  t.companies = To
+000041c0: 6f6c 6b69 7428 0a20 2020 2074 6963 6b65  olkit(.    ticke
+000041d0: 7273 3d5b 2741 4150 4c27 2c20 274d 5346  rs=['AAPL', 'MSF
+000041e0: 5427 5d2c 0a20 2020 2062 616c 616e 6365  T'],.    balance
+000041f0: 3d62 616c 616e 6365 5f67 726f 7570 6564  =balance_grouped
+00004200: 2c0a 2020 2020 696e 636f 6d65 3d69 6e63  ,.    income=inc
+00004210: 6f6d 655f 6772 6f75 7065 642c 0a20 2020  ome_grouped,.   
+00004220: 2063 6173 683d 6361 7368 5f67 726f 7570   cash=cash_group
+00004230: 6564 2c0a 2020 2020 666f 726d 6174 5f6c  ed,.    format_l
+00004240: 6f63 6174 696f 6e3d 2246 4f4c 4445 525f  ocation="FOLDER_
+00004250: 5041 5448 222c 0a20 2020 2072 6576 6572  PATH",.    rever
+00004260: 7365 5f64 6174 6573 3d46 616c 7365 2920  se_dates=False) 
+00004270: 2320 5075 7420 7468 6973 2074 6f20 5472  # Put this to Tr
+00004280: 7565 2069 6e20 6361 7365 2064 6174 6573  ue in case dates
+00004290: 2061 7265 2064 6573 6365 6e64 696e 670a   are descending.
+000042a0: 0a23 2052 6574 7572 6e20 616c 6c20 5261  .# Return all Ra
+000042b0: 7469 6f73 0a63 6f6d 7061 6e69 6573 2e72  tios.companies.r
+000042c0: 6174 696f 732e 636f 6c6c 6563 745f 616c  atios.collect_al
+000042d0: 6c5f 7261 7469 6f73 2829 0a60 6060 0a0a  l_ratios().```..
+000042e0: 5468 6973 2077 696c 6c20 7265 7475 726e  This will return
+000042f0: 2061 6c6c 2066 696e 616e 6369 616c 2072   all financial r
+00004300: 6174 696f 7320 7468 6174 2063 616e 2062  atios that can b
+00004310: 6520 636f 6c6c 6563 7465 6420 6261 7365  e collected base
+00004320: 6420 6f6e 2074 6865 2070 726f 7669 6465  d on the provide
+00004330: 6420 6461 7461 2061 6e64 2074 6865 2066  d data and the f
+00004340: 6f72 6d61 742e 0a0a 215b 4f75 7470 7574  ormat...![Output
+00004350: 206f 6620 5265 7375 6c74 5d28 6874 7470   of Result](http
+00004360: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4a  s://github.com/J
+00004370: 6572 426f 756d 612f 4669 6e61 6e63 6554  erBouma/FinanceT
+00004380: 6f6f 6c6b 6974 2f61 7373 6574 732f 3436  oolkit/assets/46
+00004390: 3335 3533 3634 2f32 6139 3935 3433 302d  355364/2a995430-
+000043a0: 6238 6438 2d34 3233 362d 3839 3263 2d65  b8d8-4236-892c-e
+000043b0: 6462 3437 3034 3264 3661 6629 0a0a 2320  db47042d6af)..# 
+000043c0: 436f 6e74 6163 740a 4966 2079 6f75 2068  Contact.If you h
+000043d0: 6176 6520 616e 7920 7175 6573 7469 6f6e  ave any question
+000043e0: 7320 6162 6f75 7420 7468 6520 4669 6e61  s about the Fina
+000043f0: 6e63 6554 6f6f 6c6b 6974 206f 7220 776f  nceToolkit or wo
+00004400: 756c 6420 6c69 6b65 2074 6f20 7368 6172  uld like to shar
+00004410: 6520 7769 7468 206d 6520 7768 6174 2079  e with me what y
+00004420: 6f75 2068 6176 6520 6265 656e 2077 6f72  ou have been wor
+00004430: 6b69 6e67 206f 6e2c 2066 6565 6c20 6672  king on, feel fr
+00004440: 6565 2074 6f20 7265 6163 6820 6f75 7420  ee to reach out 
+00004450: 746f 206d 6520 7669 613a 0a0a 2d20 2a2a  to me via:..- **
+00004460: 4c69 6e6b 6564 496e 3a2a 2a20 6874 7470  LinkedIn:** http
+00004470: 733a 2f2f 7777 772e 6c69 6e6b 6564 696e  s://www.linkedin
+00004480: 2e63 6f6d 2f69 6e2f 626f 756d 616a 6572  .com/in/boumajer
+00004490: 6f65 6e2f 0a2d 2020 2a2a 456d 6169 6c3a  oen/.-  **Email:
+000044a0: 2a2a 206a 6572 2e62 6f75 6d61 4067 6d61  ** jer.bouma@gma
+000044b0: 696c 2e63 6f6d 0a0a 4966 2079 6f75 2764  il.com..If you'd
+000044c0: 206c 696b 6520 746f 2073 7570 706f 7274   like to support
+000044d0: 206d 7920 6566 666f 7274 732c 2065 6974   my efforts, eit
+000044e0: 6865 7220 6865 6c70 206d 6520 6f75 7420  her help me out 
+000044f0: 6279 2063 6f6e 7472 6962 7574 696e 6720  by contributing 
+00004500: 746f 2074 6865 2070 6163 6b61 6765 206f  to the package o
+00004510: 7220 5b42 7579 206d 6520 6120 436f 6666  r [Buy me a Coff
+00004520: 6565 5d28 6874 7470 733a 2f2f 7777 772e  ee](https://www.
+00004530: 6275 796d 6561 636f 6666 6565 2e63 6f6d  buymeacoffee.com
+00004540: 2f6a 6572 626f 756d 6129 2e0a 0a5b 215b  /jerbouma)...[![
+00004550: 5374 6172 2048 6973 746f 7279 2043 6861  Star History Cha
+00004560: 7274 5d28 6874 7470 733a 2f2f 6170 692e  rt](https://api.
+00004570: 7374 6172 2d68 6973 746f 7279 2e63 6f6d  star-history.com
+00004580: 2f73 7667 3f72 6570 6f73 3d4a 6572 426f  /svg?repos=JerBo
+00004590: 756d 612f 4669 6e61 6e63 6554 6f6f 6c6b  uma/FinanceToolk
+000045a0: 6974 2674 7970 653d 4461 7465 295d 2868  it&type=Date)](h
+000045b0: 7474 7073 3a2f 2f73 7461 722d 6869 7374  ttps://star-hist
+000045c0: 6f72 792e 636f 6d2f 234a 6572 426f 756d  ory.com/#JerBoum
+000045d0: 612f 4669 6e61 6e63 6554 6f6f 6c6b 6974  a/FinanceToolkit
+000045e0: 2644 6174 6529 0a                        &Date).
```

### Comparing `financetoolkit-1.1.2/PKG-INFO` & `financetoolkit-1.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: financetoolkit
-Version: 1.1.2
+Version: 1.2.0
 Summary: Transparent and Efficient Financial Analysis
 Home-page: https://www.jeroenbouma.com/
 License: MIT
 Author: Jeroen Bouma
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Financial and Insurance Industry
@@ -12,46 +12,49 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://github.com/JerBouma/FinanceToolkit
 Description-Content-Type: text/markdown
 
 ![FinanceToolkitCropped](https://github.com/JerBouma/FinanceToolkit/assets/46355364/198d47bd-e1b3-492d-acc4-5d9f02d1d009)
 
 [![BuyMeACoffee](https://img.shields.io/badge/Buy%20Me%20A%20Coffee-Donate-brightgreen?logo=buymeacoffee)](https://www.buymeacoffee.com/jerbouma)
-[![Website](https://img.shields.io/badge/Website-Learn%20more%20about%20me%20here-brightgreen?logo=ReadMe)](https://jeroenbouma.com/)
+[![Website](https://img.shields.io/badge/Read_More-website?logo=readme&label=Website)](https://jeroenbouma.com/)
+[![Discord](https://img.shields.io/badge/Chat-hello?logo=discord&label=Discord)](https://discordapp.com/users/547886981468782613)
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/financetoolkit)](https://pypi.org/project/FinanceToolkit/)
 [![PYPI Version](https://img.shields.io/pypi/v/FinanceToolkit)](https://pypi.org/project/FinanceToolkit/)
 [![PYPI Downloads](https://img.shields.io/pypi/dm/FinanceToolkit)](https://pypi.org/project/FinanceToolkit/)
 
 While browsing a variety of websites, I kept finding that the same financial metric can greatly vary per source and so do the financial statements reported while little information is given how the metric was calculated.
 
 For example, Microsoft's Price-to-Earnings (PE) ratio on the 6th of May, 2023 is reported to be 28.93 (Stockopedia), 32.05 (Morningstar), 32.66 (Macrotrends), 33.09 (Finance Charts), 33.66 (Y Charts), 33.67 (Wall Street Journal), 33.80 (Yahoo Finance) and 34.4 (Companies Market Cap). All of these calculations are correct, however the method applied varies leading to different results. Therefore, collecting data from multiple sources can lead to wrong interpretation of the results given that one source could be applying a different calculation method than another. And that is, if it is even freely available. Often the calculation is hidden behind a paid subscription.
 
 **This is why I designed the FinanceToolkit**, this is an open-source toolkit in which all relevant financial ratios (50+), indicators and performance measurements are written down in the most simplistic way allowing for complete transparency of the calculation method. This allows you to not have to rely on metrics from other providers and, given a financial statement, allow for efficient manual calculations. This leads to one uniform method of calculation being applied that is available and understood by everyone.
 
 The Finance Toolkit is complimented very well with the [Finance Database 🌎](https://github.com/JerBouma/FinanceDatabase), a database that features 300.000+ symbols containing Equities, ETFs, Funds, Indices, Currencies, Cryptocurrencies and Money Markets. By utilising both, it is possible to do a fully-fledged competitive analysis with the tickers found from the FinanceDatabase inputted into the FinanceToolkit.
 
 <p align="center">
-    <img src="examples/Finance Toolkit - 5. Video Demo.gif" alt="Finance Toolkit Illustration" width="100%" onerror='this.style.display = "none"'/>
+    <img src="examples/Finance Toolkit - 6. Video Demo.gif" alt="Finance Toolkit Illustration" width="100%" onerror="this.style.display = 'none'"/>
 </p>
 
 ---
 
 # Table of Contents
 
 1. [Installation](#installation)
 2. [Basic Usage](#basic-usage)
     1. [Using the Finance Toolkit](#using-the-finance-toolkit)
-    2. [Working with other Datasets](#working-with-other-datasets)
+    2. [Defining Custom Ratios](#defining-custom-ratios)
     3. [Calling Functions Directly](#calling-functions-directly)
+    4. [Working with other Datasets](#working-with-other-datasets)
 3. [Contact](#contact)
 
 # Installation
 
 To install the FinanceToolkit it simply requires the following:
 
 ```
@@ -59,23 +62,22 @@
 ````
 
 Then within Python use:
 
 ```python
 from financetoolkit import Toolkit
 ```
-To be able to get started, you need to obtain an API Key from FinancialModelingPrep. Use the following instructions to obtain a _free_ API Key. Note that these keys are limited to 250 requests per day but the premium plans are kept at a low cost in case you do run out of the limit or have a need for access to more data. **It is possible to use your own set of financial statements and not rely on FinancialModelingPrep, please have a look [here](#working-with-other-datasets).**
+To be able to get started, you need to obtain an API Key from FinancialModelingPrep. This is used to gain access to 30+ years of financial statement both annually and quarterly. Note that the Free plan is limited to 250 requests each day, 5 years of data and only features companies listed on US exchanges.
 
-1. Go to [FinancialModellingPrep's API](https://financialmodelingprep.com/developer/docs/)
-2. Under "Get your Free API Key Today!" click on "Get my API KEY here"
-3. Sign-up to the website and select the Free Plan
-4. Obtain the API Key as found [here](https://financialmodelingprep.com/developer/docs/)
-5. Start using this package.
+___ 
+
+<b><div align="center">Obtain an API Key from FinancialModelingPrep <a href="https://site.financialmodelingprep.com/developer/docs/pricing/jeroen/">here</a>.</div></b>
+___
 
-Note that I am in no way affiliated FinancialModelingprep and never will be. I have chosen their source as I find it to be the most transparent and reliable. When you notice that data is inaccurate or have any other issue related to the data, note that I simply provide the means to access this data and I am not responsible for the accuracy of the data itself. For this, use [their contact form](https://site.financialmodelingprep.com/contact) or provide the data yourself. 
+Through the link you are able to subscribe for the free plan and also premium plans at a *15% discount*. This is an affiliate link and thus supports the project at the same time. I have chosen FinancialModelingPrep as a source as I find it to be the most transparent, reliable and at an affordable price. When you notice that data is inaccurate or have any other issue related to the data, note that I simply provide the means to access this data and I am not responsible for the accuracy of the data itself. For this, use [their contact form](https://site.financialmodelingprep.com/contact) or provide the data yourself. 
 
 # Basic Usage
 
 This section explains in detail how the Finance Toolkit can utilitised effectively. Also see the Jupyter Notebook in which you can run the examples also demonstrated here.
 
 ___ 
 
@@ -85,34 +87,34 @@
 Within this package the following things are included:
 
 - Company profiles (`profile`), including country, sector, ISIN and general characteristics (from FinancialModelingPrep)
 - Company quotes (`quote`), including 52 week highs and lows, volume metrics and current shares outstanding (from FinancialModelingPrep)
 - Market cap and enterprise values (`enterprise`), including every intermediate step (from FinancialModelingPrep)
 - Company ratings (`rating`), based on key indicators like PE and DE ratios (from FinancialModelingPrep)
 - Historical market data (`historical_data`), which can be retrieved on a daily, weekly, monthly and yearly basis (from Yahoo Finance)
-- Balance Sheet Statements (`balance_sheet_statement`), Income Statements (`income_statement`) and Cash Flow Statements (`cash_flow_statement`), obtainable from FinancialModelingPrep or the source of your choosing through custom input. These functions are accompanied with a normalization function so that for any source, the same ratio analysis can be performed. Please see this Jupyter Notebook that explains how to use a custom source.
-- Efficiency ratios (`efficiency_ratios`), liquidity ratios (`liquidity_ratios`), profitability ratios (`profitability_ratios`), solvency ratios (`solvency_ratios`) and valuation ratios (`valuation_ratios`) functionality that automatically calculates the most important ratios based on the inputted balance sheet, income and cash flow statements.
+- Balance Sheet Statements (`balance_sheet_statement`), Income Statements (`income_statement`), Cash Flow Statements (`cash_flow_statement`) and Statistics Statement (`statistics_statement`), obtainable from FinancialModelingPrep or the source of your choosing through custom input. These functions are accompanied with a normalization function so that for any source, the same ratio analysis can be performed. Please see this Jupyter Notebook that explains how to use a custom source.
+- Efficiency ratios (`efficiency_ratios`), liquidity ratios (`liquidity_ratios`), profitability ratios (`profitability_ratios`), solvency ratios (`solvency_ratios`) and valuation ratios (`valuation_ratios`) functionality that automatically calculates the most important ratios based on the inputted balance sheet, income and cash flow statements. Next to that, it is also possible to input your own custom ratios (`custom_ratios`).
 - Models (`models`) like DUPONT analysis that can be used to perform in-depth financial analysis through a single function.
 
-The dependencies of the package are on purpose *very slim* so that it will work well with any combination of packages and not result in conflicts. I've also been careful with my selection in which I leave out functionality like technical analysis in which [ta-lib](https://ta-lib.org/) does an excellent job as well as portfolio attribution and optimisation in which [Riskfolio-lib](https://riskfolio-lib.readthedocs.io/en/latest/index.html) shines and lastly allow for any source to be incorporated to allow for the incorporation of data sources from [OpenBB](https://openbb.co/).
+The dependencies of the package are on purpose *very slim* so that it will work well with any combination of packages and not result in conflicts. I've also been careful with my selection in which I leave out functionality like technical analysis in which [ta-lib](https://ta-lib.org/) does an excellent job as well as portfolio attribution and optimisation in which [Riskfolio-lib](https://riskfolio-lib.readthedocs.io/en/latest/index.html) shines.
 
 ## Using the Finance Toolkit
 
 A basic example of how to initialise the Finance Toolkit is shown below, also see [this notebook](https://github.com/JerBouma/FinanceToolkit/blob/main/examples/Finance%20Toolkit%20-%201.%20Getting%20Started.ipynb) for a detailed Getting Started guide as well as [this notebook](https://github.com/JerBouma/FinanceToolkit/blob/main/examples/Finance%20Toolkit%20-%202.%20Combining%20the%20Finance%20Toolkit%20with%20the%20Finance%20Database.ipynb) that includes the [Finance Database 🌎](https://github.com/JerBouma/FinanceDatabase) and a proper financial analysis.
 
 ````python
 from financetoolkit import Toolkit
 
-companies = Toolkit(['AAPL', 'MSFT'], api_key="FMP_KEY")
+companies = Toolkit(['AAPL', 'MSFT'], api_key="FMP_KEY", start_date='2017-12-31')
 
 # an Enterprise example
 enterprise = companies.get_enterprise()
 
 # a Historical example
-historical_data = companies.get_historical_data(start='2000-01-01', end='2020-01-01')
+historical_data = companies.get_historical_data()
 
 # a Financial Statement example
 balance_sheet_statement = companies.get_balance_sheet_statement()
 
 # a Ratios example
 profitability_ratios = companies.ratios.collect_profitability_ratios()
 
@@ -138,65 +140,53 @@
 | Return on Tangible Assets                   | 0.555601 | 0.610645 | 0.878664 | 1.50071  | 1.96959  |
 | Income Quality Ratio                        | 1.30073  | 1.25581  | 1.4052   | 1.09884  | 1.22392  |
 | Net Income per EBT                          | 0.816578 | 0.840562 | 0.855718 | 0.866977 | 0.837955 |
 | Free Cash Flow to Operating Cash Flow Ratio | 0.828073 | 0.848756 | 0.909401 | 0.893452 | 0.912338 |
 | EBT to EBIT Ratio                           | 0.957448 | 0.948408 | 0.958936 | 0.976353 | 0.975982 |
 | EBIT to Revenue                             | 0.286688 | 0.26641  | 0.254864 | 0.305759 | 0.309473 |
 
-## Working with other Datasets
-
-The Finance Toolkit shines in its ability to leverage custom datasets from any data provider as well. This makes it possible to work with your preferred data and not be limited to the data source the Finance Toolkit currently provides. A detailed example can be found [here](https://github.com/JerBouma/FinanceToolkit/blob/main/examples/Finance%20Toolkit%20-%203.%20Using%20External%20Datasets%20(OpenBB).ipynb) but to get started see the code below.
-
-```python
-from financetoolkit import Toolkit
-
-# Initialize the Finance Toolkit
-companies = Toolkit(['AAPL', 'MSFT'])
-
-# Copy the normalization files
-companies.get_normalization_files()
-```
-This copies over three files, `balance.csv`, `income.csv` and `cash.csv` which will contain a structure like the following:
-
-![Normalization Format](https://github.com/JerBouma/FinanceToolkit/assets/46355364/ea4ebf87-1a27-4c40-a1fb-40d0eb0634bc)
+## Defining Custom Ratios
 
-By replacing the first column with the names from your dataset (e.g. replace `cashAndCashEquivalents` with `Cash` if this is how it is called in your dataset), it will automatically normalize the dataset when you initialize the Finance Toolkit. Note that the DataFrame needs to be a multi-index in case you use multiple tickers structured as `Ticker x Financial Statement Item x Periods`.
-
-As an example:
+The Finance Toolkit has an abundance of financial ratios, however it could be that you are looking for a specific ratio that is currently not provided. First and foremost, I encourage to [create a Pull Request](https://github.com/JerBouma/FinanceToolkit/pulls) to add these ratios in but there is also an option to add custom ratios as follows. This feature was designed by [sword134](https://github.com/sword134). Find a Notebook example [here](https://github.com/JerBouma/FinanceToolkit/blob/main/examples/Finance%20Toolkit%20-%203.%20Defining%20Custom%20Ratios.ipynb).
 
-![Dataset Example](https://github.com/JerBouma/FinanceToolkit/assets/46355364/fe0e3db0-3e88-41d2-a355-5f68110fdcf3)
-
-If you have individual DataFrames for each company, you can do the following which will return the DataFrame structure that is required:
+Define how each custom ratio needs to be calculated. This follows the structure `Name of Ratio`: `Financial Statement Item * Financial Statement Item`. Note that you adhere to the normalization files naming. This can be viewed relatively easy by initializing the Toolkit and running for example `get_balance_sheet_statement`.
 
 ```python
-from financetoolkit.base import helpers
-
-balance_grouped = helpers.combine_dataframes({'AAPL': balance_apple, 'MSFT': balance_msft})
+custom_ratios = {
+    'WC / Net Income': 'Working Capital / Net Income',
+    'Net Income / Total Assets': 'Net Income / Total Assets',
+    'Current Assets Inventory': 'Total Current Assets - Inventory',
+    'Quick Ratio Current': 'Current Assets Inventory / Total Current Liabilities',
+    'Quick Ratio Total': 'Current Assets Inventory / Total Liabilities'
+}
 ```
 
-Once all of this is set-up you can feed this information to the Toolkit and use the Toolkit as normally.
+Initializing the Finance Toolkit. Make sure to set the parameter `custom_ratios` with the above dictionary. Note that `quarterly=True` doesn't work without a Premium plan.
 
 ```python
+from financetoolkit import Toolkit
 
-# Initialize the Toolkit
+# Initialize the Finance Toolkit
 companies = Toolkit(
-    tickers=['AAPL', 'MSFT'],
-    balance=balance_grouped,
-    income=income_grouped,
-    cash=cash_grouped,
-    format_location="FOLDER_PATH",
-    reverse_dates=False) # Put this to True in case dates are descending
-
-# Return all Ratios
-companies.ratios.collect_all_ratios()
+    ["AAPL", "MSFT", "GOOGL", "AMZN"], api_key=API_KEY, start_date="2022-08-10",
+    custom_ratios=custom_ratios, quarterly=True
+)
 ```
 
-This will return all financial ratios that can be collected based on the provided data and the format.
+By then running `ratios.collect_custom_ratios` it automatically calculates the given ratios. Note the ratios 'Quick Ratio Current' and 'Quick Ratio Total' which rely on an earlier defined ratio ('Current Assets Inventory'). This is an example of how you can create a custom ratio based on another custom ratio.
 
-![Output of Result](https://github.com/JerBouma/FinanceToolkit/assets/46355364/2a995430-b8d8-4236-892c-edb47042d6af)
+Below you can find the custom ratios from GOOGL which has been selected with `.loc['GOOGL]`. The Notebook as found [here](https://github.com/JerBouma/FinanceToolkit/blob/main/examples/Finance%20Toolkit%20-%203.%20Defining%20Custom%20Ratios.ipynb) shows the full output.
+
+|                           |      2022Q3 |      2022Q4 |     2023Q1 |      2023Q2 |
+|:--------------------------|------------:|------------:|-----------:|------------:|
+| Current Assets Inventory  | 1.62953e+11 | 1.62125e+11 | 1.5967e+11 | 1.66557e+11 |
+| Net Income / Total Assets | 0.0388271   | 0.037299    | 0.0407344  | 0.0479527   |
+| Quick Ratio Current       | 2.46977     | 2.33947     | 2.31896    | 2.14334     |
+| Quick Ratio Total         | 1.55744     | 1.48575     | 1.4703     | 1.43704     |
+| WC / Net Income           | 7.19842     | 7.00932     | 6.1877     | 4.95857     |
 
 ## Calling Functions Directly
 
 It also possible to call any ratio or model directly as shown below. This allows access to 50+ ratios with custom data. Also see [this notebook](https://github.com/JerBouma/FinanceToolkit/blob/main/examples/Finance%20Toolkit%20-%204.%20Calling%20Functions%20Directly.ipynb).
 
 ```python
 import pandas as pd
@@ -236,14 +226,66 @@
 |                   |       2018 |     2019 |     2020 |     2021 |     2022 |
 |:------------------|-----------:|---------:|---------:|---------:|---------:|
 | Net Profit Margin |   0.224142 | 0.212381 | 0.209136 | 0.258818 | 0.253096 |
 | Asset Turnover    | nan        | 0.738878 | 0.828845 | 1.08408  | 1.12064  |
 | Equity Multiplier | nan        | 3.56334  | 4.25089  | 5.25497  | 6.18622  |
 | Return on Equity  | nan        | 0.559172 | 0.736856 | 1.47443  | 1.75459  |
 
+## Working with other Datasets
+
+The Finance Toolkit has the ability to leverage custom datasets from any data provider as well. This makes it possible to work with your preferred data and not be limited to the data source the Finance Toolkit currently provides. A detailed example can be found [here](https://github.com/JerBouma/FinanceToolkit/blob/main/examples/Finance%20Toolkit%20-%205.%20Using%20External%20Datasets.ipynb) but to get started see the code below.
+
+```python
+from financetoolkit import Toolkit
+
+# Initialize the Finance Toolkit
+companies = Toolkit(['AAPL', 'MSFT'])
+
+# Copy the normalization files
+companies.get_normalization_files()
+```
+This copies over three files, `balance.csv`, `income.csv` and `cash.csv` which will contain a structure like the following:
+
+![Normalization Format](https://github.com/JerBouma/FinanceToolkit/assets/46355364/ea4ebf87-1a27-4c40-a1fb-40d0eb0634bc)
+
+By replacing the first column with the names from your dataset (e.g. replace `cashAndCashEquivalents` with `Cash` if this is how it is called in your dataset), it will automatically normalize the dataset when you initialize the Finance Toolkit. Note that the DataFrame needs to be a multi-index in case you use multiple tickers structured as `Ticker x Financial Statement Item x Periods`.
+
+As an example:
+
+![Dataset Example](https://github.com/JerBouma/FinanceToolkit/assets/46355364/fe0e3db0-3e88-41d2-a355-5f68110fdcf3)
+
+If you have individual DataFrames for each company, you can do the following which will return the DataFrame structure that is required:
+
+```python
+from financetoolkit.base import helpers
+
+balance_grouped = helpers.combine_dataframes({'AAPL': balance_apple, 'MSFT': balance_msft})
+```
+
+Once all of this is set-up you can feed this information to the Toolkit and use the Toolkit as normally.
+
+```python
+
+# Initialize the Toolkit
+companies = Toolkit(
+    tickers=['AAPL', 'MSFT'],
+    balance=balance_grouped,
+    income=income_grouped,
+    cash=cash_grouped,
+    format_location="FOLDER_PATH",
+    reverse_dates=False) # Put this to True in case dates are descending
+
+# Return all Ratios
+companies.ratios.collect_all_ratios()
+```
+
+This will return all financial ratios that can be collected based on the provided data and the format.
+
+![Output of Result](https://github.com/JerBouma/FinanceToolkit/assets/46355364/2a995430-b8d8-4236-892c-edb47042d6af)
+
 # Contact
 If you have any questions about the FinanceToolkit or would like to share with me what you have been working on, feel free to reach out to me via:
 
 - **LinkedIn:** https://www.linkedin.com/in/boumajeroen/
 -  **Email:** jer.bouma@gmail.com
 
 If you'd like to support my efforts, either help me out by contributing to the package or [Buy me a Coffee](https://www.buymeacoffee.com/jerbouma).
```

