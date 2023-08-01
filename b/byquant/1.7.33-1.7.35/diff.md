# Comparing `tmp/byquant-1.7.33.tar.gz` & `tmp/byquant-1.7.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byquant-1.7.33.tar", last modified: Mon Jul 31 09:41:03 2023, max compression
+gzip compressed data, was "byquant-1.7.35.tar", last modified: Tue Aug  1 10:47:14 2023, max compression
```

## Comparing `byquant-1.7.33.tar` & `byquant-1.7.35.tar`

### file list

```diff
@@ -1,162 +1,228 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 09:41:03.708782 byquant-1.7.33/
--rw-rw-rw-   0        0        0     1451 2023-07-31 09:41:03.706788 byquant-1.7.33/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-05-16 07:39:16.000000 byquant-1.7.33/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 09:41:02.950033 byquant-1.7.33/byquant/
--rw-rw-rw-   0        0        0     7788 2023-07-31 04:54:48.000000 byquant-1.7.33/byquant/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 09:41:02.999556 byquant-1.7.33/byquant/crypto/
--rw-rw-rw-   0        0        0       63 2023-06-27 01:17:34.000000 byquant-1.7.33/byquant/crypto/__init__.py
--rw-rw-rw-   0        0        0    17167 2023-06-27 01:17:45.000000 byquant-1.7.33/byquant/crypto/broker.py
--rw-rw-rw-   0        0        0     8092 2023-06-27 01:17:57.000000 byquant-1.7.33/byquant/crypto/feed.py
--rw-rw-rw-   0        0        0     7942 2021-09-04 05:54:05.000000 byquant-1.7.33/byquant/crypto/store.py
-drwxrwxrwx   0        0        0        0 2023-07-31 09:41:03.010531 byquant-1.7.33/byquant/data/
--rw-rw-rw-   0        0        0     1143 2023-07-31 09:40:19.000000 byquant-1.7.33/byquant/data/__init__.py
--rw-rw-rw-   0        0        0    29387 2023-07-31 09:40:10.000000 byquant-1.7.33/byquant/data/get.py
-drwxrwxrwx   0        0        0        0 2023-07-31 09:41:03.618291 byquant-1.7.33/byquant/exchange/
--rw-rw-rw-   0        0        0    14497 2023-07-28 11:41:17.000000 byquant-1.7.33/byquant/exchange/__init__.py
--rw-rw-rw-   0        0        0    41329 2023-05-15 07:52:05.000000 byquant-1.7.33/byquant/exchange/ace.py
--rw-rw-rw-   0        0        0    33161 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/alpaca.py
--rw-rw-rw-   0        0        0   129270 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/ascendex.py
--rw-rw-rw-   0        0        0     1136 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/bequant.py
--rw-rw-rw-   0        0        0    62340 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/bigone.py
--rw-rw-rw-   0        0        0   378516 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/binance.py
--rw-rw-rw-   0        0        0     1645 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/binancecoinm.py
--rw-rw-rw-   0        0        0     2151 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/binanceus.py
--rw-rw-rw-   0        0        0     2480 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/binanceusdm.py
--rw-rw-rw-   0        0        0    35482 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/bit2c.py
--rw-rw-rw-   0        0        0    39008 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/bitbank.py
--rw-rw-rw-   0        0        0      448 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/bitbay.py
--rw-rw-rw-   0        0        0    45973 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/bitbns.py
--rw-rw-rw-   0        0        0      467 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/bitcoincom.py
--rw-rw-rw-   0        0        0    69312 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/bitfinex.py
--rw-rw-rw-   0        0        0   111509 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/bitfinex2.py
--rw-rw-rw-   0        0        0    37741 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/bitflyer.py
--rw-rw-rw-   0        0        0    28316 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/bitforex.py
--rw-rw-rw-   0        0        0   204946 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/bitget.py
--rw-rw-rw-   0        0        0    42572 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/bithumb.py
--rw-rw-rw-   0        0        0   131429 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/bitmart.py
--rw-rw-rw-   0        0        0   119564 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/bitmex.py
--rw-rw-rw-   0        0        0    63261 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/bitopro.py
--rw-rw-rw-   0        0        0    87308 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/bitpanda.py
--rw-rw-rw-   0        0        0    88097 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/bitrue.py
--rw-rw-rw-   0        0        0    68449 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/bitso.py
--rw-rw-rw-   0        0        0    82190 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/bitstamp.py
--rw-rw-rw-   0        0        0    17785 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/bitstamp1.py
--rw-rw-rw-   0        0        0    93397 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/bittrex.py
--rw-rw-rw-   0        0        0    76761 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/bitvavo.py
--rw-rw-rw-   0        0        0    74167 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/bkex.py
--rw-rw-rw-   0        0        0    16241 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/bl3p.py
--rw-rw-rw-   0        0        0    47120 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/blockchaincom.py
--rw-rw-rw-   0        0        0    35160 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/btcalpha.py
--rw-rw-rw-   0        0        0    22489 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/btcbox.py
--rw-rw-rw-   0        0        0   110784 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/btcex.py
--rw-rw-rw-   0        0        0    48547 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/btcmarkets.py
--rw-rw-rw-   0        0        0    22177 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/btctradeua.py
--rw-rw-rw-   0        0        0    35384 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/btcturk.py
--rw-rw-rw-   0        0        0    45591 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/buda.py
--rw-rw-rw-   0        0        0   393944 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/bybit.py
--rw-rw-rw-   0        0        0    64922 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/cex.py
--rw-rw-rw-   0        0        0   124582 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/coinbase.py
--rw-rw-rw-   0        0        0     1219 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/coinbaseprime.py
--rw-rw-rw-   0        0        0    73787 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/coinbasepro.py
--rw-rw-rw-   0        0        0    34208 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/coincheck.py
--rw-rw-rw-   0        0        0   191859 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/coinex.py
--rw-rw-rw-   0        0        0    38956 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/coinfalcon.py
--rw-rw-rw-   0        0        0    39461 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/coinmate.py
--rw-rw-rw-   0        0        0    34455 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/coinone.py
--rw-rw-rw-   0        0        0    81092 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/coinsph.py
--rw-rw-rw-   0        0        0    18778 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/coinspot.py
--rw-rw-rw-   0        0        0   108248 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/cryptocom.py
--rw-rw-rw-   0        0        0    79611 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/currencycom.py
--rw-rw-rw-   0        0        0    84060 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/delta.py
--rw-rw-rw-   0        0        0   119018 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/deribit.py
--rw-rw-rw-   0        0        0   152160 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/digifinex.py
--rw-rw-rw-   0        0        0    88724 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/exmo.py
--rw-rw-rw-   0        0        0     1169 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/flowbtc.py
--rw-rw-rw-   0        0        0     1238 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/fmfwio.py
--rw-rw-rw-   0        0        0   221725 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/gate.py
--rw-rw-rw-   0        0        0      445 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/gateio.py
--rw-rw-rw-   0        0        0    69001 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/gemini.py
--rw-rw-rw-   0        0        0    62241 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/hitbtc.py
--rw-rw-rw-   0        0        0   116511 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/hitbtc3.py
--rw-rw-rw-   0        0        0    69194 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/hollaex.py
--rw-rw-rw-   0        0        0   362643 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/huobi.py
--rw-rw-rw-   0        0        0    86605 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/huobijp.py
--rw-rw-rw-   0        0        0      572 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/huobipro.py
--rw-rw-rw-   0        0        0    67332 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/idex.py
--rw-rw-rw-   0        0        0    29810 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/independentreserve.py
--rw-rw-rw-   0        0        0    42437 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/indodax.py
--rw-rw-rw-   0        0        0    34960 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/itbit.py
--rw-rw-rw-   0        0        0   101404 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/kraken.py
--rw-rw-rw-   0        0        0    81722 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/krakenfutures.py
--rw-rw-rw-   0        0        0   160363 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/kucoin.py
--rw-rw-rw-   0        0        0   101171 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/kucoinfutures.py
--rw-rw-rw-   0        0        0    37750 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/kuna.py
--rw-rw-rw-   0        0        0    70007 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/latoken.py
--rw-rw-rw-   0        0        0    33717 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/lbank.py
--rw-rw-rw-   0        0        0    97857 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/lbank2.py
--rw-rw-rw-   0        0        0    40473 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/luno.py
--rw-rw-rw-   0        0        0    48461 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/lykke.py
--rw-rw-rw-   0        0        0    34639 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/mercado.py
--rw-rw-rw-   0        0        0   209226 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/mexc.py
--rw-rw-rw-   0        0        0      441 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/mexc3.py
--rw-rw-rw-   0        0        0   106106 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/ndax.py
--rw-rw-rw-   0        0        0    61638 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/novadax.py
--rw-rw-rw-   0        0        0    37055 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/oceanex.py
--rw-rw-rw-   0        0        0   177794 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/okcoin.py
--rw-rw-rw-   0        0        0      434 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/okex.py
--rw-rw-rw-   0        0        0      441 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/okex5.py
--rw-rw-rw-   0        0        0   264399 2023-06-15 05:48:33.000000 byquant-1.7.33/byquant/exchange/okx.py
--rw-rw-rw-   0        0        0    22745 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/paymium.py
--rw-rw-rw-   0        0        0   191805 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/phemex.py
--rw-rw-rw-   0        0        0    88311 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/poloniex.py
--rw-rw-rw-   0        0        0    75104 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/poloniexfutures.py
--rw-rw-rw-   0        0        0    69774 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/probit.py
--rw-rw-rw-   0        0        0    47325 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/ripio.py
--rw-rw-rw-   0        0        0   117868 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/stex.py
--rw-rw-rw-   0        0        0    42407 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/tidex.py
--rw-rw-rw-   0        0        0    65452 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/timex.py
--rw-rw-rw-   0        0        0   119250 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/tokocrypto.py
--rw-rw-rw-   0        0        0    75531 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/upbit.py
--rw-rw-rw-   0        0        0   103453 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/wavesexchange.py
--rw-rw-rw-   0        0        0    35544 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/wazirx.py
--rw-rw-rw-   0        0        0    92139 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/whitebit.py
--rw-rw-rw-   0        0        0    94453 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/woo.py
--rw-rw-rw-   0        0        0   196488 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/xt.py
--rw-rw-rw-   0        0        0    51368 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/yobit.py
--rw-rw-rw-   0        0        0    28777 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/zaif.py
--rw-rw-rw-   0        0        0   183857 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/zb.py
--rw-rw-rw-   0        0        0    74036 2023-05-14 16:20:52.000000 byquant-1.7.33/byquant/exchange/zonda.py
-drwxrwxrwx   0        0        0        0 2023-07-31 09:41:03.661153 byquant-1.7.33/byquant/indicator/
--rw-rw-rw-   0        0        0     1017 2023-07-28 11:52:03.000000 byquant-1.7.33/byquant/indicator/__init__.py
--rw-rw-rw-   0        0        0     1097 2023-07-31 02:51:15.000000 byquant-1.7.33/byquant/indicator/atr.py
--rw-rw-rw-   0        0        0     1157 2023-07-31 02:50:20.000000 byquant-1.7.33/byquant/indicator/bbands.py
--rw-rw-rw-   0        0        0     1099 2023-07-31 02:47:05.000000 byquant-1.7.33/byquant/indicator/cci.py
--rw-rw-rw-   0        0        0     1078 2023-07-31 02:50:51.000000 byquant-1.7.33/byquant/indicator/dema.py
--rw-rw-rw-   0        0        0     1074 2023-07-31 02:51:06.000000 byquant-1.7.33/byquant/indicator/ma.py
--rw-rw-rw-   0        0        0     1161 2023-07-31 02:46:47.000000 byquant-1.7.33/byquant/indicator/macd.py
--rw-rw-rw-   0        0        0     1105 2023-07-31 02:47:46.000000 byquant-1.7.33/byquant/indicator/rsi.py
--rw-rw-rw-   0        0        0     1081 2023-07-31 02:43:20.000000 byquant-1.7.33/byquant/indicator/sma.py
-drwxrwxrwx   0        0        0        0 2023-07-31 09:41:03.690140 byquant-1.7.33/byquant/indicators/
--rw-rw-rw-   0        0        0     1017 2023-07-28 11:52:03.000000 byquant-1.7.33/byquant/indicators/__init__.py
--rw-rw-rw-   0        0        0     1253 2023-07-30 04:22:54.000000 byquant-1.7.33/byquant/indicators/atr.py
--rw-rw-rw-   0        0        0     1253 2023-07-30 04:22:48.000000 byquant-1.7.33/byquant/indicators/cci.py
--rw-rw-rw-   0        0        0     1254 2023-07-30 04:22:40.000000 byquant-1.7.33/byquant/indicators/macd.py
--rw-rw-rw-   0        0        0     1254 2023-07-30 04:22:36.000000 byquant-1.7.33/byquant/indicators/rsi.py
--rw-rw-rw-   0        0        0     1254 2023-07-30 04:24:59.000000 byquant-1.7.33/byquant/indicators/sma.py
--rw-rw-rw-   0        0        0     2317 2023-07-31 07:31:07.000000 byquant-1.7.33/byquant/metabacktest.py
--rw-rw-rw-   0        0        0     1117 2023-07-30 04:29:44.000000 byquant-1.7.33/byquant/metastrategy.py
-drwxrwxrwx   0        0        0        0 2023-07-31 09:41:03.694816 byquant-1.7.33/byquant/strategy/
--rw-rw-rw-   0        0        0      922 2023-07-30 04:49:12.000000 byquant-1.7.33/byquant/strategy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 09:41:03.700807 byquant-1.7.33/byquant/tool/
--rw-rw-rw-   0        0        0        0 2023-06-27 01:25:40.000000 byquant-1.7.33/byquant/tool/__init__.py
--rw-rw-rw-   0        0        0     3427 2023-02-15 05:30:28.000000 byquant-1.7.33/byquant/tool/tawPlus.py
-drwxrwxrwx   0        0        0        0 2023-07-31 09:41:02.979413 byquant-1.7.33/byquant.egg-info/
--rw-rw-rw-   0        0        0     1451 2023-07-31 09:41:02.000000 byquant-1.7.33/byquant.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4079 2023-07-31 09:41:02.000000 byquant-1.7.33/byquant.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 09:41:02.000000 byquant-1.7.33/byquant.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-07-31 09:41:02.000000 byquant-1.7.33/byquant.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-31 09:41:02.000000 byquant-1.7.33/byquant.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-05-15 09:08:59.000000 byquant-1.7.33/byquant.egg-info/zip-safe
--rw-rw-rw-   0        0        0      190 2023-07-31 09:40:32.000000 byquant-1.7.33/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-31 09:41:03.709780 byquant-1.7.33/setup.cfg
--rw-rw-rw-   0        0        0     2880 2023-07-31 09:40:36.000000 byquant-1.7.33/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 10:47:14.403360 byquant-1.7.35/
+-rw-rw-rw-   0        0        0     1451 2023-08-01 10:47:14.401367 byquant-1.7.35/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2023-05-16 07:39:16.000000 byquant-1.7.35/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 10:47:13.340510 byquant-1.7.35/byquant/
+-rw-rw-rw-   0        0        0     7788 2023-07-31 04:54:48.000000 byquant-1.7.35/byquant/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 10:47:13.381403 byquant-1.7.35/byquant/chart/
+-rw-rw-rw-   0        0        0      971 2023-08-01 10:34:29.000000 byquant-1.7.35/byquant/chart/__init__.py
+-rw-rw-rw-   0        0        0     1061 2023-08-01 10:34:31.000000 byquant-1.7.35/byquant/chart/matplotlib.py
+-rw-rw-rw-   0        0        0     1089 2023-08-01 10:34:29.000000 byquant-1.7.35/byquant/chart/seaborn.py
+drwxrwxrwx   0        0        0        0 2023-08-01 10:47:13.400353 byquant-1.7.35/byquant/crypto/
+-rw-rw-rw-   0        0        0       63 2023-06-27 01:17:34.000000 byquant-1.7.35/byquant/crypto/__init__.py
+-rw-rw-rw-   0        0        0    17167 2023-06-27 01:17:45.000000 byquant-1.7.35/byquant/crypto/broker.py
+-rw-rw-rw-   0        0        0     8092 2023-06-27 01:17:57.000000 byquant-1.7.35/byquant/crypto/feed.py
+-rw-rw-rw-   0        0        0     7942 2021-09-04 05:54:05.000000 byquant-1.7.35/byquant/crypto/store.py
+drwxrwxrwx   0        0        0        0 2023-08-01 10:47:13.409805 byquant-1.7.35/byquant/data/
+-rw-rw-rw-   0        0        0     1143 2023-08-01 10:34:26.000000 byquant-1.7.35/byquant/data/__init__.py
+-rw-rw-rw-   0        0        0    28661 2023-08-01 10:34:25.000000 byquant-1.7.35/byquant/data/get.py
+drwxrwxrwx   0        0        0        0 2023-08-01 10:47:13.992882 byquant-1.7.35/byquant/exchange/
+-rw-rw-rw-   0        0        0    14497 2023-07-28 11:41:17.000000 byquant-1.7.35/byquant/exchange/__init__.py
+-rw-rw-rw-   0        0        0    41329 2023-05-15 07:52:05.000000 byquant-1.7.35/byquant/exchange/ace.py
+-rw-rw-rw-   0        0        0    33161 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/alpaca.py
+-rw-rw-rw-   0        0        0   129270 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/ascendex.py
+-rw-rw-rw-   0        0        0     1136 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/bequant.py
+-rw-rw-rw-   0        0        0    62340 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/bigone.py
+-rw-rw-rw-   0        0        0   378516 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/binance.py
+-rw-rw-rw-   0        0        0     1645 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/binancecoinm.py
+-rw-rw-rw-   0        0        0     2151 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/binanceus.py
+-rw-rw-rw-   0        0        0     2480 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/binanceusdm.py
+-rw-rw-rw-   0        0        0    35482 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/bit2c.py
+-rw-rw-rw-   0        0        0    39008 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/bitbank.py
+-rw-rw-rw-   0        0        0      448 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/bitbay.py
+-rw-rw-rw-   0        0        0    45973 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/bitbns.py
+-rw-rw-rw-   0        0        0      467 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/bitcoincom.py
+-rw-rw-rw-   0        0        0    69312 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/bitfinex.py
+-rw-rw-rw-   0        0        0   111509 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/bitfinex2.py
+-rw-rw-rw-   0        0        0    37741 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/bitflyer.py
+-rw-rw-rw-   0        0        0    28316 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/bitforex.py
+-rw-rw-rw-   0        0        0   204946 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/bitget.py
+-rw-rw-rw-   0        0        0    42572 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/bithumb.py
+-rw-rw-rw-   0        0        0   131429 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/bitmart.py
+-rw-rw-rw-   0        0        0   119564 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/bitmex.py
+-rw-rw-rw-   0        0        0    63261 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/bitopro.py
+-rw-rw-rw-   0        0        0    87308 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/bitpanda.py
+-rw-rw-rw-   0        0        0    88097 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/bitrue.py
+-rw-rw-rw-   0        0        0    68449 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/bitso.py
+-rw-rw-rw-   0        0        0    82190 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/bitstamp.py
+-rw-rw-rw-   0        0        0    17785 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/bitstamp1.py
+-rw-rw-rw-   0        0        0    93397 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/bittrex.py
+-rw-rw-rw-   0        0        0    76761 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/bitvavo.py
+-rw-rw-rw-   0        0        0    74167 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/bkex.py
+-rw-rw-rw-   0        0        0    16241 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/bl3p.py
+-rw-rw-rw-   0        0        0    47120 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/blockchaincom.py
+-rw-rw-rw-   0        0        0    35160 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/btcalpha.py
+-rw-rw-rw-   0        0        0    22489 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/btcbox.py
+-rw-rw-rw-   0        0        0   110784 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/btcex.py
+-rw-rw-rw-   0        0        0    48547 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/btcmarkets.py
+-rw-rw-rw-   0        0        0    22177 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/btctradeua.py
+-rw-rw-rw-   0        0        0    35384 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/btcturk.py
+-rw-rw-rw-   0        0        0    45591 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/buda.py
+-rw-rw-rw-   0        0        0   393944 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/bybit.py
+-rw-rw-rw-   0        0        0    64922 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/cex.py
+-rw-rw-rw-   0        0        0   124582 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/coinbase.py
+-rw-rw-rw-   0        0        0     1219 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/coinbaseprime.py
+-rw-rw-rw-   0        0        0    73787 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/coinbasepro.py
+-rw-rw-rw-   0        0        0    34208 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/coincheck.py
+-rw-rw-rw-   0        0        0   191859 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/coinex.py
+-rw-rw-rw-   0        0        0    38956 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/coinfalcon.py
+-rw-rw-rw-   0        0        0    39461 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/coinmate.py
+-rw-rw-rw-   0        0        0    34455 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/coinone.py
+-rw-rw-rw-   0        0        0    81092 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/coinsph.py
+-rw-rw-rw-   0        0        0    18778 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/coinspot.py
+-rw-rw-rw-   0        0        0   108248 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/cryptocom.py
+-rw-rw-rw-   0        0        0    79611 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/currencycom.py
+-rw-rw-rw-   0        0        0    84060 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/delta.py
+-rw-rw-rw-   0        0        0   119018 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/deribit.py
+-rw-rw-rw-   0        0        0   152160 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/digifinex.py
+-rw-rw-rw-   0        0        0    88724 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/exmo.py
+-rw-rw-rw-   0        0        0     1169 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/flowbtc.py
+-rw-rw-rw-   0        0        0     1238 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/fmfwio.py
+-rw-rw-rw-   0        0        0   221725 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/gate.py
+-rw-rw-rw-   0        0        0      445 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/gateio.py
+-rw-rw-rw-   0        0        0    69001 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/gemini.py
+-rw-rw-rw-   0        0        0    62241 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/hitbtc.py
+-rw-rw-rw-   0        0        0   116511 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/hitbtc3.py
+-rw-rw-rw-   0        0        0    69194 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/hollaex.py
+-rw-rw-rw-   0        0        0   362643 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/huobi.py
+-rw-rw-rw-   0        0        0    86605 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/huobijp.py
+-rw-rw-rw-   0        0        0      572 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/huobipro.py
+-rw-rw-rw-   0        0        0    67332 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/idex.py
+-rw-rw-rw-   0        0        0    29810 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/independentreserve.py
+-rw-rw-rw-   0        0        0    42437 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/indodax.py
+-rw-rw-rw-   0        0        0    34960 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/itbit.py
+-rw-rw-rw-   0        0        0   101404 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/kraken.py
+-rw-rw-rw-   0        0        0    81722 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/krakenfutures.py
+-rw-rw-rw-   0        0        0   160363 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/kucoin.py
+-rw-rw-rw-   0        0        0   101171 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/kucoinfutures.py
+-rw-rw-rw-   0        0        0    37750 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/kuna.py
+-rw-rw-rw-   0        0        0    70007 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/latoken.py
+-rw-rw-rw-   0        0        0    33717 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/lbank.py
+-rw-rw-rw-   0        0        0    97857 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/lbank2.py
+-rw-rw-rw-   0        0        0    40473 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/luno.py
+-rw-rw-rw-   0        0        0    48461 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/lykke.py
+-rw-rw-rw-   0        0        0    34639 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/mercado.py
+-rw-rw-rw-   0        0        0   209226 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/mexc.py
+-rw-rw-rw-   0        0        0      441 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/mexc3.py
+-rw-rw-rw-   0        0        0   106106 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/ndax.py
+-rw-rw-rw-   0        0        0    61638 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/novadax.py
+-rw-rw-rw-   0        0        0    37055 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/oceanex.py
+-rw-rw-rw-   0        0        0   177794 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/okcoin.py
+-rw-rw-rw-   0        0        0      434 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/okex.py
+-rw-rw-rw-   0        0        0      441 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/okex5.py
+-rw-rw-rw-   0        0        0   264399 2023-06-15 05:48:33.000000 byquant-1.7.35/byquant/exchange/okx.py
+-rw-rw-rw-   0        0        0    22745 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/paymium.py
+-rw-rw-rw-   0        0        0   191805 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/phemex.py
+-rw-rw-rw-   0        0        0    88311 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/poloniex.py
+-rw-rw-rw-   0        0        0    75104 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/poloniexfutures.py
+-rw-rw-rw-   0        0        0    69774 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/probit.py
+-rw-rw-rw-   0        0        0    47325 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/ripio.py
+-rw-rw-rw-   0        0        0   117868 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/stex.py
+-rw-rw-rw-   0        0        0    42407 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/tidex.py
+-rw-rw-rw-   0        0        0    65452 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/timex.py
+-rw-rw-rw-   0        0        0   119250 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/tokocrypto.py
+-rw-rw-rw-   0        0        0    75531 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/upbit.py
+-rw-rw-rw-   0        0        0   103453 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/wavesexchange.py
+-rw-rw-rw-   0        0        0    35544 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/wazirx.py
+-rw-rw-rw-   0        0        0    92139 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/whitebit.py
+-rw-rw-rw-   0        0        0    94453 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/woo.py
+-rw-rw-rw-   0        0        0   196488 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/xt.py
+-rw-rw-rw-   0        0        0    51368 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/yobit.py
+-rw-rw-rw-   0        0        0    28777 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/zaif.py
+-rw-rw-rw-   0        0        0   183857 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/zb.py
+-rw-rw-rw-   0        0        0    74036 2023-05-14 16:20:52.000000 byquant-1.7.35/byquant/exchange/zonda.py
+drwxrwxrwx   0        0        0        0 2023-08-01 10:47:14.313652 byquant-1.7.35/byquant/indicator/
+-rw-rw-rw-   0        0        0     1120 2023-08-01 10:34:25.000000 byquant-1.7.35/byquant/indicator/__init__.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:19.000000 byquant-1.7.35/byquant/indicator/ad.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:19.000000 byquant-1.7.35/byquant/indicator/adosc.py
+-rw-rw-rw-   0        0        0     1099 2023-08-01 10:33:20.000000 byquant-1.7.35/byquant/indicator/adx.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:21.000000 byquant-1.7.35/byquant/indicator/adxr.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:22.000000 byquant-1.7.35/byquant/indicator/apo.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:23.000000 byquant-1.7.35/byquant/indicator/aroon.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:25.000000 byquant-1.7.35/byquant/indicator/aroonosc.py
+-rw-rw-rw-   0        0        0     1097 2023-08-01 10:33:25.000000 byquant-1.7.35/byquant/indicator/atr.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:27.000000 byquant-1.7.35/byquant/indicator/avgprice.py
+-rw-rw-rw-   0        0        0     1444 2023-08-01 10:33:29.000000 byquant-1.7.35/byquant/indicator/bbands.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:30.000000 byquant-1.7.35/byquant/indicator/beta.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:31.000000 byquant-1.7.35/byquant/indicator/bop.py
+-rw-rw-rw-   0        0        0     1099 2023-08-01 10:33:32.000000 byquant-1.7.35/byquant/indicator/cci.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:32.000000 byquant-1.7.35/byquant/indicator/cmo.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:34.000000 byquant-1.7.35/byquant/indicator/correl.py
+-rw-rw-rw-   0        0        0     1126 2023-08-01 10:33:34.000000 byquant-1.7.35/byquant/indicator/dema.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:35.000000 byquant-1.7.35/byquant/indicator/dx.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:37.000000 byquant-1.7.35/byquant/indicator/ema.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:38.000000 byquant-1.7.35/byquant/indicator/ht_dcperiod.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:39.000000 byquant-1.7.35/byquant/indicator/ht_dcphase.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:40.000000 byquant-1.7.35/byquant/indicator/ht_phasor.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:42.000000 byquant-1.7.35/byquant/indicator/ht_sine.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:43.000000 byquant-1.7.35/byquant/indicator/ht_trendmode.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:44.000000 byquant-1.7.35/byquant/indicator/kama.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:44.000000 byquant-1.7.35/byquant/indicator/linearreg.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:46.000000 byquant-1.7.35/byquant/indicator/linearreg_angle.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:47.000000 byquant-1.7.35/byquant/indicator/linearreg_intercept.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:48.000000 byquant-1.7.35/byquant/indicator/linearreg_slope.py
+-rw-rw-rw-   0        0        0     1074 2023-08-01 10:33:48.000000 byquant-1.7.35/byquant/indicator/ma.py
+-rw-rw-rw-   0        0        0     1161 2023-08-01 10:33:51.000000 byquant-1.7.35/byquant/indicator/macd.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:51.000000 byquant-1.7.35/byquant/indicator/macdext.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:52.000000 byquant-1.7.35/byquant/indicator/medprice.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:52.000000 byquant-1.7.35/byquant/indicator/mfi.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:54.000000 byquant-1.7.35/byquant/indicator/midprice.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:54.000000 byquant-1.7.35/byquant/indicator/minus_di.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:56.000000 byquant-1.7.35/byquant/indicator/minus_dm.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:56.000000 byquant-1.7.35/byquant/indicator/mom.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:57.000000 byquant-1.7.35/byquant/indicator/natr.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:58.000000 byquant-1.7.35/byquant/indicator/obv.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:59.000000 byquant-1.7.35/byquant/indicator/plus_di.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:34:00.000000 byquant-1.7.35/byquant/indicator/plus_dm.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:34:02.000000 byquant-1.7.35/byquant/indicator/pro.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:34:03.000000 byquant-1.7.35/byquant/indicator/roc.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:34:04.000000 byquant-1.7.35/byquant/indicator/rocp.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:34:05.000000 byquant-1.7.35/byquant/indicator/rocr.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:34:06.000000 byquant-1.7.35/byquant/indicator/rocr100.py
+-rw-rw-rw-   0        0        0     1105 2023-08-01 10:34:08.000000 byquant-1.7.35/byquant/indicator/rsi.py
+-rw-rw-rw-   0        0        0     1298 2023-08-01 10:34:09.000000 byquant-1.7.35/byquant/indicator/sar.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:34:10.000000 byquant-1.7.35/byquant/indicator/sarext.py
+-rw-rw-rw-   0        0        0     1205 2023-08-01 10:34:11.000000 byquant-1.7.35/byquant/indicator/sma.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:34:12.000000 byquant-1.7.35/byquant/indicator/stddev.py
+-rw-rw-rw-   0        0        0     1870 2023-08-01 10:34:13.000000 byquant-1.7.35/byquant/indicator/stoch.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:34:14.000000 byquant-1.7.35/byquant/indicator/stochf.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:34:15.000000 byquant-1.7.35/byquant/indicator/stochrsi.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:34:16.000000 byquant-1.7.35/byquant/indicator/t3.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:34:17.000000 byquant-1.7.35/byquant/indicator/tema.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:34:18.000000 byquant-1.7.35/byquant/indicator/trange.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:34:19.000000 byquant-1.7.35/byquant/indicator/trix.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:34:19.000000 byquant-1.7.35/byquant/indicator/tsf.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:34:20.000000 byquant-1.7.35/byquant/indicator/typprice.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:34:21.000000 byquant-1.7.35/byquant/indicator/ultosc.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:34:22.000000 byquant-1.7.35/byquant/indicator/var.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:34:22.000000 byquant-1.7.35/byquant/indicator/wclprice.py
+-rw-rw-rw-   0        0        0     1102 2023-08-01 10:34:23.000000 byquant-1.7.35/byquant/indicator/willr.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:34:24.000000 byquant-1.7.35/byquant/indicator/wma.py
+drwxrwxrwx   0        0        0        0 2023-08-01 10:47:14.375457 byquant-1.7.35/byquant/indicators/
+-rw-rw-rw-   0        0        0     1132 2023-08-01 10:33:11.000000 byquant-1.7.35/byquant/indicators/__init__.py
+-rw-rw-rw-   0        0        0     1134 2023-08-01 10:33:02.000000 byquant-1.7.35/byquant/indicators/adx.py
+-rw-rw-rw-   0        0        0     1253 2023-08-01 10:33:03.000000 byquant-1.7.35/byquant/indicators/atr.py
+-rw-rw-rw-   0        0        0     1144 2023-08-01 10:33:04.000000 byquant-1.7.35/byquant/indicators/bollinger.py
+-rw-rw-rw-   0        0        0     1253 2023-08-01 10:33:05.000000 byquant-1.7.35/byquant/indicators/cci.py
+-rw-rw-rw-   0        0        0     1828 2023-08-01 10:33:06.000000 byquant-1.7.35/byquant/indicators/macd.py
+-rw-rw-rw-   0        0        0     1245 2023-08-01 10:33:07.000000 byquant-1.7.35/byquant/indicators/rsi.py
+-rw-rw-rw-   0        0        0     1503 2023-08-01 10:33:08.000000 byquant-1.7.35/byquant/indicators/sar.py
+-rw-rw-rw-   0        0        0     1408 2023-08-01 10:33:09.000000 byquant-1.7.35/byquant/indicators/sma.py
+-rw-rw-rw-   0        0        0     1144 2023-08-01 10:33:09.000000 byquant-1.7.35/byquant/indicators/stochastic.py
+-rw-rw-rw-   0        0        0     1143 2023-08-01 10:33:11.000000 byquant-1.7.35/byquant/indicators/williams.py
+-rw-rw-rw-   0        0        0     2317 2023-07-31 07:31:07.000000 byquant-1.7.35/byquant/metabacktest.py
+-rw-rw-rw-   0        0        0     1117 2023-07-30 04:29:44.000000 byquant-1.7.35/byquant/metastrategy.py
+drwxrwxrwx   0        0        0        0 2023-08-01 10:47:14.385408 byquant-1.7.35/byquant/strategy/
+-rw-rw-rw-   0        0        0      922 2023-07-30 04:49:12.000000 byquant-1.7.35/byquant/strategy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 10:47:14.396380 byquant-1.7.35/byquant/tool/
+-rw-rw-rw-   0        0        0        0 2023-06-27 01:25:40.000000 byquant-1.7.35/byquant/tool/__init__.py
+-rw-rw-rw-   0        0        0     3427 2023-02-15 05:30:28.000000 byquant-1.7.35/byquant/tool/tawPlus.py
+drwxrwxrwx   0        0        0        0 2023-08-01 10:47:13.368439 byquant-1.7.35/byquant.egg-info/
+-rw-rw-rw-   0        0        0     1451 2023-08-01 10:47:13.000000 byquant-1.7.35/byquant.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5903 2023-08-01 10:47:13.000000 byquant-1.7.35/byquant.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 10:47:13.000000 byquant-1.7.35/byquant.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-08-01 10:47:13.000000 byquant-1.7.35/byquant.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-01 10:47:13.000000 byquant-1.7.35/byquant.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-15 09:08:59.000000 byquant-1.7.35/byquant.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      190 2023-08-01 10:46:35.000000 byquant-1.7.35/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-01 10:47:14.403360 byquant-1.7.35/setup.cfg
+-rw-rw-rw-   0        0        0     2880 2023-08-01 10:46:39.000000 byquant-1.7.35/setup.py
```

### Comparing `byquant-1.7.33/PKG-INFO` & `byquant-1.7.35/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byquant
-Version: 1.7.33
+Version: 1.7.35
 Summary: ByQuant.com is AI Quantitative Strategy Competition Training Community
 Home-page: https://byquant.com
 Author: Uakeey
 Author-email: uakee@outlook.com
 License: GPL
 Project-URL: Homepage, https://byquant.com
 Keywords: quant,strategy,algorithmic,algotrading
```

### Comparing `byquant-1.7.33/byquant/__init__.py` & `byquant-1.7.35/byquant/__init__.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/crypto/broker.py` & `byquant-1.7.35/byquant/crypto/broker.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/crypto/feed.py` & `byquant-1.7.35/byquant/crypto/feed.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/crypto/store.py` & `byquant-1.7.35/byquant/crypto/store.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/data/__init__.py` & `byquant-1.7.35/byquant/data/__init__.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/data/get.py` & `byquant-1.7.35/byquant/data/get.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,777 +1,778 @@
-#!/usr/bin/env python
-# -*- coding: utf-8; py-indent-offset:4 -*-
-###############################################################################
-#
-# Copyright (C) 2022-2023 ByQuant.com
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-###############################################################################
-
-from __future__ import (absolute_import, division, print_function,unicode_literals)
-
-import os
-import time
-import ccxt
-import platform
-import yfinance as yf
-import tushare as ts
-import pandas as pd
-from datetime import date, datetime, timedelta
-# from market import signals as tawSignal
-from alpaca.data.historical import CryptoHistoricalDataClient, StockHistoricalDataClient
-from alpaca.data.requests import CryptoBarsRequest, StockBarsRequest
-from alpaca.data.timeframe import TimeFrame
-from alpaca.trading.client import TradingClient
-from alpaca.trading.requests import GetAssetsRequest
-from alpaca.trading.enums import AssetClass
-from alpaca.trading.requests import GetOrdersRequest
-from alpaca.trading.enums import OrderSide, QueryOrderStatus
-from alpaca.trading.requests import MarketOrderRequest, LimitOrderRequest, StopOrderRequest, StopLimitOrderRequest, \
-    TrailingStopOrderRequest
-from alpaca.data.requests import CryptoLatestQuoteRequest
-
-from alpaca.broker.models import Contact, Identity, Disclosures, Agreement
-from alpaca.broker.requests import CreateAccountRequest
-from alpaca.broker.enums import TaxIdType, FundingSource, AgreementType
-from alpaca.broker.requests import CreateJournalRequest
-from alpaca.broker.enums import JournalEntryType
-from alpaca.broker.client import BrokerClient
-from alpaca.broker.requests import CreateACHTransferRequest
-from alpaca.broker.enums import TransferDirection, TransferTiming
-from alpaca.trading.enums import OrderSide, TimeInForce
-
-from alpaca.broker.requests import CreateACHRelationshipRequest
-from alpaca.broker.enums import BankAccountType
-# import byquant
-from byquant import exchange
-
-
-# from market import models as marketModels
-
-class Bar():
-
-    def __init__(self, symbol, ktype='quote', freq='1d', tawtime=86400, renew='0', cache=False, start='', end='', limit=''):
-        self.symbol = symbol
-        self.market = self.getSymbolInfo()['market']
-        self.limit = 1000
-        self.offset = 0
-        self.ktype = ktype
-        self.freq = freq
-        self.start = start
-        self.end = end
-        self.limit=limit
-        
-
-
-
-
-        self.tawtime = tawtime
-        self.renew = renew
-        self.cache = cache
-        self.haskey = 'no'
-        self.exchange = self.symbol.split('.')[-1]
-        self.underlying = self.symbol.replace('~', '/').replace('$', ':').replace('.' + self.exchange, '')
-        self.MARKET_DATA_PATH = '~/temp/%s/' % (self.ktype)
-        if not os.path.isdir('~/temp/'):
-            os.makedirs('~/temp/')
-            if not os.path.isdir(self.MARKET_DATA_PATH):
-                os.makedirs(self.MARKET_DATA_PATH)
-        self.tushareKey = 'Your  API  Token'
-        self.filepath = self.MARKET_DATA_PATH + '%s/%s/%s.csv' % (
-        self.exchange, self.freq, self.symbol.replace('.' + self.exchange, ''))
-
-        self.underlying_ex = self.underlying
-        if self.exchange == 'SSE':
-            self.underlying_ex = self.underlying_ex.replace('SH', '') + '.SH'
-        elif self.exchange == 'SZSE':
-            self.underlying_ex = self.underlying_ex.replace('SZ', '') + '.SZ'
-        elif self.exchange == 'BSE':
-            self.underlying_ex = self.underlying_ex.replace('BJ', '') + '.BJ'
-        elif self.exchange == 'HKEX':
-            self.underlying_ex = self.underlying_ex.replace('HK', '') + '.HK'
-
-        # print(self.tushareKey)
-        # print(self.market)
-
-    def quote(self):
-
-        # print(self.haskey)
-        self.haskey = self.checkKey()
-        # print(self.filepath)
-        # print(self.symbol)
-        # print(self.haskey)
-        # print(self.haskey)
-        if not os.path.exists(self.filepath):
-            result = self.createQuote()
-        elif self.haskey == 'no':
-            result = self.createQuote()
-        elif self.renew == '0':
-            result = self.readCSV()
-        else:
-            fileTime = int(os.path.getmtime(self.filepath))
-            nowTime = time.time()
-            expireTime = fileTime + self.tawtime
-            if nowTime > expireTime:
-                result = self.updateQuote()
-            else:
-                result = self.readCSV()
-
-        result.rename(columns={"quote_time": "datetime"}, inplace=True)
-        result['datetime'] = pd.to_datetime(result['datetime'])
-        result = result.sort_values('datetime')  # 数据顺序排列
-
-        return result
-
-    def quoteTimeSort(self):
-
-        result = self.quote()
-        result.rename(columns={"quote_time": "datetime"}, inplace=True)
-        result['datetime'] = pd.to_datetime(result['datetime'])
-        # print(df)
-        result = result.sort_values('datetime')  # 数据顺序排列
-        # print(df)
-
-        return result
-
-    def signal(self):
-        self.haskey = self.checkKey()
-        if not os.path.exists(self.filepath):
-            result = self.createSignal()
-        elif self.haskey == 'no':
-            result = self.createSignal()
-        else:
-            result = self.readCSV()
-        return result
-
-    def createQuote(self):
-        df = {}
-        try:
-
-            if self.exchange in ['SSE', 'SZSE', 'BSE', 'AMEX', 'ARCA', 'BATS', 'HKEX', 'NASDAQ', 'NYSE', 'OTC',
-                                 'NYSEARCA', 'FTXU', 'CBSE', 'GNSS', 'ERSX']:
-                # print('yahoo_0')
-                df = self.yahooApi()
-
-                if len(df) < 10:
-                    if self.exchange in ['SSE', 'SZSE', 'BSE']:
-                        # print('tushare_cn')
-                        if self.market == 'FUND':
-                            df = self.tushareFundApi()
-                        elif self.market == 'STOCK':
-                            df = self.tushareStockApi()
-                        else:
-                            pass
-
-
-                    elif self.exchange in ['AMEX', 'ARCA', 'BATS', 'NASDAQ', 'NYSE', 'OTC', 'NYSEARCA', 'FTXU', 'CBSE',
-                                           'GNSS', 'ERSX']:
-
-                        # print('alpaca_1')
-
-                        df = self.tushareCNStockApi()
-                    elif self.exchange in ['HKEX']:
-                        # print('tushare_hk')
-                        df = self.tushareHKStockApi()  # 没有权限
-
-
-            elif self.exchange == 'ALPACA':
-                df = self.alpacaCryptoApi()
-
-            else:
-                df = self.ccxtApi()
-
-            if len(df) > 0 and self.cache:
-                self.saveCSV(df)
-
-
-
-        except Exception as e:
-            print(e.args)
-            pass
-
-        ###########
-
-        return df
-
-    def yahooApi(self):
-        df = {}
-        try:
-            if self.freq == 'D' or self.freq == '1d':
-                periodlUS = '10y'
-                intervalUS = '1d'
-            elif self.freq == '1min' or self.freq == '1m':
-                periodlUS = '7d'
-                intervalUS = '1m'
-            elif self.freq == '5min':
-                periodlUS = '60d'
-                intervalUS = '5m'
-            elif self.freq == '15min':
-                periodlUS = '60d'
-                intervalUS = '15m'
-            elif self.freq == '30min':
-                periodlUS = '60d'
-                intervalUS = '30m'
-            elif self.freq == '60min' or self.freq == '1h':
-                periodlUS = '1y'
-                intervalUS = '1h'
-            elif self.freq == 'W':
-                periodlUS = '1y'
-                intervalUS = '1wk'
-            elif self.freq == 'M':
-                periodlUS = '1y'
-                intervalUS = '1mo'
-
-            self.underlying_ex = self.underlying_ex.replace('.SH', '.SS')
-            if self.start == '':
-                dfTemp = yf.download(  # or pdr.get_data_yahoo(...
-                    tickers=self.underlying_ex,  # tickers list or string as well
-                    period=periodlUS,
-                    # use "period" instead of start/end # valid periods: 1d,5d,1mo,3mo,6mo,1y,2y,5y,10y,ytd,max# (optional, default is '1mo')
-                    interval=intervalUS,
-                    # valid intervals: 1m,2m,5m,15m,30m,60m,90m,1h,1d,5d,1wk,1mo,3mo  # fetch data by interval (including intraday if period < 60 days) # (optional, default is '1d')
-                    ignore_tz=False,
-                    # Whether to ignore timezone when aligning ticker data from # different timezones. Default is False.
-                    group_by='ticker',  # group by ticker (to access via data['SPY']) # (optional, default is 'column')
-                    auto_adjust=True,  # adjust all OHLC automatically # (optional, default is False)
-                    repair=False,  # attempt repair of missing data or currency mixups e.g. $/cents
-                    prepost=True,  # download pre/post regular market hours data # (optional, default is False)
-                    threads=True,
-                    # use threads for mass downloading? (True/False/Integer) # (optional, default is True)
-                    proxy=None  # proxy URL scheme use use when downloading?# (optional, default is None)
-                )
-            else:
-                if self.end == '':
-                    self.end = date.today()
-                
-                dfTemp = yf.download(  # or pdr.get_data_yahoo(...
-                    tickers=self.underlying_ex,  # tickers list or string as well
-                    start=self.start,
-                    end=self.end,
-                    # use "period" instead of start/end # valid periods: 1d,5d,1mo,3mo,6mo,1y,2y,5y,10y,ytd,max# (optional, default is '1mo')
-                    interval=intervalUS,
-                    # valid intervals: 1m,2m,5m,15m,30m,60m,90m,1h,1d,5d,1wk,1mo,3mo  # fetch data by interval (including intraday if period < 60 days) # (optional, default is '1d')
-                    ignore_tz=False,
-                    # Whether to ignore timezone when aligning ticker data from # different timezones. Default is False.
-                    group_by='ticker',  # group by ticker (to access via data['SPY']) # (optional, default is 'column')
-                    auto_adjust=True,  # adjust all OHLC automatically # (optional, default is False)
-                    repair=False,  # attempt repair of missing data or currency mixups e.g. $/cents
-                    prepost=True,  # download pre/post regular market hours data # (optional, default is False)
-                    threads=True,
-                    # use threads for mass downloading? (True/False/Integer) # (optional, default is True)
-                    proxy=None  # proxy URL scheme use use when downloading?# (optional, default is None)
-                )
-
-            dfTemp.reset_index(drop=False, inplace=True)
-            if self.freq == 'D' or self.freq == '1d' or self.freq == 'W' or self.freq == 'M':
-                dfTemp['Datetime'] = dfTemp['Date']
-                dfTemp['Datetime'] = dfTemp['Datetime'].dt.tz_convert('UTC')
-                dfTemp['Datetime'] = dfTemp['Datetime'].dt.tz_localize(None)
-            # dfTemp['symbol'] = self.symbol
-
-            df = pd.DataFrame()
-            df['quote_time'] = dfTemp['Datetime']
-            df['open'] = dfTemp['Open']
-            df['high'] = dfTemp['High']
-            df['low'] = dfTemp['Low']
-            df['close'] = dfTemp['Close']
-            df['volume'] = dfTemp['Volume']
-
-
-
-
-        except Exception as e:
-            print(e.args)
-            pass
-
-        ###########
-
-        return df
-
-    def tushareCNStockApi(self):
-        df = {}
-        try:
-            pro = ts.pro_api(self.tushareKey)
-            # underlying = self.symbol.replace('~', '/').replace('$', ':').replace('.' + self.exchange, '')
-            if self.exchange == 'SSE':
-                self.underlying_ex = self.underlying_ex.replace('.SS', '.SH')
-            # 拉取数据
-
-            """if self.start == '':
-                self.start = date.today() + timedelta(days=-1000)
-            if self.freq == '1m':
-                self.start = date.today() + timedelta(days=-15)
-            if self.end == '':
-                self.end = date.today()"""
-
-
-            startDay = date.today() + timedelta(days=-1000)
-            if self.freq == '1m':
-                startDay = date.today() + timedelta(days=-15)
-            startDay = format(startDay.strftime('%Y%m%d'))
-            # print(LastWeek)
-            toDay = date.today()
-            toDay = format(toDay.strftime('%Y%m%d'))
-            # print(startDay)
-            # print(toDay)
-            # print(self.underlying)
-            dfTemp = pro.daily(**{
-                "ts_code": self.underlying_ex, "trade_date": "", "start_date": startDay, "end_date": toDay,
-                "offset": "",
-                "limit": ""
-            }, fields=[
-                "ts_code", "trade_date", "open", "high", "low", "close", "pre_close", "change", "pct_chg", "vol",
-                "amount"
-            ])
-            # print(dfTemp)
-
-            df = pd.DataFrame()
-            df['quote_time'] = dfTemp['trade_date']
-            df['open'] = dfTemp['open']
-            df['high'] = dfTemp['high']
-            df['low'] = dfTemp['low']
-            df['close'] = dfTemp['close']
-            df['volume'] = dfTemp['vol']
-
-
-
-
-        except Exception as e:
-            print(e.args)
-            pass
-
-        ###########
-
-        return df
-
-    def tushareHKStockApi(self):
-        df = {}
-        try:
-            pro = ts.pro_api(self.tushareKey)
-            startDay = date.today() + timedelta(days=-1000)
-            if self.freq == '1m':
-                startDay = date.today() + timedelta(days=-15)
-            startDay = format(startDay.strftime('%Y%m%d'))
-            # print(LastWeek)
-            toDay = date.today()
-            toDay = format(toDay.strftime('%Y%m%d'))
-            # print(startDay)
-            # print(toDay)
-            # print(self.underlying)
-            dfTemp = pro.hk_daily(**{
-                "ts_code": self.underlying, "trade_date": "", "start_date": startDay, "end_date": toDay, "offset": "",
-                "limit": ""
-            }, fields=[
-                "ts_code", "trade_date", "open", "high", "low", "close", "pre_close", "change", "pct_chg", "vol",
-                "amount"
-            ])
-            # print(dfTemp)
-
-            df = pd.DataFrame()
-            df['quote_time'] = dfTemp['trade_date']
-            df['open'] = dfTemp['open']
-            df['high'] = dfTemp['high']
-            df['low'] = dfTemp['low']
-            df['close'] = dfTemp['close']
-            df['volume'] = dfTemp['vol']
-
-
-
-
-        except Exception as e:
-            print(e.args)
-            pass
-
-        ###########
-
-        return df
-
-    def tushareFundApi(self):
-        df = {}
-        try:
-            pro = ts.pro_api(self.tushareKey)
-            # underlying = self.symbol.replace('~', '/').replace('$', ':').replace('.' + self.exchange, '')
-            if self.exchange == 'SSE':
-                self.underlying = self.underlying.replace('.SS', '.SH')
-            # 拉取数据
-
-            startDay = date.today() + timedelta(days=-1000)
-            if self.freq == '1m':
-                startDay = date.today() + timedelta(days=-15)
-            startDay = format(startDay.strftime('%Y%m%d'))
-            # print(LastWeek)
-            toDay = date.today()
-            toDay = format(toDay.strftime('%Y%m%d'))
-            # print(startDay)
-            # print(toDay)
-            # print(self.underlying)
-            dfTemp = pro.fund_daily(**{
-                "ts_code": self.underlying, "trade_date": "", "start_date": startDay, "end_date": toDay, "offset": "",
-                "limit": ""
-            }, fields=[
-                "ts_code", "trade_date", "open", "high", "low", "close", "pre_close", "change", "pct_chg", "vol",
-                "amount"
-            ])
-            # print(dfTemp)
-
-            df = pd.DataFrame()
-            df['quote_time'] = dfTemp['trade_date']
-            df['open'] = dfTemp['open']
-            df['high'] = dfTemp['high']
-            df['low'] = dfTemp['low']
-            df['close'] = dfTemp['close']
-            df['volume'] = dfTemp['vol']
-
-
-
-
-        except Exception as e:
-            print(e.args)
-            pass
-
-        ###########
-
-        return df
-
-    def ccxtApi(self):
-        df = {}
-        try:
-            # getExchange = tawCCXT(self.exchange)
-            # getExchange = byquant.getExchange(self.exchange)
-            getExchange = exchange.get(self.exchange)
-            getExchange.load_markets()
-
-            strFreq = self.freq
-            if strFreq == '1min':
-                strFreq = '1m'
-            elif strFreq == 'H':
-                strFreq = '1h'
-            elif strFreq == 'D':
-                strFreq = '1d'
-            elif strFreq == 'M':
-                strFreq = '1M'
-            elif strFreq == 'Y':
-                strFreq = '1y'
-            #limit = 1000
-            if self.limit == '':
-                self.limit = 1000
-            
-            since_date = datetime.strptime(self.start, "%Y-%m-%d")
-            # 将 datetime 对象转换为毫秒级时间戳
-            since_timestamp = int(since_date.timestamp() * 1000)
-
-            if getExchange.has['fetchOHLCV']:
-                # time.sleep(getExchange.rateLimit / 1000)  # time.sleep wants seconds
-                quotes = []
-                df = {}
-                # underlying = self.symbol.replace('~', '/').replace('$', ':').replace('.' + self.exchange, '')
-                ohlcvData = getExchange.fetchOHLCV(self.underlying, timeframe=strFreq, since =since_timestamp, limit=self.limit, params={})
-
-                for ohlcv in ohlcvData:
-                    quote = {}
-                    quoteTime = time.localtime(ohlcv[0] / 1000)
-                    quote_time = time.strftime("%Y-%m-%d %H:%M:%S", quoteTime)
-                    quote['quote_time'] = quote_time
-                    quote['open'] = ohlcv[1]
-                    quote['high'] = ohlcv[2]
-                    quote['low'] = ohlcv[3]
-                    quote['close'] = ohlcv[4]
-                    quote['volume'] = ohlcv[5]
-                    quotes.append(quote)
-
-                # df['open'] = df['ohlcv'][0]
-                df = pd.DataFrame(quotes)
-
-
-
-
-
-        except Exception as e:
-            print(e.args)
-            pass
-
-        ###########
-
-        return df
-
-    def alpacaCryptoApi(self):
-        df = {}
-        try:
-            # underlying = self.symbol.replace('~', '/').replace('$', ':').replace('.' + self.exchange.upper(), '')
-            # print([freq])
-            # toDay = date.today()
-            # toDay = format(toDay.strftime('%Y-%m-%d'))
-            client = CryptoHistoricalDataClient("Key", "KeyI")
-            # strFreq = freq
-            if self.freq == '1m':
-                # strFreq = '1m'
-                startTime = (date.today() + timedelta(days=-7)).strftime("%Y-%m-%d %H:%M:%S")
-                request_params = CryptoBarsRequest(
-                    symbol_or_symbols=[self.underlying],
-                    timeframe=TimeFrame.Minute,
-                    start=datetime.strptime(startTime, '%Y-%m-%d %H:%M:%S')
-                )
-            elif self.freq == '1h':
-                startTime = (date.today() + timedelta(days=-90)).strftime("%Y-%m-%d %H:%M:%S")
-                request_params = CryptoBarsRequest(
-                    symbol_or_symbols=[self.underlying],
-                    timeframe=TimeFrame.Hour,
-                    start=datetime.strptime(startTime, '%Y-%m-%d %H:%M:%S')
-                )
-            elif self.freq == '1d':
-                # strFreq = '1d'
-                startTime = (date.today() + timedelta(days=-1000)).strftime("%Y-%m-%d")
-                request_params = CryptoBarsRequest(
-                    symbol_or_symbols=[self.underlying],
-                    timeframe=TimeFrame.Day,
-                    start=datetime.strptime(startTime, '%Y-%m-%d')
-                )
-            else:
-                startTime = (date.today() + timedelta(days=-1000)).strftime("%Y-%m-%d")
-                request_params = CryptoBarsRequest(
-                    symbol_or_symbols=[self.underlying],
-                    timeframe=TimeFrame.Day,
-                    start=datetime.strptime(startTime, '%Y-%m-%d')
-                )
-
-            barsInfo = client.get_crypto_bars(request_params)
-            barsData = barsInfo.data
-            # print(type(barData))
-            barsList = barsData[self.underlying]
-
-            # print(barsList)
-            barList = []
-            for bars in barsList:
-                barDict = dict(bars)
-                barTemp = {}
-                barTemp['quote_time'] = str(barDict['timestamp'])
-                barTemp['open'] = float(barDict['open'])
-                barTemp['high'] = str(barDict['high'])
-                barTemp['low'] = float(barDict['low'])
-                barTemp['close'] = float(barDict['close'])
-                barTemp['volume'] = float(barDict['volume'])
-                # barTemp['trade_count'] = float(barDict['trade_count'])
-                barTemp['vwap'] = str(barDict['vwap'])
-
-                # print(tickTemp)
-                barList.append(barTemp)
-
-            dfTemp = pd.DataFrame(barList)
-            # dfTemp['symbol'] = symbol
-            df = dfTemp.tail(1000)
-            # print(df)
-
-
-
-
-
-        except Exception as e:
-            print(e.args)
-            pass
-
-        ###########
-
-        return df
-
-    def alpacaStockApi(self):
-        df = {}
-        try:
-            # underlying = self.symbol.replace('~', '/').replace('$', ':').replace('.' + self.exchange.upper(), '')
-            # print([freq])
-            # toDay = date.today()
-            # toDay = format(toDay.strftime('%Y-%m-%d'))
-            client = StockHistoricalDataClient("KEY", "KEYI")
-            # strFreq = freq
-            if self.freq == '1m':
-                # strFreq = '1m'
-                startTime = (date.today() + timedelta(days=-7)).strftime("%Y-%m-%d %H:%M:%S")
-                request_params = StockBarsRequest(
-                    symbol_or_symbols=[self.underlying],
-                    timeframe=TimeFrame.Minute,
-                    start=datetime.strptime(startTime, '%Y-%m-%d %H:%M:%S')
-                )
-            elif self.freq == '1h':
-                startTime = (date.today() + timedelta(days=-90)).strftime("%Y-%m-%d %H:%M:%S")
-                request_params = StockBarsRequest(
-                    symbol_or_symbols=[self.underlying],
-                    timeframe=TimeFrame.Hour,
-                    start=datetime.strptime(startTime, '%Y-%m-%d %H:%M:%S')
-                )
-            elif self.freq == '1d':
-                # strFreq = '1d'
-                startTime = (date.today() + timedelta(days=-1000)).strftime("%Y-%m-%d")
-                request_params = StockBarsRequest(
-                    symbol_or_symbols=[self.underlying],
-                    timeframe=TimeFrame.Day,
-                    start=datetime.strptime(startTime, '%Y-%m-%d')
-                )
-            else:
-                startTime = (date.today() + timedelta(days=-1000)).strftime("%Y-%m-%d")
-                request_params = StockBarsRequest(
-                    symbol_or_symbols=[self.underlying],
-                    timeframe=TimeFrame.Day,
-                    start=datetime.strptime(startTime, '%Y-%m-%d')
-                )
-
-            barsInfo = client.get_stock_bars(request_params)
-            barsData = barsInfo.data
-            # print(type(barData))
-            barsList = barsData[self.underlying]
-
-            # print(barsList)
-            barList = []
-            for bars in barsList:
-                barDict = dict(bars)
-                barTemp = {}
-                barTemp['quote_time'] = str(barDict['timestamp'])
-                barTemp['open'] = float(barDict['open'])
-                barTemp['high'] = str(barDict['high'])
-                barTemp['low'] = float(barDict['low'])
-                barTemp['close'] = float(barDict['close'])
-                barTemp['volume'] = float(barDict['volume'])
-                # barTemp['trade_count'] = float(barDict['trade_count'])
-                barTemp['vwap'] = str(barDict['vwap'])
-
-                # print(tickTemp)
-                barList.append(barTemp)
-
-            dfTemp = pd.DataFrame(barList)
-            # dfTemp['symbol'] = symbol
-            df = dfTemp.tail(1000)
-            # print(df)
-
-
-
-
-
-        except Exception as e:
-            print(e.args)
-            pass
-
-        ###########
-
-        return df
-
-    def saveHDF(self, data):  # 将放弃
-        result = False
-        df = data
-        try:
-
-            if len(df) > 0:
-                result = df
-                df.fillna("0", inplace=True)
-                df.sort_values(by="quote_time", ascending=False, inplace=True)
-
-                filedir = self.MARKET_DATA_PATH + '%s' % (self.exchange)
-                if not os.path.isdir(filedir):
-                    os.makedirs(filedir)
-                filepath = self.MARKET_DATA_PATH + '%s/%s.hdf' % (self.exchange, self.symbol)
-                df.to_hdf(filepath, mode='a', key='quote_%s' % (self.freq), complevel=9, complib='blosc',
-                          format='table')
-                result = True
-
-
-
-        except Exception as e:
-            print(e.args)
-            pass
-
-        ###########
-
-        return result
-
-    def saveCSV(self, data):
-        result = False
-        df = data
-        try:
-
-            if len(df) > 0:
-                result = df
-                df.fillna("0", inplace=True)
-                df.sort_values(by="quote_time", ascending=True, inplace=True)
-
-                filedir = self.MARKET_DATA_PATH + '%s' % (self.exchange)
-                if not os.path.isdir(filedir):
-                    os.makedirs(filedir)
-
-                mfiledir = self.MARKET_DATA_PATH + '%s/%s' % (self.exchange, self.freq)
-                if not os.path.isdir(mfiledir):
-                    os.makedirs(mfiledir)
-
-                df.to_csv(self.filepath, index=False)
-                """filepath = self.MARKET_DATA_PATH + '%s/%s.hdf' % (self.exchange, self.symbol)
-                df.to_hdf(filepath, mode='a', key='quote_%s' % (self.freq), complevel=9, complib='blosc',
-                          format='table')"""
-                result = True
-
-
-
-        except Exception as e:
-            print(e.args)
-            pass
-
-        ###########
-
-        return result
-
-    def createSignal(self):
-        result = tawSignal.autoStrategy(self.symbol, self.market, self.freq, self.limit, self.offset, self.tawtime)
-        return result
-
-    def updateQuote(self):
-        result = self.createQuote()  ##暂定
-        return result
-
-    """def read(self):
-        readHdf = pd.read_hdf(self.filepath, key='%s_%s' % (self.ktype, self.freq),mode='a')
-        result = pd.DataFrame(readHdf)
-        return result"""
-
-    def readHDF(self):  # 将放弃
-        readResult = pd.read_hdf(self.filepath, key='%s_%s' % (self.ktype, self.freq))
-        self.result = pd.DataFrame(readResult)
-        return self.result
-
-    def readCSV(self):
-        readResult = pd.read_csv(self.filepath)
-        self.result = pd.DataFrame(readResult)
-        return self.result
-
-    def checkKey(self):
-        result = 'no'
-        if os.path.exists(self.filepath):
-            keyName = '%s_%s' % (self.ktype, self.freq)
-            getStore = pd.HDFStore(self.filepath, 'a')
-            keyArr = getStore.keys()
-            getStore.close()
-            if keyName in keyArr:
-                result = 'yes'
-        return result
-
-    def getSymbolInfo(self):
-        result = {}
-        result['market'] = 'CRYPTO'
-        # try:
-        #    result = marketModels.Underlying.objects.filter(symbol = self.symbol).values('market')
-        # except Exception as e:
-        #    print(e.args)
-        #    pass
-        return result
-
-
-
-
-
-
-
+#!/usr/bin/env python
+# -*- coding: utf-8; py-indent-offset:4 -*-
+###############################################################################
+#
+# Copyright (C) 2022-2023 ByQuant.com
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+#
+###############################################################################
+
+from __future__ import (absolute_import, division, print_function,unicode_literals)
+
+import os
+import time
+import ccxt
+import platform
+import yfinance as yf
+import tushare as ts
+import pandas as pd
+from datetime import date, datetime, timedelta
+# from market import signals as tawSignal
+from alpaca.data.historical import CryptoHistoricalDataClient, StockHistoricalDataClient
+from alpaca.data.requests import CryptoBarsRequest, StockBarsRequest
+from alpaca.data.timeframe import TimeFrame
+from alpaca.trading.client import TradingClient
+from alpaca.trading.requests import GetAssetsRequest
+from alpaca.trading.enums import AssetClass
+from alpaca.trading.requests import GetOrdersRequest
+from alpaca.trading.enums import OrderSide, QueryOrderStatus
+from alpaca.trading.requests import MarketOrderRequest, LimitOrderRequest, StopOrderRequest, StopLimitOrderRequest, \
+    TrailingStopOrderRequest
+from alpaca.data.requests import CryptoLatestQuoteRequest
+
+from alpaca.broker.models import Contact, Identity, Disclosures, Agreement
+from alpaca.broker.requests import CreateAccountRequest
+from alpaca.broker.enums import TaxIdType, FundingSource, AgreementType
+from alpaca.broker.requests import CreateJournalRequest
+from alpaca.broker.enums import JournalEntryType
+from alpaca.broker.client import BrokerClient
+from alpaca.broker.requests import CreateACHTransferRequest
+from alpaca.broker.enums import TransferDirection, TransferTiming
+from alpaca.trading.enums import OrderSide, TimeInForce
+
+from alpaca.broker.requests import CreateACHRelationshipRequest
+from alpaca.broker.enums import BankAccountType
+# import byquant
+from byquant import exchange
+
+
+# from market import models as marketModels
+
+class Bar():
+
+    def __init__(self, symbol, ktype='quote', freq='1d', tawtime=86400, renew='0', cache=False, start='', end='', limit=''):
+        self.symbol = symbol
+        self.market = self.getSymbolInfo()['market']
+        self.limit = 1000
+        self.offset = 0
+        self.ktype = ktype
+        self.freq = freq
+        self.start = start
+        self.end = end
+        self.limit=limit
+        
+
+
+
+
+        self.tawtime = tawtime
+        self.renew = renew
+        self.cache = cache
+        self.haskey = 'no'
+        self.exchange = self.symbol.split('.')[-1]
+        self.underlying = self.symbol.replace('~', '/').replace('$', ':').replace('.' + self.exchange, '')
+        self.MARKET_DATA_PATH = '~/temp/%s/' % (self.ktype)
+        if not os.path.isdir('~/temp/'):
+            os.makedirs('~/temp/')
+            if not os.path.isdir(self.MARKET_DATA_PATH):
+                os.makedirs(self.MARKET_DATA_PATH)
+        self.tushareKey = 'Your  API  Token'
+        self.filepath = self.MARKET_DATA_PATH + '%s/%s/%s.csv' % (
+        self.exchange, self.freq, self.symbol.replace('.' + self.exchange, ''))
+
+        self.underlying_ex = self.underlying
+        if self.exchange == 'SSE':
+            self.underlying_ex = self.underlying_ex.replace('SH', '') + '.SH'
+        elif self.exchange == 'SZSE':
+            self.underlying_ex = self.underlying_ex.replace('SZ', '') + '.SZ'
+        elif self.exchange == 'BSE':
+            self.underlying_ex = self.underlying_ex.replace('BJ', '') + '.BJ'
+        elif self.exchange == 'HKEX':
+            self.underlying_ex = self.underlying_ex.replace('HK', '') + '.HK'
+
+        # print(self.tushareKey)
+        # print(self.market)
+
+    def quote(self):
+
+        # print(self.haskey)
+        self.haskey = self.checkKey()
+        # print(self.filepath)
+        # print(self.symbol)
+        # print(self.haskey)
+        # print(self.haskey)
+        if not os.path.exists(self.filepath):
+            result = self.createQuote()
+        elif self.haskey == 'no':
+            result = self.createQuote()
+        elif self.renew == '0':
+            result = self.readCSV()
+        else:
+            fileTime = int(os.path.getmtime(self.filepath))
+            nowTime = time.time()
+            expireTime = fileTime + self.tawtime
+            if nowTime > expireTime:
+                result = self.updateQuote()
+            else:
+                result = self.readCSV()
+
+        result.rename(columns={"quote_time": "datetime"}, inplace=True)
+        result['datetime'] = pd.to_datetime(result['datetime'])
+        result = result.sort_values('datetime')  # 数据顺序排列
+        result.set_index('datetime', inplace=True)
+
+        return result
+
+    def quoteTimeSort(self):
+
+        result = self.quote()
+        result.rename(columns={"quote_time": "datetime"}, inplace=True)
+        result['datetime'] = pd.to_datetime(result['datetime'])
+        # print(df)
+        result = result.sort_values('datetime')  # 数据顺序排列
+        # print(df)
+
+        return result
+
+    def signal(self):
+        self.haskey = self.checkKey()
+        if not os.path.exists(self.filepath):
+            result = self.createSignal()
+        elif self.haskey == 'no':
+            result = self.createSignal()
+        else:
+            result = self.readCSV()
+        return result
+
+    def createQuote(self):
+        df = {}
+        try:
+
+            if self.exchange in ['SSE', 'SZSE', 'BSE', 'AMEX', 'ARCA', 'BATS', 'HKEX', 'NASDAQ', 'NYSE', 'OTC',
+                                 'NYSEARCA', 'FTXU', 'CBSE', 'GNSS', 'ERSX']:
+                # print('yahoo_0')
+                df = self.yahooApi()
+
+                if len(df) < 10:
+                    if self.exchange in ['SSE', 'SZSE', 'BSE']:
+                        # print('tushare_cn')
+                        if self.market == 'FUND':
+                            df = self.tushareFundApi()
+                        elif self.market == 'STOCK':
+                            df = self.tushareStockApi()
+                        else:
+                            pass
+
+
+                    elif self.exchange in ['AMEX', 'ARCA', 'BATS', 'NASDAQ', 'NYSE', 'OTC', 'NYSEARCA', 'FTXU', 'CBSE',
+                                           'GNSS', 'ERSX']:
+
+                        # print('alpaca_1')
+
+                        df = self.tushareCNStockApi()
+                    elif self.exchange in ['HKEX']:
+                        # print('tushare_hk')
+                        df = self.tushareHKStockApi()  # 没有权限
+
+
+            elif self.exchange == 'ALPACA':
+                df = self.alpacaCryptoApi()
+
+            else:
+                df = self.ccxtApi()
+
+            if len(df) > 0 and self.cache:
+                self.saveCSV(df)
+
+
+
+        except Exception as e:
+            print(e.args)
+            pass
+
+        ###########
+
+        return df
+
+    def yahooApi(self):
+        df = {}
+        try:
+            if self.freq == 'D' or self.freq == '1d':
+                periodlUS = '10y'
+                intervalUS = '1d'
+            elif self.freq == '1min' or self.freq == '1m':
+                periodlUS = '7d'
+                intervalUS = '1m'
+            elif self.freq == '5min':
+                periodlUS = '60d'
+                intervalUS = '5m'
+            elif self.freq == '15min':
+                periodlUS = '60d'
+                intervalUS = '15m'
+            elif self.freq == '30min':
+                periodlUS = '60d'
+                intervalUS = '30m'
+            elif self.freq == '60min' or self.freq == '1h':
+                periodlUS = '1y'
+                intervalUS = '1h'
+            elif self.freq == 'W':
+                periodlUS = '1y'
+                intervalUS = '1wk'
+            elif self.freq == 'M':
+                periodlUS = '1y'
+                intervalUS = '1mo'
+
+            self.underlying_ex = self.underlying_ex.replace('.SH', '.SS')
+            if self.start == '':
+                dfTemp = yf.download(  # or pdr.get_data_yahoo(...
+                    tickers=self.underlying_ex,  # tickers list or string as well
+                    period=periodlUS,
+                    # use "period" instead of start/end # valid periods: 1d,5d,1mo,3mo,6mo,1y,2y,5y,10y,ytd,max# (optional, default is '1mo')
+                    interval=intervalUS,
+                    # valid intervals: 1m,2m,5m,15m,30m,60m,90m,1h,1d,5d,1wk,1mo,3mo  # fetch data by interval (including intraday if period < 60 days) # (optional, default is '1d')
+                    ignore_tz=False,
+                    # Whether to ignore timezone when aligning ticker data from # different timezones. Default is False.
+                    group_by='ticker',  # group by ticker (to access via data['SPY']) # (optional, default is 'column')
+                    auto_adjust=True,  # adjust all OHLC automatically # (optional, default is False)
+                    repair=False,  # attempt repair of missing data or currency mixups e.g. $/cents
+                    prepost=True,  # download pre/post regular market hours data # (optional, default is False)
+                    threads=True,
+                    # use threads for mass downloading? (True/False/Integer) # (optional, default is True)
+                    proxy=None  # proxy URL scheme use use when downloading?# (optional, default is None)
+                )
+            else:
+                if self.end == '':
+                    self.end = date.today()
+                
+                dfTemp = yf.download(  # or pdr.get_data_yahoo(...
+                    tickers=self.underlying_ex,  # tickers list or string as well
+                    start=self.start,
+                    end=self.end,
+                    # use "period" instead of start/end # valid periods: 1d,5d,1mo,3mo,6mo,1y,2y,5y,10y,ytd,max# (optional, default is '1mo')
+                    interval=intervalUS,
+                    # valid intervals: 1m,2m,5m,15m,30m,60m,90m,1h,1d,5d,1wk,1mo,3mo  # fetch data by interval (including intraday if period < 60 days) # (optional, default is '1d')
+                    ignore_tz=False,
+                    # Whether to ignore timezone when aligning ticker data from # different timezones. Default is False.
+                    group_by='ticker',  # group by ticker (to access via data['SPY']) # (optional, default is 'column')
+                    auto_adjust=True,  # adjust all OHLC automatically # (optional, default is False)
+                    repair=False,  # attempt repair of missing data or currency mixups e.g. $/cents
+                    prepost=True,  # download pre/post regular market hours data # (optional, default is False)
+                    threads=True,
+                    # use threads for mass downloading? (True/False/Integer) # (optional, default is True)
+                    proxy=None  # proxy URL scheme use use when downloading?# (optional, default is None)
+                )
+
+            dfTemp.reset_index(drop=False, inplace=True)
+            if self.freq == 'D' or self.freq == '1d' or self.freq == 'W' or self.freq == 'M':
+                dfTemp['Datetime'] = dfTemp['Date']
+                dfTemp['Datetime'] = dfTemp['Datetime'].dt.tz_convert('UTC')
+                dfTemp['Datetime'] = dfTemp['Datetime'].dt.tz_localize(None)
+            # dfTemp['symbol'] = self.symbol
+
+            df = pd.DataFrame()
+            df['quote_time'] = dfTemp['Datetime']
+            df['open'] = dfTemp['Open']
+            df['high'] = dfTemp['High']
+            df['low'] = dfTemp['Low']
+            df['close'] = dfTemp['Close']
+            df['volume'] = dfTemp['Volume']
+
+
+
+
+        except Exception as e:
+            print(e.args)
+            pass
+
+        ###########
+
+        return df
+
+    def tushareCNStockApi(self):
+        df = {}
+        try:
+            pro = ts.pro_api(self.tushareKey)
+            # underlying = self.symbol.replace('~', '/').replace('$', ':').replace('.' + self.exchange, '')
+            if self.exchange == 'SSE':
+                self.underlying_ex = self.underlying_ex.replace('.SS', '.SH')
+            # 拉取数据
+
+            """if self.start == '':
+                self.start = date.today() + timedelta(days=-1000)
+            if self.freq == '1m':
+                self.start = date.today() + timedelta(days=-15)
+            if self.end == '':
+                self.end = date.today()"""
+
+
+            startDay = date.today() + timedelta(days=-1000)
+            if self.freq == '1m':
+                startDay = date.today() + timedelta(days=-15)
+            startDay = format(startDay.strftime('%Y%m%d'))
+            # print(LastWeek)
+            toDay = date.today()
+            toDay = format(toDay.strftime('%Y%m%d'))
+            # print(startDay)
+            # print(toDay)
+            # print(self.underlying)
+            dfTemp = pro.daily(**{
+                "ts_code": self.underlying_ex, "trade_date": "", "start_date": startDay, "end_date": toDay,
+                "offset": "",
+                "limit": ""
+            }, fields=[
+                "ts_code", "trade_date", "open", "high", "low", "close", "pre_close", "change", "pct_chg", "vol",
+                "amount"
+            ])
+            # print(dfTemp)
+
+            df = pd.DataFrame()
+            df['quote_time'] = dfTemp['trade_date']
+            df['open'] = dfTemp['open']
+            df['high'] = dfTemp['high']
+            df['low'] = dfTemp['low']
+            df['close'] = dfTemp['close']
+            df['volume'] = dfTemp['vol']
+
+
+
+
+        except Exception as e:
+            print(e.args)
+            pass
+
+        ###########
+
+        return df
+
+    def tushareHKStockApi(self):
+        df = {}
+        try:
+            pro = ts.pro_api(self.tushareKey)
+            startDay = date.today() + timedelta(days=-1000)
+            if self.freq == '1m':
+                startDay = date.today() + timedelta(days=-15)
+            startDay = format(startDay.strftime('%Y%m%d'))
+            # print(LastWeek)
+            toDay = date.today()
+            toDay = format(toDay.strftime('%Y%m%d'))
+            # print(startDay)
+            # print(toDay)
+            # print(self.underlying)
+            dfTemp = pro.hk_daily(**{
+                "ts_code": self.underlying, "trade_date": "", "start_date": startDay, "end_date": toDay, "offset": "",
+                "limit": ""
+            }, fields=[
+                "ts_code", "trade_date", "open", "high", "low", "close", "pre_close", "change", "pct_chg", "vol",
+                "amount"
+            ])
+            # print(dfTemp)
+
+            df = pd.DataFrame()
+            df['quote_time'] = dfTemp['trade_date']
+            df['open'] = dfTemp['open']
+            df['high'] = dfTemp['high']
+            df['low'] = dfTemp['low']
+            df['close'] = dfTemp['close']
+            df['volume'] = dfTemp['vol']
+
+
+
+
+        except Exception as e:
+            print(e.args)
+            pass
+
+        ###########
+
+        return df
+
+    def tushareFundApi(self):
+        df = {}
+        try:
+            pro = ts.pro_api(self.tushareKey)
+            # underlying = self.symbol.replace('~', '/').replace('$', ':').replace('.' + self.exchange, '')
+            if self.exchange == 'SSE':
+                self.underlying = self.underlying.replace('.SS', '.SH')
+            # 拉取数据
+
+            startDay = date.today() + timedelta(days=-1000)
+            if self.freq == '1m':
+                startDay = date.today() + timedelta(days=-15)
+            startDay = format(startDay.strftime('%Y%m%d'))
+            # print(LastWeek)
+            toDay = date.today()
+            toDay = format(toDay.strftime('%Y%m%d'))
+            # print(startDay)
+            # print(toDay)
+            # print(self.underlying)
+            dfTemp = pro.fund_daily(**{
+                "ts_code": self.underlying, "trade_date": "", "start_date": startDay, "end_date": toDay, "offset": "",
+                "limit": ""
+            }, fields=[
+                "ts_code", "trade_date", "open", "high", "low", "close", "pre_close", "change", "pct_chg", "vol",
+                "amount"
+            ])
+            # print(dfTemp)
+
+            df = pd.DataFrame()
+            df['quote_time'] = dfTemp['trade_date']
+            df['open'] = dfTemp['open']
+            df['high'] = dfTemp['high']
+            df['low'] = dfTemp['low']
+            df['close'] = dfTemp['close']
+            df['volume'] = dfTemp['vol']
+
+
+
+
+        except Exception as e:
+            print(e.args)
+            pass
+
+        ###########
+
+        return df
+
+    def ccxtApi(self):
+        df = {}
+        try:
+            # getExchange = tawCCXT(self.exchange)
+            # getExchange = byquant.getExchange(self.exchange)
+            getExchange = exchange.get(self.exchange)
+            getExchange.load_markets()
+
+            strFreq = self.freq
+            if strFreq == '1min':
+                strFreq = '1m'
+            elif strFreq == 'H':
+                strFreq = '1h'
+            elif strFreq == 'D':
+                strFreq = '1d'
+            elif strFreq == 'M':
+                strFreq = '1M'
+            elif strFreq == 'Y':
+                strFreq = '1y'
+            #limit = 1000
+            if self.limit == '':
+                self.limit = 1000
+            
+            since_date = datetime.strptime(self.start, "%Y-%m-%d")
+            # 将 datetime 对象转换为毫秒级时间戳
+            since_timestamp = int(since_date.timestamp() * 1000)
+
+            if getExchange.has['fetchOHLCV']:
+                # time.sleep(getExchange.rateLimit / 1000)  # time.sleep wants seconds
+                quotes = []
+                df = {}
+                # underlying = self.symbol.replace('~', '/').replace('$', ':').replace('.' + self.exchange, '')
+                ohlcvData = getExchange.fetchOHLCV(self.underlying, timeframe=strFreq, since =since_timestamp, limit=self.limit, params={})
+
+                for ohlcv in ohlcvData:
+                    quote = {}
+                    quoteTime = time.localtime(ohlcv[0] / 1000)
+                    quote_time = time.strftime("%Y-%m-%d %H:%M:%S", quoteTime)
+                    quote['quote_time'] = quote_time
+                    quote['open'] = ohlcv[1]
+                    quote['high'] = ohlcv[2]
+                    quote['low'] = ohlcv[3]
+                    quote['close'] = ohlcv[4]
+                    quote['volume'] = ohlcv[5]
+                    quotes.append(quote)
+
+                # df['open'] = df['ohlcv'][0]
+                df = pd.DataFrame(quotes)
+
+
+
+
+
+        except Exception as e:
+            print(e.args)
+            pass
+
+        ###########
+
+        return df
+
+    def alpacaCryptoApi(self):
+        df = {}
+        try:
+            # underlying = self.symbol.replace('~', '/').replace('$', ':').replace('.' + self.exchange.upper(), '')
+            # print([freq])
+            # toDay = date.today()
+            # toDay = format(toDay.strftime('%Y-%m-%d'))
+            client = CryptoHistoricalDataClient("Key", "KeyI")
+            # strFreq = freq
+            if self.freq == '1m':
+                # strFreq = '1m'
+                startTime = (date.today() + timedelta(days=-7)).strftime("%Y-%m-%d %H:%M:%S")
+                request_params = CryptoBarsRequest(
+                    symbol_or_symbols=[self.underlying],
+                    timeframe=TimeFrame.Minute,
+                    start=datetime.strptime(startTime, '%Y-%m-%d %H:%M:%S')
+                )
+            elif self.freq == '1h':
+                startTime = (date.today() + timedelta(days=-90)).strftime("%Y-%m-%d %H:%M:%S")
+                request_params = CryptoBarsRequest(
+                    symbol_or_symbols=[self.underlying],
+                    timeframe=TimeFrame.Hour,
+                    start=datetime.strptime(startTime, '%Y-%m-%d %H:%M:%S')
+                )
+            elif self.freq == '1d':
+                # strFreq = '1d'
+                startTime = (date.today() + timedelta(days=-1000)).strftime("%Y-%m-%d")
+                request_params = CryptoBarsRequest(
+                    symbol_or_symbols=[self.underlying],
+                    timeframe=TimeFrame.Day,
+                    start=datetime.strptime(startTime, '%Y-%m-%d')
+                )
+            else:
+                startTime = (date.today() + timedelta(days=-1000)).strftime("%Y-%m-%d")
+                request_params = CryptoBarsRequest(
+                    symbol_or_symbols=[self.underlying],
+                    timeframe=TimeFrame.Day,
+                    start=datetime.strptime(startTime, '%Y-%m-%d')
+                )
+
+            barsInfo = client.get_crypto_bars(request_params)
+            barsData = barsInfo.data
+            # print(type(barData))
+            barsList = barsData[self.underlying]
+
+            # print(barsList)
+            barList = []
+            for bars in barsList:
+                barDict = dict(bars)
+                barTemp = {}
+                barTemp['quote_time'] = str(barDict['timestamp'])
+                barTemp['open'] = float(barDict['open'])
+                barTemp['high'] = str(barDict['high'])
+                barTemp['low'] = float(barDict['low'])
+                barTemp['close'] = float(barDict['close'])
+                barTemp['volume'] = float(barDict['volume'])
+                # barTemp['trade_count'] = float(barDict['trade_count'])
+                barTemp['vwap'] = str(barDict['vwap'])
+
+                # print(tickTemp)
+                barList.append(barTemp)
+
+            dfTemp = pd.DataFrame(barList)
+            # dfTemp['symbol'] = symbol
+            df = dfTemp.tail(1000)
+            # print(df)
+
+
+
+
+
+        except Exception as e:
+            print(e.args)
+            pass
+
+        ###########
+
+        return df
+
+    def alpacaStockApi(self):
+        df = {}
+        try:
+            # underlying = self.symbol.replace('~', '/').replace('$', ':').replace('.' + self.exchange.upper(), '')
+            # print([freq])
+            # toDay = date.today()
+            # toDay = format(toDay.strftime('%Y-%m-%d'))
+            client = StockHistoricalDataClient("KEY", "KEYI")
+            # strFreq = freq
+            if self.freq == '1m':
+                # strFreq = '1m'
+                startTime = (date.today() + timedelta(days=-7)).strftime("%Y-%m-%d %H:%M:%S")
+                request_params = StockBarsRequest(
+                    symbol_or_symbols=[self.underlying],
+                    timeframe=TimeFrame.Minute,
+                    start=datetime.strptime(startTime, '%Y-%m-%d %H:%M:%S')
+                )
+            elif self.freq == '1h':
+                startTime = (date.today() + timedelta(days=-90)).strftime("%Y-%m-%d %H:%M:%S")
+                request_params = StockBarsRequest(
+                    symbol_or_symbols=[self.underlying],
+                    timeframe=TimeFrame.Hour,
+                    start=datetime.strptime(startTime, '%Y-%m-%d %H:%M:%S')
+                )
+            elif self.freq == '1d':
+                # strFreq = '1d'
+                startTime = (date.today() + timedelta(days=-1000)).strftime("%Y-%m-%d")
+                request_params = StockBarsRequest(
+                    symbol_or_symbols=[self.underlying],
+                    timeframe=TimeFrame.Day,
+                    start=datetime.strptime(startTime, '%Y-%m-%d')
+                )
+            else:
+                startTime = (date.today() + timedelta(days=-1000)).strftime("%Y-%m-%d")
+                request_params = StockBarsRequest(
+                    symbol_or_symbols=[self.underlying],
+                    timeframe=TimeFrame.Day,
+                    start=datetime.strptime(startTime, '%Y-%m-%d')
+                )
+
+            barsInfo = client.get_stock_bars(request_params)
+            barsData = barsInfo.data
+            # print(type(barData))
+            barsList = barsData[self.underlying]
+
+            # print(barsList)
+            barList = []
+            for bars in barsList:
+                barDict = dict(bars)
+                barTemp = {}
+                barTemp['quote_time'] = str(barDict['timestamp'])
+                barTemp['open'] = float(barDict['open'])
+                barTemp['high'] = str(barDict['high'])
+                barTemp['low'] = float(barDict['low'])
+                barTemp['close'] = float(barDict['close'])
+                barTemp['volume'] = float(barDict['volume'])
+                # barTemp['trade_count'] = float(barDict['trade_count'])
+                barTemp['vwap'] = str(barDict['vwap'])
+
+                # print(tickTemp)
+                barList.append(barTemp)
+
+            dfTemp = pd.DataFrame(barList)
+            # dfTemp['symbol'] = symbol
+            df = dfTemp.tail(1000)
+            # print(df)
+
+
+
+
+
+        except Exception as e:
+            print(e.args)
+            pass
+
+        ###########
+
+        return df
+
+    def saveHDF(self, data):  # 将放弃
+        result = False
+        df = data
+        try:
+
+            if len(df) > 0:
+                result = df
+                df.fillna("0", inplace=True)
+                df.sort_values(by="quote_time", ascending=False, inplace=True)
+
+                filedir = self.MARKET_DATA_PATH + '%s' % (self.exchange)
+                if not os.path.isdir(filedir):
+                    os.makedirs(filedir)
+                filepath = self.MARKET_DATA_PATH + '%s/%s.hdf' % (self.exchange, self.symbol)
+                df.to_hdf(filepath, mode='a', key='quote_%s' % (self.freq), complevel=9, complib='blosc',
+                          format='table')
+                result = True
+
+
+
+        except Exception as e:
+            print(e.args)
+            pass
+
+        ###########
+
+        return result
+
+    def saveCSV(self, data):
+        result = False
+        df = data
+        try:
+
+            if len(df) > 0:
+                result = df
+                df.fillna("0", inplace=True)
+                df.sort_values(by="quote_time", ascending=True, inplace=True)
+
+                filedir = self.MARKET_DATA_PATH + '%s' % (self.exchange)
+                if not os.path.isdir(filedir):
+                    os.makedirs(filedir)
+
+                mfiledir = self.MARKET_DATA_PATH + '%s/%s' % (self.exchange, self.freq)
+                if not os.path.isdir(mfiledir):
+                    os.makedirs(mfiledir)
+
+                df.to_csv(self.filepath, index=False)
+                """filepath = self.MARKET_DATA_PATH + '%s/%s.hdf' % (self.exchange, self.symbol)
+                df.to_hdf(filepath, mode='a', key='quote_%s' % (self.freq), complevel=9, complib='blosc',
+                          format='table')"""
+                result = True
+
+
+
+        except Exception as e:
+            print(e.args)
+            pass
+
+        ###########
+
+        return result
+
+    def createSignal(self):
+        result = tawSignal.autoStrategy(self.symbol, self.market, self.freq, self.limit, self.offset, self.tawtime)
+        return result
+
+    def updateQuote(self):
+        result = self.createQuote()  ##暂定
+        return result
+
+    """def read(self):
+        readHdf = pd.read_hdf(self.filepath, key='%s_%s' % (self.ktype, self.freq),mode='a')
+        result = pd.DataFrame(readHdf)
+        return result"""
+
+    def readHDF(self):  # 将放弃
+        readResult = pd.read_hdf(self.filepath, key='%s_%s' % (self.ktype, self.freq))
+        self.result = pd.DataFrame(readResult)
+        return self.result
+
+    def readCSV(self):
+        readResult = pd.read_csv(self.filepath)
+        self.result = pd.DataFrame(readResult)
+        return self.result
+
+    def checkKey(self):
+        result = 'no'
+        if os.path.exists(self.filepath):
+            keyName = '%s_%s' % (self.ktype, self.freq)
+            getStore = pd.HDFStore(self.filepath, 'a')
+            keyArr = getStore.keys()
+            getStore.close()
+            if keyName in keyArr:
+                result = 'yes'
+        return result
+
+    def getSymbolInfo(self):
+        result = {}
+        result['market'] = 'CRYPTO'
+        # try:
+        #    result = marketModels.Underlying.objects.filter(symbol = self.symbol).values('market')
+        # except Exception as e:
+        #    print(e.args)
+        #    pass
+        return result
+
+
+
+
+
+
+
```

### Comparing `byquant-1.7.33/byquant/exchange/__init__.py` & `byquant-1.7.35/byquant/exchange/__init__.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/ace.py` & `byquant-1.7.35/byquant/exchange/ace.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/alpaca.py` & `byquant-1.7.35/byquant/exchange/alpaca.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/ascendex.py` & `byquant-1.7.35/byquant/exchange/ascendex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/bequant.py` & `byquant-1.7.35/byquant/exchange/bequant.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/bigone.py` & `byquant-1.7.35/byquant/exchange/bigone.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/binance.py` & `byquant-1.7.35/byquant/exchange/binance.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/binancecoinm.py` & `byquant-1.7.35/byquant/exchange/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/binanceus.py` & `byquant-1.7.35/byquant/exchange/binanceus.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/binanceusdm.py` & `byquant-1.7.35/byquant/exchange/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/bit2c.py` & `byquant-1.7.35/byquant/exchange/bit2c.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/bitbank.py` & `byquant-1.7.35/byquant/exchange/bitbank.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/bitbns.py` & `byquant-1.7.35/byquant/exchange/bitbns.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/bitfinex.py` & `byquant-1.7.35/byquant/exchange/bitfinex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/bitfinex2.py` & `byquant-1.7.35/byquant/exchange/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/bitflyer.py` & `byquant-1.7.35/byquant/exchange/bitflyer.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/bitforex.py` & `byquant-1.7.35/byquant/exchange/bitforex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/bitget.py` & `byquant-1.7.35/byquant/exchange/bitget.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/bithumb.py` & `byquant-1.7.35/byquant/exchange/bithumb.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/bitmart.py` & `byquant-1.7.35/byquant/exchange/bitmart.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/bitmex.py` & `byquant-1.7.35/byquant/exchange/bitmex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/bitopro.py` & `byquant-1.7.35/byquant/exchange/bitopro.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/bitpanda.py` & `byquant-1.7.35/byquant/exchange/bitpanda.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/bitrue.py` & `byquant-1.7.35/byquant/exchange/bitrue.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/bitso.py` & `byquant-1.7.35/byquant/exchange/bitso.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/bitstamp.py` & `byquant-1.7.35/byquant/exchange/bitstamp.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/bitstamp1.py` & `byquant-1.7.35/byquant/exchange/bitstamp1.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/bittrex.py` & `byquant-1.7.35/byquant/exchange/bittrex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/bitvavo.py` & `byquant-1.7.35/byquant/exchange/bitvavo.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/bkex.py` & `byquant-1.7.35/byquant/exchange/bkex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/bl3p.py` & `byquant-1.7.35/byquant/exchange/bl3p.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/blockchaincom.py` & `byquant-1.7.35/byquant/exchange/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/btcalpha.py` & `byquant-1.7.35/byquant/exchange/btcalpha.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/btcbox.py` & `byquant-1.7.35/byquant/exchange/btcbox.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/btcex.py` & `byquant-1.7.35/byquant/exchange/btcex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/btcmarkets.py` & `byquant-1.7.35/byquant/exchange/btcmarkets.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/btctradeua.py` & `byquant-1.7.35/byquant/exchange/btctradeua.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/btcturk.py` & `byquant-1.7.35/byquant/exchange/btcturk.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/buda.py` & `byquant-1.7.35/byquant/exchange/buda.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/bybit.py` & `byquant-1.7.35/byquant/exchange/bybit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/cex.py` & `byquant-1.7.35/byquant/exchange/cex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/coinbase.py` & `byquant-1.7.35/byquant/exchange/coinbase.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/coinbaseprime.py` & `byquant-1.7.35/byquant/exchange/coinbaseprime.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/coinbasepro.py` & `byquant-1.7.35/byquant/exchange/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/coincheck.py` & `byquant-1.7.35/byquant/exchange/coincheck.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/coinex.py` & `byquant-1.7.35/byquant/exchange/coinex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/coinfalcon.py` & `byquant-1.7.35/byquant/exchange/coinfalcon.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/coinmate.py` & `byquant-1.7.35/byquant/exchange/coinmate.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/coinone.py` & `byquant-1.7.35/byquant/exchange/coinone.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/coinsph.py` & `byquant-1.7.35/byquant/exchange/coinsph.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/coinspot.py` & `byquant-1.7.35/byquant/exchange/coinspot.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/cryptocom.py` & `byquant-1.7.35/byquant/exchange/cryptocom.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/currencycom.py` & `byquant-1.7.35/byquant/exchange/currencycom.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/delta.py` & `byquant-1.7.35/byquant/exchange/delta.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/deribit.py` & `byquant-1.7.35/byquant/exchange/deribit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/digifinex.py` & `byquant-1.7.35/byquant/exchange/digifinex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/exmo.py` & `byquant-1.7.35/byquant/exchange/exmo.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/flowbtc.py` & `byquant-1.7.35/byquant/exchange/flowbtc.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/fmfwio.py` & `byquant-1.7.35/byquant/exchange/fmfwio.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/gate.py` & `byquant-1.7.35/byquant/exchange/gate.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/gemini.py` & `byquant-1.7.35/byquant/exchange/gemini.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/hitbtc.py` & `byquant-1.7.35/byquant/exchange/hitbtc.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/hitbtc3.py` & `byquant-1.7.35/byquant/exchange/hitbtc3.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/hollaex.py` & `byquant-1.7.35/byquant/exchange/hollaex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/huobi.py` & `byquant-1.7.35/byquant/exchange/huobi.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/huobijp.py` & `byquant-1.7.35/byquant/exchange/huobijp.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/huobipro.py` & `byquant-1.7.35/byquant/exchange/huobipro.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/idex.py` & `byquant-1.7.35/byquant/exchange/idex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/independentreserve.py` & `byquant-1.7.35/byquant/exchange/independentreserve.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/indodax.py` & `byquant-1.7.35/byquant/exchange/indodax.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/itbit.py` & `byquant-1.7.35/byquant/exchange/itbit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/kraken.py` & `byquant-1.7.35/byquant/exchange/kraken.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/krakenfutures.py` & `byquant-1.7.35/byquant/exchange/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/kucoin.py` & `byquant-1.7.35/byquant/exchange/kucoin.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/kucoinfutures.py` & `byquant-1.7.35/byquant/exchange/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/kuna.py` & `byquant-1.7.35/byquant/exchange/kuna.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/latoken.py` & `byquant-1.7.35/byquant/exchange/latoken.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/lbank.py` & `byquant-1.7.35/byquant/exchange/lbank.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/lbank2.py` & `byquant-1.7.35/byquant/exchange/lbank2.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/luno.py` & `byquant-1.7.35/byquant/exchange/luno.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/lykke.py` & `byquant-1.7.35/byquant/exchange/lykke.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/mercado.py` & `byquant-1.7.35/byquant/exchange/mercado.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/mexc.py` & `byquant-1.7.35/byquant/exchange/mexc.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/ndax.py` & `byquant-1.7.35/byquant/exchange/ndax.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/novadax.py` & `byquant-1.7.35/byquant/exchange/novadax.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/oceanex.py` & `byquant-1.7.35/byquant/exchange/oceanex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/okcoin.py` & `byquant-1.7.35/byquant/exchange/okcoin.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/okx.py` & `byquant-1.7.35/byquant/exchange/okx.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/paymium.py` & `byquant-1.7.35/byquant/exchange/paymium.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/phemex.py` & `byquant-1.7.35/byquant/exchange/phemex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/poloniex.py` & `byquant-1.7.35/byquant/exchange/poloniex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/poloniexfutures.py` & `byquant-1.7.35/byquant/exchange/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/probit.py` & `byquant-1.7.35/byquant/exchange/probit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/ripio.py` & `byquant-1.7.35/byquant/exchange/ripio.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/stex.py` & `byquant-1.7.35/byquant/exchange/stex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/tidex.py` & `byquant-1.7.35/byquant/exchange/tidex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/timex.py` & `byquant-1.7.35/byquant/exchange/timex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/tokocrypto.py` & `byquant-1.7.35/byquant/exchange/tokocrypto.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/upbit.py` & `byquant-1.7.35/byquant/exchange/upbit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/wavesexchange.py` & `byquant-1.7.35/byquant/exchange/wavesexchange.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/wazirx.py` & `byquant-1.7.35/byquant/exchange/wazirx.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/whitebit.py` & `byquant-1.7.35/byquant/exchange/whitebit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/woo.py` & `byquant-1.7.35/byquant/exchange/woo.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/xt.py` & `byquant-1.7.35/byquant/exchange/xt.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/yobit.py` & `byquant-1.7.35/byquant/exchange/yobit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/zaif.py` & `byquant-1.7.35/byquant/exchange/zaif.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/zb.py` & `byquant-1.7.35/byquant/exchange/zb.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/exchange/zonda.py` & `byquant-1.7.35/byquant/exchange/zonda.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/indicator/__init__.py` & `byquant-1.7.35/byquant/indicators/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,12 +16,18 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 ###############################################################################
 
+from .adx import *
 from .atr import *
+from .bollinger import *
 from .cci import *
 from .macd import *
 from .rsi import *
-from .sma import *
+from .sar import *
+from .sma import *
+from .stochastic import *
+from .williams import *
+
```

### Comparing `byquant-1.7.33/byquant/indicator/atr.py` & `byquant-1.7.35/byquant/indicator/atr.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/indicator/bbands.py` & `byquant-1.7.35/byquant/indicator/willr.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,10 +18,11 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 ###############################################################################
 
 from __future__ import (absolute_import, division, print_function,unicode_literals)
 import talib
 
-def BBANDS(data,period):
-    upper, middle, lower = talib.BBANDS(data.close, timeperiod=period,matype = talib.MA_Type.EMA)
-    return upper, middle, lower
+def WILLR(data,period):
+    return talib.WILLR(data.high,data.low,data.close, timeperiod=period)
+
+
```

### Comparing `byquant-1.7.33/byquant/indicator/cci.py` & `byquant-1.7.35/byquant/indicator/cci.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/indicator/dema.py` & `byquant-1.7.35/byquant/indicator/ma.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,9 +18,9 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 ###############################################################################
 
 from __future__ import (absolute_import, division, print_function,unicode_literals)
 import talib
 
-def DEMA(data,period):
-    return talib.DEMA(data.close, timeperiod=period)
+def MA(data,period):
+    return talib.MA(data.close, timeperiod=period)
```

### Comparing `byquant-1.7.33/byquant/indicator/ma.py` & `byquant-1.7.35/byquant/chart/matplotlib.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,11 +16,14 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 ###############################################################################
 
 from __future__ import (absolute_import, division, print_function,unicode_literals)
-import talib
 
-def MA(data,period):
-    return talib.MA(data.close, timeperiod=period)
+import matplotlib.pyplot as plt
+
+def close():
+    return plt.close()
+
+
```

### Comparing `byquant-1.7.33/byquant/indicator/macd.py` & `byquant-1.7.35/byquant/indicator/macd.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/indicator/rsi.py` & `byquant-1.7.35/byquant/indicator/rsi.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/indicator/sma.py` & `byquant-1.7.35/byquant/indicator/ad.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/indicators/__init__.py` & `byquant-1.7.35/byquant/indicator/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,12 +16,17 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 ###############################################################################
 
+from .adx import *
 from .atr import *
+from .bbands import *
 from .cci import *
 from .macd import *
 from .rsi import *
-from .sma import *
+from .sar import *
+from .sma import *
+from .stoch import *
+from .willr import *
```

### Comparing `byquant-1.7.33/byquant/indicators/atr.py` & `byquant-1.7.35/byquant/indicators/atr.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/indicators/cci.py` & `byquant-1.7.35/byquant/indicators/cci.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/indicators/macd.py` & `byquant-1.7.35/byquant/metastrategy.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,26 @@
-#!/usr/bin/env python
-# -*- coding: utf-8; py-indent-offset:4 -*-
-###############################################################################
-#
-# Copyright (C) 2022-2023 ByQuant.com
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-###############################################################################
-
-from __future__ import (absolute_import, division, print_function,unicode_literals)
-
-import backtrader as bt
-
-class RSI(bt.Indicator):
-    lines = ('_bydo',)
-    params = (('period', 14),)
-    def __init__(self):
-        self._bydo = bt.indicators.RSI(self.data, period=self.p.period)
-
-    def next(self):
-        self.lines._bydo[0] = self._bydo[0]
+#!/usr/bin/env python
+# -*- coding: utf-8; py-indent-offset:4 -*-
+###############################################################################
+#
+# Copyright (C) 2022-2023 ByQuant.com
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+#
+###############################################################################
+
+from __future__ import (absolute_import, division, print_function,unicode_literals)
+import backtrader as bt
+class Strategy(bt.Strategy):
+    def __init__(self):
+        super().__init__()
```

### Comparing `byquant-1.7.33/byquant/indicators/rsi.py` & `byquant-1.7.35/byquant/indicators/sar.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,15 +19,31 @@
 #
 ###############################################################################
 
 from __future__ import (absolute_import, division, print_function,unicode_literals)
 
 import backtrader as bt
 
-class RSI(bt.Indicator):
-    lines = ('_bydo',)
-    params = (('period', 14),)
-    def __init__(self):
-        self._bydo = bt.indicators.RSI(self.data, period=self.p.period)
+#__all__ = ['PSAR']
 
-    def next(self):
-        self.lines._bydo[0] = self._bydo[0]
+class PSAR_Stop():
+    #alias = ('ParabolicSAR',)
+    def __init__(self,data,af,afmax):
+        self.data=data
+        self.af=af
+        self.afmax=afmax
+
+    def __call__(self):
+        result = bt.indicators.PSAR(
+            self.data,
+            af=self.af,
+            afmax=self.afmax,
+        )
+        return result
+        
+    
+def PSAR(data,af,afmax):
+    return bt.indicators.PSAR(
+            data,
+            af=af,
+            afmax=afmax,
+        )
```

### Comparing `byquant-1.7.33/byquant/indicators/sma.py` & `byquant-1.7.35/byquant/indicators/rsi.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,15 +19,18 @@
 #
 ###############################################################################
 
 from __future__ import (absolute_import, division, print_function,unicode_literals)
 
 import backtrader as bt
 
-class SMA(bt.Indicator):
-    lines = ('_bydo',)
-    params = (('period', 14),)
-    def __init__(self):
-        self._bydo = bt.indicators.SMA(self.data, period=self.p.period)
-
-    def next(self):
-        self.lines._bydo[0] = self._bydo[0]
+def RSI(data,period):
+    return bt.indicators.RSI(
+            data,
+            period=period,
+        )
+        
+def RSI_SMA(data,period):
+    return bt.indicators.RSI_SMA(
+            data,
+            period=period,
+        )
```

### Comparing `byquant-1.7.33/byquant/metabacktest.py` & `byquant-1.7.35/byquant/metabacktest.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/metastrategy.py` & `byquant-1.7.35/byquant/indicator/sar.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,29 @@
-#!/usr/bin/env python
-# -*- coding: utf-8; py-indent-offset:4 -*-
-###############################################################################
-#
-# Copyright (C) 2022-2023 ByQuant.com
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-###############################################################################
-
-from __future__ import (absolute_import, division, print_function,unicode_literals)
-import backtrader as bt
-class Strategy(bt.Strategy):
-    def __init__(self):
-        super().__init__()
+#!/usr/bin/env python
+# -*- coding: utf-8; py-indent-offset:4 -*-
+###############################################################################
+#
+# Copyright (C) 2022-2023 ByQuant.com
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+#
+###############################################################################
+
+from __future__ import (absolute_import, division, print_function,unicode_literals)
+import talib
+
+#SAR：抛物线指标
+# SAR(high, low, acceleration=0, maximum=0)
+# 参数说明：high：最高价；low:最低价；acceleration：加速因子；maximum：极点价
+def SAR(data, acceleration=0,maximum=0):
+    return talib.SAR(data.high, data.low, acceleration=acceleration, maximum=maximum)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `byquant-1.7.33/byquant/strategy/__init__.py` & `byquant-1.7.35/byquant/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant/tool/tawPlus.py` & `byquant-1.7.35/byquant/tool/tawPlus.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.33/byquant.egg-info/PKG-INFO` & `byquant-1.7.35/byquant.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byquant
-Version: 1.7.33
+Version: 1.7.35
 Summary: ByQuant.com is AI Quantitative Strategy Competition Training Community
 Home-page: https://byquant.com
 Author: Uakeey
 Author-email: uakee@outlook.com
 License: GPL
 Project-URL: Homepage, https://byquant.com
 Keywords: quant,strategy,algorithmic,algotrading
```

### Comparing `byquant-1.7.33/setup.py` & `byquant-1.7.35/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 here = path.abspath(path.dirname(__file__))
 root = path.dirname(here)
 
 readme = path.join(here, 'README.md')
 package = {
   "name": "byquant",
-  "version": "1.7.33",
+  "version": "1.7.35",
   "description": "ByQuant.com is AI Quantitative Strategy Competition Training Community",
   "type": "module",
   "readme": "README.md",
   "package_json": "package.json",
   "author": {
     "name": "Uakeey",
     "email": "uakee@outlook.com",
```

