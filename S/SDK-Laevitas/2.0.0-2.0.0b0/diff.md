# Comparing `tmp/SDK-Laevitas-2.0.0.tar.gz` & `tmp/SDK-Laevitas-2.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SDK-Laevitas-2.0.0.tar", last modified: Tue Aug  1 14:27:20 2023, max compression
+gzip compressed data, was "SDK-Laevitas-2.0.0b0.tar", last modified: Thu Jul 20 14:56:42 2023, max compression
```

## Comparing `SDK-Laevitas-2.0.0.tar` & `SDK-Laevitas-2.0.0b0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 14:27:20.282919 SDK-Laevitas-2.0.0/
--rw-rw-rw-   0        0        0    11539 2023-08-01 09:56:43.000000 SDK-Laevitas-2.0.0/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-08-01 14:27:20.256875 SDK-Laevitas-2.0.0/Laevitas/
--rw-rw-rw-   0        0        0   197811 2023-08-01 13:23:27.000000 SDK-Laevitas-2.0.0/Laevitas/SDK.py
--rw-rw-rw-   0        0        0       33 2023-08-01 09:56:43.000000 SDK-Laevitas-2.0.0/Laevitas/__init__.py
--rw-rw-rw-   0        0        0      925 2023-08-01 09:56:43.000000 SDK-Laevitas-2.0.0/Laevitas/consts.py
--rw-rw-rw-   0        0        0     4204 2023-08-01 09:56:43.000000 SDK-Laevitas-2.0.0/Laevitas/dataclasses.py
--rw-rw-rw-   0        0        0    34320 2023-08-01 12:58:54.000000 SDK-Laevitas-2.0.0/Laevitas/test_SDK.py
--rw-rw-rw-   0        0        0     1336 2023-08-01 14:27:20.283979 SDK-Laevitas-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      983 2023-08-01 13:06:27.000000 SDK-Laevitas-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 14:27:20.282919 SDK-Laevitas-2.0.0/SDK_Laevitas.egg-info/
--rw-rw-rw-   0        0        0     1336 2023-08-01 14:27:20.000000 SDK-Laevitas-2.0.0/SDK_Laevitas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-08-01 14:27:20.000000 SDK-Laevitas-2.0.0/SDK_Laevitas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 14:27:20.000000 SDK-Laevitas-2.0.0/SDK_Laevitas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-08-01 14:27:20.000000 SDK-Laevitas-2.0.0/SDK_Laevitas.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-08-01 14:27:20.000000 SDK-Laevitas-2.0.0/SDK_Laevitas.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-08-01 14:27:20.284966 SDK-Laevitas-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0      631 2023-08-01 13:38:03.000000 SDK-Laevitas-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 14:56:42.287998 SDK-Laevitas-2.0.0b0/
+-rw-rw-rw-   0        0        0    11539 2023-07-17 15:51:26.000000 SDK-Laevitas-2.0.0b0/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-07-20 14:56:42.260406 SDK-Laevitas-2.0.0b0/Laevitas/
+-rw-rw-rw-   0        0        0   197829 2023-07-20 14:41:43.000000 SDK-Laevitas-2.0.0b0/Laevitas/SDK.py
+-rw-rw-rw-   0        0        0       33 2023-07-18 16:13:43.000000 SDK-Laevitas-2.0.0b0/Laevitas/__init__.py
+-rw-rw-rw-   0        0        0      925 2023-07-20 14:28:32.000000 SDK-Laevitas-2.0.0b0/Laevitas/consts.py
+-rw-rw-rw-   0        0        0     4204 2023-07-17 15:51:26.000000 SDK-Laevitas-2.0.0b0/Laevitas/dataclasses.py
+-rw-rw-rw-   0        0        0    34344 2023-07-17 15:51:26.000000 SDK-Laevitas-2.0.0b0/Laevitas/test_SDK.py
+-rw-rw-rw-   0        0        0    23425 2023-07-20 14:56:42.288998 SDK-Laevitas-2.0.0b0/PKG-INFO
+-rw-rw-rw-   0        0        0    23073 2023-07-17 15:51:26.000000 SDK-Laevitas-2.0.0b0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-20 14:56:42.287076 SDK-Laevitas-2.0.0b0/SDK_Laevitas.egg-info/
+-rw-rw-rw-   0        0        0    23425 2023-07-20 14:56:41.000000 SDK-Laevitas-2.0.0b0/SDK_Laevitas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-07-20 14:56:42.000000 SDK-Laevitas-2.0.0b0/SDK_Laevitas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 14:56:41.000000 SDK-Laevitas-2.0.0b0/SDK_Laevitas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-20 14:56:41.000000 SDK-Laevitas-2.0.0b0/SDK_Laevitas.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-20 14:56:41.000000 SDK-Laevitas-2.0.0b0/SDK_Laevitas.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-20 14:56:42.290034 SDK-Laevitas-2.0.0b0/setup.cfg
+-rw-rw-rw-   0        0        0      634 2023-07-20 14:54:12.000000 SDK-Laevitas-2.0.0b0/setup.py
```

### Comparing `SDK-Laevitas-2.0.0/LICENSE.txt` & `SDK-Laevitas-2.0.0b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SDK-Laevitas-2.0.0/Laevitas/SDK.py` & `SDK-Laevitas-2.0.0b0/Laevitas/SDK.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import requests
 from Laevitas.dataclasses import *
 # from dataclasses import dataclass, field, make_dataclass
 from Laevitas.consts import prepare_query, MARKET_CONSTS
 
 
-class api:
+class api():
     header = {"apiKey": 'none'}
 
     def __init__(self, key="none"):
         self.header["apiKey"] = key
         self.r = self.analytics()
 
     @classmethod
-    def configure(cls, header):
-        cls.header["apiKey"] = header
+    def configure(self, header):
+        self.header["apiKey"] = header
 
     class analytics:
         def __init__(self):
             self.option = self.options()
 
         class options:
             url = "https://api.laevitas.ch/analytics/options/"
             pass
 
             @classmethod
-            def instruments(cls, market="BINANCE", currency="BTC", maturity="", strike="", optiontype="C"):
+            def instruments(self, market="BINANCE", currency="BTC", maturity="", strike="", optiontype="C"):
 
                 """
                 :param market: BIT  | DERIBIT  | BYBIT  | OKEX  | POWERTRADE | DELTA_EXCHANGE | LYRA_ARBITRUM | AEVO | BINANCE | LYRA
                 :type market:
                 :param currency: BTC | ETH | BCH | SOL | XRP | BNB | ADA | ARB | OP
                 :type currency:
                 :param maturity: Uppercase (DMMMYY), e.g., 30JUN23 or "all" ,Check analytics/options/maturities for more information about available maturity
@@ -38,40 +38,40 @@
                 :param optiontype: C,P
                 :type optiontype:
                 :return: json data of dovs
                 :rtype:
                 """
                 makequery = prepare_query(market=market, currency=currency, maturity=maturity, strike=strike,
                                           optiontype=optiontype)
-                api_url = cls.url + "Instruments" + makequery
+                api_url = self.url + "Instruments" + makequery
                 responsedata = requests.get(api_url, headers=api.header).json()
                 return responsedata
 
             @classmethod
-            def atm_iv_ts(cls, market: str, currency: str):
+            def atm_iv_ts(self, market: str, currency: str):
                 """
 
                 :param market: BIT  | DERIBIT  | BYBIT  | OKEX  | POWERTRADE | DELTA_EXCHANGE | LYRA_ARBITRUM | AEVO | BINANCE | LYRA
                 :type market:
                 :param currency: ADA,BTC,ETH,TONCOIN,1MLADYS,SOL,BNB,XRP , Check analytics/options/Instruments for more information about available currency
                 :type currency:
-                :return: This endpoint retrieves ATM (At-The-Money) implied volatility time-lapse for a specific market and currency. The response includes implied volatility data for various time periods, such as today, yesterday, 2 days ago, 1 week ago, 2 weeks ago, 3 weeks ago, and 1 month ago. For each time period, the response includes an array of objects with the maturity of the option and the corresponding implied volatility.
+                :return: This endpoint retrieves ATM (At-The-Money) implied volatility time lapse for a specific market and currency. The response includes implied volatility data for various time periods, such as today, yesterday, 2 days ago, 1 week ago, 2 weeks ago, 3 weeks ago, and 1 month ago. For each time period, the response includes an array of objects with the maturity of the option and the corresponding implied volatility.
                 :rtype:
                 """
                 market = market.upper()
                 currency = currency.upper()
                 if market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "atm_iv_ts/" + market + "/" + currency
+                    api_url = self.url + "atm_iv_ts/" + market + "/" + currency
                     responsedata = requests.get(api_url, headers=api.header).json()
                     return responsedata
 
             @classmethod
-            def gex_date(cls, market: str, currency: str, maturity: str):
+            def gex_date(self, market: str, currency: str, maturity: str):
                 """
 
                 :param market: BIT  | DERIBIT  | BYBIT  | OKEX  | POWERTRADE | DELTA_EXCHANGE | LYRA_ARBITRUM | AEVO | BINANCE | LYRA
                 :type market:
                 :param currency: BTC | ETH | ADA | SOL | XRP | BNB | ARB | OP
                 :type currency:
                 :param maturity: Uppercase (DMMMYY), e.g., 30JUN23 or "all" ,Check analytics/options/maturities for more information about available maturity
@@ -81,223 +81,223 @@
                 """
                 market = market.upper()
                 currency = currency.upper()
                 maturity = maturity.upper()
                 if market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "gex_date/" + market + "/" + currency + "/" + maturity
+                    api_url = self.url + "gex_date/" + market + "/" + currency + "/" + maturity
                     responsedata = requests.get(api_url, headers=api.header).json()
 
                 return responsedata
 
             @classmethod
-            def gex_date_all(cls, market: str, currency: str):
+            def gex_date_all(self, market: str, currency: str):
                 """
 
                 :param market: BIT  | DERIBIT  | BYBIT  | OKEX  | POWERTRADE | DELTA_EXCHANGE | LYRA_ARBITRUM | AEVO | BINANCE | LYRA
                 :type market:
                 :param currency: BTC | ETH | BCH | SOL | XRP | BNB | ADA | ARB | OP , Check analytics/options/Instruments for more information about available currency
                 :type currency:
                 :return: This endpoint retrieves GEX (Gamma Exposure) data for all options on a specific market and currency. The response includes an array of objects, where each object represents an option and provides information such as the strike price, option type (call or put), and the corresponding Gamma Exposure value. The Gamma Exposure value indicates the sensitivity of an options book's value to changes in the underlying asset's price.
                 :rtype:
                 """
                 market = market.upper()
                 currency = currency.upper()
                 if market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "gex_date_all/" + market + "/" + currency
+                    api_url = self.url + "gex_date_all/" + market + "/" + currency
                     responsedata = requests.get(api_url, headers=api.header).json()
 
                 return responsedata
 
             @classmethod
-            def maturities(cls, market: str, currency: str):
+            def maturities(self, market: str, currency: str):
                 """
 
                 :param market: AGGREGATE | BIT  | DERIBIT  | BYBIT  | OKEX  | POWERTRADE | DELTA_EXCHANGE | LYRA_ARBITRUM | AEVO | BINANCE | LYRA
                 :type market:
                 :param currency: BTC | ETH | BCH | SOL | XRP | BNB | ADA | ARB | OP , Check analytics/options/Instruments for more information about available currency
                 :type currency:
                 :return: This endpoint provides a list of available maturities for options in a specific market and currency.
                 :rtype:
                 """
                 market = market.upper()
                 currency = currency.upper()
                 if market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "maturities/" + market + "/" + currency
+                    api_url = self.url + "maturities/" + market + "/" + currency
                     responsedata = requests.get(api_url, headers=api.header).json()
                     return responsedata
 
             @classmethod
-            def oi_expiry(cls, market: str, currency: str):
+            def oi_expiry(self, market: str, currency: str):
                 """
 
                 :param market: AGGREGATE | BIT  | DERIBIT  | BYBIT  | OKEX  | POWERTRADE | DELTA_EXCHANGE | LYRA_ARBITRUM | AEVO | BINANCE | LYRA
                 :type market:
                 :param currency: BTC | ETH | BCH | SOL | XRP | BNB | ADA | ARB | OP , Check analytics/options/Instruments for more information about available currency
                 :type currency:
                 :return: This endpoint provides the open interest data for options by expiry in a specific market and currency. The response includes the open interest for call and put options, as well as their corresponding notional and premium values.
                 :rtype:
                 """
                 market = market.upper()
                 currency = currency.upper()
                 if market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "oi_expiry/" + market + "/" + currency
+                    api_url = self.url + "oi_expiry/" + market + "/" + currency
                     responsedata = requests.get(api_url, headers=api.header).json()
                 return responsedata
 
             @classmethod
-            def oi_strike_all(cls, market: str, currency: str):
+            def oi_strike_all(self, market: str, currency: str):
                 """
 
                 :param market: AGGREGATE | BIT  | DERIBIT  | BYBIT  | OKEX  | POWERTRADE | DELTA_EXCHANGE | LYRA_ARBITRUM | AEVO | BINANCE | LYRA
                 :type market:
                 :param currency: BTC | ETH | BCH | SOL | XRP | BNB | ADA | ARB | OP , Check analytics/options/Instruments for more information about available currency
                 :type currency:
                 :return: This endpoint provides the open interest data for options by strike in a specific market and currency. The response includes the open interest for call and put options at each strike, as well as their corresponding notional and premium values.
                 :rtype:
                 """
                 market = market.upper()
                 currency = currency.upper()
                 if market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "oi_strike_all/" + market + "/" + currency
+                    api_url = self.url + "oi_strike_all/" + market + "/" + currency
                     responsedata = requests.get(api_url, headers=api.header).json()
                     Response = Ioi_strike_all(responsedata, responsedata['date'])
                     for i in range(len(responsedata['data'])):
                         Response.data.append(oi_strike_all_data(responsedata['data'][i]['strike'],
                                                                 responsedata['data'][i]['c'],
                                                                 responsedata['data'][i]['p'],
                                                                 responsedata['data'][i]['notional_c'],
                                                                 responsedata['data'][i]['notional_p']))
                     return Response
 
             @classmethod
-            def oi_type(cls, market: str, currency: str):
+            def oi_type(self, market: str, currency: str):
                 """
 
                 :param market: AGGREGATE | BIT  | DERIBIT  | BYBIT  | OKEX  | POWERTRADE | DELTA_EXCHANGE | LYRA_ARBITRUM | AEVO | BINANCE | LYRA
                 :type market:
                 :param currency: BTC | ETH | BCH | SOL | XRP | BNB | ADA | ARB | OP , Check analytics/options/Instruments for more information about available currency
                 :type currency:
                 :return: This endpoint provides the open interest data for options by type in a specific market and currency. The response includes the open interest, notional value, and premium value for call and put options separately.
                 :rtype:
                 """
                 market = market.upper()
                 currency = currency.upper()
                 if market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "oi_type/" + market + "/" + currency
+                    api_url = self.url + "oi_type/" + market + "/" + currency
                     responsedata = requests.get(api_url, headers=api.header).json()
                     return responsedata
 
             @classmethod
-            def top_traded_option(cls, market: str, currency: str):
+            def top_traded_option(self, market: str, currency: str):
                 """
 
                 :param market: AGGREGATE | BIT  | DERIBIT  | BYBIT  | OKEX  | POWERTRADE | DELTA_EXCHANGE | LYRA_ARBITRUM | AEVO | BINANCE | LYRA
                 :type market:
                 :param currency: BTC | ETH | BCH | SOL | XRP | BNB | ADA | ARB | OP , Check analytics/options/Instruments for more information about available currency
                 :type currency:
                 :return: This endpoint provides information about the top traded options in a specific market and currency. The response includes the trading volume, instrument symbol, trading volume in USD, mark price, and premium value for each option.
                 :rtype:
                 """
                 market = market.upper()
                 currency = currency.upper()
                 if market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "top_traded_option/" + market + "/" + currency
+                    api_url = self.url + "top_traded_option/" + market + "/" + currency
                     responsedata = requests.get(api_url, headers=api.header).json()
                 return responsedata
 
             @classmethod
-            def v_expiry(cls, market: str, currency: str):
+            def v_expiry(self, market: str, currency: str):
                 """
 
                 :param market: AGGREGATE | BIT  | DERIBIT  | BYBIT  | OKEX  | POWERTRADE | DELTA_EXCHANGE | LYRA_ARBITRUM | AEVO | BINANCE | LYRA
                 :type market:
                 :param currency: BTC | ETH | BCH | SOL | XRP | BNB | ADA | ARB | OP , Check analytics/options/Instruments for more information about available currency
                 :type currency:
                 :return: This endpoint provides information about the options volume by expiry in a specific market and currency. The response includes the expiry date, volume of call options, volume of put options, notional value of call options, notional value of put options, premium value of call options, and premium value of put options for each expiry.
                 :rtype:
                 """
                 market = market.upper()
                 currency = currency.upper()
                 if market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "v_expiry/" + market + "/" + currency
+                    api_url = self.url + "v_expiry/" + market + "/" + currency
                     responsedata = requests.get(api_url, headers=api.header).json()
                     Response = Iexpiry(responsedata, responsedata['date'])
                     for i in range(len(responsedata['data'])):
                         Response.data.append(expiry_data(responsedata['data'][i]['maturity'],
                                                          responsedata['data'][i]['c'],
                                                          responsedata['data'][i]['p'],
                                                          responsedata['data'][i]['notional_c'],
                                                          responsedata['data'][i]['notional_p']))
                     return Response
 
             @classmethod
-            def v_strike_all(cls, market: str, currency: str):
+            def v_strike_all(self, market: str, currency: str):
                 """
 
                 :param market: AGGREGATE | BIT  | DERIBIT  | BYBIT  | OKEX  | POWERTRADE | DELTA_EXCHANGE | LYRA_ARBITRUM | AEVO | BINANCE | LYRA
                 :type market:
                 :param currency: BTC | ETH | BCH | SOL | XRP | BNB | ADA | ARB | OP , Check analytics/options/Instruments for more information about available currency
                 :type currency:
                 :return: This endpoint provides information about the options volume by strike in a specific market and currency. The response includes the strike price, volume of call options, volume of put options, notional value of call options, and notional value of put options for each strike.
                 :rtype:
                 """
                 market = market.upper()
                 currency = currency.upper()
                 if market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "v_strike_all/" + market + "/" + currency
+                    api_url = self.url + "v_strike_all/" + market + "/" + currency
                     responsedata = requests.get(api_url, headers=api.header).json()
                     Response = v_strike_alli(responsedata, responsedata['date'])
                     for i in range(len(responsedata['data'])):
                         Response.data.append(v_strike_all_data(responsedata['data'][i]['strike'],
                                                                responsedata['data'][i]['C'],
                                                                responsedata['data'][i]['P'],
                                                                responsedata['data'][i]['USDVC'],
                                                                responsedata['data'][i]['USDVP']))
                     return Response
 
             @classmethod
-            def volume_buy_sell_all(cls, market: str, currency: str):
+            def volume_buy_sell_all(self, market: str, currency: str):
                 """
 
                 :param market: BIT  | DERIBIT  | BYBIT | OKEX
                 :type market:
                 :param currency: BTC | ETH | ADA | SOL
                 :type currency:
                 :return: This endpoint provides information about the options volume by buy/sell in a specific market and currency. The response includes the strike price, volume of call options bought, volume of call options sold, volume of put options bought, volume of put options sold, premium paid for call options bought, premium received from call options sold, premium paid for put options bought, premium received from put options sold, notional value of call options bought, notional value of call options sold, notional value of put options bought, and notional value of put options sold for each strike.
                 :rtype:
                 """
                 market = market.upper()
                 currency = currency.upper()
                 if market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "volume_buy_sell_all/" + market.lower() + "/" + currency.lower()
+                    api_url = self.url + "volume_buy_sell_all/" + market.lower() + "/" + currency.lower()
                     responsedata = requests.get(api_url, headers=api.header).json()
                     return responsedata
 
             @classmethod
-            def iv_strike(cls, market: str, currency: str, strike: str):
+            def iv_strike(self, market: str, currency: str, strike: str):
                 """
 
                 :param market: BIT  | DERIBIT  | BYBIT  | OKEX  | POWERTRADE | DELTA_EXCHANGE | LYRA_ARBITRUM | AEVO | BINANCE | LYRA
                 :type market:
                 :param currency: BTC | ETH | BCH | SOL | XRP | BNB | ADA | ARB | OP , Check analytics/options/Instruments for more information about available currency
                 :type currency:
                 :param strike: e.g., 25000 Check analytics/options/Instruments for more information about available strike
@@ -306,20 +306,20 @@
                 :rtype:
                 """
                 market = market.upper()
                 currency = currency.upper()
                 if market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "iv_strike/" + market + "/" + currency + "/" + str(strike)
+                    api_url = self.url + "iv_strike/" + market + "/" + currency + "/" + str(strike)
                     responsedata = requests.get(api_url, headers=api.header).json()
                     return responsedata
 
             @classmethod
-            def oi_strike(cls, market: str, currency: str, maturity: str):
+            def oi_strike(self, market: str, currency: str, maturity: str):
                 """
 
                 :param market: AGGREGATE | BIT  | DERIBIT  | BYBIT  | OKEX  | POWERTRADE | DELTA_EXCHANGE | LYRA_ARBITRUM | AEVO | BINANCE | LYRA
                 :type market:
                 :param currency: BTC | ETH | BCH | SOL | XRP | BNB | ADA | ARB | OP , Check analytics/options/Instruments for more information about available currency
                 :type currency:
                 :param maturity: Uppercase (DMMMYY), e.g., 30JUN23 or "all" ,Check analytics/options/maturities for more information about available maturity
@@ -329,20 +329,20 @@
                 """
                 market = market.upper()
                 currency = currency.upper()
                 maturity = maturity.upper()
                 if market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "oi_strike/" + market.lower() + "/" + currency.lower() + "/" + maturity.upper()
+                    api_url = self.url + "oi_strike/" + market.lower() + "/" + currency.lower() + "/" + maturity.upper()
                     responsedata = requests.get(api_url, headers=api.header).json()
                     return responsedata
 
             @classmethod
-            def oi_net_change_all(cls, market: str, currency: str, hours: str):
+            def oi_net_change_all(self, market: str, currency: str, hours: str):
                 """
 
                 :param market: BIT  | DERIBIT  | BYBIT  | OKEX  | POWERTRADE | DELTA_EXCHANGE | LYRA_ARBITRUM | AEVO | BINANCE | LYRA
                 :type market:
                 :param currency: BTC | ETH | ADA | BNB | SOL | XRP | TONCOIN , Check analytics/options/Instruments for more information about available currency
                 :type currency:
                 :param hours: 1, 2, 4, 8, 12, 18, 24, 48, 168, 336, 504, 720
@@ -351,20 +351,20 @@
                 :rtype:
                 """
                 market = market.upper()
                 currency = currency.upper()
                 if market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "oi_net_change_all/" + market + "/" + currency + "/" + hours
+                    api_url = self.url + "oi_net_change_all/" + market + "/" + currency + "/" + hours
                     responsedata = requests.get(api_url, headers=api.header).json()
                     return responsedata
 
             @classmethod
-            def top_instrument_oi_change(cls, market: str, currency: str, hours: str):
+            def top_instrument_oi_change(self, market: str, currency: str, hours: str):
                 """
 
                 :param market: BIT  | DERIBIT  | BYBIT  | OKEX  | POWERTRADE | DELTA_EXCHANGE | LYRA_ARBITRUM | AEVO | BINANCE | LYRA
                 :type market:
                 :param currency: BTC | ETH | ADA | BNB | SOL | XRP | TONCOIN , Check analytics/options/Instruments for more information about available currency
                 :type currency:
                 :param hours: 1, 2, 4, 8, 12, 18, 24, 48, 168, 336, 504, 720
@@ -373,21 +373,21 @@
                 :rtype:
                 """
                 market = market.upper()
                 currency = currency.upper()
                 if market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "top_instrument_oi_change/" + market.lower() + "/" + currency.lower() + "/" + str(
+                    api_url = self.url + "top_instrument_oi_change/" + market.lower() + "/" + currency.lower() + "/" + str(
                         hours)
                     responsedata = requests.get(api_url, headers=api.header).json()
                     return responsedata
 
             @classmethod
-            def volume_buy_sell(cls, market: str, currency: str, maturity: str):
+            def volume_buy_sell(self, market: str, currency: str, maturity: str):
                 """
 
                 :param market: BIT | DERIBIT | BYBIT | OKEX
                 :type market:
                 :param currency: BTC | ETH | SOL | ADA , Check analytics/options/Instruments for more information about available currency
                 :type currency:
                 :param maturity: Uppercase (DMMMYY), e.g., 30JUN23 or "all" ,Check analytics/options/maturities for more information about available maturity
@@ -397,20 +397,20 @@
                 """
                 market = market.upper()
                 currency = currency.upper()
                 maturity = maturity.upper()
                 if market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "volume_buy_sell/" + market.lower() + "/" + currency.lower() + "/" + maturity.upper()
+                    api_url = self.url + "volume_buy_sell/" + market.lower() + "/" + currency.lower() + "/" + maturity.upper()
                     responsedata = requests.get(api_url, headers=api.header).json()
                     return responsedata
 
             @classmethod
-            def v_strike(cls, market: str, currency: str, maturity: str):
+            def v_strike(self, market: str, currency: str, maturity: str):
                 """
 
                 :param market: AGGREGATE | BIT  | DERIBIT  | BYBIT  | OKEX  | POWERTRADE | DELTA_EXCHANGE | LYRA_ARBITRUM | AEVO | BINANCE | LYRA
                 :type market:
                 :param currency: BTC | ETH | BCH | SOL | XRP | BNB | ADA | ARB | OP , Check analytics/options/Instruments for more information about available currency
                 :type currency:
                 :param maturity: Uppercase (DMMMYY), e.g., 30JUN23 or "all" ,Check analytics/options/maturities for more information about available maturity
@@ -420,20 +420,20 @@
                 """
                 market = market.upper()
                 currency = currency.upper()
                 maturity = maturity.upper()
                 if market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "v_strike/" + market.lower() + "/" + currency.lower() + "/" + maturity.upper()
+                    api_url = self.url + "v_strike/" + market.lower() + "/" + currency.lower() + "/" + maturity.upper()
                     responsedata = requests.get(api_url, headers=api.header).json()
                     return responsedata
 
             @classmethod
-            def summary_trades(cls, market: str, currency: str, hours: str):
+            def summary_trades(self, market: str, currency: str, hours: str):
                 """
 
                 :param market: BIT | DERIBIT
                 :type market:
                 :param currency: BTC | ETH | ADA , Check analytics/options/Instruments for more information about available currency
                 :type currency:
                 :param hours: 1, 2, 4, 8, 12, 18, 24, 48, 168, 336, 504, 720
@@ -442,20 +442,20 @@
                 :rtype:
                 """
                 market = market.upper()
                 currency = currency.upper()
                 if market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "summary_trades/" + market + "/" + currency + "/" + str(hours)
+                    api_url = self.url + "summary_trades/" + market + "/" + currency + "/" + str(hours)
                     responsedata = requests.get(api_url, headers=api.header).json()
                     return responsedata
 
             @classmethod
-            def greeks(cls, market: str, currency: str, maturity: str, optiontype: str):
+            def greeks(self, market: str, currency: str, maturity: str, optiontype: str):
                 """
 
                 :param market: BIT  | DERIBIT  | BYBIT  | OKEX  | POWERTRADE | DELTA_EXCHANGE | LYRA_ARBITRUM | AEVO | BINANCE | LYRA
                 :type market:
                 :param currency: BTC | ETH | SOL | XRP | BNB | ADA | ARB | OP , Check analytics/options/Instruments for more information about available currency
                 :type currency:
                 :param maturity: Uppercase (DMMMYY), e.g., 30JUN23 or "all" ,Check analytics/options/maturities for more information about available maturity
@@ -471,30 +471,31 @@
                 optiontype = optiontype.upper()
                 if market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 elif optiontype not in ["P", "C"]:
                     raise TypeError("type is either C or P")
                 else:
                     maturity = maturity.upper()
-                    api_url = cls.url + "greeks/" + market + "/" + currency + "/" + maturity + "/" + optiontype
+                    api_url = self.url + "greeks/" + market + "/" + currency + "/" + maturity + "/" + optiontype
                     responsedata = requests.get(api_url, headers=api.header).json()
                     # Response = Igreeks(responsedata, responsedata['date'])
                     # for i in range(len(responsedata['data'])):
                     #     Response.data.append(greeks_data(responsedata['data'][i]['strike'],
                     #                                      responsedata['data'][i]['underlying_price'],
                     #                                      responsedata['data'][i]['delta'],
                     #                                      responsedata['data'][i]['gamma'],
                     #                                      responsedata['data'][i]['theta'],
                     #                                      responsedata['data'][i]['vega']
                     #                                      ))
                     return responsedata
 
             @classmethod
-            def iv_all(cls, market: str, currency: str, maturity: str, type: str):
+            def iv_all(self, market: str, currency: str, maturity: str, type: str):
                 """
+
                 :param market: BIT  | DERIBIT  | BYBIT  | OKEX  | POWERTRADE | DELTA_EXCHANGE | LYRA_ARBITRUM | AEVO | BINANCE | LYRA
                 :type market:
                 :param currency: BTC | ETH | SOL | XRP | BNB | ADA | ARB | OP , Check analytics/options/Instruments for more information about available currency
                 :type currency:
                 :param maturity: Uppercase (DMMMYY), e.g., 30JUN23 or "all" ,Check analytics/options/maturities for more information about available maturity
                 :type maturity:
                 :param type: C , P
@@ -503,40 +504,40 @@
                 :rtype:
                 """
                 market = market.upper()
                 currency = currency.upper()
                 if market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "iv_all/" + market.lower() + "/" + currency.lower() + "/" + maturity.upper() + "/" + type.upper()
+                    api_url = self.url + "iv_all/" + market.lower() + "/" + currency.lower() + "/" + maturity.upper() + "/" + type.upper()
                     responsedata = requests.get(api_url, headers=api.header).json()
                     return responsedata
 
             @classmethod
-            def iv_table(cls, market: str, currency: str):
+            def iv_table(self, market: str, currency: str):
                 """
 
                 :param market: BIT  | DERIBIT  | BYBIT  | OKEX  | POWERTRADE | DELTA_EXCHANGE | LYRA_ARBITRUM | AEVO | BINANCE | LYRA
                 :type market:
                 :param currency: BTC | ETH | SOL | XRP | BNB | ADA | ARB | OP , Check analytics/options/Instruments for more information about available currency
                 :type currency:
                 :return: This endpoint allows users to retrieve the implied volatility table for options based on the specified market and currency. Implied volatility is a crucial factor in options pricing, and having access to this data helps traders and investors analyze and make informed decisions about their options trading strategies.
                 :rtype:
                 """
                 market = market.upper()
                 currency = currency.upper()
                 if market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "iv_table/" + market + "/" + currency
+                    api_url = self.url + "iv_table/" + market + "/" + currency
                     responsedata = requests.get(api_url, headers=api.header).json()
                     return responsedata
 
             @classmethod
-            def oi_net_change(cls, market: str, currency: str, maturity: str, hour: str):
+            def oi_net_change(self, market: str, currency: str, maturity: str, hour: str):
                 """
 
                 :param market: BIT  | DERIBIT  | BYBIT  | OKEX  | POWERTRADE | DELTA_EXCHANGE | LYRA_ARBITRUM | AEVO | BINANCE | LYRA
                 :type market:
                 :param currency: BTC | ETH | ADA | SOL | XRP | BNB | TONCOIN , Check analytics/options/Instruments for more information about available currency
                 :type currency:
                 :param maturity: Uppercase (DMMMYY), e.g., 30JUN23 or "all" ,Check analytics/options/maturities for more information about available maturity
@@ -547,80 +548,78 @@
                 :rtype:
                 """
                 market = market.upper()
                 currency = currency.upper()
                 if market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "oi_net_change/" + market + "/" + currency + "/" + maturity + "/" + str(hour)
+                    api_url = self.url + "oi_net_change/" + market + "/" + currency + "/" + maturity + "/" + str(hour)
                     responsedata = requests.get(api_url, headers=api.header).json()
                     return responsedata
 
             @classmethod
-            def snapshot(cls, market: str, currency: str):
+            def snapshot(self, market: str, currency: str):
                 """
 
                 :param market: BIT  | DERIBIT  | BYBIT  | OKEX  | POWERTRADE | DELTA_EXCHANGE | LYRA_ARBITRUM | AEVO | BINANCE | LYRA
                 :type market:
                 :param currency: BTC | ETH | ADA | SOL | XRP | BNB | OP | ARB , Check analytics/options/Instruments for more information about available currency
                 :type currency:
                 :return: This endpoint allows users to retrieve a snapshot of options data for the specified market and currency. The snapshot includes comprehensive information about individual options contracts, such as strike price, expiration date, open interest, volume, pricing data, and other relevant metrics. Traders and analysts can utilize this data to gain insights into the options market, monitor market trends, evaluate trading opportunities, and make informed decisions regarding options trading strategies.
                 :rtype:
                 """
                 market = market.upper()
                 currency = currency.upper()
                 if market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "snapshot/" + market.lower() + "/" + currency.lower()
+                    api_url = self.url + "snapshot/" + market.lower() + "/" + currency.lower()
                     responsedata = requests.get(api_url, headers=api.header).json()
                     return responsedata
 
             @classmethod
-            def oi_breakdown(cls):
+            def oi_breakdown(self):
                 """
                 :return: This endpoint is essential for obtaining insights into the distribution of open interest and open value for options across different exchanges. By providing the breakdown of notional and open value data, the API response enables users to analyze the significance of options trading activity on various exchanges. Traders, investors, and analysts can leverage this information to assess market sentiment, identify liquidity sources, and make informed decisions about options trading strategies. Additionally, this endpoint facilitates the monitoring and comparison of options market participation among different exchanges, aiding in the evaluation of market dynamics and exchange performance.
                 :rtype:
                 """
-                api_url = cls.url + "oi_breakdown"
+                api_url = self.url + "oi_breakdown"
                 responsedata = requests.get(api_url, headers=api.header).json()
                 return responsedata
 
             @classmethod
-            def volume_breakdown(cls):
+            def volume_breakdown(self):
                 """
                 :return: This endpoint is crucial for obtaining insights into the distribution of trading volume and open value for options across different exchanges. By providing the breakdown of notional and open value data, the API response enables users to analyze the significance of options trading activity on various exchanges. Traders, investors, and analysts can leverage this information to assess market liquidity, identify trading opportunities, and monitor the overall trading activity for options. Additionally, this endpoint facilitates the comparison of trading volume and open value among different exchanges, aiding in the evaluation of market dynamics and exchange performance.
                 :rtype:
                 """
-                api_url = cls.url + "volume_breakdown"
+                api_url = self.url + "volume_breakdown"
                 responsedata = requests.get(api_url, headers=api.header).json()
                 return responsedata
 
             @classmethod
-            def oi_breakdown_by_currency(cls):
+            def oi_breakdown_by_currency(self):
                 """
                 :return: This endpoint is useful for obtaining insights into the distribution of open interest and open value for options by currency. By providing the breakdown of notional and open value data, the API response enables users to analyze the significance of options trading activity in different currencies. Traders, investors, and analysts can leverage this information to assess the popularity and liquidity of options contracts in various currencies. It allows for the identification of dominant currencies in options trading and provides an understanding of the market dynamics specific to each currency. Additionally, this endpoint facilitates the comparison of open interest and open value among different currencies, aiding in the evaluation of market trends and currency-specific trading opportunities.
                 :rtype:
                 """
-                api_url = cls.url + "oi_breakdown_by_currency"
+                api_url = self.url + "oi_breakdown_by_currency"
                 responsedata = requests.get(api_url, headers=api.header).json()
                 return responsedata
 
-            @classmethod
-            def volume_breakdown_by_currency(cls):
+            def volume_breakdown_by_currency(self):
                 """
                 :return: This endpoint is useful for obtaining insights into the distribution of trading volume and open value for options by currency. By providing the breakdown of notional and open value data, the API response enables users to analyze the significance of options trading activity in different currencies. Traders, investors, and analysts can leverage this information to assess the popularity and liquidity of options contracts in various currencies. It allows for the identification of dominant currencies in options trading and provides an understanding of the market dynamics specific to each currency. Additionally, this endpoint facilitates the comparison of trading volume and open value among different currencies, aiding in the evaluation of market trends and currency-specific trading opportunities.
                 :rtype:
                 """
-                api_url = cls.url + "volume_breakdown_by_currency"
+                api_url = self.url + "volume_breakdown_by_currency"
                 responsedata = requests.get(api_url, headers=api.header).json()
                 return responsedata
 
-            @classmethod
-            def expired_expiries(cls, market: str, currency: str, maturity=None):
+            def expired_expiries(self, market: str, currency: str, maturity=None):
                 """
 
                 :param market: BIT  | DERIBIT  | BYBIT  | OKEX  | POWERTRADE | DELTA_EXCHANGE | LYRA_ARBITRUM | AEVO | BINANCE | LYRA
                 :type market:
                 :param currency: BTC | ETH | SOL | XRP | BNB | ADA | ARB | OP , Check analytics/options/Instruments for more information about available currency
                 :type currency:
                 :param maturity: (optional) Uppercase (DMMMYY), e.g., 30JUN23 or "all" ,Check analytics/options/maturities for more information about available maturity
@@ -630,24 +629,23 @@
                 """
                 market = market.upper()
                 currency = currency.upper()
                 if market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 elif maturity:
                     makequery = prepare_query(maturity=maturity)
-                    api_url = cls.url + "expired_expiries/" + market + "/" + currency + makequery
+                    api_url = self.url + "expired_expiries/" + market + "/" + currency + makequery
                     responsedata = requests.get(api_url, headers=api.header).json()
                     return responsedata
                 else:
-                    api_url = cls.url + "expired_expiries/" + market + "/" + currency
+                    api_url = self.url + "expired_expiries/" + market + "/" + currency
                     responsedata = requests.get(api_url, headers=api.header).json()
                     return responsedata
 
-            @classmethod
-            def custom_change(cls, name: str, market: str, currency: str, end="", start=""):
+            def custom_change(self, name: str, market: str, currency: str, end="", start=""):
                 """
                 :param name: historical_buy_sell_volume , atmivts_historical , heatmap_change , oi_net_change , iv_table_change , time_skew, oi_gainers_and_losers
                 :type name:
                 :param market: BIT  | DERIBIT  | BYBIT  | OKEX  | POWERTRADE | DELTA_EXCHANGE | ZETA_EXCHANGE
                 :type market:
                 :param currency: BTC | ETH | SOL
                 :type currency:
@@ -661,24 +659,24 @@
                 market = market.lower()
                 currency = currency.lower()
                 name = name.lower()
                 if market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 elif start or end:
                     makequery = prepare_query(start=start, end=end)
-                    api_url = cls.url + "custom_change/" + name + "/" + market + "/" + currency + makequery
+                    api_url = self.url + "custom_change/" + name + "/" + market + "/" + currency + makequery
                     responsedata = requests.get(api_url, headers=api.header).json()
                     return responsedata
                 else:
-                    api_url = cls.url + "custom_change/" + name + "/" + market + "/" + currency
+                    api_url = self.url + "custom_change/" + name + "/" + market + "/" + currency
                     responsedata = requests.get(api_url, headers=api.header).json()
                     return responsedata
 
             @classmethod
-            def skew(cls, currency: str, maturity: str, type: str, timelapse: False):
+            def skew(self, currency: str, maturity: str, type: str, timelapse: False):
                 """
                 :param currency: BTC | ETH
                 :type currency:
                 :param maturity: Uppercase (DMMMYY), e.g., 30JUN23 or "all" ,Check analytics/options/maturities for more information about available maturity
                 :type maturity:
                 :param type: strike or delta , lowercase
                 :type type:
@@ -687,306 +685,306 @@
                 :return: Skew data provides insights into the implied volatility of options at different strikes or deltas, allowing users to analyze the market's perception of potential price movements. By retrieving the skew data, traders, investors, and analysts can assess the relative pricing of options at different strike prices or delta levels, identify potential opportunities for arbitrage or hedging strategies, and gain a deeper understanding of market sentiment and risk perception.
                 :rtype:
                 """
                 type = type.lower()
                 currency = currency.upper()
                 maturity = maturity.upper()
                 if timelapse is True:
-                    api_url = cls.url + "model_charts/skew/" + currency + "/" + maturity + "/" + type + '/time_lapse'
+                    api_url = self.url + "model_charts/skew/" + currency + "/" + maturity + "/" + type + '/time_lapse'
                     responsedata = requests.get(api_url, headers=api.header).json()
                     return responsedata
                 else:
-                    api_url = cls.url + "model_charts/skew/" + currency + "/" + maturity + "/" + type
+                    api_url = self.url + "model_charts/skew/" + currency + "/" + maturity + "/" + type
                     responsedata = requests.get(api_url, headers=api.header).json()
                     return responsedata
 
             @classmethod
-            def vol_run(cls, currency: str, maturity: str):
+            def vol_run(self, currency: str, maturity: str):
                 """
                 :param currency: BTC | ETH
                 :type currency:
                 :param maturity: Uppercase (DMMMYY), e.g., 30JUN23 or "all" ,Check analytics/options/maturities for more information about available maturity
                 :type maturity:
                 :return: Volatility run data provides insights into the implied volatility and option parameters at different delta levels, allowing users to analyze the market's perception of potential price movements and risk profiles across various option strikes. By retrieving the volatility run data, traders, investors, and analysts can assess the relative pricing and skewness of options at different delta levels, identify potential opportunities for trading strategies, and gain a deeper understanding of market sentiment and risk perception   and risk perception.
                 :rtype:
                 """
                 currency = currency.upper()
                 maturity = maturity.upper()
-                api_url = cls.url + "model_charts/vol_run/" + currency + "/" + maturity
+                api_url = self.url + "model_charts/vol_run/" + currency + "/" + maturity
                 responsedata = requests.get(api_url, headers=api.header).json()
                 return responsedata
 
             @classmethod
-            def forward_curve(cls, currency: str):
+            def forward_curve(self, currency: str):
                 """
                 :param currency: BTC | ETH
                 :type currency:
                 :return: The forward curve is an essential tool in options pricing and risk management. It provides insights into the relationship between the time-to-maturity (TTM) and the corresponding forward prices for options. By retrieving the forward curve data, traders, investors, and analysts can assess the term structure of options prices, identify potential market inefficiencies or mispricings, and make informed decisions regarding options trading and portfolio management
                 :rtype:
                 """
                 currency = currency.upper()
-                api_url = cls.url + "model_charts/forward_curve/" + currency
+                api_url = self.url + "model_charts/forward_curve/" + currency
                 responsedata = requests.get(api_url, headers=api.header).json()
                 return responsedata
 
             @classmethod
-            def term_structure_atm(cls, currency: str, timelapse: False):
+            def term_structure_atm(self, currency: str, timelapse: False):
                 """
                 :param currency: BTC | ETH
                 :type currency:
                 :param timelapse: True or False
                 :type timelapse:
                 :return: The term structure provides valuable insights into the relationship between the time-to-maturity (TTM) and the corresponding implied volatility (IV) for ATM options. Implied volatility is a critical component in options pricing, representing the market's expectation of future price volatility of the underlying asset. By analyzing the term structure, traders, investors, and analysts can gain insights into the market's perception of future volatility at different tenors and expiries
                 :rtype:
                 """
                 currency = currency.upper()
                 if timelapse is True:
-                    api_url = cls.url + "model_charts/term_structure_atm/" + currency + '/time_lapse'
+                    api_url = self.url + "model_charts/term_structure_atm/" + currency + '/time_lapse'
                     responsedata = requests.get(api_url, headers=api.header).json()
                     return responsedata
                 else:
-                    api_url = cls.url + "model_charts/term_structure_atm/" + currency
+                    api_url = self.url + "model_charts/term_structure_atm/" + currency
                     responsedata = requests.get(api_url, headers=api.header).json()
                     return responsedata
 
             @classmethod
-            def term_structure(cls, currency: str, type: str):
+            def term_structure(self, currency: str, type: str):
                 """
                 :param currency: BTC | ETH
                 :type currency:
                 :param type: strike or delta , lowercase
                 :type type:
                 :return: The term structure provides insights into the relationship between a specific parameter (delta or strike) and the corresponding implied volatility (IV) for options with different expiries. By analyzing the term structure, traders, investors, and analysts can identify patterns or anomalies in implied volatility across different option expiries
                 :rtype:
                 """
                 currency = currency.upper()
                 type = type.lower()
-                api_url = cls.url + "model_charts/term_structure/" + currency + "/" + type
+                api_url = self.url + "model_charts/term_structure/" + currency + "/" + type
                 responsedata = requests.get(api_url, headers=api.header).json()
                 return responsedata
 
             @classmethod
-            def skew_currency(cls, currency: str, maturity: str):
+            def skew_currency(self, currency: str, maturity: str):
                 """
                 :param currency: BTC | ETH
                 :type currency:
                 :param maturity: Uppercase (DMMMYY), e.g., 30JUN23 or "all" ,Check analytics/options/maturities for more information about available maturity
                 :type maturity:
                 :return: Skew data provides insights into the market's perception of potential upside or downside risks in the underlying asset
                 :rtype:
                 """
                 currency = currency.upper()
                 maturity = maturity.upper()
-                api_url = cls.url + "skew_currency/" + currency + "/" + maturity
+                api_url = self.url + "skew_currency/" + currency + "/" + maturity
                 responsedata = requests.get(api_url, headers=api.header).json()
                 return responsedata
 
             @classmethod
-            def skew_market(cls, market: str, maturity: str):
+            def skew_market(self, market: str, maturity: str):
                 """
                 :param market: BIT  | DERIBIT  | BYBIT  | OKEX  | POWERTRADE | DELTA_EXCHANGE | LYRA_ARBITRUM | AEVO | BINANCE | LYRA
                 :type market:
                 :param maturity: Uppercase (DMMMYY), e.g., 30JUN23 or "all" ,Check analytics/options/maturities for more information about available maturity
                 :type maturity:
                 :return:  Skew data provides insights into the market's perception of potential upside or downside risks in the underlying asset
                 :rtype:
                 """
                 market = market.upper()
                 maturity = maturity.upper()
-                api_url = cls.url + "skew_market/" + market + "/" + maturity
+                api_url = self.url + "skew_market/" + market + "/" + maturity
                 responsedata = requests.get(api_url, headers=api.header).json()
                 return responsedata
 
             @classmethod
-            def iv_currency(cls, currency: str):
+            def iv_currency(self, currency: str):
                 """
                 :param currency: BTC | ETH  | SOL | ADA | TONCOIN | BNB | XRP | ARB | OP
                 :type currency:
                 :return: Implied volatility (IV) is a key parameter in option pricing models. It represents the market's expectation of the future volatility of the underlying asset. IV data provides insights into the perceived level of risk and uncertainty in the market
                 :rtype:
                 """
                 currency = currency.upper()
-                api_url = cls.url + "iv_currency/" + currency
+                api_url = self.url + "iv_currency/" + currency
                 responsedata = requests.get(api_url, headers=api.header).json()
                 return responsedata
 
             @classmethod
-            def iv_market(cls, market: str):
+            def iv_market(self, market: str):
                 """
                 :param market: BIT  | DERIBIT  | BYBIT  | OKEX  | POWERTRADE | DELTA_EXCHANGE | LYRA_ARBITRUM | AEVO | BINANCE | LYRA
                 :type market:
                 :return: Implied volatility (IV) is a key parameter in option pricing models. It represents the market's expectation of the future volatility of the underlying asset. IV data provides insights into the perceived level of risk and uncertainty in the market
                 :rtype:
                 """
                 market = market.upper()
-                api_url = cls.url + "iv_market/" + market
+                api_url = self.url + "iv_market/" + market
                 responsedata = requests.get(api_url, headers=api.header).json()
                 return responsedata
 
             @classmethod
-            def eth_btc_atm_iv_term_structure(cls):
+            def eth_btc_atm_iv_term_structure(self):
                 """
                 :return: The term structure of at-the-money (ATM) implied volatility (IV) provides valuable information about the market's expectations of future volatility for Ethereum-Bitcoin (ETH-BTC) options. By analyzing the IV term structure, traders and investors can gain insights into how the market perceives the potential price movements of ETH-BTC options over different time periods
                 :rtype:
                 """
-                api_url = cls.url + "eth-btc_atm_iv_term_structure"
+                api_url = self.url + "eth-btc_atm_iv_term_structure"
                 responsedata = requests.get(api_url, headers=api.header).json()
                 return responsedata
 
             @classmethod
-            def skew_currency_market(cls, currency: str, market: str):
+            def skew_currency_market(self, currency: str, market: str):
                 """
                 :param market: BIT  | DERIBIT  | BYBIT  | OKEX  | POWERTRADE | DELTA_EXCHANGE | LYRA_ARBITRUM | AEVO | BINANCE | LYRA
                 :type market:
                 :param currency: BTC | ETH
                 :type currency:
                 :return: Skew data provides insights into the market's perception of potential upside or downside risks in the underlying asset
                 :rtype:
                 """
                 currency = currency.upper()
                 market = market.upper()
-                api_url = cls.url + "skew/" + market + "/" + currency
+                api_url = self.url + "skew/" + market + "/" + currency
                 responsedata = requests.get(api_url, headers=api.header).json()
                 return responsedata
 
         class futures:
             url = "https://api.laevitas.ch/analytics/futures/"
             pass
 
             @classmethod
-            def instruments(cls):
+            def instruments(self):
                 """
                 :return: This endpoint provides information about futures instruments, including the market, type, currency, instrument name or identifier, and expiry date.
                 :rtype:
                 """
-                api_url = cls.url + "instruments"
+                api_url = self.url + "instruments"
                 responsedata = requests.get(api_url, headers=api.header).json()
                 return responsedata
 
             @classmethod
-            def alt_currency(cls):
+            def alt_currency(self):
                 """
                 :return: json data of available futures currency
                 :rtype:
                 """
-                api_url = cls.url + "alt_currency"
+                api_url = self.url + "alt_currency"
                 responsedata = requests.get(api_url, headers=api.header).json()
                 return responsedata
 
             @classmethod
-            def perpetual_funding(cls, currency: str, type=""):
+            def perpetual_funding(self, currency: str, type=""):
                 """
 
                 :param currency: BTC,ETH ... Check analytics/futures/alt_currency For more information about available currencies
                 :type currency:
                 :param type: optional , c or d (centralized , decentralized)
                 :type type:
                 :return: This endpoint provides information about the funding rates and yields of perpetual contracts for a specific currency
                 :rtype:
                 """
                 currency = currency.upper()
                 if len(type) == 1:
-                    api_url = cls.url + "perpetual_funding/" + currency + "/" + type.lower()
+                    api_url = self.url + "perpetual_funding/" + currency + "/" + type.lower()
                     responsedata = requests.get(api_url, headers=api.header).json()
                 else:
-                    api_url = cls.url + "perpetual_funding/" + currency
+                    api_url = self.url + "perpetual_funding/" + currency
                     responsedata = requests.get(api_url, headers=api.header).json()
                 return responsedata
 
             @classmethod
-            def futures_yield(cls, currency: str):
+            def futures_yield(self, currency: str):
                 """
 
                 :param currency: ADA,BCH,BNB ... Check analytics/futures/alt_currency For more information about available currencies
                 :type currency:
                 :return: This endpoint provides information about the yield values of futures contracts for a specific currency.
                 :rtype:
                 """
                 currency = currency.upper()
-                api_url = cls.url + "futures_yield/" + currency
+                api_url = self.url + "futures_yield/" + currency
                 responsedata = requests.get(api_url, headers=api.header).json()
                 return responsedata
 
             @classmethod
-            def futures_basis(cls, currency: str):
+            def futures_basis(self, currency: str):
                 """
                 :param currency: ADA,BCH,BNB ... Check analytics/futures/alt_currency For more information about available currencies
                 :type currency:
                 :return: This endpoint provides information about the basis values of futures contracts for a specific currency.
                 :rtype:
                 """
                 currency = currency.upper()
-                api_url = cls.url + "futures_basis/" + currency
+                api_url = self.url + "futures_basis/" + currency
                 responsedata = requests.get(api_url, headers=api.header).json()
                 return responsedata
 
             @classmethod
-            def volume_breakdown(cls, currency: str, type=""):
+            def volume_breakdown(self, currency: str, type=""):
                 """
 
                 :param currency: BTC,ETH ... Check analytics/futures/alt_currency For more information about available currencies
                 :type currency:
                 :param type: optional , c or d (centralized , decentralized)
                 :type type:
                 :return: This endpoint retrieves volume breakdown data for a specific currency and type. The response includes the volume values in USD for different markets, categorized by all types, futures, and perpetual contracts.
                 :rtype:
                 """
                 currency = currency.upper()
                 if len(type) == 1:
-                    api_url = cls.url + "volume_breakdown/" + currency + '/' + type.lower()
+                    api_url = self.url + "volume_breakdown/" + currency + '/' + type.lower()
                     responsedata = requests.get(api_url, headers=api.header).json()
                 else:
-                    api_url = cls.url + "volume_breakdown/" + currency
+                    api_url = self.url + "volume_breakdown/" + currency
                     responsedata = requests.get(api_url, headers=api.header).json()
                 return responsedata
 
             @classmethod
-            def oi_breakdown(cls, currency: str, type=""):
+            def oi_breakdown(self, currency: str, type=""):
                 """
 
                 :param currency: BTC,ETH ... Check analytics/futures/alt_currency For more information about available currencies
                 :type currency:
                 :param type: optional , c or d (centralized , decentralized)
                 :type type:
                 :return: This endpoint retrieves open interest breakdown data for a specific currency and type. The response includes the open interest values in USD for different markets, categorized by all types, futures, and perpetual contracts.
                 :rtype:
                 """
                 currency = currency.upper()
                 if len(type) == 1:
-                    api_url = cls.url + "oi_breakdown/" + currency + '/' + type.lower()
+                    api_url = self.url + "oi_breakdown/" + currency + '/' + type.lower()
                     responsedata = requests.get(api_url, headers=api.header).json()
                 else:
-                    api_url = cls.url + "oi_breakdown/" + currency
+                    api_url = self.url + "oi_breakdown/" + currency
                     responsedata = requests.get(api_url, headers=api.header).json()
 
                 return responsedata
 
             @classmethod
-            def futures_curve(cls, currency: str, market=""):
+            def futures_curve(self, currency: str, market=""):
                 """
 
                 :param currency: ADA,BCH,BNB ... Check analytics/futures/alt_currency For more information about available currencies
                 :type currency:
                 :param market: (optional) BINANCE, BITMEX , BITGET , DERIBIT, HUOBI, KRAKEN, BYBIT , OKEX
                 :type market:
                 :return: This endpoint provides information about the futures curve for a specific currency and market.
                 :rtype:
                 """
                 currency = currency.upper()
                 if len(market) >= 1:
                     market = market.upper()
-                    api_url = cls.url + "futures_curve/" + currency + "/" + market
+                    api_url = self.url + "futures_curve/" + currency + "/" + market
                     responsedata = requests.get(api_url, headers=api.header).json()
                 else:
-                    api_url = cls.url + "futures_curve/" + currency
+                    api_url = self.url + "futures_curve/" + currency
                     responsedata = requests.get(api_url, headers=api.header).json()
                 return responsedata
 
             @classmethod
-            def markets_oi_gainers_and_losers(cls, currency: str, option: str, hour: str, type=""):
+            def markets_oi_gainers_and_losers(self, currency: str, option: str, hour: str, type=""):
                 """
 
                 :param currency: BTC,ETH,ADA,BCH,BNB ... Check analytics/futures/alt_currency For more information about available currencies
                 :type currency:
                 :param option: perpetual, future , all
                 :type option:
                 :param hour: 1, 2, 4, 8, 12, 18, 24, 48, 168, 336, 504, 720, ytd
@@ -994,168 +992,168 @@
                 :param type: optional , c or d (centralized , decentralized)
                 :type type:
                 :return: This endpoint provides information about the gainers and losers in open interest for futures markets of a specific currency, based on the specified option and parameter
                 :rtype:
                 """
                 currency = currency.upper()
                 if len(type) == 1:
-                    api_url = cls.url + "markets_oi_gainers_and_losers/" + currency + "/" + option.lower() + "/" + str(
+                    api_url = self.url + "markets_oi_gainers_and_losers/" + currency + "/" + option.lower() + "/" + str(
                         hour) + "/" + type.lower()
                     responsedata = requests.get(api_url, headers=api.header).json()
                 else:
-                    api_url = cls.url + "markets_oi_gainers_and_losers/" + currency + "/" + option.lower() + "/" + str(
+                    api_url = self.url + "markets_oi_gainers_and_losers/" + currency + "/" + option.lower() + "/" + str(
                         hour)
                     responsedata = requests.get(api_url, headers=api.header).json()
                 return responsedata
 
             @classmethod
-            def snapshot(cls, market: str):
+            def snapshot(self, market: str):
                 """
 
                 :param market: BINANCE, BITMEX, DERIBIT, HUOBI, KRAKEN, BYBIT , OKX
                 :type market:
                 :return: This endpoint retrieves snapshot data for a specific futures market. The response includes information such as bid price, ask price, volume, open interest, and other relevant details about the futures contract.
                 :rtype:
                 """
                 market = market.upper()
                 if market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "snapshot/" + market
+                    api_url = self.url + "snapshot/" + market
                     responsedata = requests.get(api_url, headers=api.header).json()
                     return responsedata
 
             @classmethod
-            def aggregated_future_summary(cls, currency: str):
+            def aggregated_future_summary(self, currency: str):
                 """
                 :param currency: BTC,ETH,LTC ... Check analytics/futures/alt_currency For more information about available currencies
                 :type currency:
                 :return: This endpoint retrieves aggregated future summary data for a specific currency. The response includes information such as the future symbol, currency, expiry date, price, open interest, open interest notional, volume, volume notional, yield, basis, open interest volume, and markets associated with the future.
                 :rtype:
                 """
                 currency = currency.upper()
-                api_url = cls.url + "aggregated_future_summary/" + currency
+                api_url = self.url + "aggregated_future_summary/" + currency
                 responsedata = requests.get(api_url, headers=api.header).json()
                 return responsedata
 
             @classmethod
-            def aggregated_option_summary(cls, currency: str):
+            def aggregated_option_summary(self, currency: str):
                 """
                 :param currency: BTC,ETH,LTC ... Check analytics/futures/alt_currency For more information about available currencies
                 :type currency:
                 :return: This endpoint retrieves aggregated option summary data for a specific currency. The response includes information such as the option symbol, currency, expiry date, price, open interest, open interest notional, volume, volume notional, yield, basis, open interest volume, and markets associated with the option.
                 :rtype:
                 """
                 currency = currency.upper()
-                api_url = cls.url + "aggregated_option_summary/" + currency
+                api_url = self.url + "aggregated_option_summary/" + currency
                 responsedata = requests.get(api_url, headers=api.header).json()
                 return responsedata
 
         class defi:
             url = "https://api.laevitas.ch/analytics/defi/"
             pass
 
             @classmethod
-            def dovs(cls):
+            def dovs(self):
                 """
                 :return: json data of DOVs weekly auctions
                 :rtype:
                 """
-                api_url = cls.url + "dovs"
+                api_url = self.url + "dovs"
                 responsedata = requests.get(api_url, headers=api.header).json()
                 return responsedata
 
             @classmethod
-            def ribbon(cls):
+            def ribbon(self):
                 """
                 :return: json data of ribbon weekly auctions
                 :rtype:
                 """
-                api_url = cls.url + "ribbon"
+                api_url = self.url + "ribbon"
                 responsedata = requests.get(api_url, headers=api.header).json()
                 return responsedata
 
             @classmethod
-            def friktion(cls):
+            def friktion(self):
                 """
                 :return: json data of friktion weekly auctions
                 :rtype:
                 """
-                api_url = cls.url + "friktion"
+                api_url = self.url + "friktion"
                 responsedata = requests.get(api_url, headers=api.header).json()
                 return responsedata
 
             @classmethod
-            def squeeth(cls):
+            def squeeth(self):
                 """
                 :return: json data of squeeth live data
                 :rtype:
                 """
-                api_url = cls.url + "squeeth"
+                api_url = self.url + "squeeth"
                 responsedata = requests.get(api_url, headers=api.header).json()
                 return responsedata
 
         class derivs:
             url = "https://api.laevitas.ch/analytics/derivs/"
             pass
 
             @classmethod
-            def futures(cls, market: str, currency: str, maturity: str):
+            def futures(self, market: str, currency: str, maturity: str):
                 """
 
                 :param market: Full list of supported exchanges on instruments endpoint (futures.instrument function),exp: BITMEX | BINANCE | BYBIT | DYDX | BITFINEX | DERIBIT | HUOBI | KRAKEN | OKEX | GMX | PERP-PROTOCOL
                 :type market:
                 :param currency: BTC | ETH... Check analytics/futures/alt_currency For more information about available currencies
                 :type currency:
                 :param maturity: Uppercase (DMMMYY), e.g., 30JUN23, Check analytics/futures/instruments for more information about available maturity
                 :type maturity:
                 :return: json data of futures live data
                 :rtype:
                 """
                 market = market.upper()
                 maturity = maturity.upper()
-                api_url = cls.url + "futures/" + market + "/" + currency.lower() + "/" + maturity
+                api_url = self.url + "futures/" + market + "/" + currency.lower() + "/" + maturity
                 responsedata = requests.get(api_url, headers=api.header).json()
                 return responsedata
 
             @classmethod
-            def perpetuals(cls, market: str, currency: str):
+            def perpetuals(self, market: str, currency: str):
                 """
 
                 :param market: Full list of supported exchanges on instruments endpoint (futures.instrument function),exp: BITMEX | BINANCE | BYBIT | DYDX | BITFINEX | DERIBIT | HUOBI | KRAKEN | OKEX | GMX | PERP-PROTOCOL
                 :type market:
                 :param currency: BTC | ETH... Check analytics/futures/alt_currency For more information about available currencies
                 :type currency:
                 :return: json live data of perpetual swaps
                 :rtype:
                 """
                 market = market.upper()
                 currency = currency.upper()
-                api_url = cls.url + "perpetuals/" + market + "/" + currency.lower()
+                api_url = self.url + "perpetuals/" + market + "/" + currency.lower()
                 responsedata = requests.get(api_url, headers=api.header).json()
                 return responsedata
 
             @classmethod
-            def summary(cls, currency=""):
+            def summary(self, currency=""):
                 """
                 :param currency: BTC | ETH... Check analytics/futures/alt_currency For more information about available currencies
                 :type currency:
                 :return: json data of aggregated perps summary
                 :rtype:
                 """
                 if len(currency) >= 1:
-                    api_url = cls.url + "summary/" + currency.lower()
+                    api_url = self.url + "summary/" + currency.lower()
                     responsedata = requests.get(api_url, headers=api.header).json()
                 else:
-                    api_url = cls.url + "summary"
+                    api_url = self.url + "summary"
                     responsedata = requests.get(api_url, headers=api.header).json()
                 return responsedata
 
             @classmethod
-            def oi_gainers(cls, market: str, oitype: str, period: str):
+            def oi_gainers(self, market: str, oitype: str, period: str):
                 """
                 :param market: Full list of supported exchanges on instruments endpoint (futures.instrument function),exp: BITMEX | BINANCE | BYBIT | DYDX | BITFINEX | DERIBIT | HUOBI | KRAKEN | OKEX | GMX | PERP-PROTOCOL
                 :type market:
                 :param oitype: future, perpetual
                 :type oitype:
                 :param period: 1, 2, 4, 8, 12, 18, 24, 48, 168, 336, 504, 720, ytd
                 :type period:
@@ -1165,20 +1163,20 @@
                 market = market.upper()
                 oitype = oitype.upper()
                 if oitype not in ["future", "perpetual"]:
                     raise TypeError("Type not available")
                 elif str(period) not in ["1", "2", "4", "8", "12", "18", "24", "48", "168", "336", "504", "720", "ytd"]:
                     raise TypeError("period not available")
                 else:
-                    api_url = cls.url + "oi_gainers/" + market + "/" + oitype.lower() + "/" + str(period)
+                    api_url = self.url + "oi_gainers/" + market + "/" + oitype.lower() + "/" + str(period)
                     responsedata = requests.get(api_url, headers=api.header).json()
                 return responsedata
 
             @classmethod
-            def price_gainers(cls, market: str, oitype: str, period: str):
+            def price_gainers(self, market: str, oitype: str, period: str):
                 """
 
                 :param market: Full list of supported exchanges on instruments endpoint (futures.instrument function),exp: BITMEX | BINANCE | BYBIT | DYDX | BITFINEX | DERIBIT | HUOBI | KRAKEN | OKEX | GMX | PERP-PROTOCOL
                 :type market:
                 :param oitype: future, perpetual
                 :type oitype:
                 :param period: 1, 2, 4, 8, 12, 18, 24, 48, 168, 336, 504, 720, ytd
@@ -1188,74 +1186,74 @@
                 """
                 market = market.upper()
                 if oitype not in ["future", "perpetual"]:
                     raise TypeError("Type not available")
                 elif str(period) not in ["1", "2", "4", "8", "12", "18", "24", "48", "168", "336", "504", "720", "ytd"]:
                     raise TypeError("period not available")
                 else:
-                    api_url = cls.url + "price_gainers/" + market + "/" + oitype.lower() + "/" + str(period)
+                    api_url = self.url + "price_gainers/" + market + "/" + oitype.lower() + "/" + str(period)
                     responsedata = requests.get(api_url, headers=api.header).json()
                 return responsedata
 
             @classmethod
-            def perpetuals_snapshot(cls, market: str):
+            def perpetuals_snapshot(self, market: str):
                 """
                 :param market: deribit, binance , okx, bybit
                 :type market
                 :return: json live data of perpetual swaps
                 :rtype:
                 """
                 market = market.lower()
-                api_url = cls.url + "perpetuals_snapshot/" + market
+                api_url = self.url + "perpetuals_snapshot/" + market
                 responsedata = requests.get(api_url, headers=api.header).json()
                 return responsedata
 
             @classmethod
-            def top_funding(cls, market: str):
+            def top_funding(self, market: str):
                 """
 
                 :param market: Full list of supported exchanges on instruments endpoint (futures.instrument function),exp: BITMEX | BINANCE | FTX | BYBIT | DYDX | BITFINEX | DERIBIT | HUOBI | KRAKEN | OKEX
                 :type market:
                 :return: json data of top funding
                 :rtype:
                 """
                 market = market.upper()
                 if market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "top_funding/" + market
+                    api_url = self.url + "top_funding/" + market
                     responsedata = requests.get(api_url, headers=api.header).json()
                     return responsedata
 
             @classmethod
-            def top_gainers_losers(cls, change: str, type: str):
+            def top_gainers_losers(self, change: str, type: str):
                 """
 
                 :param change: 1, 2, 4, 8, 12, 18, 24, 48, 168, 336, 504, 720
                 :type change:
                 :param type: gainers , losers
                 :type type:
                 :return: json data of top gainers and losers
                 :rtype:
                 """
 
-                api_url = cls.url + "top_gainers_losers/" + change + "/" + type
+                api_url = self.url + "top_gainers_losers/" + change + "/" + type
                 responsedata = requests.get(api_url, headers=api.header).json()
                 return responsedata
 
     class historical:
         def __init__(self):
             self.option = self.options()
 
         class options:
             url = "https://api.laevitas.ch/historical/options/"
             pass
 
             @classmethod
-            def option(cls, market: str, instrument: str, start: str, end: str, limit="", page="", granularity=""):
+            def option(self, market: str, instrument: str, start: str, end: str, limit="", page="", granularity=""):
                 """
                 :param market: BIT, DERIBIT, OKEX, POWERTRADE, BINANCE, DELTA_EXCHANGE, AEVO, LYRA , LYRA_ARBITRUM, BYBIT
                 :type market:
                 :param instrument: Currency-Maturity-Strike-C/P e.g., BTC-30JUN23-80000-C Check analytics/options/Instruments for more information about available instrument
                 :type instrument:
                 :param start: EXP:2023-07-11
                 :type end:
@@ -1275,23 +1273,23 @@
                 x = instrument.split("-")
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
                 if len(x) != 4:
                     raise TypeError("wrong instrument")
                 elif x[3] not in ["P", "C"]:
                     raise TypeError("type in instument is either C or P")
                 elif makequery != "":
-                    api_url = cls.url + market + "/" + instrument + makequery
+                    api_url = self.url + market + "/" + instrument + makequery
                     response = requests.get(api_url, headers=api.header).json()
                 else:
-                    api_url = cls.url + market + "/" + instrument
+                    api_url = self.url + market + "/" + instrument
                     response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def iv(cls, market: str, instrument: str, start: str, end: str, limit="", page="", granularity=""):
+            def iv(self, market: str, instrument: str, start: str, end: str, limit="", page="", granularity=""):
                 """
                 :param market: BIT, DERIBIT, OKEX, POWERTRADE, BINANCE, DELTA_EXCHANGE, AEVO, LYRA , LYRA_ARBITRUM, BYBIT
                 :type market:
                 :param instrument: Currency-Maturity-Strike-C/P e.g., BTC-30JUN23-80000-C Check analytics/options/Instruments for more information about available instrument
                 :type instrument:
                 :param start: EXP:2023-07-11
                 :type end:
@@ -1313,23 +1311,23 @@
                 if len(x) != 4:
                     raise TypeError("wrong instrument")
                 elif x[3] not in ["P", "C"]:
                     raise TypeError("type in instument is either C or P")
                 elif market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 elif makequery != "":
-                    api_url = cls.url + "iv/" + market + "/" + instrument + makequery
+                    api_url = self.url + "iv/" + market + "/" + instrument + makequery
                     response = requests.get(api_url, headers=api.header).json()
                 else:
-                    api_url = cls.url + "iv/" + market + "/" + instrument
+                    api_url = self.url + "iv/" + market + "/" + instrument
                     response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def price(cls, market: str, instrument: str, start: str, end: str, limit="", page="", granularity=""):
+            def price(self, market: str, instrument: str, start: str, end: str, limit="", page="", granularity=""):
                 """
                 :param market: BIT, DERIBIT, OKEX, POWERTRADE, BINANCE, DELTA_EXCHANGE, AEVO, LYRA , LYRA_ARBITRUM, BYBIT
                 :type market:
                 :param instrument: Currency-Maturity-Strike-C/P e.g., BTC-30JUN23-80000-C Check analytics/options/Instruments for more information about available instrument
                 :type instrument:
                 :param start: EXP:2023-07-11
                 :type end:
@@ -1351,20 +1349,20 @@
                 if len(x) != 4:
                     raise TypeError("wrong instrument")
                 elif x[3] not in ["P", "C"]:
                     raise TypeError("type in instument is either C or P")
                 elif market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "price/" + market + "/" + instrument + makequery
+                    api_url = self.url + "price/" + market + "/" + instrument + makequery
                     response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def oi_volume(cls, market: str, instrument: str, start: str, end: str, limit="", page="", granularity=""):
+            def oi_volume(self, market: str, instrument: str, start: str, end: str, limit="", page="", granularity=""):
                 """
                 :param market: BIT, DERIBIT, OKEX, POWERTRADE, BINANCE, DELTA_EXCHANGE, AEVO, LYRA , LYRA_ARBITRUM, BYBIT
                 :type market:
                 :param instrument: Currency-Maturity-Strike-C/P e.g., BTC-30JUN23-80000-C Check analytics/options/Instruments for more information about available instrument
                 :type instrument:
                 :param start: EXP:2023-07-11
                 :type end:
@@ -1386,23 +1384,23 @@
                 if len(x) != 4:
                     raise TypeError("wrong instrument")
                 elif x[3] not in ["P", "C"]:
                     raise TypeError("type in instument is either C or P")
                 elif market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 elif makequery != "":
-                    api_url = cls.url + "oi_volume/" + market + "/" + instrument + makequery
+                    api_url = self.url + "oi_volume/" + market + "/" + instrument + makequery
                     response = requests.get(api_url, headers=api.header).json()
                 else:
-                    api_url = cls.url + "oi_volume/" + market + "/" + instrument
+                    api_url = self.url + "oi_volume/" + market + "/" + instrument
                     response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def underlying_price(cls, market: str, instrument: str, start: str, end: str, limit="", page="",
+            def underlying_price(self, market: str, instrument: str, start: str, end: str, limit="", page="",
                                  granularity=""):
                 """
                 :param market: BIT, DERIBIT, OKEX, POWERTRADE, BINANCE, DELTA_EXCHANGE, AEVO, LYRA , LYRA_ARBITRUM, BYBIT
                 :type market:
                 :param instrument: Currency-Maturity-Strike-C/P e.g., BTC-30JUN23-80000-C Check analytics/options/Instruments for more information about available instrument
                 :type instrument:
                 :param start: EXP:2023-07-11
@@ -1425,23 +1423,23 @@
                 if len(x) != 4:
                     raise TypeError("wrong instrument")
                 elif x[3] not in ["P", "C"]:
                     raise TypeError("type in instument is either C or P")
                 elif market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 elif makequery != "":
-                    api_url = cls.url + "underlying_price/" + market + "/" + instrument + makequery
+                    api_url = self.url + "underlying_price/" + market + "/" + instrument + makequery
                     response = requests.get(api_url, headers=api.header).json()
                 else:
-                    api_url = cls.url + "underlying_price/" + market + "/" + instrument
+                    api_url = self.url + "underlying_price/" + market + "/" + instrument
                     response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def oi_strike(cls, market: str, currency: str, maturity: str, date_h: str):
+            def oi_strike(self, market: str, currency: str, maturity: str, date_h: str):
                 """
 
                 :param market: BIT, DERIBIT, OKEX, POWERTRADE, BINANCE, DELTA_EXCHANGE, AEVO, LYRA , LYRA_ARBITRUM, BYBIT
                 :type market:
                 :param currency: BTC,ETH,BCH,SOL,XRP,BNB , Check analytics/options/Instruments for more information about available currencies and instruments
                 :type currency:
                 :param maturity: Uppercase (DMMMYY), e.g., 30JUN23 Check analytics/options/Instruments for more information about available maturity
@@ -1452,20 +1450,20 @@
                 :rtype:
                 """
                 market = market.upper()
                 currency = currency.upper()
                 if market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "oi_strike/" + market.lower() + "/" + currency.lower() + "/" + maturity.upper() + "?date_h=" + date_h
+                    api_url = self.url + "oi_strike/" + market.lower() + "/" + currency.lower() + "/" + maturity.upper() + "?date_h=" + date_h
                     responsedata = requests.get(api_url, headers=api.header).json()
                 return responsedata
 
             @classmethod
-            def volume_strike(cls, market: str, currency: str, maturity: str, date_h: str):
+            def volume_strike(self, market: str, currency: str, maturity: str, date_h: str):
                 """
 
                 :param market: BIT, DERIBIT, OKEX, POWERTRADE, BINANCE, DELTA_EXCHANGE, AEVO, LYRA , LYRA_ARBITRUM, BYBIT
                 :type market:
                 :param currency: BTC,ETH,BCH,SOL,XRP,BNB , Check analytics/options/Instruments for more information about available currencies and instruments
                 :type currency:
                 :param maturity: Uppercase (DMMMYY), e.g., 30JUN23 Check analytics/options/Instruments for more information about available maturity
@@ -1474,42 +1472,46 @@
                 :type date_h :
                 :return: historical options volume data by strike
                 :rtype:
                 """
                 if market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "volume_strike/" + market.upper() + "/" + currency.upper() + "/" + maturity.upper() + "?date_h=" + date_h
+                    api_url = self.url + "volume_strike/" + market.upper() + "/" + currency.upper() + "/" + maturity.upper() + "?date_h=" + date_h
                     responsedata = requests.get(api_url, headers=api.header).json()
                 return responsedata
 
             @classmethod
-            def trades(cls, market: str, currency: str, date: str, limit="", page=""):
+            def trades(self, market: str, currency: str, date: str, limit="", page=""):
                 """
                 :param market: BIT, DERIBIT, OKEX, POWERTRADE, BINANCE, DELTA_EXCHANGE, AEVO, LYRA , LYRA_ARBITRUM, BYBIT
                 :type market:
                 :param currency: BTC,ETH,BCH,SOL,XRP,BNB , Check analytics/options/Instruments for more information about available currencies and instruments
                 :type currency:
+                :param start: EXP:2023-07-11
+                :type end:
+                :param end: EXP:2023-07-18
+                :type end :
                 :param limit: 10
                 :type limit:
                 :param page: 1
                 :type page:
                 :return: historical options volume data by strike
                 :rtype:
                 """
                 if market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
                     makequery = prepare_query(date=date, limit=limit, page=page)
-                    api_url = cls.url + "trades/" + market.upper() + "/" + currency.upper() + makequery
+                    api_url = self.url + "trades/" + market.upper() + "/" + currency.upper() + makequery
                     responsedata = requests.get(api_url, headers=api.header).json()
                 return responsedata
 
             @classmethod
-            def snapshot(cls, market: str, currency: str, start="", end="", limit="10", page="1", timezone=""):
+            def snapshot(self, market: str, currency: str, start="", end="", limit="10", page="1", timezone=""):
                 """
                 :param market: DERIBIT, OKX, BINANCE,BYBIT
                 :type market:
                 :param currency: BTC,ETH,SOL,BNB
                 :type currency:
                 :param start: EXP:2023-07-11
                 :type end:
@@ -1524,20 +1526,20 @@
                 :return: json format data of historical snapshot of options
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, timezone=timezone)
                 if market.upper() not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "snapshot/" + market.lower() + "/" + currency.lower() + makequery
+                    api_url = self.url + "snapshot/" + market.lower() + "/" + currency.lower() + makequery
                     response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def instrument_volume_buy_sell(cls, market: str, instrument: str, start: str, end="", limit="", page=""):
+            def instrument_volume_buy_sell(self, market: str, instrument: str, start: str, end="", limit="", page=""):
                 """
                 :param market: BIT, DERIBIT, OKEX, POWERTRADE, BINANCE, DELTA_EXCHANGE, AEVO, LYRA , LYRA_ARBITRUM, BYBIT
                 :type market:
                 :param instrument: Currency-Maturity-Strike-C/P e.g., BTC-30JUN23-80000-C Check analytics/options/Instruments for more information about available instrument
                 :type instrument:
                 :param start: EXP:2023-07-11
                 :type end:
@@ -1557,20 +1559,20 @@
                 if len(x) != 4:
                     raise TypeError("wrong instrument")
                 elif x[3] not in ["P", "C"]:
                     raise TypeError("type in instument is either C or P")
                 elif market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "instrument_volume_buy_sell/" + market + "/" + instrument + makequery
+                    api_url = self.url + "instrument_volume_buy_sell/" + market + "/" + instrument + makequery
                     response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def total_oi_by_market(cls, market: str, start: str, end: str, limit="", page="", granularity=""):
+            def total_oi_by_market(self, market: str, start: str, end: str, limit="", page="", granularity=""):
                 """
                 :param market: BIT, DERIBIT, OKEX, POWERTRADE, BINANCE, DELTA_EXCHANGE, AEVO, LYRA , LYRA_ARBITRUM, BYBIT
                 :type market:
                 :param start: EXP:2023-07-11
                 :type end:
                 :param end: EXP:2023-07-18
                 :type end :
@@ -1584,20 +1586,20 @@
                 :rtype:
                 """
                 market = market.upper()
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
                 if market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "total/oi_by_market/" + market + makequery
+                    api_url = self.url + "total/oi_by_market/" + market + makequery
                     response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def total_volume_by_market(cls, market: str, start: str, end: str, limit="", page="", granularity=""):
+            def total_volume_by_market(self, market: str, start: str, end: str, limit="", page="", granularity=""):
                 """
                 :param market: BIT, DERIBIT, OKEX, POWERTRADE, BINANCE, DELTA_EXCHANGE, AEVO, LYRA , LYRA_ARBITRUM, BYBIT
                 :type market:
                 :param start: EXP:2023-07-11
                 :type end:
                 :param end: EXP:2023-07-18
                 :type end :
@@ -1611,20 +1613,20 @@
                 :rtype:
                 """
                 market = market.upper()
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
                 if market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "total/volume_by_market/" + market + makequery
+                    api_url = self.url + "total/volume_by_market/" + market + makequery
                     response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def total_oi_by_currency(cls, currency: str, start: str, end: str, limit="", page="", granularity=""):
+            def total_oi_by_currency(self, currency: str, start: str, end: str, limit="", page="", granularity=""):
                 """
                 :param currency: BTC,ETH,SOL,BNB,OP,TONCOIN,ARB,XRP ADA
                 :type currency:
                 :param start: EXP:2023-07-11
                 :type end:
                 :param end: EXP:2023-07-18
                 :type end :
@@ -1634,21 +1636,21 @@
                 :type page:
                 :param granularity: 5m,15m,30m,1h,2h,4h,6h,12h,1d
                 :type end :
                 :return: historical total open interest per currency
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
-                api_url = cls.url + "total/oi_by_currency/" + currency.upper() + makequery
+                api_url = self.url + "total/oi_by_currency/" + currency.upper() + makequery
                 response = requests.get(api_url, headers=api.header).json()
 
                 return response
 
             @classmethod
-            def total_volume_by_currency(cls, currency: str, start: str, end: str, limit="", page="", granularity=""):
+            def total_volume_by_currency(self, currency: str, start: str, end: str, limit="", page="", granularity=""):
                 """
                 :param currency: BTC,ETH,SOL,BNB,OP,TONCOIN,ARB,XRP ADA
                 :type currency:
                 :param start: EXP:2023-07-11
                 :type end:
                 :param end: EXP:2023-07-18
                 :type end :
@@ -1658,21 +1660,21 @@
                 :type page:
                 :param granularity: 5m,15m,30m,1h,2h,4h,6h,12h,1d
                 :type end :
                 :return: historical total volume per currency
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
-                api_url = cls.url + "total/volume_by_currency/" + currency.upper() + makequery
+                api_url = self.url + "total/volume_by_currency/" + currency.upper() + makequery
                 response = requests.get(api_url, headers=api.header).json()
 
                 return response
 
             @classmethod
-            def iv_rv(cls, market: str, currency: str, start: str, end: str, limit="", page="", granularity=""):
+            def iv_rv(self, market: str, currency: str, start: str, end: str, limit="", page="", granularity=""):
                 """
                 :param market: BIT, DERIBIT, OKEX, POWERTRADE, BINANCE, DELTA_EXCHANGE, AEVO, LYRA , LYRA_ARBITRUM, BYBIT
                 :type market:
                 :param currency: BTC,ETH,SOL,BNB,OP,TONCOIN,ARB,XRP ADA
                 :type currency:
                 :param start: EXP:2023-07-11
                 :type end:
@@ -1687,20 +1689,20 @@
                 :return: historical implied volatility (IV) and realized volatility (RV) by market and currency
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
                 if market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "iv_rv/" + market.upper() + "/" + currency.upper() + makequery
+                    api_url = self.url + "iv_rv/" + market.upper() + "/" + currency.upper() + makequery
                     response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def dvol(cls, market: str, currency: str, start: str, end: str, limit="", page="", granularity=""):
+            def dvol(self, market: str, currency: str, start: str, end: str, limit="", page="", granularity=""):
                 """
                 :param market: DERIBIT
                 :type market:
                 :param currency: BTC,ETH
                 :type currency:
                 :param start: EXP:2023-07-11
                 :type end:
@@ -1715,20 +1717,20 @@
                 :return: historical delta volatility (DVOL) data by market and currency
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
                 if market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "dvol/" + market.upper() + "/" + currency.upper() + makequery
+                    api_url = self.url + "dvol/" + market.upper() + "/" + currency.upper() + makequery
                     response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def vix(cls, market: str, currency: str, start: str, end: str, limit="", page="", granularity=""):
+            def vix(self, market: str, currency: str, start: str, end: str, limit="", page="", granularity=""):
                 """
                 :param market: DERIBIT
                 :type market:
                 :param currency: BTC,ETH
                 :type currency:
                 :param start: EXP:2023-07-11
                 :type end:
@@ -1743,20 +1745,20 @@
                 :return: historical volatility index (VIX) data by market and currency
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
                 if market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "vix/" + market.upper() + "/" + currency.upper() + makequery
+                    api_url = self.url + "vix/" + market.upper() + "/" + currency.upper() + makequery
                     response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def oi_total(cls, market: str, currency: str, start: str, end: str, limit="10", page="1", granularity=""):
+            def oi_total(self, market: str, currency: str, start: str, end: str, limit="10", page="1", granularity=""):
                 """
                 :param market: BIT, DERIBIT, OKEX, POWERTRADE, BINANCE, DELTA_EXCHANGE, AEVO, LYRA , LYRA_ARBITRUM, BYBIT
                 :type market:
                 :param currency: BTC,ETH,SOL,BNB,ARB,XRP ADA
                 :type currency:
                 :param start: EXP:2023-07-11
                 :type end:
@@ -1771,20 +1773,20 @@
                 :return: historical total open interest (OI) data by market and currency
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
                 if market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "oi_total/" + market.upper() + "/" + currency.upper() + makequery
+                    api_url = self.url + "oi_total/" + market.upper() + "/" + currency.upper() + makequery
                     response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def oi_pc_ratio(cls, market: str, currency: str, start: str, end: str, limit="10", page="1",
+            def oi_pc_ratio(self, market: str, currency: str, start: str, end: str, limit="10", page="1",
                             granularity=""):
                 """
                 :param market: BIT, DERIBIT, OKEX, POWERTRADE, BINANCE, DELTA_EXCHANGE, AEVO, LYRA , LYRA_ARBITRUM, BYBIT
                 :type market:
                 :param currency: BTC,ETH,SOL,BNB,ARB,XRP ADA
                 :type currency:
                 :param start: EXP:2023-07-11
@@ -1800,20 +1802,20 @@
                 :return: historical pull cal ratio (PC) data by market and currency
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
                 if market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "oi_pc_ratio/" + market.upper() + "/" + currency.upper() + makequery
+                    api_url = self.url + "oi_pc_ratio/" + market.upper() + "/" + currency.upper() + makequery
                     response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def volume_total(cls, market: str, currency: str, start: str, end: str, limit="10", page="1",
+            def volume_total(self, market: str, currency: str, start: str, end: str, limit="10", page="1",
                              granularity=""):
                 """
                  :param market: BIT, DERIBIT, OKEX, POWERTRADE, BINANCE, DELTA_EXCHANGE, AEVO, LYRA , LYRA_ARBITRUM, BYBIT
                  :type market:
                  :param currency: BTC,ETH,SOL,BNB,ARB,XRP ADA
                  :type currency:
                  :param start: EXP:2023-07-11
@@ -1829,20 +1831,20 @@
                  :return: historical total volume data by market and currency
                  :rtype:
                  """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
                 if market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "volume_total/" + market.upper() + "/" + currency.upper() + makequery
+                    api_url = self.url + "volume_total/" + market.upper() + "/" + currency.upper() + makequery
                     response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def atm_iv(cls, market: str, currency: str, start: str, end: str, limit="10", page="1", granularity=""):
+            def atm_iv(self, market: str, currency: str, start: str, end: str, limit="10", page="1", granularity=""):
                 """
                  :param market: BIT, DERIBIT, OKEX, POWERTRADE, BINANCE, DELTA_EXCHANGE, AEVO, LYRA , LYRA_ARBITRUM, BYBIT
                  :type market:
                  :param currency: BTC,ETH,SOL,BNB,ARB,XRP ADA, TONCOIN
                  :type currency:
                  :param start: EXP:2023-07-11
                  :type end:
@@ -1857,20 +1859,20 @@
                  :return: historical ATM implied volatility data by market and currency
                  :rtype:
                  """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
                 if market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "atm_iv/" + market.upper() + "/" + currency.upper() + makequery
+                    api_url = self.url + "atm_iv/" + market.upper() + "/" + currency.upper() + makequery
                     response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def gex_index(cls, market: str, currency: str, start: str, end: str, limit="10", page="1", granularity=""):
+            def gex_index(self, market: str, currency: str, start: str, end: str, limit="10", page="1", granularity=""):
                 """
                  :param market: BIT, DERIBIT, OKEX, POWERTRADE, BINANCE, DELTA_EXCHANGE, AEVO, LYRA , LYRA_ARBITRUM, BYBIT
                  :type market:
                  :param currency: BTC,ETH,SOL,BNB,ARB,XRP ADA
                  :type currency:
                  :param start: EXP:2023-07-11
                  :type end:
@@ -1885,20 +1887,20 @@
                  :return: historical GEX index data by market and currency
                  :rtype:
                  """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
                 if market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "gex_index/" + market.upper() + "/" + currency.upper() + makequery
+                    api_url = self.url + "gex_index/" + market.upper() + "/" + currency.upper() + makequery
                     response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def max_pain(cls, market: str, currency: str, start: str, end: str, limit="10", page="1", granularity=""):
+            def max_pain(self, market: str, currency: str, start: str, end: str, limit="10", page="1", granularity=""):
                 """
                  :param market: AGGREGATE, BIT, DERIBIT, OKEX, POWERTRADE, BINANCE, DELTA_EXCHANGE, AEVO, LYRA , LYRA_ARBITRUM, BYBIT
                  :type market:
                  :param currency: BTC,ETH,SOL,BNB,ARB,XRP ADA, TONCOIN
                  :type currency:
                  :param start: EXP:2023-07-11
                  :type end:
@@ -1913,20 +1915,20 @@
                  :return: historical MAX pain data by market and currency
                  :rtype:
                  """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
                 if market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "max_pain/" + market.upper() + "/" + currency.upper() + makequery
+                    api_url = self.url + "max_pain/" + market.upper() + "/" + currency.upper() + makequery
                     response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def volume_pc_ratio(cls, market: str, currency: str, start: str, end: str, limit="10", page="1",
+            def volume_pc_ratio(self, market: str, currency: str, start: str, end: str, limit="10", page="1",
                                 granularity=""):
                 """
                  :param market: AGGREGATE, BIT, DERIBIT, OKEX, POWERTRADE, BINANCE, DELTA_EXCHANGE, AEVO, LYRA , LYRA_ARBITRUM, BYBIT
                  :type market:
                  :param currency: BTC,ETH,SOL,BNB,ARB,XRP ADA, TONCOIN
                  :type currency:
                  :param start: EXP:2023-07-11
@@ -1942,20 +1944,20 @@
                  :return: historical pull/call ratio data by market and currency
                  :rtype:
                  """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
                 if market not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "volume_pc_ratio/" + market.upper() + "/" + currency.upper() + makequery
+                    api_url = self.url + "volume_pc_ratio/" + market.upper() + "/" + currency.upper() + makequery
                     response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def iv_bid_ask(cls, market: str, currency: str, type: str, start: str, end: str, limit="10", page="1",
+            def iv_bid_ask(self, market: str, currency: str, type: str, start: str, end: str, limit="10", page="1",
                            granularity=""):
                 """
                 :param market: BYBIT, DERIBIT,
                 :type market:
                 :param currency: BTC,ETH,SOL
                 :type currency:
                 :param type: p_25, p_10, c_25, c_10 , p_atm , c_atm
@@ -1973,20 +1975,20 @@
                 :return: historical implied volatility bid ask by market currency and type
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
                 if market.upper() not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "type/iv_bid_ask/" + market.lower() + "/" + currency.lower() + "/" + type + makequery
+                    api_url = self.url + "type/iv_bid_ask/" + market.lower() + "/" + currency.lower() + "/" + type + makequery
                     response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def atm_iv_model(cls, market: str, currency: str, type: str, start: str, end: str, limit="10", page="1",
+            def atm_iv_model(self, market: str, currency: str, type: str, start: str, end: str, limit="10", page="1",
                              granularity=""):
                 """
                 :param market: DERIBIT
                 :type market:
                 :param currency: BTC,ETH
                 :type currency:
                 :param type: 25P ,15P, 10P , 25C, 10C, 15C, 25C, 35C, 35P, ATM
@@ -2004,20 +2006,20 @@
                 :return: historical At-The-Money Implied Volatility (ATM IV) Model data for the specified currency, market, and option type.
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
                 if market.upper() not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "type/butterfly_model/" + market.lower() + "/" + currency.lower() + "/" + type + makequery
+                    api_url = self.url + "type/butterfly_model/" + market.lower() + "/" + currency.lower() + "/" + type + makequery
                     response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def butterfly(cls, market: str, currency: str, type: str, start: str, end: str, limit="10", page="1",
+            def butterfly(self, market: str, currency: str, type: str, start: str, end: str, limit="10", page="1",
                           granularity=""):
                 """
                 :param market: BIT, DERIBIT, OKEX, POWERTRADE, BINANCE, DELTA_EXCHANGE, AEVO, LYRA , LYRA_ARBITRUM, BYBIT
                 :type market:
                 :param currency: BTC,ETH,SOL,BNB,ARB,XRP ADA, TONCOIN
                 :type currency:
                 :param type:  10D , 25D
@@ -2035,20 +2037,20 @@
                 :return: historical butterfly data by market currency and type
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
                 if market.upper() not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "type/butterfly/" + market.lower() + "/" + currency.lower() + "/" + type + makequery
+                    api_url = self.url + "type/butterfly/" + market.lower() + "/" + currency.lower() + "/" + type + makequery
                     response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def butterfly_model(cls, market: str, currency: str, type: str, start: str, end: str, limit="10", page="1",
+            def butterfly_model(self, market: str, currency: str, type: str, start: str, end: str, limit="10", page="1",
                                 granularity=""):
                 """
                 :param market: DERIBIT
                 :type market:
                 :param currency: BTC,ETH
                 :type currency:
                 :param type: 25D , 15D, 10D, 35D
@@ -2066,20 +2068,20 @@
                 :return: historical butterfly model data by market currency and type
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
                 if market.upper() not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "type/butterfly_model/" + market.lower() + "/" + currency.lower() + "/" + type + makequery
+                    api_url = self.url + "type/butterfly_model/" + market.lower() + "/" + currency.lower() + "/" + type + makequery
                     response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def skew(cls, market: str, currency: str, type: str, start: str, end: str, limit="10", page="1",
+            def skew(self, market: str, currency: str, type: str, start: str, end: str, limit="10", page="1",
                      granularity=""):
                 """
                 :param market: BIT, DERIBIT, OKEX, POWERTRADE, BINANCE, DELTA_EXCHANGE, AEVO, LYRA , LYRA_ARBITRUM, BYBIT
                 :type market:
                 :param currency: BTC,ETH,SOL,BNB,ARB,XRP ADA
                 :type currency:
                 :param type:  10D , 25D
@@ -2097,20 +2099,20 @@
                 :return: historical skew data by market currency and type
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
                 if market.upper() not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "type/skew/" + market.lower() + "/" + currency.lower() + "/" + type + makequery
+                    api_url = self.url + "type/skew/" + market.lower() + "/" + currency.lower() + "/" + type + makequery
                     response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def skew_model(cls, market: str, currency: str, type: str, start: str, end: str, limit="10", page="1",
+            def skew_model(self, market: str, currency: str, type: str, start: str, end: str, limit="10", page="1",
                            granularity=""):
                 """
                 :param market: DERIBIT
                 :type market:
                 :param currency: BTC,ETH
                 :type currency:
                 :param type: 25D , 15D, 10D, 35D
@@ -2128,20 +2130,20 @@
                 :return: historical skew model by market currency and type
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
                 if market.upper() not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "type/skew_model/" + market.lower() + "/" + currency.lower() + "/" + type + makequery
+                    api_url = self.url + "type/skew_model/" + market.lower() + "/" + currency.lower() + "/" + type + makequery
                     response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def risk_reversal(cls, market: str, currency: str, type: str, start: str, end: str, limit="10", page="1",
+            def risk_reversal(self, market: str, currency: str, type: str, start: str, end: str, limit="10", page="1",
                               granularity=""):
                 """
                 :param market: BIT, DERIBIT, OKEX, POWERTRADE, BINANCE, DELTA_EXCHANGE, AEVO, LYRA , LYRA_ARBITRUM, BYBIT
                 :type market:
                 :param currency: BTC,ETH,SOL,BNB,ARB,XRP ADA
                 :type currency:
                 :param type:  10D , 25D
@@ -2159,20 +2161,20 @@
                 :return: historical risk reversal data by market currency and type
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
                 if market.upper() not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "type/risk_reversal/" + market.lower() + "/" + currency.lower() + "/" + type + makequery
+                    api_url = self.url + "type/risk_reversal/" + market.lower() + "/" + currency.lower() + "/" + type + makequery
                     response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def risk_reversal_model(cls, market: str, currency: str, type: str, start: str, end: str, limit="10",
+            def risk_reversal_model(self, market: str, currency: str, type: str, start: str, end: str, limit="10",
                                     page="1",
                                     granularity=""):
                 """
                 :param market: DERIBIT
                 :type market:
                 :param currency: BTC,ETH
                 :type currency:
@@ -2191,20 +2193,20 @@
                 :return: historical risk_reversal_model by market currency and type
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
                 if market.upper() not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "type/risk_reversal_model/" + market.lower() + "/" + currency.lower() + "/" + type + makequery
+                    api_url = self.url + "type/risk_reversal_model/" + market.lower() + "/" + currency.lower() + "/" + type + makequery
                     response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def gamma_bands(cls, market: str, currency: str, type: str, start: str, end: str, limit="10", page="1",
+            def gamma_bands(self, market: str, currency: str, type: str, start: str, end: str, limit="10", page="1",
                             granularity=""):
                 """
                 :param market: BIT, DERIBIT, OKEX, POWERTRADE, BINANCE, DELTA_EXCHANGE, AEVO, LYRA , LYRA_ARBITRUM, BYBIT
                 :type market:
                 :param currency: BTC,ETH,SOL,BNB,ARB,XRP ADA
                 :type currency:
                 :param type: 1D , 7D 30D
@@ -2222,20 +2224,20 @@
                 :return: historical gamma bands by market currency and type
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
                 if market.upper() not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "type/gamma_bands/" + market.lower() + "/" + currency.lower() + "/" + type + makequery
+                    api_url = self.url + "type/gamma_bands/" + market.lower() + "/" + currency.lower() + "/" + type + makequery
                     response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def spread_skew(cls, market: str, type: str, start: str, end: str, limit="10", page="1", granularity=""):
+            def spread_skew(self, market: str, type: str, start: str, end: str, limit="10", page="1", granularity=""):
                 """
                 :param market: BIT, DERIBIT, OKEX, POWERTRADE, BINANCE, DELTA_EXCHANGE, AEVO, LYRA , LYRA_ARBITRUM, BYBIT
                 :type market:
                 :param type:  10D , 25D
                 :type type:
                 :param start: EXP:2022-06-07
                 :type end:
@@ -2250,20 +2252,20 @@
                 :return: This endpoint provides historical skew data for the specified market and type for a spread (ETH - BTC). The skew values are given for various days to maturity. In options trading, skew refers to the difference in implied volatility of different strike prices across the same maturity options. This can be used as an indicator of the market's sentiment about the future variability of the underlying assets in the context of the spread (ETH - BTC).
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
                 if market.upper() not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "spread/type/skew/" + market.lower() + "/" + type + makequery
+                    api_url = self.url + "spread/type/skew/" + market.lower() + "/" + type + makequery
                     response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def maturity_total_oi(cls, market: str, currency: str, maturity: str, start: str, end: str, limit="10",
+            def maturity_total_oi(self, market: str, currency: str, maturity: str, start: str, end: str, limit="10",
                                   page="1", granularity=""):
                 """
                 :param market:  AGGREGATE,BIT, DERIBIT, OKEX, POWERTRADE, BINANCE, DELTA_EXCHANGE, AEVO, LYRA , LYRA_ARBITRUM, BYBIT
                 :type market:
                 :param currency: BTC,ETH,SOL,BNB,ARB,XRP,ADA,TONCOIN
                 :type currency:
                 :param maturity: all | Uppercase (DMMMYY), e.g., 30JUN23 Check analytics/options/Instruments for more information about available maturity
@@ -2272,30 +2274,28 @@
                 :type end:
                 :param end: EXP:2022-06-14
                 :type end :
                 :param limit: 10
                 :type limit:
                 :param page: 1
                 :type page:
-                :param granularity: 5m,15m,30m,1h,2h,4h,6h,12h,1d
-                :type granularity :
                 :return: This endpoint provides historical total open interest (OI) data for the specified market, currency, and maturity. The open interest data is given in total, for put options, for call options, and the ratio between put and call. Open interest represents the total number of outstanding derivative contracts, such as options or futures, that have not been settled. This can be used as an indicator of the market's liquidity and activity for the specific maturity.
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
                 if market.upper() not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "maturity/total_oi/" + market.upper() + "/" + currency.upper() + "/" + maturity.upper() + makequery
+                    api_url = self.url + "maturity/total_oi/" + market.upper() + "/" + currency.upper() + "/" + maturity.upper() + makequery
                     response = requests.get(api_url, headers=api.header).json()
 
                 return response
 
             @classmethod
-            def maturity_total_volume(cls, market: str, currency: str, maturity: str, start: str, end: str, limit="10",
+            def maturity_total_volume(self, market: str, currency: str, maturity: str, start: str, end: str, limit="10",
                                       page="1", granularity=""):
                 """
                 :param market:  AGGREGATE, BIT, DERIBIT, OKEX, POWERTRADE, BINANCE, DELTA_EXCHANGE, AEVO, LYRA , LYRA_ARBITRUM, BYBIT
                 :type market:
                 :param currency: BTC,ETH,SOL,BNB,ARB,XRP,ADA,TONCOIN
                 :type currency:
                 :param maturity: all | Uppercase (DMMMYY), e.g., 30JUN23 Check analytics/options/Instruments for more information about available maturity
@@ -2304,30 +2304,28 @@
                 :type end:
                 :param end: EXP:2022-06-14
                 :type end :
                 :param limit: 10
                 :type limit:
                 :param page: 1
                 :type page:
-                :param granularity: 5m,15m,30m,1h,2h,4h,6h,12h,1d
-                :type granularity :
                 :return: This endpoint provides historical total volume data for the specified market, currency, and maturity. The volume data is given in total, for put options, for call options, and the ratio between put and call. Volume represents the number of contracts traded during a given period. This can be used as an indicator of the market's activity and liquidity for the specific maturity.
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
                 if market.upper() not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "maturity/total_volume/" + market.upper() + "/" + currency.upper() + "/" + maturity.upper() + makequery
+                    api_url = self.url + "maturity/total_volume/" + market.upper() + "/" + currency.upper() + "/" + maturity.upper() + makequery
                     response = requests.get(api_url, headers=api.header).json()
 
                 return response
 
             @classmethod
-            def atm_iv_h(cls, market: str, currency: str, maturity: str, start: str, end: str, limit="10", page="1",
+            def atm_iv_h(self, market: str, currency: str, maturity: str, start: str, end: str, limit="10", page="1",
                          granularity=""):
                 """
                 :param market:  BIT, DERIBIT, OKEX, POWERTRADE, BINANCE, DELTA_EXCHANGE, AEVO, LYRA , LYRA_ARBITRUM, BYBIT
                 :type market:
                 :param currency: BTC,ETH,SOL,BNB,ARB,XRP,ADA
                 :type currency:
                 :param maturity: all | Uppercase (DMMMYY), e.g., 30JUN23 Check analytics/options/Instruments for more information about available maturity
@@ -2336,30 +2334,28 @@
                 :type end:
                 :param end: EXP:2022-06-14
                 :type end :
                 :param limit: 10
                 :type limit:
                 :param page: 1
                 :type page:
-                :param granularity: 5m,15m,30m,1h,2h,4h,6h,12h,1d
-                :type granularity :
                 :return: This endpoint provides historical ATM IV data for the specified market, currency, and maturity. ATM IV is a key metric in options pricing, as it provides a measure of the market's expectations for future volatility. High IV values generally suggest that the market anticipates significant price movement, while low IV values indicate an expectation of relatively stable prices.
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
                 if market.upper() not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "maturity/atm_iv_h/" + market.upper() + "/" + currency.upper() + "/" + maturity.upper() + makequery
+                    api_url = self.url + "maturity/atm_iv_h/" + market.upper() + "/" + currency.upper() + "/" + maturity.upper() + makequery
                     response = requests.get(api_url, headers=api.header).json()
 
                 return response
 
             @classmethod
-            def maturity_oi_volume(cls, market: str, currency: str, maturity: str, start: str, end: str, limit="10",
+            def maturity_oi_volume(self, market: str, currency: str, maturity: str, start: str, end: str, limit="10",
                                    page="1", granularity=""):
                 """
                 :param market:  AGGREGATE, BIT, DERIBIT, OKEX, POWERTRADE, BINANCE, DELTA_EXCHANGE, AEVO, LYRA , LYRA_ARBITRUM, BYBIT
                 :type market:
                 :param currency: BTC,ETH,SOL,BNB,ARB,XRP,ADA,TONCOIN
                 :type currency:
                 :param maturity: all | Uppercase (DMMMYY), e.g., 30JUN23 Check analytics/options/Instruments for more information about available maturity
@@ -2368,30 +2364,28 @@
                 :type end:
                 :param end: EXP:2022-06-14
                 :type end :
                 :param limit: 10
                 :type limit:
                 :param page: 1
                 :type page:
-                :param granularity: 5m,15m,30m,1h,2h,4h,6h,12h,1d
-                :type granularity :
                 :return: This endpoint provides historical OI and volume data for the specified market, currency, and maturity. These metrics provide insights into market activity and investor sentiment. High OI values suggest that a large number of contracts are open and could result in significant future trading activity, while high volume values indicate a high level of recent trading activity.
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
                 if market.upper() not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "maturity/oi_volume/" + market.upper() + "/" + currency.upper() + "/" + maturity.upper() + makequery
+                    api_url = self.url + "maturity/oi_volume/" + market.upper() + "/" + currency.upper() + "/" + maturity.upper() + makequery
                     response = requests.get(api_url, headers=api.header).json()
 
                 return response
 
             @classmethod
-            def orbit_dig(cls, currency: str, maturity_name: str, field: str, start: str, end: str, limit="", page=""):
+            def orbit_dig(self, currency: str, maturity_name: str, field: str, start: str, end: str, limit="", page=""):
                 """
 
                 :param currency: BTC,ETH,AVAX,SOL
                 :type currency:
                 :param maturity_name: 1W , 2W, 1M, 3M, 6M
                 :type maturity_name:
                 :param field: 5,10,15,20
@@ -2404,20 +2398,20 @@
                 :type limit:
                 :param page: 1
                 :type page:
                 :return: This endpoint provides historical options orbit data for the specified currency and maturity. The orbit data, including the strike prices for call and put options and the price of the underlying index, are key factors that traders consider when analyzing and predicting market trends.
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page)
-                api_url = cls.url + "orbit_dig/" + currency.upper() + "/" + maturity_name + "/" + field + makequery
+                api_url = self.url + "orbit_dig/" + currency.upper() + "/" + maturity_name + "/" + field + makequery
                 response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def actual_vol_risk_reversal_model(cls, market: str, currency: str, type: str, days: str, start: str,
+            def actual_vol_risk_reversal_model(self, market: str, currency: str, type: str, days: str, start: str,
                                                end: str, limit="10", page="1",
                                                granularity=""):
                 """
                 :param market: DERIBIT
                 :type market:
                 :param currency: BTC,ETH
                 :type currency:
@@ -2438,21 +2432,21 @@
                 :return: This endpoint provides historical options actual volatility data using the Skew Model for the specified market, currency, option type (call or put), and a certain number of days. Volatility skew is a measure of the disparity of option volatility for option contracts with different strikes but the same expiration.
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
                 if market.upper() not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "actual_vol/risk_reversal_model/" + market.upper() + "/" + currency.upper() + "/" + str(
+                    api_url = self.url + "actual_vol/risk_reversal_model/" + market.upper() + "/" + currency.upper() + "/" + str(
                         type) + "/" + str(days) + makequery
                     response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def actual_vol_skew_model(cls, market: str, currency: str, type: str, days: str, start: str, end: str,
+            def actual_vol_skew_model(self, market: str, currency: str, type: str, days: str, start: str, end: str,
                                       limit="10", page="1",
                                       granularity=""):
                 """
                 :param market: DERIBIT
                 :type market:
                 :param currency: BTC,ETH
                 :type currency:
@@ -2473,21 +2467,21 @@
                 :return: This endpoint provides historical options actual volatility data using the Skew Model for the specified market, currency, option type (call or put), and a certain number of days. Volatility skew is a measure of the disparity of option volatility for option contracts with different strikes but the same expiration.
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
                 if market.upper() not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "actual_vol/skew_model/" + market.upper() + "/" + currency.upper() + "/" + str(
+                    api_url = self.url + "actual_vol/skew_model/" + market.upper() + "/" + currency.upper() + "/" + str(
                         type) + "/" + str(days) + makequery
                     response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def actual_vol_butterfly_model(cls, market: str, currency: str, type: str, days: str, start: str, end: str,
+            def actual_vol_butterfly_model(self, market: str, currency: str, type: str, days: str, start: str, end: str,
                                            limit="10", page="1",
                                            granularity=""):
                 """
                 :param market: DERIBIT
                 :type market:
                 :param currency: BTC,ETH
                 :type currency:
@@ -2508,25 +2502,25 @@
                 :return: This endpoint provides historical options actual volatility data using the Butterfly Model for the specified market, currency, option type (call or put), and a certain number of days. Volatility is a key factor that traders consider when analyzing and predicting market trends.
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
                 if market.upper() not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "actual_vol/butterfly_model/" + market.upper() + "/" + currency.upper() + "/" + str(
+                    api_url = self.url + "actual_vol/butterfly_model/" + market.upper() + "/" + currency.upper() + "/" + str(
                         type) + "/" + str(days) + makequery
                     response = requests.get(api_url, headers=api.header).json()
                 return response
 
         class futures:
             url = "https://api.laevitas.ch/historical/futures/"
             pass
 
             @classmethod
-            def snapshot(cls, market: str, currency: str, start: str, end: str, limit="10", page="1", timezone="0"):
+            def snapshot(self, market: str, currency: str, start: str, end: str, limit="10", page="1", timezone="0"):
                 """
                 :param market: BINANCE, BITMEX, BYBIT, DERIBIT, HUOBI, KRAKEN, OKX
                 :type market:
                 :param currency: BTC,ETH,ADA... Check analytics/futures/alt_currency For more information about available currencies
                 :type currency:
                 :param start: EXP:2022-06-07
                 :type end:
@@ -2538,20 +2532,20 @@
                 :type page:
                 :param timezone: exp : 0
                 :type timezone:
                 :return: This endpoint provides historical futures snapshot data for the specified market and currency. A futures contract is a legal agreement to buy or sell a particular commodity or asset at a predetermined price at a specified time in the future.
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, timezone=timezone)
-                api_url = cls.url + "snapshot/" + market.upper() + '/' + currency.upper() + makequery
+                api_url = self.url + "snapshot/" + market.upper() + '/' + currency.upper() + makequery
                 response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def realized_volatility(cls, currency: str, start: str, end: str, limit="10", page="1", granularity=""):
+            def realized_volatility(self, currency: str, start: str, end: str, limit="10", page="1", granularity=""):
                 """
                 :param currency: BTC,ETH,AVAX... Check analytics/futures/alt_currency For more information about available currencies
                 :type currency:
                 :param start: EXP:2022-06-07
                 :type end:
                 :param end: EXP:2022-06-14
                 :type end :
@@ -2561,20 +2555,20 @@
                 :type page:
                 :param granularity: 1h, 2h, 4h, 6h, 12h, 1d
                 :type granularity:
                 :return: This endpoint provides historical futures realized volatility data for the specified currency. Realized volatility is a measure of price changes of an asset or currency over time, showing how much the price deviated from its mean in the past.
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
-                api_url = cls.url + "realized_volatility/" + currency.upper() + makequery
+                api_url = self.url + "realized_volatility/" + currency.upper() + makequery
                 response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def oi_weighted_funding(cls, currency: str, start: str, end: str, limit="10", page="1", granularity=""):
+            def oi_weighted_funding(self, currency: str, start: str, end: str, limit="10", page="1", granularity=""):
                 """
                 :param currency: BTC,ETH,AVAX... Check analytics/futures/alt_currency For more information about available currencies
                 :type currency:
                 :param start: EXP:2022-06-07
                 :type end:
                 :param end: EXP:2022-06-14
                 :type end :
@@ -2584,20 +2578,20 @@
                 :type page:
                 :param granularity: 5m, 15m, 30m 1h, 2h, 4h, 6h, 12h, 1d
                 :type granularity:
                 :return: This endpoint provides historical futures open interest weighted funding data for the specified currency. Open interest weighted funding represents the funding costs associated with holding positions in futures contracts, taking into account the open interest and the funding rates.
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
-                api_url = cls.url + "oi_weighted_funding/" + currency.upper() + makequery
+                api_url = self.url + "oi_weighted_funding/" + currency.upper() + makequery
                 response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def oi_weighted_volume_funding(cls, currency: str, start: str, end: str, limit="10", page="1",
+            def oi_weighted_volume_funding(self, currency: str, start: str, end: str, limit="10", page="1",
                                            granularity=""):
                 """
                 :param currency: BTC,ETH,AVAX... Check analytics/futures/alt_currency For more information about available currencies
                 :type currency:
                 :param start: EXP:2022-06-07
                 :type end:
                 :param end: EXP:2022-06-14
@@ -2608,20 +2602,20 @@
                 :type page:
                 :param granularity: 5m, 15m, 30m, 1h, 2h, 4h, 6h, 12h, 1d
                 :type granularity:
                 :return: This endpoint provides historical futures open interest weighted funding data
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
-                api_url = cls.url + "oi_weighted_volume_funding/" + currency.upper() + makequery
+                api_url = self.url + "oi_weighted_volume_funding/" + currency.upper() + makequery
                 response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def oi_weighted_basis(cls, currency: str, start: str, end: str, limit="", page="", granularity=""):
+            def oi_weighted_basis(self, currency: str, start: str, end: str, limit="", page="", granularity=""):
                 """
                 :param currency: BTC,ETH,AVAX... Check analytics/futures/alt_currency For more information about available currencies
                 :type currency:
                 :param start: EXP:2022-06-07
                 :type end:
                 :param end: EXP:2022-06-14
                 :type end :
@@ -2631,20 +2625,20 @@
                 :type page:
                 :param granularity: 5m, 15m, 30m, 1h, 2h, 4h, 6h, 12h, 1d
                 :type granularity:
                 :return:
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
-                api_url = cls.url + "oi_weighted_basis/" + currency.upper() + makequery
+                api_url = self.url + "oi_weighted_basis/" + currency.upper() + makequery
                 response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def total_oi(cls, currency: str, start: str, end: str, limit="", page="", granularity=""):
+            def total_oi(self, currency: str, start: str, end: str, limit="", page="", granularity=""):
                 """
                 :param currency: BTC,ETH,AVAX... Check analytics/futures/alt_currency For more information about available currencies
                 :type currency:
                 :param start: EXP:2022-06-07
                 :type end:
                 :param end: EXP:2022-06-14
                 :type end :
@@ -2654,20 +2648,20 @@
                 :type page:
                 :param granularity: 5m, 15m, 30m, 1h, 2h, 4h, 6h, 12h, 1d
                 :type granularity:
                 :return: This endpoint provides historical futures total open interest data for the specified currency. The data includes open interest and notional value for both perpetual futures contracts and futures contracts with specific expiration dates on various exchanges.
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
-                api_url = cls.url + "total_oi/" + currency.upper() + makequery
+                api_url = self.url + "total_oi/" + currency.upper() + makequery
                 response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def total_oi_by_margin(cls, currency: str, start: str, end: str, limit="", page="", granularity=""):
+            def total_oi_by_margin(self, currency: str, start: str, end: str, limit="", page="", granularity=""):
                 """
                 :param currency: BTC,ETH,AVAX... Check analytics/futures/alt_currency For more information about available currencies
                 :type currency:
                 :param start: EXP:2022-06-07
                 :type end:
                 :param end: EXP:2022-06-14
                 :type end :
@@ -2677,20 +2671,20 @@
                 :type page:
                 :param granularity: 5m, 15m, 30m, 1h, 2h, 4h, 6h, 12h, 1d
                 :type granularity:
                 :return: This endpoint provides historical futures total open interest data for the specified currency. The data includes open interest and notional value for both perpetual futures contracts and futures contracts with specific expiration dates on various exchanges.
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
-                api_url = cls.url + "total_oi_by_margin/" + currency.upper() + makequery
+                api_url = self.url + "total_oi_by_margin/" + currency.upper() + makequery
                 response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def total_volume(cls, currency: str, start: str, end: str, limit="", page="", granularity=""):
+            def total_volume(self, currency: str, start: str, end: str, limit="", page="", granularity=""):
                 """
                 :param currency: BTC,ETH,AVAX... Check analytics/futures/alt_currency For more information about available currencies
                 :type currency:
                 :param start: EXP:2022-06-07
                 :type end:
                 :param end: EXP:2022-06-14
                 :type end :
@@ -2700,20 +2694,20 @@
                 :type page:
                 :param granularity: 5m, 15m, 30m, 1h, 2h, 4h, 6h, 12h, 1d
                 :type granularity:
                 :return: This endpoint provides historical futures total volume for the specified currency. The data includes volume and notional value for both perpetual futures contracts and futures contracts on various exchanges.
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
-                api_url = cls.url + "total_volume/" + currency.upper() + makequery
+                api_url = self.url + "total_volume/" + currency.upper() + makequery
                 response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def total_volume_by_margin(cls, currency: str, start: str, end: str, limit="", page="", granularity=""):
+            def total_volume_by_margin(self, currency: str, start: str, end: str, limit="", page="", granularity=""):
                 """
                 :param currency: BTC,ETH,AVAX... Check analytics/futures/alt_currency For more information about available currencies
                 :type currency:
                 :param start: EXP:2022-06-07
                 :type end:
                 :param end: EXP:2022-06-14
                 :type end :
@@ -2723,20 +2717,20 @@
                 :type page:
                 :param granularity: 5m, 15m, 30m, 1h, 2h, 4h, 6h, 12h, 1d
                 :type granularity:
                 :return: This endpoint provides historical futures total volume by margin for the specified currency. The data includes volume and notional value for futures contracts and perpetual futures contracts on both centralized and decentralized exchanges.
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
-                api_url = cls.url + "total_volume_by_margin/" + currency.upper() + makequery
+                api_url = self.url + "total_volume_by_margin/" + currency.upper() + makequery
                 response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def alt_summary(cls, currency: str, start: str, end: str, limit="", page="", granularity=""):
+            def alt_summary(self, currency: str, start: str, end: str, limit="", page="", granularity=""):
                 """
                 :param currency: BTC,ETH,AVAX... Check analytics/futures/alt_currency For more information about available currencies
                 :type currency:
                 :param start: EXP:2022-06-07
                 :type end:
                 :param end: EXP:2022-06-14
                 :type end :
@@ -2746,20 +2740,20 @@
                 :type page:
                 :param granularity: 5m, 15m, 30m, 1h, 2h, 4h, 6h, 12h, 1d
                 :type granularity:
                 :return: This endpoint provides historical altcoin summary for the specified currency in futures trading. The data includes price, open interest, volume, funding rate, yield, liquidations, market capitalization, and open interest volume for the past 24 hours.
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
-                api_url = cls.url + "alt_summary/" + currency.upper() + makequery
+                api_url = self.url + "alt_summary/" + currency.upper() + makequery
                 response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def market_index(cls, index: str, start: str, end: str, limit="10", page="1", granularity=""):
+            def market_index(self, index: str, start: str, end: str, limit="10", page="1", granularity=""):
                 """
                 :param index: privacy, oracle_data nft_gaming, memecoin, layer1 , layer2, exchange, defi , digital_asset
                 :type index:
                 :param start: EXP:2022-06-07
                 :type end:
                 :param end: EXP:2022-06-14
                 :type end :
@@ -2769,20 +2763,20 @@
                 :type page:
                 :param granularity: 5m, 15m, 30m, 1h, 2h, 4h, 6h, 12h, 1d
                 :type granularity:
                 :return: This endpoint provides historical market index data for the specified index in futures trading. The data includes information about each altcoin in the index, such as open interest, trading volume, market capitalization, liquidations, funding rate, yield, and price.
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
-                api_url = cls.url + "market_index/" + index.lower() + makequery
+                api_url = self.url + "market_index/" + index.lower() + makequery
                 response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def alt_markets(cls, market: str, start: str, end: str, limit="10", page="1", granularity=""):
+            def alt_markets(self, market: str, start: str, end: str, limit="10", page="1", granularity=""):
                 """
                 :param market: DERIBIT, GMX, BITGET, BITMEX, VERTEX, BITFINEX, OKEX, BINANCE, KRAKEN, KWENTA, PERP-PROTOCOL, BYBIT, DYDX, HUOBI
                 :type market:
                 :param start: EXP:2022-06-07
                 :type end:
                 :param end: EXP:2022-06-14
                 :type end :
@@ -2792,20 +2786,20 @@
                 :type page:
                 :param granularity: 5m, 15m, 30m, 1h, 2h, 4h, 6h, 12h, 1d
                 :type granularity:
                 :return: This endpoint provides historical data for altcoin markets in futures trading. The data includes information such as open interest, trading volume, funding rate, and liquidations (both long and short). The data is organized by date for each altcoin market within the specified market.
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
-                api_url = cls.url + "market_index/" + market.upper() + makequery
+                api_url = self.url + "market_index/" + market.upper() + makequery
                 response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def indices_price(cls, index: str, start: str, end: str, limit="10", page="1", granularity=""):
+            def indices_price(self, index: str, start: str, end: str, limit="10", page="1", granularity=""):
                 """
                 :param index: privacy,oracle_data,nft_gaming,memecoin,layer2,layer1,exchange,digital_asset,defi
                 :type index:
                 :param start: EXP:2022-06-07
                 :type end:
                 :param end: EXP:2022-06-14
                 :type end :
@@ -2815,20 +2809,20 @@
                 :type page:
                 :param granularity: 5m, 15m, 30m, 1h, 2h, 4h, 6h, 12h, 1d
                 :type granularity:
                 :return: This endpoint provides historical price data for indices. The data includes the date and price for each index.
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
-                api_url = cls.url + "indices_price/" + index.upper() + makequery
+                api_url = self.url + "indices_price/" + index.upper() + makequery
                 response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def futures_annualized_basis(cls, currency: str, days: str, start: str, end: str, limit="10", page="1",
+            def futures_annualized_basis(self, currency: str, days: str, start: str, end: str, limit="10", page="1",
                                          granularity=""):
                 """
                 :param currency: BTC,ETH,AVAX... Check analytics/futures/alt_currency For more information about available currencies
                 :type currency:
                 :param days : 3 | 7 | 30 | 60 | 90 | 180 | 270 | 365
                 :type days :
                 :param start: EXP:2022-06-07
@@ -2841,20 +2835,20 @@
                 :type page:
                 :param granularity: 5m, 15m, 30m, 1h, 2h, 4h, 6h, 12h, 1d
                 :type granularity:
                 :return: This endpoint provides historical data for the annualized basis of futures contracts. The data includes the date and the annualized basis values for different exchanges such as DERIBIT, HUOBI, and OKEX.
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
-                api_url = cls.url + "futures_annualized_basis/" + currency.upper() + "/" + str(days) + makequery
+                api_url = self.url + "futures_annualized_basis/" + currency.upper() + "/" + str(days) + makequery
                 response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def perpetual_funding_exchange(cls, currency: str, option: str, start: str, end: str, limit="10", page="1",
+            def perpetual_funding_exchange(self, currency: str, option: str, start: str, end: str, limit="10", page="1",
                                            granularity=""):
                 """
                 :param currency: BTC,ETH,AVAX... Check analytics/futures/alt_currency For more information about available currencies
                 :type currency:
                 :param option  : C , D
                 :type option  :
                 :param start: EXP:2022-06-07
@@ -2867,20 +2861,20 @@
                 :type page:
                 :param granularity: 5m, 15m, 30m, 1h, 2h, 4h, 6h, 12h, 1d
                 :type granularity:
                 :return: This endpoint provides historical data for the funding rates and yields of perpetual contracts on various exchanges. The data includes the date, as well as information such as the yield, funding rate, market name, and symbol for each perpetual contract.
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
-                api_url = cls.url + "perpetual_funding_exchange/" + currency.upper() + "/" + option.upper() + makequery
+                api_url = self.url + "perpetual_funding_exchange/" + currency.upper() + "/" + option.upper() + makequery
                 response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def total_oi_by_exchange(cls, currency: str, option: str, start: str, end: str, limit="10", page="1",
+            def total_oi_by_exchange(self, currency: str, option: str, start: str, end: str, limit="10", page="1",
                                      granularity=""):
                 """
                 :param currency: BTC,ETH,AVAX... Check analytics/futures/alt_currency For more information about available currencies
                 :type currency:
                 :param option  : C , D
                 :type option  :
                 :param start: EXP:2023-07-13
@@ -2893,21 +2887,21 @@
                 :type page:
                 :param granularity: 5m, 15m, 30m, 1h, 2h, 4h, 6h, 12h, 1d
                 :type granularity:
                 :return: This endpoint provides historical data for the total open interest and notional values of perpetual and futures contracts on various exchanges. The data includes the date, as well as the open interest and notional values for each exchange and contract type (perpetual or future).
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
-                api_url = cls.url + "total_oi_by_exchange/" + currency.upper() + "/" + option.upper() + makequery
+                api_url = self.url + "total_oi_by_exchange/" + currency.upper() + "/" + option.upper() + makequery
                 response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def total_volume_by_exchange(cls, currency: str, option: str, start: str, end: str, limit="10", page="1",
-                                         granularity=""):
+            def total_volume_by_exchange(self, currency: str, option: str, start: str, end: str, limit="10", page="1",
+                                     granularity=""):
                 """
                 :param currency: BTC,ETH,AVAX... Check analytics/futures/alt_currency For more information about available currencies
                 :type currency:
                 :param option  : C , D
                 :type option  :
                 :param start: EXP:2023-07-13
                 :type end:
@@ -2919,21 +2913,21 @@
                 :type page:
                 :param granularity: 5m, 15m, 30m, 1h, 2h, 4h, 6h, 12h, 1d
                 :type granularity:
                 :return: This endpoint provides historical data for the total trading volume and notional values of perpetual and futures contracts on various exchanges. The data includes the date, as well as the volume and notional values for each exchange and contract type (perpetual or future).
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
-                api_url = cls.url + "total_volume_by_exchange/" + currency.upper() + "/" + option.upper() + makequery
+                api_url = self.url + "total_volume_by_exchange/" + currency.upper() + "/" + option.upper() + makequery
                 response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def perpetual_yield(cls, market: str, currency: str, start: str, end: str, limit="10", page="1",
-                                granularity=""):
+            def perpetual_yield(self, market: str, currency: str, start: str, end: str, limit="10", page="1",
+                                     granularity=""):
                 """
                 :param market: DERIBIT, GMX, BITGET, BITMEX, VERTEX, BITFINEX, OKEX, BINANCE, KRAKEN, KWENTA, PERP-PROTOCOL, BYBIT, DYDX, HUOBI
                 :type market:
                 :param currency: BTC,ETH,BCH try the analytics future alt_currency function for more available currency
                 :type currency:
                 :param start: EXP:2022-06-07
                 :type end:
@@ -2944,22 +2938,22 @@
                 :param page: 1
                 :type page:
                 :param granularity: 5m, 15m, 30m, 1h, 2h, 4h, 6h, 12h, 1d
                 :type granularity:
                 :return: This endpoint provides historical data for the yield of perpetual contracts in a specific currency and market. The data includes the date and the yield value for each perpetual contract symbol.
                 :rtype:
                 """
-                makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
-                api_url = cls.url + "perpetual_yield/" + currency.upper() + "/" + market.upper() + makequery
+                makequery = prepare_query(start=start, end=end, limit=limit, page=page,granularity=granularity)
+                api_url = self.url + "perpetual_yield/" + currency.upper() + "/" + market.upper() + makequery
                 response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def perpetual_funding(cls, market: str, currency: str, start: str, end: str, limit="10", page="1",
-                                  granularity=""):
+            def perpetual_funding(self, market: str, currency: str, start: str, end: str, limit="10", page="1",
+                                     granularity=""):
                 """
                 :param market: DERIBIT, GMX, BITGET, BITMEX, VERTEX, BITFINEX, OKEX, BINANCE, KRAKEN, KWENTA, PERP-PROTOCOL, BYBIT, DYDX, HUOBI
                 :type market:
                 :param currency: BTC,ETH,BCH try the analytics future alt_currency function for more available currency
                 :type currency:
                 :param start: EXP:2022-06-07
                 :type end:
@@ -2970,22 +2964,22 @@
                 :param page: 1
                 :type page:
                 :param granularity: 5m, 15m, 30m, 1h, 2h, 4h, 6h, 12h, 1d
                 :type granularity:
                 :return: This endpoint provides historical data for the funding of perpetual contracts in a specific currency and market. The data includes the date and the funding value for each perpetual contract symbol.
                 :rtype:
                 """
-                makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
-                api_url = cls.url + "perpetual_funding/" + currency.upper() + "/" + market.upper() + makequery
+                makequery = prepare_query(start=start, end=end, limit=limit, page=page,granularity=granularity)
+                api_url = self.url + "perpetual_funding/" + currency.upper() + "/" + market.upper() + makequery
                 response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def global_activity_futures(cls, market: str, start: str, end: str, limit="10", page="1",
-                                        granularity=""):
+            def global_activity_futures(self, market: str, start: str, end: str, limit="10", page="1",
+                                     granularity=""):
                 """
                 :param market: DERIBIT, BITGET, BITMEX, OKEX, BINANCE, KRAKEN, BYBIT, HUOBI
                 :type market:
                 :param start: EXP:2022-06-07
                 :type end:
                 :param end: EXP:2022-06-14
                 :type end :
@@ -2994,25 +2988,25 @@
                 :param page: 1
                 :type page:
                 :param granularity: 5m, 15m, 30m, 1h, 2h, 4h, 6h, 12h, 1d
                 :type granularity:
                 :return: This endpoint provides historical data for the global activity of futures in a specific market. The data includes the date, open interest, trading volume, yield value, and the number of liquidations for long and short positions.
                 :rtype:
                 """
-                makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
+                makequery = prepare_query(start=start, end=end, limit=limit, page=page,granularity=granularity)
                 if market.upper() not in MARKET_CONSTS.__members__:
                     raise TypeError("Market not available")
                 else:
-                    api_url = cls.url + "global_activity_futures/" + market.upper() + makequery
+                    api_url = self.url + "global_activity_futures/" + market.upper() + makequery
                     response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def oi_total_global_activity(cls, start: str, end: str, limit="10", page="1",
-                                         granularity=""):
+            def oi_total_global_activity(self,start: str, end: str, limit="10", page="1",
+                                        granularity=""):
                 """
                 :param start: EXP:2022-06-07
                 :type end:
                 :param end: EXP:2022-06-14
                 :type end :
                 :param limit: 10
                 :type limit:
@@ -3020,21 +3014,22 @@
                 :type page:
                 :param granularity: 5m, 15m, 30m, 1h, 2h, 4h, 6h, 12h, 1d
                 :type granularity:
                 :return: This endpoint provides historical data for the total global open interest activity. It includes the date and the total open interest for futures, options, and perpetual contracts.
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
-                api_url = cls.url + "oi_total_global_activity" + makequery
+                api_url = self.url + "oi_total_global_activity" + makequery
                 response = requests.get(api_url, headers=api.header).json()
                 return response
 
+
             @classmethod
-            def volume_total_global_activity(cls, start: str, end: str, limit="10", page="1",
-                                             granularity=""):
+            def volume_total_global_activity(self,start: str, end: str, limit="10", page="1",
+                                        granularity=""):
                 """
                 :param start: EXP:2022-06-07
                 :type end:
                 :param end: EXP:2022-06-14
                 :type end :
                 :param limit: 10
                 :type limit:
@@ -3042,24 +3037,24 @@
                 :type page:
                 :param granularity: 5m, 15m, 30m, 1h, 2h, 4h, 6h, 12h, 1d
                 :type granularity:
                 :return: This endpoint provides historical data for the total global volume activity. It includes the date and the total volume for futures, options, and perpetual contracts.
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
-                api_url = cls.url + "volume_total_global_activity" + makequery
+                api_url = self.url + "volume_total_global_activity" + makequery
                 response = requests.get(api_url, headers=api.header).json()
                 return response
 
         # class move:
         #     url = "https://api.laevitas.ch/historical/move/"
         #     pass
         #
         #     @classmethod
-        #     def total_oi(cls, market="ftx", currency="btc", start="", end="", limit="", page=""):
+        #     def total_oi(self, market="ftx", currency="btc", start="", end="", limit="", page=""):
         #         """
         #         :param market: FTX
         #         :type market:
         #         :param currency: BTC
         #         :type currency:
         #         :param start: EXP:2022-06-07
         #         :type end:
@@ -3074,38 +3069,38 @@
         #         """
         #         makequery = query(start=start, end=end, limit=limit, page=page)
         #         if market.upper() not in MARKET_CONSTS.__members__:
         #             raise TypeError("Market not available")
         #         elif currency.upper() not in CURRENCY.__members__:
         #             raise TypeError("Currency not available")
         #         elif makequery != "":
-        #             api_url = cls.url + "total_oi/" + market.lower() + "/" + currency.lower() + makequery
+        #             api_url = self.url + "total_oi/" + market.lower() + "/" + currency.lower() + makequery
         #             response = requests.get(api_url, headers=api.header).json()
         #             Response = Ipagination(response,
         #                                    Ipaginationmeta(response['meta']['total'], response['meta']['page'],
         #                                                    response['meta']['items'])
         #
         #                                    )
         #             for i in range(len(response['items'])):
         #                 Response.items.append(IDateV(response['items'][i]['v'], response['items'][i]['date']))
         #             return Response
         #         else:
-        #             api_url = cls.url + "total_oi/" + market.lower() + "/" + currency.lower()
+        #             api_url = self.url + "total_oi/" + market.lower() + "/" + currency.lower()
         #             response = requests.get(api_url, headers=api.header).json()
         #             Response = Ipagination(response,
         #                                    Ipaginationmeta(response['meta']['total'], response['meta']['page'],
         #                                                    response['meta']['items'])
         #
         #                                    )
         #             for i in range(len(response['items'])):
         #                 Response.items.append(IDateV(response['items'][i]['v'], response['items'][i]['date']))
         #             return Response
         #
         #     @classmethod
-        #     def volume_buy_sell(cls, market="ftx", currency="btc", start="", end="", limit="", page=""):
+        #     def volume_buy_sell(self, market="ftx", currency="btc", start="", end="", limit="", page=""):
         #         """
         #
         #         :param market: FTX
         #         :type market:
         #         :param currency: BTC
         #         :type currency:
         #         :param start: EXP:2022-06-07
@@ -3121,23 +3116,23 @@
         #         """
         #         makequery = query(start=start, end=end, limit=limit, page=page)
         #         if market.upper() not in MARKET_CONSTS.__members__:
         #             raise TypeError("Market not available")
         #         if currency.upper() not in CURRENCY.__members__:
         #             raise TypeError("Currency not available")
         #         elif makequery != "":
-        #             api_url = cls.url + "volume_buy_sell/" + market.lower() + "/" + currency.lower() + makequery
+        #             api_url = self.url + "volume_buy_sell/" + market.lower() + "/" + currency.lower() + makequery
         #             response = requests.get(api_url, headers=api.header).json()
         #         else:
-        #             api_url = cls.url + "volume_buy_sell/" + market.lower() + "/" + currency.lower()
+        #             api_url = self.url + "volume_buy_sell/" + market.lower() + "/" + currency.lower()
         #             response = requests.get(api_url, headers=api.header).json()
         #         return response
         #
         #     @classmethod
-        #     def iv_type(cls, market: str, currency: str, type: str, start="", end="", limit="", page=""):
+        #     def iv_type(self, market: str, currency: str, type: str, start="", end="", limit="", page=""):
         #         """
         #
         #         :param market: FTX
         #         :type market:
         #         :param currency: BTC
         #         :type currency:
         #         :param type: daily, weekly, quarterly
@@ -3155,23 +3150,23 @@
         #         """
         #         makequery = query(start=start, end=end, limit=limit, page=page)
         #         if market.upper() not in MARKET_CONSTS.__members__:
         #             raise TypeError("Market not available")
         #         if currency.upper() not in CURRENCY.__members__:
         #             raise TypeError("Currency not available")
         #         elif makequery != "":
-        #             api_url = cls.url + "iv_type/" + market.lower() + "/" + currency.lower() + "/" + type + makequery
+        #             api_url = self.url + "iv_type/" + market.lower() + "/" + currency.lower() + "/" + type + makequery
         #             response = requests.get(api_url, headers=api.header).json()
         #         else:
-        #             api_url = cls.url + "iv_type/" + market.lower() + "/" + currency.lower() + "/" + type
+        #             api_url = self.url + "iv_type/" + market.lower() + "/" + currency.lower() + "/" + type
         #             response = requests.get(api_url, headers=api.header).json()
         #         return response
         #
         #     @classmethod
-        #     def iv_historical_open_future(cls, market: str, currency: str, is_open: str, start="", end="", limit="",
+        #     def iv_historical_open_future(self, market: str, currency: str, is_open: str, start="", end="", limit="",
         #                                   page=""):
         #         """
         #
         #         :param market: FTX
         #         :type market:
         #         :param currency: BTC
         #         :type currency:
@@ -3190,23 +3185,23 @@
         #         """
         #         makequery = query(start=start, end=end, limit=limit, page=page)
         #         if market.upper() not in MARKET_CONSTS.__members__:
         #             raise TypeError("Market not available")
         #         if currency.upper() not in CURRENCY.__members__:
         #             raise TypeError("Currency not available")
         #         elif makequery != "":
-        #             api_url = cls.url + "iv_historical_open_future/" + market.lower() + "/" + currency.lower() + "/" + is_open.lower() + makequery
+        #             api_url = self.url + "iv_historical_open_future/" + market.lower() + "/" + currency.lower() + "/" + is_open.lower() + makequery
         #             response = requests.get(api_url, headers=api.header).json()
         #         else:
-        #             api_url = cls.url + "iv_historical_open_future/" + market.lower() + "/" + currency.lower() + "/" + is_open.lower()
+        #             api_url = self.url + "iv_historical_open_future/" + market.lower() + "/" + currency.lower() + "/" + is_open.lower()
         #             response = requests.get(api_url, headers=api.header).json()
         #         return response
         #
         #     @classmethod
-        #     def total_volume(cls, market="ftx", currency="btc", start="", end="", limit="", page=""):
+        #     def total_volume(self, market="ftx", currency="btc", start="", end="", limit="", page=""):
         #         """
         #
         #         :param market: FTX
         #         :type market:
         #         :param currency: BTC
         #         :type currency:
         #         :param start: EXP:2022-06-07
@@ -3222,23 +3217,23 @@
         #         """
         #         makequery = query(start=start, end=end, limit=limit, page=page)
         #         if market.upper() not in MARKET_CONSTS.__members__:
         #             raise TypeError("Market not available")
         #         if currency.upper() not in CURRENCY.__members__:
         #             raise TypeError("Currency not available")
         #         elif makequery != "":
-        #             api_url = cls.url + "total_volume/" + market.lower() + "/" + currency.lower() + makequery
+        #             api_url = self.url + "total_volume/" + market.lower() + "/" + currency.lower() + makequery
         #             response = requests.get(api_url, headers=api.header).json()
         #         else:
-        #             api_url = cls.url + "total_volume/" + market.lower() + "/" + currency.lower()
+        #             api_url = self.url + "total_volume/" + market.lower() + "/" + currency.lower()
         #             response = requests.get(api_url, headers=api.header).json()
         #         return response
         #
         #     @classmethod
-        #     def historical_iv(cls, contract_name: str, market="ftx", start="", end="", limit="", page=""):
+        #     def historical_iv(self, contract_name: str, market="ftx", start="", end="", limit="", page=""):
         #         """
         #
         #         :param market: FTX
         #         :type market:
         #         :param contract_name: try realtime.move.contract_name function for contract names. EXP : BTC-MOVE-2022Q4
         #         :type contract_name:
         #         :param start: EXP:2022-06-07
@@ -3252,23 +3247,23 @@
         #         :return: json data of historical implied volatility
         #         :rtype:
         #         """
         #         makequery = query(start=start, end=end, limit=limit, page=page)
         #         if market.upper() not in MARKET_CONSTS.__members__:
         #             raise TypeError("Market not available")
         #         elif makequery != "":
-        #             api_url = cls.url + "historical_iv/" + market.lower() + "/" + contract_name.lower() + makequery
+        #             api_url = self.url + "historical_iv/" + market.lower() + "/" + contract_name.lower() + makequery
         #             response = requests.get(api_url, headers=api.header).json()
         #         else:
-        #             api_url = cls.url + "historical_iv/" + market.lower() + "/" + contract_name.lower()
+        #             api_url = self.url + "historical_iv/" + market.lower() + "/" + contract_name.lower()
         #             response = requests.get(api_url, headers=api.header).json()
         #         return response
         #
         #     @classmethod
-        #     def historical_oi(cls, contract_name: str, market="ftx", start="", end="", limit="", page=""):
+        #     def historical_oi(self, contract_name: str, market="ftx", start="", end="", limit="", page=""):
         #         """
         #
         #         :param market: FTX
         #         :type market:
         #         :param contract_name: try realtime.move.contract_name function for contract names. EXP : BTC-MOVE-2022Q4
         #         :type contract_name:
         #         :param start: EXP:2022-06-07
@@ -3282,23 +3277,23 @@
         #         :return: json data of historical open interest
         #         :rtype:
         #         """
         #         makequery = query(start=start, end=end, limit=limit, page=page)
         #         if market.upper() not in MARKET_CONSTS.__members__:
         #             raise TypeError("Market not available")
         #         elif makequery != "":
-        #             api_url = cls.url + "historical_oi/" + market.lower() + "/" + contract_name.lower() + makequery
+        #             api_url = self.url + "historical_oi/" + market.lower() + "/" + contract_name.lower() + makequery
         #             response = requests.get(api_url, headers=api.header).json()
         #         else:
-        #             api_url = cls.url + "historical_oi/" + market.lower() + "/" + contract_name.lower()
+        #             api_url = self.url + "historical_oi/" + market.lower() + "/" + contract_name.lower()
         #             response = requests.get(api_url, headers=api.header).json()
         #         return response
         #
         #     @classmethod
-        #     def historical_price(cls, contract_name: str, market="ftx", start="", end="", limit="", page=""):
+        #     def historical_price(self, contract_name: str, market="ftx", start="", end="", limit="", page=""):
         #         """
         #
         #         :param market: FTX
         #         :type market:
         #         :param contract_name: try realtime.move.contract_name function for contract names. EXP : BTC-MOVE-2022Q4
         #         :type contract_name:
         #         :param start: EXP:2022-06-07
@@ -3312,23 +3307,23 @@
         #         :return: json data of historical price
         #         :rtype:
         #         """
         #         makequery = query(start=start, end=end, limit=limit, page=page)
         #         if market.upper() not in MARKET_CONSTS.__members__:
         #             raise TypeError("Market not available")
         #         elif makequery != "":
-        #             api_url = cls.url + "historical_price/" + market.lower() + "/" + contract_name.lower() + makequery
+        #             api_url = self.url + "historical_price/" + market.lower() + "/" + contract_name.lower() + makequery
         #             response = requests.get(api_url, headers=api.header).json()
         #         else:
-        #             api_url = cls.url + "historical_price/" + market.lower() + "/" + contract_name.lower()
+        #             api_url = self.url + "historical_price/" + market.lower() + "/" + contract_name.lower()
         #             response = requests.get(api_url, headers=api.header).json()
         #         return response
         #
         #     @classmethod
-        #     def historical_volume(cls, contract_name: str, market="ftx", start="", end="", limit="", page=""):
+        #     def historical_volume(self, contract_name: str, market="ftx", start="", end="", limit="", page=""):
         #         """
         #
         #         :param market: FTX
         #         :type market:
         #         :param contract_name: try realtime.move.contract_name function for contract names. EXP : BTC-MOVE-2022Q4
         #         :type contract_name:
         #         :param start: EXP:2022-06-07
@@ -3342,39 +3337,39 @@
         #         :return: json data of historical volume
         #         :rtype:
         #         """
         #         makequery = query(start=start, end=end, limit=limit, page=page)
         #         if market.upper() not in MARKET_CONSTS.__members__:
         #             raise TypeError("Market not available")
         #         elif makequery != "":
-        #             api_url = cls.url + "historical_volume/" + market.lower() + "/" + contract_name.lower() + makequery
+        #             api_url = self.url + "historical_volume/" + market.lower() + "/" + contract_name.lower() + makequery
         #             response = requests.get(api_url, headers=api.header).json()
         #         else:
-        #             api_url = cls.url + "historical_volume/" + market.lower() + "/" + contract_name.lower()
+        #             api_url = self.url + "historical_volume/" + market.lower() + "/" + contract_name.lower()
         #             response = requests.get(api_url, headers=api.header).json()
         #         return response
         #
         #     @classmethod
-        #     def open_future(cls, contract_type: str):
+        #     def open_future(self, contract_type: str):
         #         """
         #         :param contract_type: daily, weekly, quarterly
         #         :type contract_type:
         #         :return: json data of open future
         #         :rtype:
         #         """
-        #         api_url = cls.url + "open_future/" + contract_type
+        #         api_url = self.url + "open_future/" + contract_type
         #         response = requests.get(api_url, headers=api.header).json()
         #         return response
 
         class defi:
             url = "https://api.laevitas.ch/historical/defi/"
             pass
 
             @classmethod
-            def dovs_auctions(cls, protocol: str, start="", end="", currency="", limit="", page=""):
+            def dovs_auctions(self, protocol: str, start="", end="", currency="", limit="", page=""):
                 """
 
                 :param protocol: ribbon, friktion, thetanuts
                 :type protocol:
                 :param start: EXP:2022-06-07
                 :type end:
                 :param end: EXP:2022-06-14
@@ -3386,27 +3381,27 @@
                 :param page: 1
                 :type page:
                 :return: json data of dovs auctions
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, currency=currency, limit=limit, page=page)
                 if makequery != "":
-                    api_url = cls.url + "dovs/auctions/" + protocol.lower() + makequery
+                    api_url = self.url + "dovs/auctions/" + protocol.lower() + makequery
                     response = requests.get(api_url, headers=api.header).json()
                 else:
-                    api_url = cls.url + "dovs/auctions/" + protocol.lower()
+                    api_url = self.url + "dovs/auctions/" + protocol.lower()
                     response = requests.get(api_url, headers=api.header).json()
                 return response
 
         class derivs:
             url = "https://api.laevitas.ch/historical/derivs/"
             pass
 
             @classmethod
-            def perpetuals(cls, market: str, symbol: str, start: str, end: str, limit="10", page="1", granularity=""):
+            def perpetuals(self, market: str, symbol: str, start: str, end: str, limit="10", page="1", granularity=""):
                 """
                 :param market:  BITMEX | BINANCE | BYBIT | DYDX | BITFINEX | DERIBIT | HUOBI | KRAKEN | OKEX | KWENTA | GMX | VERTEX | PERP-PROTOCOL | BITGET
                 :type market:
                 :param symbol: exp : BTC-USDT , BTCUSDT , XBTUSD , depending on the market
                 :type symbol:
                 :param start: EXP:2022-06-07
                 :type end:
@@ -3418,20 +3413,21 @@
                 :type page:
                 :param granularity: 5m,15m,30m,1h,2h,4h,6h,12h,1d
                 :type granularity :
                 :return:
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
-                api_url = cls.url + "perpetuals/" + market.upper() + "/" + symbol.upper() + makequery
-                response = requests.get(api_url, headers=api.header).json()
+                if makequery != "":
+                    api_url = self.url + "perpetuals/" + market.upper() + "/" + symbol.upper() + makequery
+                    response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def futures(cls, market: str, symbol: str, start: str, end: str, limit="10", page="1", granularity=""):
+            def futures(self, market: str, symbol: str, start: str, end: str, limit="10", page="1", granularity=""):
                 """
                 :param market: BITMEX | BINANCE | BYBIT | DYDX | BITFINEX | DERIBIT | HUOBI | KRAKEN | OKEX | KWENTA | GMX | VERTEX | PERP-PROTOCOL | BITGET
                 :type market:
                 :param symbol: exp : ETH-USDT-230707 , XBTZ23 depending on the market
                 :type symbol:
                 :param start: EXP:2022-06-07
                 :type end:
@@ -3443,20 +3439,20 @@
                 :type page:
                 :param granularity: 5m,15m,30m,1h,2h,4h,6h,12h,1d
                 :type granularity :
                 :return:
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
-                api_url = cls.url + "futures/" + market.upper() + "/" + symbol.upper() + makequery
+                api_url = self.url + "futures/" + market.upper() + "/" + symbol.upper() + makequery
                 response = requests.get(api_url, headers=api.header).json()
                 return response
 
             @classmethod
-            def summary(cls, currency: str, start="", end="", limit="10", page="1", granularity=""):
+            def summary(self, currency: str, start="", end="", limit="10", page="1", granularity=""):
                 """
                 :param currency: BTC | ETH | ALTS (Full list of supported assets on instruments endpoint)
                 :type currency:
                 :param start: EXP:2022-06-07
                 :type end:
                 :param end: EXP:2022-06-14
                 :type end :
@@ -3466,20 +3462,21 @@
                 :type page:
                 :param granularity: 5m,15m,30m,1h,2h,4h,6h,12h,1d
                 :type granularity :
                 :return: json data of summary
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, granularity=granularity)
-                api_url = cls.url + "summary/" + currency.upper() + makequery
+                api_url = self.url + "summary/" + currency.upper() + makequery
                 response = requests.get(api_url, headers=api.header).json()
                 return response
 
+
             @classmethod
-            def snapshot(cls, market: str, currency: str, start: str, end: str, limit="10", page="1", timezone="0"):
+            def snapshot(self, market: str, currency: str, start: str, end: str, limit="10", page="1", timezone="0"):
                 """
                 :param market: BITMEX | BINANCE | BYBIT |  BITFINEX | DERIBIT | HUOBI | KRAKEN | OKX
                 :type market:
                 :param currency: BTC,ETH,BCH try the analytics future alt_currency function for more available currency
                 :type currency:
                 :param start: EXP:2022-06-07
                 :type end:
@@ -3491,64 +3488,65 @@
                 :type page:
                 :param timezone: exp : 0
                 :type timezone :
                 :return:
                 :rtype:
                 """
                 makequery = prepare_query(start=start, end=end, limit=limit, page=page, timezone=timezone)
-                api_url = cls.url + "snapshot/" + market.upper() + "/" + currency.upper() + makequery
+                api_url = self.url + "snapshot/" + market.upper() + "/" + currency.upper() + makequery
                 response = requests.get(api_url, headers=api.header).json()
                 return response
 
     class pricer:
         url = "https://api.laevitas.ch/pricer/"
         pass
 
         @classmethod
-        def risk_slide_shocked(cls, market: str, currency: str, atm_iv_shock, spot_shock):
+        def risk_slide_shocked(self, market: str, currency: str, atm_iv_shock, spot_shock):
             """
             :param market: deribit , binance
             :type market:
             :param currency: BTC | ETH ... check risk_slide_instruments
             :type currency:
             :param atm_iv_shock: -5
             :type atm_iv_shock:
             :param spot_shock: 0.1
             :type spot_shock:
             :return:
             :rtype:
             """
             makequery = prepare_query(atm_iv_shock=atm_iv_shock, spot_shock=spot_shock)
-            api_url = cls.url + "risk_slide_shocked" + "/" + market.lower() + "/" + currency.upper() + makequery
+            api_url = self.url + "risk_slide_shocked" + "/" + market.lower() + "/" + currency.upper() + makequery
             responsedata = requests.get(api_url, headers=api.header).json()
             return responsedata
 
         @classmethod
-        def risk_slide_instruments(cls, market: str):
+        def risk_slide_instruments(self, market: str):
             """
             :param market: deribit , binance
             :type market:
             :return:
             :rtype:
             """
-            api_url = cls.url + "risk_slide_instruments" + "/" + market.lower()
+            api_url = self.url + "risk_slide_instruments" + "/" + market.lower()
             responsedata = requests.get(api_url, headers=api.header).json()
             return responsedata
 
+
         @classmethod
-        def risk_slide(cls, market: str, currency: str, atm_iv_shock, spot_shock):
+        def risk_slide(self, market: str, currency: str, atm_iv_shock, spot_shock):
             """
             :param market: deribit , binance
             :type market:
             :param currency: BTC | ETH ... check risk_slide_instruments
             :type currency:
             :param atm_iv_shock: -5
             :type atm_iv_shock:
             :param spot_shock: 0.1
             :type spot_shock:
             :return:
             :rtype:
             """
             makequery = prepare_query(atm_iv_shock=atm_iv_shock, spot_shock=spot_shock)
-            api_url = cls.url + "risk_slide_shocked" + "/" + market.lower() + "/" + currency.upper() + makequery
+            api_url = self.url + "risk_slide_shocked" + "/" + market.lower() + "/" + currency.upper() + makequery
             responsedata = requests.get(api_url, headers=api.header).json()
             return responsedata
```

### Comparing `SDK-Laevitas-2.0.0/Laevitas/consts.py` & `SDK-Laevitas-2.0.0b0/Laevitas/consts.py`

 * *Files identical despite different names*

### Comparing `SDK-Laevitas-2.0.0/Laevitas/dataclasses.py` & `SDK-Laevitas-2.0.0b0/Laevitas/dataclasses.py`

 * *Files identical despite different names*

### Comparing `SDK-Laevitas-2.0.0/Laevitas/test_SDK.py` & `SDK-Laevitas-2.0.0b0/Laevitas/test_SDK.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from unittest import TestCase
 from unittest.mock import MagicMock, patch
 from Laevitas import SDK
 
 sdk = SDK.api()
-sdk.configure('your-api-key')
+sdk.configure('35ee699f-7003-4fad-948f-921d4fdb7603')
 
 
 class Testoptions(TestCase):
     def test_instruments(self):
         message = "Test value is not true."
         response = sdk.realtime.options.instruments(market="deribit", currency="btc")
         self.assertTrue(response, message)
```

### Comparing `SDK-Laevitas-2.0.0/setup.py` & `SDK-Laevitas-2.0.0b0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup
 
 
 with open("README.md") as readme:
     README = readme.read()
 setup(
     name='SDK-Laevitas',
-    version='2.0.0',
+    version='v2.0.0-beta',
     packages=['Laevitas'],
-    url='https://github.com/Laevitas/Laevitas-sdk',
-    download_url='https://github.com/Laevitas/Laevitas-sdk/archive/refs/tags/v2.0.0.tar.gz',
+    url='https://github.com/Elyesbdakhlia',
+    download_url='https://github.com/Elyesbdakhlia/API-SDK/archive/refs/tags/v2.0.0-beta.tar.gz',
     license='apache-2.0',
     author='Elyes',
     author_email='elyes@laevitas.ch',
     description='SDK',
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     install_requires=[
```

