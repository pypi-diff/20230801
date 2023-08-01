# Comparing `tmp/intrinio-sdk-6.24.1.tar.gz` & `tmp/intrinio-sdk-6.25.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/intrinio-sdk-6.24.1.tar", last modified: Wed Jul 12 21:15:33 2023, max compression
+gzip compressed data, was "intrinio-sdk-6.25.0.tar", last modified: Tue Aug  1 21:44:04 2023, max compression
```

## Comparing `intrinio-sdk-6.24.1.tar` & `intrinio-sdk-6.25.0.tar`

### file list

```diff
@@ -1,596 +1,596 @@
-drwxr-xr-x   0 shawn      (503) staff       (20)        0 2023-07-12 21:15:33.000000 intrinio-sdk-6.24.1/
-drwxr-xr-x   0 shawn      (503) staff       (20)        0 2023-07-12 21:15:33.000000 intrinio-sdk-6.24.1/intrinio_sdk/
--rw-r--r--   0 shawn      (503) staff       (20)     8604 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/configuration.py
--rw-r--r--   0 shawn      (503) staff       (20)    13819 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/rest.py
--rw-r--r--   0 shawn      (503) staff       (20)    25844 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/__init__.py
-drwxr-xr-x   0 shawn      (503) staff       (20)        0 2023-07-12 21:15:33.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/
--rw-r--r--   0 shawn      (503) staff       (20)    26373 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/zacks_target_price_consensus.py
--rw-r--r--   0 shawn      (503) staff       (20)     9009 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_zacks_sales_surprises.py
--rw-r--r--   0 shawn      (503) staff       (20)     6524 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/detrended_price_oscillator_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)    40363 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/zacks_sales_surprise_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     6602 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_options.py
--rw-r--r--   0 shawn      (503) staff       (20)     6656 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_municipalities.py
--rw-r--r--   0 shawn      (503) staff       (20)    10646 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_williams_r.py
--rw-r--r--   0 shawn      (503) staff       (20)     7658 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/forex_currency.py
--rw-r--r--   0 shawn      (503) staff       (20)    32532 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/zacks_institutional_holding_company_detail.py
--rw-r--r--   0 shawn      (503) staff       (20)    10844 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_vortex_indicator.py
--rw-r--r--   0 shawn      (503) staff       (20)    10910 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_awesome_oscillator.py
--rw-r--r--   0 shawn      (503) staff       (20)     4570 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_securities_search.py
--rw-r--r--   0 shawn      (503) staff       (20)     8175 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_company_filings.py
--rw-r--r--   0 shawn      (503) staff       (20)     6593 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_filing_notes.py
--rw-r--r--   0 shawn      (503) staff       (20)     6229 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/williams_r_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     7946 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_options_stats_realtime.py
--rw-r--r--   0 shawn      (503) staff       (20)    22943 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/security_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)    14290 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/stock_price_adjustment.py
--rw-r--r--   0 shawn      (503) staff       (20)     4691 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_options_prices_batch_realtime.py
--rw-r--r--   0 shawn      (503) staff       (20)     4746 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_options_chain.py
--rw-r--r--   0 shawn      (503) staff       (20)     8872 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_standardized_financials.py
--rw-r--r--   0 shawn      (503) staff       (20)    19333 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/stock_market_index_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     8463 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_sic_index_historical_data.py
--rw-r--r--   0 shawn      (503) staff       (20)     8068 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_company_news.py
--rw-r--r--   0 shawn      (503) staff       (20)    24031 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/option_unusual_trade.py
--rw-r--r--   0 shawn      (503) staff       (20)     4354 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_data_tags_search.py
--rw-r--r--   0 shawn      (503) staff       (20)    32022 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/institutional_holding.py
--rw-r--r--   0 shawn      (503) staff       (20)     4539 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_company_recognize.py
--rw-r--r--   0 shawn      (503) staff       (20)     4571 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_economic_indices_search.py
--rw-r--r--   0 shawn      (503) staff       (20)    18849 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/zacks_analyst_rating_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)    79809 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/etf_stats.py
--rw-r--r--   0 shawn      (503) staff       (20)     6357 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/standardized_financials_dimension.py
--rw-r--r--   0 shawn      (503) staff       (20)    57040 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/zacks_long_term_growth_rate.py
--rw-r--r--   0 shawn      (503) staff       (20)     8325 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_company_securities.py
--rw-r--r--   0 shawn      (503) staff       (20)    70186 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/company.py
--rw-r--r--   0 shawn      (503) staff       (20)     7058 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_zacks_eps_growth_rates.py
--rw-r--r--   0 shawn      (503) staff       (20)    12984 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/company_news.py
--rw-r--r--   0 shawn      (503) staff       (20)    23120 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/etf_analytics.py
--rw-r--r--   0 shawn      (503) staff       (20)     8401 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/reported_financial.py
--rw-r--r--   0 shawn      (503) staff       (20)    37102 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/municipality.py
--rw-r--r--   0 shawn      (503) staff       (20)    21150 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/company_filing.py
--rw-r--r--   0 shawn      (503) staff       (20)    14903 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/company_shares_outstanding.py
--rw-r--r--   0 shawn      (503) staff       (20)     6794 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_zacks_analyst_ratings.py
--rw-r--r--   0 shawn      (503) staff       (20)     4642 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_filing_notes_search.py
--rw-r--r--   0 shawn      (503) staff       (20)     6244 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/force_index_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     8641 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_economic_index_historical_data.py
--rw-r--r--   0 shawn      (503) staff       (20)     6470 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/commodity_channel_index_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     9762 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_company_answers.py
--rw-r--r--   0 shawn      (503) staff       (20)     7063 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_zacks_eps_surprises.py
--rw-r--r--   0 shawn      (503) staff       (20)     8528 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_company_historical_data.py
--rw-r--r--   0 shawn      (503) staff       (20)    16762 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/option_interval_mover.py
--rw-r--r--   0 shawn      (503) staff       (20)    11274 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/moving_average_convergence_divergence_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     8244 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_forex_prices.py
--rw-r--r--   0 shawn      (503) staff       (20)     4894 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_options_chain_realtime.py
--rw-r--r--   0 shawn      (503) staff       (20)     6482 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/zacks_institutional_holding_owner_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)    14640 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/option.py
--rw-r--r--   0 shawn      (503) staff       (20)    40823 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/stock_price_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)    19534 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/filing_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)    19707 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/forex_price.py
--rw-r--r--   0 shawn      (503) staff       (20)    11154 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_volume_weighted_average_price.py
--rw-r--r--   0 shawn      (503) staff       (20)    23701 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/zacks_analyst_rating_snapshot.py
--rw-r--r--   0 shawn      (503) staff       (20)    10878 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_ichimoku_kinko_hyo.py
--rw-r--r--   0 shawn      (503) staff       (20)     6465 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/volume_weighted_average_price_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     5890 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/option_chain_eod.py
--rw-r--r--   0 shawn      (503) staff       (20)     6050 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/bulk_download_links.py
--rw-r--r--   0 shawn      (503) staff       (20)    10878 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_volume_price_trend.py
--rw-r--r--   0 shawn      (503) staff       (20)    14988 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/security_trades.py
--rw-r--r--   0 shawn      (503) staff       (20)    37768 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/etf_holding.py
--rw-r--r--   0 shawn      (503) staff       (20)     6434 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/simple_moving_average_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     4823 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_options_unusual_activity.py
--rw-r--r--   0 shawn      (503) staff       (20)     8432 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/zacks_institutional_holding_company_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     9138 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_stock_exchange_securities.py
--rw-r--r--   0 shawn      (503) staff       (20)     9875 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_stock_exchange_stock_price_adjustments.py
--rw-r--r--   0 shawn      (503) staff       (20)    10811 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_keltner_channel.py
--rw-r--r--   0 shawn      (503) staff       (20)     8931 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_stock_prices.py
--rw-r--r--   0 shawn      (503) staff       (20)    11009 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_stochastic_oscillator.py
--rw-r--r--   0 shawn      (503) staff       (20)    14869 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/ichimoku_kinko_hyo_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     8723 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_stock_market_index_historical_data.py
--rw-r--r--   0 shawn      (503) staff       (20)    50532 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/company_initial_public_offering.py
--rw-r--r--   0 shawn      (503) staff       (20)    13643 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/esg_company_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)   253901 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/etf.py
--rw-r--r--   0 shawn      (503) staff       (20)    11109 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_average_directional_index.py
--rw-r--r--   0 shawn      (503) staff       (20)    10812 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_ease_of_movement.py
--rw-r--r--   0 shawn      (503) staff       (20)    41799 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/stock_price.py
--rw-r--r--   0 shawn      (503) staff       (20)     6371 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/owner_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)    15061 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/zacks_etf_holding.py
--rw-r--r--   0 shawn      (503) staff       (20)    10482 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/keltner_channel_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     8463 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/vortex_indicator_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)    16643 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/security_interval_mover.py
--rw-r--r--   0 shawn      (503) staff       (20)    16848 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/intraday_stock_price.py
--rw-r--r--   0 shawn      (503) staff       (20)    20665 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/stock_price_interval.py
--rw-r--r--   0 shawn      (503) staff       (20)    14644 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/option_stats_realtime.py
--rw-r--r--   0 shawn      (503) staff       (20)    54424 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/security.py
--rw-r--r--   0 shawn      (503) staff       (20)     6737 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_zacks_etf_holdings.py
--rw-r--r--   0 shawn      (503) staff       (20)    26231 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/filing.py
--rw-r--r--   0 shawn      (503) staff       (20)     6398 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/true_strength_index_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)    23216 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/dividend_record.py
--rw-r--r--   0 shawn      (503) staff       (20)     6570 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/average_daily_trading_volume_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)    20362 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/zacks_analyst_rating.py
--rw-r--r--   0 shawn      (503) staff       (20)     6469 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_companies.py
--rw-r--r--   0 shawn      (503) staff       (20)     5782 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/option_chain.py
--rw-r--r--   0 shawn      (503) staff       (20)    10809 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/security_intervals_movers_result.py
--rw-r--r--   0 shawn      (503) staff       (20)     6739 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/zacks_institutional_holding_historical_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     7091 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_zacks_institutional_holding_owners.py
--rw-r--r--   0 shawn      (503) staff       (20)     4530 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_companies_search.py
--rw-r--r--   0 shawn      (503) staff       (20)     8284 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/security_screen_clause.py
--rw-r--r--   0 shawn      (503) staff       (20)     8133 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/security_screen_result_data.py
--rw-r--r--   0 shawn      (503) staff       (20)     6370 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/awesome_oscillator_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)    12679 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/option_realtime.py
--rw-r--r--   0 shawn      (503) staff       (20)     9528 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/filing_note.py
--rw-r--r--   0 shawn      (503) staff       (20)    24625 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/__init__.py
--rw-r--r--   0 shawn      (503) staff       (20)     6614 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/accumulation_distribution_index_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     6251 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_news.py
--rw-r--r--   0 shawn      (503) staff       (20)    10943 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_ultimate_oscillator.py
--rw-r--r--   0 shawn      (503) staff       (20)     4340 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/option_contracts_list.py
--rw-r--r--   0 shawn      (503) staff       (20)    22944 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/economic_index_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)    18458 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/option_interval.py
--rw-r--r--   0 shawn      (503) staff       (20)    11043 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_relative_strength_index.py
--rw-r--r--   0 shawn      (503) staff       (20)     6533 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_esg_companies.py
--rw-r--r--   0 shawn      (503) staff       (20)     6122 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/technical_indicator.py
--rw-r--r--   0 shawn      (503) staff       (20)     7632 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/option_chain_realtime.py
--rw-r--r--   0 shawn      (503) staff       (20)    18293 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/esg_rating_with_company.py
--rw-r--r--   0 shawn      (503) staff       (20)    25762 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/owner.py
--rw-r--r--   0 shawn      (503) staff       (20)     5995 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/historical_data.py
--rw-r--r--   0 shawn      (503) staff       (20)    10988 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_insider_transaction_filings.py
--rw-r--r--   0 shawn      (503) staff       (20)    10878 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_average_true_range.py
--rw-r--r--   0 shawn      (503) staff       (20)     8711 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_esg_company_comprehensive_rating_history.py
--rw-r--r--   0 shawn      (503) staff       (20)   114262 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/esg_comprehensive_rating.py
--rw-r--r--   0 shawn      (503) staff       (20)    36893 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/zacks_eps_surprise.py
--rw-r--r--   0 shawn      (503) staff       (20)     8905 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_zacks_eps_surprises.py
--rw-r--r--   0 shawn      (503) staff       (20)     4344 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_options_tickers.py
--rw-r--r--   0 shawn      (503) staff       (20)    10320 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/filing_note_filing.py
--rw-r--r--   0 shawn      (503) staff       (20)     6233 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/standardized_financial.py
--rw-r--r--   0 shawn      (503) staff       (20)     9185 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_company_insider_transaction_filings.py
--rw-r--r--   0 shawn      (503) staff       (20)    16235 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/esg_rating.py
--rw-r--r--   0 shawn      (503) staff       (20)     8664 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_reported_financials.py
--rw-r--r--   0 shawn      (503) staff       (20)    10878 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_chaikin_money_flow.py
--rw-r--r--   0 shawn      (503) staff       (20)    34497 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/zacks_eps_estimate.py
--rw-r--r--   0 shawn      (503) staff       (20)     6075 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/option_price_batch_realtime.py
--rw-r--r--   0 shawn      (503) staff       (20)     6522 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_municipalitiy_financials.py
--rw-r--r--   0 shawn      (503) staff       (20)    14908 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/option_factors_realtime.py
--rw-r--r--   0 shawn      (503) staff       (20)     6562 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/on_balance_volume_mean_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)    11142 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_detrended_price_oscillator.py
--rw-r--r--   0 shawn      (503) staff       (20)     8400 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/thea_entity_answer.py
--rw-r--r--   0 shawn      (503) staff       (20)     6515 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_securities.py
--rw-r--r--   0 shawn      (503) staff       (20)    22029 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/data_tag.py
--rw-r--r--   0 shawn      (503) staff       (20)     6287 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_data_tags.py
--rw-r--r--   0 shawn      (503) staff       (20)    16293 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/etf_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     6694 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_historical_data.py
--rw-r--r--   0 shawn      (503) staff       (20)     7995 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_etf_holdings.py
--rw-r--r--   0 shawn      (503) staff       (20)     6344 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/money_flow_index_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)    11155 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_interval_prices.py
--rw-r--r--   0 shawn      (503) staff       (20)    11307 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_accumulation_distribution_index.py
--rw-r--r--   0 shawn      (503) staff       (20)    56139 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/zacks_eps_growth_rate.py
--rw-r--r--   0 shawn      (503) staff       (20)     9510 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_stock_price_adjustments.py
--rw-r--r--   0 shawn      (503) staff       (20)     9686 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_filing_answers.py
--rw-r--r--   0 shawn      (503) staff       (20)     8397 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_options_prices_eod.py
--rw-r--r--   0 shawn      (503) staff       (20)    20794 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/stock_market_index.py
--rw-r--r--   0 shawn      (503) staff       (20)     6362 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/on_balance_volume_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)    43221 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/insider_transaction.py
--rw-r--r--   0 shawn      (503) staff       (20)     6470 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/relative_strength_index_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)    40407 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/option_price_eod.py
--rw-r--r--   0 shawn      (503) staff       (20)    11140 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_intraday_prices.py
--rw-r--r--   0 shawn      (503) staff       (20)    29315 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/zacks_institutional_holding.py
--rw-r--r--   0 shawn      (503) staff       (20)     6245 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_et_fs.py
--rw-r--r--   0 shawn      (503) staff       (20)     7226 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_zacks_institutional_holding_companies.py
--rw-r--r--   0 shawn      (503) staff       (20)     6380 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/volume_price_trend_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)   118624 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/esg_comprehensive_rating_with_company.py
--rw-r--r--   0 shawn      (503) staff       (20)     6688 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_stock_exchanges.py
--rw-r--r--   0 shawn      (503) staff       (20)    45403 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/zacks_institutional_holding_owner_detail.py
--rw-r--r--   0 shawn      (503) staff       (20)     8290 2023-07-10 17:08:34.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/security_screen_group.py
--rw-r--r--   0 shawn      (503) staff       (20)    10812 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_money_flow_index.py
--rw-r--r--   0 shawn      (503) staff       (20)     4549 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_forex_currencies.py
--rw-r--r--   0 shawn      (503) staff       (20)     4355 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_forex_pairs.py
--rw-r--r--   0 shawn      (503) staff       (20)    10779 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_know_sure_thing.py
--rw-r--r--   0 shawn      (503) staff       (20)     6731 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_esg_latest_comprehensive.py
--rw-r--r--   0 shawn      (503) staff       (20)    11043 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_commodity_channel_index.py
--rw-r--r--   0 shawn      (503) staff       (20)    16239 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/insider_transaction_filing.py
--rw-r--r--   0 shawn      (503) staff       (20)     7161 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_zacks_sales_surprises.py
--rw-r--r--   0 shawn      (503) staff       (20)     6240 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/security_snapshot_group.py
--rw-r--r--   0 shawn      (503) staff       (20)     6832 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_institutional_ownership.py
--rw-r--r--   0 shawn      (503) staff       (20)     6500 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_owners.py
--rw-r--r--   0 shawn      (503) staff       (20)     8595 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/donchian_channel_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)    10977 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_simple_moving_average.py
--rw-r--r--   0 shawn      (503) staff       (20)     4617 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_stock_market_indices_search.py
--rw-r--r--   0 shawn      (503) staff       (20)     8383 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_filing_fundamentals.py
--rw-r--r--   0 shawn      (503) staff       (20)     9296 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_stock_exchange_stock_prices.py
--rw-r--r--   0 shawn      (503) staff       (20)     8094 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/forex_pair.py
--rw-r--r--   0 shawn      (503) staff       (20)     7800 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/security_replay_file_result.py
--rw-r--r--   0 shawn      (503) staff       (20)     8359 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_esg_company_rating_history.py
--rw-r--r--   0 shawn      (503) staff       (20)     7447 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_zacks_target_price_consensuses.py
--rw-r--r--   0 shawn      (503) staff       (20)     6380 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/average_true_range_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)    10811 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_bollinger_bands.py
--rw-r--r--   0 shawn      (503) staff       (20)     7125 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_initial_public_offerings.py
--rw-r--r--   0 shawn      (503) staff       (20)     4453 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_sic_indices_search.py
--rw-r--r--   0 shawn      (503) staff       (20)     8703 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/security_trades_result.py
--rw-r--r--   0 shawn      (503) staff       (20)     4754 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_options_expirations.py
--rw-r--r--   0 shawn      (503) staff       (20)     6101 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/security_screen_result.py
--rw-r--r--   0 shawn      (503) staff       (20)     6326 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/know_sure_thing_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     6380 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/chaikin_money_flow_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     8580 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_historical_data.py
--rw-r--r--   0 shawn      (503) staff       (20)     6546 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_economic_indices.py
--rw-r--r--   0 shawn      (503) staff       (20)    35692 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/zacks_eps_surprise_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)    10845 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_on_balance_volume.py
--rw-r--r--   0 shawn      (503) staff       (20)     9009 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_zacks_analyst_ratings.py
--rw-r--r--   0 shawn      (503) staff       (20)     9486 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_stock_exchange_realtime_stock_prices.py
--rw-r--r--   0 shawn      (503) staff       (20)     6344 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/ease_of_movement_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)    13776 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/bulk_download_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)    10679 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_force_index.py
--rw-r--r--   0 shawn      (503) staff       (20)     6977 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_zacks_institutional_holdings.py
--rw-r--r--   0 shawn      (503) staff       (20)     6610 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_stock_market_indices.py
--rw-r--r--   0 shawn      (503) staff       (20)     6457 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_esg_latest.py
--rw-r--r--   0 shawn      (503) staff       (20)    11790 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/realtime_stock_price_security.py
--rw-r--r--   0 shawn      (503) staff       (20)     7884 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_options_price_realtime.py
--rw-r--r--   0 shawn      (503) staff       (20)     9075 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_owner_insider_transaction_filings.py
--rw-r--r--   0 shawn      (503) staff       (20)     6340 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_filings.py
--rw-r--r--   0 shawn      (503) staff       (20)     6434 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/negative_volume_index_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)    10907 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/sic_index.py
--rw-r--r--   0 shawn      (503) staff       (20)     4847 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/security_snapshots_result.py
--rw-r--r--   0 shawn      (503) staff       (20)    23168 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/institutional_ownership.py
--rw-r--r--   0 shawn      (503) staff       (20)    16540 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/data_tag_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)    11361 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/company_news_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)    10743 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/option_intervals_movers_result.py
--rw-r--r--   0 shawn      (503) staff       (20)    10844 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_donchian_channel.py
--rw-r--r--   0 shawn      (503) staff       (20)     4704 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_bulk_download_links.py
--rw-r--r--   0 shawn      (503) staff       (20)     8290 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_option_prices.py
--rw-r--r--   0 shawn      (503) staff       (20)    31195 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/option_price.py
--rw-r--r--   0 shawn      (503) staff       (20)     8917 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_standardized_financials_dimensions.py
--rw-r--r--   0 shawn      (503) staff       (20)     6855 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_zacks_eps_estimates.py
--rw-r--r--   0 shawn      (503) staff       (20)     4742 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_options_realtime.py
--rw-r--r--   0 shawn      (503) staff       (20)    11092 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/company_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     4819 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_options_chain_eod.py
--rw-r--r--   0 shawn      (503) staff       (20)    11473 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_moving_average_convergence_divergence.py
--rw-r--r--   0 shawn      (503) staff       (20)    50157 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/realtime_stock_price.py
--rw-r--r--   0 shawn      (503) staff       (20)     8435 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_company_fundamentals.py
--rw-r--r--   0 shawn      (503) staff       (20)    10151 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/average_directional_index_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)    20554 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/stock_exchange.py
--rw-r--r--   0 shawn      (503) staff       (20)     6398 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_sic_indices.py
--rw-r--r--   0 shawn      (503) staff       (20)    21288 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/fundamental.py
--rw-r--r--   0 shawn      (503) staff       (20)    24303 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/economic_index.py
--rw-r--r--   0 shawn      (503) staff       (20)    10977 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_negative_volume_index.py
--rw-r--r--   0 shawn      (503) staff       (20)     7753 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/filing_note_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)    24804 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/option_price_realtime.py
--rw-r--r--   0 shawn      (503) staff       (20)     6226 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/mass_index_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)    13209 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/option_eod.py
--rw-r--r--   0 shawn      (503) staff       (20)    10911 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_true_strength_index.py
--rw-r--r--   0 shawn      (503) staff       (20)     6388 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/ultimate_oscillator_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     6560 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_owner_institutional_holdings.py
--rw-r--r--   0 shawn      (503) staff       (20)     6884 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_zacks_analyst_ratings_snapshot.py
--rw-r--r--   0 shawn      (503) staff       (20)    37674 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/zacks_sales_surprise.py
--rw-r--r--   0 shawn      (503) staff       (20)     4817 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/option_snapshots_result.py
--rw-r--r--   0 shawn      (503) staff       (20)     8557 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/option_intervals_result.py
--rw-r--r--   0 shawn      (503) staff       (20)    17338 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/fundamental_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)    14527 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/reported_tag.py
--rw-r--r--   0 shawn      (503) staff       (20)    11142 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_triple_exponential_average.py
--rw-r--r--   0 shawn      (503) staff       (20)     7396 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_zacks_long_term_growth_rates.py
--rw-r--r--   0 shawn      (503) staff       (20)    10662 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/bollinger_bands_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     6167 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/reported_financial_dimension.py
--rw-r--r--   0 shawn      (503) staff       (20)     6145 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/thea_source_document.py
--rw-r--r--   0 shawn      (503) staff       (20)    12624 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/stock_price_adjustment_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)   136507 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/municipality_financial.py
--rw-r--r--   0 shawn      (503) staff       (20)    10646 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_mass_index.py
--rw-r--r--   0 shawn      (503) staff       (20)    10978 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_on_balance_volume_mean.py
--rw-r--r--   0 shawn      (503) staff       (20)     6644 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_company_shares_outstanding.py
--rw-r--r--   0 shawn      (503) staff       (20)     8341 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/stochastic_oscillator_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)    52025 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/earnings_record.py
--rw-r--r--   0 shawn      (503) staff       (20)     6210 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/option_snapshot_group.py
--rw-r--r--   0 shawn      (503) staff       (20)     6549 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/triple_exponential_average_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)    11176 2023-07-10 17:08:17.000000 intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_average_daily_trading_volume.py
-drwxr-xr-x   0 shawn      (503) staff       (20)        0 2023-07-12 21:15:33.000000 intrinio-sdk-6.24.1/intrinio_sdk/api/
--rw-r--r--   0 shawn      (503) staff       (20)    10452 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/api/data_point_api.py
--rw-r--r--   0 shawn      (503) staff       (20)    84166 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/api/index_api.py
--rw-r--r--   0 shawn      (503) staff       (20)    25579 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/api/owners_api.py
--rw-r--r--   0 shawn      (503) staff       (20)    26155 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/api/et_fs_api.py
--rw-r--r--   0 shawn      (503) staff       (20)    95784 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/api/company_api.py
--rw-r--r--   0 shawn      (503) staff       (20)    16465 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/api/municipality_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     1157 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/api/__init__.py
--rw-r--r--   0 shawn      (503) staff       (20)   359486 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/api/security_api.py
--rw-r--r--   0 shawn      (503) staff       (20)   213664 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/api/technical_api.py
--rw-r--r--   0 shawn      (503) staff       (20)   127971 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/api/options_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     6358 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/api/insider_transaction_filings_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     7996 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/api/historical_data_api.py
--rw-r--r--   0 shawn      (503) staff       (20)    31234 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/api/fundamentals_api.py
--rw-r--r--   0 shawn      (503) staff       (20)    30181 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/api/stock_exchange_api.py
--rw-r--r--   0 shawn      (503) staff       (20)    51756 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/api/filing_api.py
--rw-r--r--   0 shawn      (503) staff       (20)    14009 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/api/data_tag_api.py
--rw-r--r--   0 shawn      (503) staff       (20)    14832 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/api/forex_api.py
--rw-r--r--   0 shawn      (503) staff       (20)    74950 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/api/zacks_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     4435 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/api/bulk_downloads_api.py
--rw-r--r--   0 shawn      (503) staff       (20)    22700 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/api/esg_api.py
--rw-r--r--   0 shawn      (503) staff       (20)    26891 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/intrinio_sdk/api_client.py
--rw-r--r--   0 shawn      (503) staff       (20)      776 2023-07-12 21:15:33.000000 intrinio-sdk-6.24.1/PKG-INFO
-drwxr-xr-x   0 shawn      (503) staff       (20)        0 2023-07-12 21:15:33.000000 intrinio-sdk-6.24.1/intrinio_sdk.egg-info/
--rw-r--r--   0 shawn      (503) staff       (20)      776 2023-07-12 21:15:32.000000 intrinio-sdk-6.24.1/intrinio_sdk.egg-info/PKG-INFO
--rw-r--r--   0 shawn      (503) staff       (20)    27307 2023-07-12 21:15:32.000000 intrinio-sdk-6.24.1/intrinio_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 shawn      (503) staff       (20)       64 2023-07-12 21:15:32.000000 intrinio-sdk-6.24.1/intrinio_sdk.egg-info/requires.txt
--rw-r--r--   0 shawn      (503) staff       (20)       18 2023-07-12 21:15:32.000000 intrinio-sdk-6.24.1/intrinio_sdk.egg-info/top_level.txt
--rw-r--r--   0 shawn      (503) staff       (20)        1 2023-07-12 21:15:32.000000 intrinio-sdk-6.24.1/intrinio_sdk.egg-info/dependency_links.txt
-drwxr-xr-x   0 shawn      (503) staff       (20)        0 2023-07-12 21:15:33.000000 intrinio-sdk-6.24.1/test/
--rw-r--r--   0 shawn      (503) staff       (20)     1292 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_etf_holding.py
--rw-r--r--   0 shawn      (503) staff       (20)     1540 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_security_commodity_channel_index.py
--rw-r--r--   0 shawn      (503) staff       (20)     1500 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_security_ichimoku_kinko_hyo.py
--rw-r--r--   0 shawn      (503) staff       (20)     1458 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_zacks_analyst_ratings.py
--rw-r--r--   0 shawn      (503) staff       (20)     1546 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_security_institutional_ownership.py
--rw-r--r--   0 shawn      (503) staff       (20)     1440 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_company_securities.py
--rw-r--r--   0 shawn      (503) staff       (20)     1300 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_option_price.py
--rw-r--r--   0 shawn      (503) staff       (20)     1276 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_sic_index.py
--rw-r--r--   0 shawn      (503) staff       (20)     1582 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_stock_exchange_stock_price_adjustments.py
--rw-r--r--   0 shawn      (503) staff       (20)     1234 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_etf.py
--rw-r--r--   0 shawn      (503) staff       (20)     1442 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_filing_notes_search.py
--rw-r--r--   0 shawn      (503) staff       (20)     1382 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_option_factors_realtime.py
--rw-r--r--   0 shawn      (503) staff       (20)     1460 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_zacks_eps_growth_rates.py
--rw-r--r--   0 shawn      (503) staff       (20)     1326 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_data_tag_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     1426 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_options_chain_eod.py
--rw-r--r--   0 shawn      (503) staff       (20)     1266 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_company.py
--rw-r--r--   0 shawn      (503) staff       (20)     1442 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_zacks_eps_surprises.py
--rw-r--r--   0 shawn      (503) staff       (20)     1466 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_options_chain_realtime.py
--rw-r--r--   0 shawn      (503) staff       (20)     1424 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_forex_currencies.py
--rw-r--r--   0 shawn      (503) staff       (20)     1350 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_esg_company_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     1384 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_sic_indices.py
--rw-r--r--   0 shawn      (503) staff       (20)     1400 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_mass_index_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1292 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_stock_price.py
--rw-r--r--   0 shawn      (503) staff       (20)     1274 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_security.py
--rw-r--r--   0 shawn      (503) staff       (20)     1540 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_security_stock_price_adjustments.py
--rw-r--r--   0 shawn      (503) staff       (20)     1350 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_bulk_download_links.py
--rw-r--r--   0 shawn      (503) staff       (20)     1308 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_etf_analytics.py
--rw-r--r--   0 shawn      (503) staff       (20)     1376 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_esg_rating_with_company.py
--rw-r--r--   0 shawn      (503) staff       (20)     1466 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_volume_weighted_average_price_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1358 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_filings.py
--rw-r--r--   0 shawn      (503) staff       (20)     1374 2023-07-10 16:51:28.000000 intrinio-sdk-6.24.1/test/test_security_trades_result.py
--rw-r--r--   0 shawn      (503) staff       (20)     1432 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_option_intervals_movers_result.py
--rw-r--r--   0 shawn      (503) staff       (20)     1598 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_esg_company_comprehensive_rating_history.py
--rw-r--r--   0 shawn      (503) staff       (20)     1374 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_security_screen_result.py
--rw-r--r--   0 shawn      (503) staff       (20)     1382 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_security_interval_mover.py
--rw-r--r--   0 shawn      (503) staff       (20)     4107 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_company_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     1366 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_option_snapshot_group.py
--rw-r--r--   0 shawn      (503) staff       (20)     1408 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_security_screen_result_data.py
--rw-r--r--   0 shawn      (503) staff       (20)     1488 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_stochastic_oscillator_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1292 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_filing_note.py
--rw-r--r--   0 shawn      (503) staff       (20)     1484 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_sic_index_historical_data.py
--rw-r--r--   0 shawn      (503) staff       (20)     1442 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_security_williams_r.py
--rw-r--r--   0 shawn      (503) staff       (20)     1508 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_security_zacks_eps_surprises.py
--rw-r--r--   0 shawn      (503) staff       (20)     1432 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_stock_price_adjustment_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     1466 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_options_stats_realtime.py
--rw-r--r--   0 shawn      (503) staff       (20)     1564 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_security_detrended_price_oscillator.py
--rw-r--r--   0 shawn      (503) staff       (20)     1300 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_reported_tag.py
--rw-r--r--   0 shawn      (503) staff       (20)     1400 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_option_prices.py
--rw-r--r--   0 shawn      (503) staff       (20)     1564 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_company_insider_transaction_filings.py
--rw-r--r--   0 shawn      (503) staff       (20)     1530 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_security_stochastic_oscillator.py
--rw-r--r--   0 shawn      (503) staff       (20)     1316 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_economic_index.py
--rw-r--r--   0 shawn      (503) staff       (20)     1424 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_realtime_stock_price_security.py
--rw-r--r--   0 shawn      (503) staff       (20)     1284 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_option_eod.py
--rw-r--r--   0 shawn      (503) staff       (20)     1316 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_stock_exchange.py
--rw-r--r--   0 shawn      (503) staff       (20)     1392 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_etf_holdings.py
--rw-r--r--   0 shawn      (503) staff       (20)     1356 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_technical_indicator.py
--rw-r--r--   0 shawn      (503) staff       (20)     1310 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_bulk_downloads_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     1368 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_data_tags.py
--rw-r--r--   0 shawn      (503) staff       (20)     1422 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_reported_financial_dimension.py
--rw-r--r--   0 shawn      (503) staff       (20)     1506 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_security_awesome_oscillator.py
--rw-r--r--   0 shawn      (503) staff       (20)     1530 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_zacks_institutional_holding_company_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     1424 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_economic_indices.py
--rw-r--r--   0 shawn      (503) staff       (20)     1562 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_standardized_financials_dimensions.py
--rw-r--r--   0 shawn      (503) staff       (20)     1514 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_security_ultimate_oscillator.py
--rw-r--r--   0 shawn      (503) staff       (20)     1366 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_option_price_realtime.py
--rw-r--r--   0 shawn      (503) staff       (20)     1408 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_option_price_batch_realtime.py
--rw-r--r--   0 shawn      (503) staff       (20)     1548 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_owner_insider_transaction_filings.py
--rw-r--r--   0 shawn      (503) staff       (20)     1490 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_security_vortex_indicator.py
--rw-r--r--   0 shawn      (503) staff       (20)     1500 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_security_chaikin_money_flow.py
--rw-r--r--   0 shawn      (503) staff       (20)     1448 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_security_intervals_movers_result.py
--rw-r--r--   0 shawn      (503) staff       (20)     1414 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_municipalities.py
--rw-r--r--   0 shawn      (503) staff       (20)     1416 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_historical_data.py
--rw-r--r--   0 shawn      (503) staff       (20)     1366 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_security_screen_group.py
--rw-r--r--   0 shawn      (503) staff       (20)     1358 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_realtime_stock_price.py
--rw-r--r--   0 shawn      (503) staff       (20)     1590 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_security_zacks_analyst_ratings_snapshot.py
--rw-r--r--   0 shawn      (503) staff       (20)     1476 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_security_know_sure_thing.py
--rw-r--r--   0 shawn      (503) staff       (20)     1482 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_esg_latest_comprehensive.py
--rw-r--r--   0 shawn      (503) staff       (20)     1506 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_insider_transaction_filings.py
--rw-r--r--   0 shawn      (503) staff       (20)     6812 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_technical_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     1482 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_security_intraday_prices.py
--rw-r--r--   0 shawn      (503) staff       (20)     1500 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_security_average_true_range.py
--rw-r--r--   0 shawn      (503) staff       (20)     1380 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_municipality_financial.py
--rw-r--r--   0 shawn      (503) staff       (20)     1484 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_on_balance_volume_mean_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1358 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_zacks_sales_surprise.py
--rw-r--r--   0 shawn      (503) staff       (20)     1482 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_esg_comprehensive_rating_with_company.py
--rw-r--r--   0 shawn      (503) staff       (20)     1400 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_zacks_eps_surprise_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     1336 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_et_fs.py
--rw-r--r--   0 shawn      (503) staff       (20)     1524 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_economic_index_historical_data.py
--rw-r--r--   0 shawn      (503) staff       (20)     1464 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_awesome_oscillator_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1482 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_security_interval_prices.py
--rw-r--r--   0 shawn      (503) staff       (20)     1526 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_security_on_balance_volume_mean.py
--rw-r--r--   0 shawn      (503) staff       (20)     1424 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_options_realtime.py
--rw-r--r--   0 shawn      (503) staff       (20)     1360 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_zacks_eps_growth_rate.py
--rw-r--r--   0 shawn      (503) staff       (20)     1342 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_stock_market_index.py
--rw-r--r--   0 shawn      (503) staff       (20)     1342 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_thea_entity_answer.py
--rw-r--r--   0 shawn      (503) staff       (20)     1416 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_stock_exchanges.py
--rw-r--r--   0 shawn      (503) staff       (20)     1462 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_standardized_financials_dimension.py
--rw-r--r--   0 shawn      (503) staff       (20)     1448 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_reported_financials.py
--rw-r--r--   0 shawn      (503) staff       (20)     1324 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_earnings_record.py
--rw-r--r--   0 shawn      (503) staff       (20)     3094 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_zacks_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     1326 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_option_price_eod.py
--rw-r--r--   0 shawn      (503) staff       (20)     1358 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_thea_source_document.py
--rw-r--r--   0 shawn      (503) staff       (20)     1604 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_moving_average_convergence_divergence_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     2223 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_fundamentals_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     1402 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_zacks_long_term_growth_rate.py
--rw-r--r--   0 shawn      (503) staff       (20)     1308 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_owner_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     1498 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_commodity_channel_index_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1350 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_stock_price_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     1406 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_insider_transaction_filing.py
--rw-r--r--   0 shawn      (503) staff       (20)     1458 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_security_stock_prices.py
--rw-r--r--   0 shawn      (503) staff       (20)     1482 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_negative_volume_index_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1484 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_security_ease_of_movement.py
--rw-r--r--   0 shawn      (503) staff       (20)     1458 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_ichimoku_kinko_hyo_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1514 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_zacks_institutional_holding_owner_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)        0 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/test/__init__.py
--rw-r--r--   0 shawn      (503) staff       (20)     1559 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_data_tag_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     1366 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_bulk_download_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     1522 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_triple_exponential_average_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1358 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_company_news_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     1440 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_company_initial_public_offering.py
--rw-r--r--   0 shawn      (503) staff       (20)     1482 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_security_historical_data.py
--rw-r--r--   0 shawn      (503) staff       (20)     1384 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_forex_pairs.py
--rw-r--r--   0 shawn      (503) staff       (20)     2673 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_filing_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     1490 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_stock_exchange_securities.py
--rw-r--r--   0 shawn      (503) staff       (20)     1440 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_keltner_channel_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1398 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_security_snapshots_result.py
--rw-r--r--   0 shawn      (503) staff       (20)     2236 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_stock_exchange_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     1448 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_vortex_indicator_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1408 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_force_index_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1482 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_initial_public_offerings.py
--rw-r--r--   0 shawn      (503) staff       (20)     1558 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_forex_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     1500 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_security_volume_price_trend.py
--rw-r--r--   0 shawn      (503) staff       (20)     1292 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_forex_price.py
--rw-r--r--   0 shawn      (503) staff       (20)     1434 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_zacks_etf_holdings.py
--rw-r--r--   0 shawn      (503) staff       (20)     1324 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_company_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     1284 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_forex_pair.py
--rw-r--r--   0 shawn      (503) staff       (20)     1482 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_security_bollinger_bands.py
--rw-r--r--   0 shawn      (503) staff       (20)     1524 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_security_zacks_sales_surprises.py
--rw-r--r--   0 shawn      (503) staff       (20)     1582 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_security_volume_weighted_average_price.py
--rw-r--r--   0 shawn      (503) staff       (20)     1466 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_true_strength_index_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1516 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_options_prices_batch_realtime.py
--rw-r--r--   0 shawn      (503) staff       (20)     1556 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_zacks_institutional_holding_owners.py
--rw-r--r--   0 shawn      (503) staff       (20)     1448 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_filing_fundamentals.py
--rw-r--r--   0 shawn      (503) staff       (20)     1448 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_donchian_channel_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1390 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_esg_comprehensive_rating.py
--rw-r--r--   0 shawn      (503) staff       (20)     1392 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_forex_prices.py
--rw-r--r--   0 shawn      (503) staff       (20)     1382 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_option_intervals_result.py
--rw-r--r--   0 shawn      (503) staff       (20)     1366 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_option_stats_realtime.py
--rw-r--r--   0 shawn      (503) staff       (20)     1562 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_accumulation_distribution_index_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1434 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_sic_indices_search.py
--rw-r--r--   0 shawn      (503) staff       (20)     1458 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_average_true_range_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1448 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_options_expirations.py
--rw-r--r--   0 shawn      (503) staff       (20)     1434 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_know_sure_thing_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1522 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_detrended_price_oscillator_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1276 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_etf_stats.py
--rw-r--r--   0 shawn      (503) staff       (20)     1418 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_data_tags_search.py
--rw-r--r--   0 shawn      (503) staff       (20)     1400 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_esg_companies.py
--rw-r--r--   0 shawn      (503) staff       (20)     1442 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_ease_of_movement_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1482 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_security_keltner_channel.py
--rw-r--r--   0 shawn      (503) staff       (20)     1918 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_owners_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     1458 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_chaikin_money_flow_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1482 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_options_unusual_activity.py
--rw-r--r--   0 shawn      (503) staff       (20)     1482 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_simple_moving_average_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1524 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_security_negative_volume_index.py
--rw-r--r--   0 shawn      (503) staff       (20)     1466 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_options_price_realtime.py
--rw-r--r--   0 shawn      (503) staff       (20)     1382 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_option_snapshots_result.py
--rw-r--r--   0 shawn      (503) staff       (20)     1522 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_zacks_institutional_holding_company_detail.py
--rw-r--r--   0 shawn      (503) staff       (20)     1500 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_stock_market_indices_search.py
--rw-r--r--   0 shawn      (503) staff       (20)     1500 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_stock_exchange_stock_prices.py
--rw-r--r--   0 shawn      (503) staff       (20)     1574 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_security_average_daily_trading_volume.py
--rw-r--r--   0 shawn      (503) staff       (20)     1456 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_company_fundamentals.py
--rw-r--r--   0 shawn      (503) staff       (20)     1564 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_security_triple_exponential_average.py
--rw-r--r--   0 shawn      (503) staff       (20)     1342 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_zacks_eps_surprise.py
--rw-r--r--   0 shawn      (503) staff       (20)     1284 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_esg_rating.py
--rw-r--r--   0 shawn      (503) staff       (20)     1342 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_filing_note_filing.py
--rw-r--r--   0 shawn      (503) staff       (20)     1488 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_municipalitiy_financials.py
--rw-r--r--   0 shawn      (503) staff       (20)     1392 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_company_news.py
--rw-r--r--   0 shawn      (503) staff       (20)     1374 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_stock_price_adjustment.py
--rw-r--r--   0 shawn      (503) staff       (20)     1342 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_zacks_eps_estimate.py
--rw-r--r--   0 shawn      (503) staff       (20)     1502 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_zacks_long_term_growth_rates.py
--rw-r--r--   0 shawn      (503) staff       (20)     1506 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_zacks_institutional_holding_owner_detail.py
--rw-r--r--   0 shawn      (503) staff       (20)     1442 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_money_flow_index_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1358 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_options.py
--rw-r--r--   0 shawn      (503) staff       (20)     1298 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_fundamental.py
--rw-r--r--   0 shawn      (503) staff       (20)     1356 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_fundamental_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     1556 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_security_average_directional_index.py
--rw-r--r--   0 shawn      (503) staff       (20)     1434 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_options_prices_eod.py
--rw-r--r--   0 shawn      (503) staff       (20)     1550 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_stock_market_index_historical_data.py
--rw-r--r--   0 shawn      (503) staff       (20)     1648 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_municipality_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     1498 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_company_shares_outstanding.py
--rw-r--r--   0 shawn      (503) staff       (20)     1484 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_security_money_flow_index.py
--rw-r--r--   0 shawn      (503) staff       (20)     1514 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_average_directional_index_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1366 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_option_chain_realtime.py
--rw-r--r--   0 shawn      (503) staff       (20)     1366 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_option_contracts_list.py
--rw-r--r--   0 shawn      (503) staff       (20)    10454 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_security_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     1424 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_zacks_analyst_rating_snapshot.py
--rw-r--r--   0 shawn      (503) staff       (20)     1458 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_zacks_sales_surprises.py
--rw-r--r--   0 shawn      (503) staff       (20)     1388 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_institutional_ownership.py
--rw-r--r--   0 shawn      (503) staff       (20)     1508 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_security_true_strength_index.py
--rw-r--r--   0 shawn      (503) staff       (20)     1416 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_options_tickers.py
--rw-r--r--   0 shawn      (503) staff       (20)     1514 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_owner_institutional_holdings.py
--rw-r--r--   0 shawn      (503) staff       (20)     1431 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_insider_transaction_filings_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     1392 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_filing_notes.py
--rw-r--r--   0 shawn      (503) staff       (20)     1358 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_option_unusual_trade.py
--rw-r--r--   0 shawn      (503) staff       (20)     1300 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_option_chain.py
--rw-r--r--   0 shawn      (503) staff       (20)     1458 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_volume_price_trend_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1350 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_filing_note_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     1258 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_option.py
--rw-r--r--   0 shawn      (503) staff       (20)     1416 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_zacks_target_price_consensus.py
--rw-r--r--   0 shawn      (503) staff       (20)     1292 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_etf_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     1474 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_company_historical_data.py
--rw-r--r--   0 shawn      (503) staff       (20)     1498 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_relative_strength_index_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1416 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_zacks_sales_surprise_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     1324 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_option_realtime.py
--rw-r--r--   0 shawn      (503) staff       (20)     1450 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_stock_market_indices.py
--rw-r--r--   0 shawn      (503) staff       (20)     1372 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_institutional_holding.py
--rw-r--r--   0 shawn      (503) staff       (20)     1350 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_owners.py
--rw-r--r--   0 shawn      (503) staff       (20)     1324 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_option_interval.py
--rw-r--r--   0 shawn      (503) staff       (20)     1450 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_security_force_index.py
--rw-r--r--   0 shawn      (503) staff       (20)     1524 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_security_zacks_analyst_ratings.py
--rw-r--r--   0 shawn      (503) staff       (20)     1408 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_filing_answers.py
--rw-r--r--   0 shawn      (503) staff       (20)     1268 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_data_tag.py
--rw-r--r--   0 shawn      (503) staff       (20)     1356 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_insider_transaction.py
--rw-r--r--   0 shawn      (503) staff       (20)     1380 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_standardized_financial.py
--rw-r--r--   0 shawn      (503) staff       (20)     1566 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_stock_exchange_realtime_stock_prices.py
--rw-r--r--   0 shawn      (503) staff       (20)     5109 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_options_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     1416 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_company_filings.py
--rw-r--r--   0 shawn      (503) staff       (20)     1472 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_ultimate_oscillator_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1432 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_company_recognize.py
--rw-r--r--   0 shawn      (503) staff       (20)     1376 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_esg_latest.py
--rw-r--r--   0 shawn      (503) staff       (20)     1934 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_esg_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     1414 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_zacks_institutional_holding.py
--rw-r--r--   0 shawn      (503) staff       (20)     1374 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_security_screen_clause.py
--rw-r--r--   0 shawn      (503) staff       (20)     1406 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_company_shares_outstanding.py
--rw-r--r--   0 shawn      (503) staff       (20)     1440 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_bollinger_bands_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1324 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_historical_data.py
--rw-r--r--   0 shawn      (503) staff       (20)     1332 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_security_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     1442 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_security_mass_index.py
--rw-r--r--   0 shawn      (503) staff       (20)     1432 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_securities_search.py
--rw-r--r--   0 shawn      (503) staff       (20)     1316 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_forex_currency.py
--rw-r--r--   0 shawn      (503) staff       (20)     1374 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_economic_index_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     1524 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_security_simple_moving_average.py
--rw-r--r--   0 shawn      (503) staff       (20)     1258 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_filing.py
--rw-r--r--   0 shawn      (503) staff       (20)     1334 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_zacks_etf_holding.py
--rw-r--r--   0 shawn      (503) staff       (20)     1524 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_zacks_target_price_consensuses.py
--rw-r--r--   0 shawn      (503) staff       (20)     1324 2023-07-10 16:51:28.000000 intrinio-sdk-6.24.1/test/test_security_trades.py
--rw-r--r--   0 shawn      (503) staff       (20)     1416 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_zacks_analyst_rating_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     1924 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_et_fs_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     1554 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_zacks_institutional_holding_historical_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     1604 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_security_accumulation_distribution_index.py
--rw-r--r--   0 shawn      (503) staff       (20)     1334 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_news.py
--rw-r--r--   0 shawn      (503) staff       (20)     1444 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_data_point_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     1492 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_security_on_balance_volume.py
--rw-r--r--   0 shawn      (503) staff       (20)     1408 2023-07-10 16:51:28.000000 intrinio-sdk-6.24.1/test/test_security_replay_file_result.py
--rw-r--r--   0 shawn      (503) staff       (20)     1480 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_standardized_financials.py
--rw-r--r--   0 shawn      (503) staff       (20)     1400 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_stock_market_index_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     1646 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_security_moving_average_convergence_divergence.py
--rw-r--r--   0 shawn      (503) staff       (20)     1316 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_filing_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     1514 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_zacks_institutional_holdings.py
--rw-r--r--   0 shawn      (503) staff       (20)     1382 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_security_snapshot_group.py
--rw-r--r--   0 shawn      (503) staff       (20)     1400 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_options_chain.py
--rw-r--r--   0 shawn      (503) staff       (20)     1366 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_option_interval_mover.py
--rw-r--r--   0 shawn      (503) staff       (20)     1424 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_companies_search.py
--rw-r--r--   0 shawn      (503) staff       (20)     1474 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_economic_indices_search.py
--rw-r--r--   0 shawn      (503) staff       (20)     1374 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_companies.py
--rw-r--r--   0 shawn      (503) staff       (20)     1450 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_on_balance_volume_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1492 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_esg_company_rating_history.py
--rw-r--r--   0 shawn      (503) staff       (20)     1416 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_company_answers.py
--rw-r--r--   0 shawn      (503) staff       (20)     1358 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_intraday_stock_price.py
--rw-r--r--   0 shawn      (503) staff       (20)     1348 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_reported_financial.py
--rw-r--r--   0 shawn      (503) staff       (20)     1540 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_security_relative_strength_index.py
--rw-r--r--   0 shawn      (503) staff       (20)     1442 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_bulk_download_links.py
--rw-r--r--   0 shawn      (503) staff       (20)     4422 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_index_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     1358 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_stock_price_interval.py
--rw-r--r--   0 shawn      (503) staff       (20)     1400 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_williams_r_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1532 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_average_daily_trading_volume_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1300 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_company_news.py
--rw-r--r--   0 shawn      (503) staff       (20)     1382 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_securities.py
--rw-r--r--   0 shawn      (503) staff       (20)     1326 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_option_chain_eod.py
--rw-r--r--   0 shawn      (503) staff       (20)     1580 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_zacks_institutional_holding_companies.py
--rw-r--r--   0 shawn      (503) staff       (20)     1306 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_municipality.py
--rw-r--r--   0 shawn      (503) staff       (20)     1490 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_security_donchian_channel.py
--rw-r--r--   0 shawn      (503) staff       (20)     1316 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_company_filing.py
--rw-r--r--   0 shawn      (503) staff       (20)     1314 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_historical_data_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     1358 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_zacks_analyst_rating.py
--rw-r--r--   0 shawn      (503) staff       (20)     1250 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_owner.py
--rw-r--r--   0 shawn      (503) staff       (20)     1442 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_api_response_zacks_eps_estimates.py
--rw-r--r--   0 shawn      (503) staff       (20)     1324 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.1/test/test_dividend_record.py
--rw-r--r--   0 shawn      (503) staff       (20)    57774 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/README.md
--rw-r--r--   0 shawn      (503) staff       (20)     1844 2023-07-10 17:08:18.000000 intrinio-sdk-6.24.1/setup.py
--rw-r--r--   0 shawn      (503) staff       (20)       38 2023-07-12 21:15:33.000000 intrinio-sdk-6.24.1/setup.cfg
+drwxr-xr-x   0 redbeard  (1000) redbeard  (1000)        0 2023-08-01 21:44:04.222494 intrinio-sdk-6.25.0/
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)      698 2023-08-01 21:44:04.218495 intrinio-sdk-6.25.0/PKG-INFO
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    57774 2023-08-01 21:03:10.000000 intrinio-sdk-6.25.0/README.md
+drwxr-xr-x   0 redbeard  (1000) redbeard  (1000)        0 2023-08-01 21:44:04.118498 intrinio-sdk-6.25.0/intrinio_sdk/
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    25844 2023-08-01 21:03:10.000000 intrinio-sdk-6.25.0/intrinio_sdk/__init__.py
+drwxr-xr-x   0 redbeard  (1000) redbeard  (1000)        0 2023-08-01 21:44:04.122498 intrinio-sdk-6.25.0/intrinio_sdk/api/
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1157 2023-08-01 21:03:10.000000 intrinio-sdk-6.25.0/intrinio_sdk/api/__init__.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     4435 2023-08-01 21:03:10.000000 intrinio-sdk-6.25.0/intrinio_sdk/api/bulk_downloads_api.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    95784 2023-08-01 21:03:10.000000 intrinio-sdk-6.25.0/intrinio_sdk/api/company_api.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    10452 2023-08-01 21:03:10.000000 intrinio-sdk-6.25.0/intrinio_sdk/api/data_point_api.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    14009 2023-08-01 21:03:10.000000 intrinio-sdk-6.25.0/intrinio_sdk/api/data_tag_api.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    22700 2023-08-01 21:03:10.000000 intrinio-sdk-6.25.0/intrinio_sdk/api/esg_api.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    26155 2023-08-01 21:03:10.000000 intrinio-sdk-6.25.0/intrinio_sdk/api/et_fs_api.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    51756 2023-08-01 21:03:10.000000 intrinio-sdk-6.25.0/intrinio_sdk/api/filing_api.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    14832 2023-08-01 21:03:10.000000 intrinio-sdk-6.25.0/intrinio_sdk/api/forex_api.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    31234 2023-08-01 21:03:10.000000 intrinio-sdk-6.25.0/intrinio_sdk/api/fundamentals_api.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     7996 2023-08-01 21:03:10.000000 intrinio-sdk-6.25.0/intrinio_sdk/api/historical_data_api.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    84166 2023-08-01 21:03:10.000000 intrinio-sdk-6.25.0/intrinio_sdk/api/index_api.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6358 2023-08-01 21:03:10.000000 intrinio-sdk-6.25.0/intrinio_sdk/api/insider_transaction_filings_api.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    16465 2023-08-01 21:03:10.000000 intrinio-sdk-6.25.0/intrinio_sdk/api/municipality_api.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)   130515 2023-08-01 21:03:10.000000 intrinio-sdk-6.25.0/intrinio_sdk/api/options_api.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    25579 2023-08-01 21:03:10.000000 intrinio-sdk-6.25.0/intrinio_sdk/api/owners_api.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)   359486 2023-08-01 21:03:10.000000 intrinio-sdk-6.25.0/intrinio_sdk/api/security_api.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    30181 2023-08-01 21:03:10.000000 intrinio-sdk-6.25.0/intrinio_sdk/api/stock_exchange_api.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)   213664 2023-08-01 21:03:10.000000 intrinio-sdk-6.25.0/intrinio_sdk/api/technical_api.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    74950 2023-08-01 21:03:10.000000 intrinio-sdk-6.25.0/intrinio_sdk/api/zacks_api.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    26891 2023-08-01 21:03:10.000000 intrinio-sdk-6.25.0/intrinio_sdk/api_client.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     8604 2023-08-01 21:03:10.000000 intrinio-sdk-6.25.0/intrinio_sdk/configuration.py
+drwxr-xr-x   0 redbeard  (1000) redbeard  (1000)        0 2023-08-01 21:44:04.174496 intrinio-sdk-6.25.0/intrinio_sdk/models/
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    24625 2023-08-01 21:03:10.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/__init__.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6614 2023-08-01 21:03:08.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/accumulation_distribution_index_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     4704 2023-08-01 21:03:08.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_bulk_download_links.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6469 2023-08-01 21:03:08.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_companies.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     4530 2023-08-01 21:03:08.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_companies_search.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     9762 2023-08-01 21:03:08.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_company_answers.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     8175 2023-08-01 21:03:08.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_company_filings.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     8435 2023-08-01 21:03:08.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_company_fundamentals.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     8528 2023-08-01 21:03:08.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_company_historical_data.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     9185 2023-08-01 21:03:08.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_company_insider_transaction_filings.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     8068 2023-08-01 21:03:08.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_company_news.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     4539 2023-08-01 21:03:08.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_company_recognize.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     8325 2023-08-01 21:03:08.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_company_securities.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6644 2023-08-01 21:03:08.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_company_shares_outstanding.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6287 2023-08-01 21:03:08.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_data_tags.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     4354 2023-08-01 21:03:08.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_data_tags_search.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     8641 2023-08-01 21:03:08.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_economic_index_historical_data.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6546 2023-08-01 21:03:08.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_economic_indices.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     4571 2023-08-01 21:03:08.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_economic_indices_search.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6533 2023-08-01 21:03:08.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_esg_companies.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     8711 2023-08-01 21:03:08.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_esg_company_comprehensive_rating_history.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     8359 2023-08-01 21:03:08.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_esg_company_rating_history.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6457 2023-08-01 21:03:08.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_esg_latest.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6731 2023-08-01 21:03:08.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_esg_latest_comprehensive.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6245 2023-08-01 21:03:08.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_et_fs.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     7995 2023-08-01 21:03:08.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_etf_holdings.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     9686 2023-08-01 21:03:08.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_filing_answers.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     8383 2023-08-01 21:03:08.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_filing_fundamentals.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6593 2023-08-01 21:03:08.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_filing_notes.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     4642 2023-08-01 21:03:08.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_filing_notes_search.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6340 2023-08-01 21:03:08.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_filings.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     4549 2023-08-01 21:03:08.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_forex_currencies.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     4355 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_forex_pairs.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     8244 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_forex_prices.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6694 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_historical_data.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     7125 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_initial_public_offerings.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    10988 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_insider_transaction_filings.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6656 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_municipalities.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6522 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_municipalitiy_financials.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6251 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_news.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     8290 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_option_prices.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6602 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_options.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     4746 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_options_chain.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     4819 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_options_chain_eod.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     4894 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_options_chain_realtime.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     4754 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_options_expirations.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     7884 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_options_price_realtime.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     4691 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_options_prices_batch_realtime.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     8397 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_options_prices_eod.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     4742 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_options_realtime.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     7946 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_options_stats_realtime.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     4344 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_options_tickers.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     4823 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_options_unusual_activity.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     9075 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_owner_insider_transaction_filings.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6560 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_owner_institutional_holdings.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6500 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_owners.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     8664 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_reported_financials.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6515 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_securities.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     4570 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_securities_search.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    11307 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_accumulation_distribution_index.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    11176 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_average_daily_trading_volume.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    11109 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_average_directional_index.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    10878 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_average_true_range.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    10910 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_awesome_oscillator.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    10811 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_bollinger_bands.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    10878 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_chaikin_money_flow.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    11043 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_commodity_channel_index.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    11142 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_detrended_price_oscillator.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    10844 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_donchian_channel.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    10812 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_ease_of_movement.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    10679 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_force_index.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     8580 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_historical_data.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    10878 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_ichimoku_kinko_hyo.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6832 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_institutional_ownership.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    11155 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_interval_prices.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    11164 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_intraday_prices.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    10811 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_keltner_channel.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    10779 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_know_sure_thing.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    10646 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_mass_index.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    10812 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_money_flow_index.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    11473 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_moving_average_convergence_divergence.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    10977 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_negative_volume_index.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    10845 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_on_balance_volume.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    10978 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_on_balance_volume_mean.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    11043 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_relative_strength_index.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    10977 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_simple_moving_average.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    11009 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_stochastic_oscillator.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     9510 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_stock_price_adjustments.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     8931 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_stock_prices.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    11142 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_triple_exponential_average.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    10911 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_true_strength_index.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    10943 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_ultimate_oscillator.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    10878 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_volume_price_trend.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    11154 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_volume_weighted_average_price.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    10844 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_vortex_indicator.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    10646 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_williams_r.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     9009 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_zacks_analyst_ratings.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6884 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_zacks_analyst_ratings_snapshot.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     8905 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_zacks_eps_surprises.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     9009 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_zacks_sales_surprises.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     8463 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_sic_index_historical_data.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6398 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_sic_indices.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     4453 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_sic_indices_search.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     8872 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_standardized_financials.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     8917 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_standardized_financials_dimensions.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     9486 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_stock_exchange_realtime_stock_prices.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     9138 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_stock_exchange_securities.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     9875 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_stock_exchange_stock_price_adjustments.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     9296 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_stock_exchange_stock_prices.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6688 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_stock_exchanges.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     8723 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_stock_market_index_historical_data.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6610 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_stock_market_indices.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     4617 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_stock_market_indices_search.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6794 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_zacks_analyst_ratings.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6855 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_zacks_eps_estimates.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     7058 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_zacks_eps_growth_rates.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     7063 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_zacks_eps_surprises.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6737 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_zacks_etf_holdings.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     7226 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_zacks_institutional_holding_companies.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     7091 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_zacks_institutional_holding_owners.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6977 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_zacks_institutional_holdings.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     7396 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_zacks_long_term_growth_rates.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     7161 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_zacks_sales_surprises.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     7447 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_zacks_target_price_consensuses.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6570 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/average_daily_trading_volume_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    10151 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/average_directional_index_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6380 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/average_true_range_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6370 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/awesome_oscillator_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    10662 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/bollinger_bands_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6050 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/bulk_download_links.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    13776 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/bulk_download_summary.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6380 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/chaikin_money_flow_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6470 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/commodity_channel_index_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    70186 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/company.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    21150 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/company_filing.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    50532 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/company_initial_public_offering.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    12984 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/company_news.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    11361 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/company_news_summary.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    14903 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/company_shares_outstanding.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    11092 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/company_summary.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    22029 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/data_tag.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    16540 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/data_tag_summary.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6524 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/detrended_price_oscillator_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    23216 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/dividend_record.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     8595 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/donchian_channel_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    52025 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/earnings_record.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6344 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/ease_of_movement_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    24303 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/economic_index.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    22944 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/economic_index_summary.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    13643 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/esg_company_summary.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)   114262 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/esg_comprehensive_rating.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)   118624 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/esg_comprehensive_rating_with_company.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    16235 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/esg_rating.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    18293 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/esg_rating_with_company.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)   253901 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/etf.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    23120 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/etf_analytics.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    37768 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/etf_holding.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    79809 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/etf_stats.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    16293 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/etf_summary.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    26231 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/filing.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     9528 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/filing_note.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    10320 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/filing_note_filing.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     7753 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/filing_note_summary.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    19534 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/filing_summary.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6244 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/force_index_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     7658 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/forex_currency.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     8094 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/forex_pair.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    19707 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/forex_price.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    21288 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/fundamental.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    17338 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/fundamental_summary.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     5995 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/historical_data.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    14869 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/ichimoku_kinko_hyo_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    43221 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/insider_transaction.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    16239 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/insider_transaction_filing.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    32022 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/institutional_holding.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    23168 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/institutional_ownership.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    16848 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/intraday_stock_price.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    10482 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/keltner_channel_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6326 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/know_sure_thing_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6226 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/mass_index_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6344 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/money_flow_index_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    11274 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/moving_average_convergence_divergence_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    37102 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/municipality.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)   136507 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/municipality_financial.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6434 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/negative_volume_index_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6562 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/on_balance_volume_mean_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6362 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/on_balance_volume_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    14640 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/option.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     5782 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/option_chain.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     5890 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/option_chain_eod.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     7632 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/option_chain_realtime.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     4340 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/option_contracts_list.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    13209 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/option_eod.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    14908 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/option_factors_realtime.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    18458 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/option_interval.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    16762 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/option_interval_mover.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    10743 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/option_intervals_movers_result.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     8557 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/option_intervals_result.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    31195 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/option_price.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6075 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/option_price_batch_realtime.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    40407 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/option_price_eod.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    24804 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/option_price_realtime.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    12679 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/option_realtime.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6210 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/option_snapshot_group.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     4817 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/option_snapshots_result.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    14644 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/option_stats_realtime.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    24031 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/option_unusual_trade.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    25762 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/owner.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6371 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/owner_summary.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    50157 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/realtime_stock_price.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    11790 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/realtime_stock_price_security.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6470 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/relative_strength_index_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     8401 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/reported_financial.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6167 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/reported_financial_dimension.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    14527 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/reported_tag.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    54424 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/security.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    16643 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/security_interval_mover.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    10809 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/security_intervals_movers_result.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     7800 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/security_replay_file_result.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     8284 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/security_screen_clause.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     8290 2023-08-01 21:03:26.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/security_screen_group.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6101 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/security_screen_result.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     8133 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/security_screen_result_data.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6240 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/security_snapshot_group.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     4847 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/security_snapshots_result.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    22943 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/security_summary.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    14988 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/security_trades.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     8703 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/security_trades_result.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    10907 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/sic_index.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6434 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/simple_moving_average_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6233 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/standardized_financial.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6357 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/standardized_financials_dimension.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     8341 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/stochastic_oscillator_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    20554 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/stock_exchange.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    20794 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/stock_market_index.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    19333 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/stock_market_index_summary.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    41799 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/stock_price.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    14290 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/stock_price_adjustment.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    12624 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/stock_price_adjustment_summary.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    20665 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/stock_price_interval.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    40823 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/stock_price_summary.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6122 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/technical_indicator.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     8400 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/thea_entity_answer.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6145 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/thea_source_document.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6549 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/triple_exponential_average_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6398 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/true_strength_index_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6388 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/ultimate_oscillator_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6380 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/volume_price_trend_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6465 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/volume_weighted_average_price_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     8463 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/vortex_indicator_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6229 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/williams_r_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    20362 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/zacks_analyst_rating.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    23701 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/zacks_analyst_rating_snapshot.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    18849 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/zacks_analyst_rating_summary.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    34497 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/zacks_eps_estimate.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    56139 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/zacks_eps_growth_rate.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    36893 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/zacks_eps_surprise.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    35692 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/zacks_eps_surprise_summary.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    15061 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/zacks_etf_holding.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    29315 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/zacks_institutional_holding.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    32532 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/zacks_institutional_holding_company_detail.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     8432 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/zacks_institutional_holding_company_summary.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6739 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/zacks_institutional_holding_historical_summary.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    45403 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/zacks_institutional_holding_owner_detail.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6482 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/zacks_institutional_holding_owner_summary.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    57040 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/zacks_long_term_growth_rate.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    37674 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/zacks_sales_surprise.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    40363 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/zacks_sales_surprise_summary.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    26373 2023-08-01 21:03:09.000000 intrinio-sdk-6.25.0/intrinio_sdk/models/zacks_target_price_consensus.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    13819 2023-08-01 21:03:10.000000 intrinio-sdk-6.25.0/intrinio_sdk/rest.py
+drwxr-xr-x   0 redbeard  (1000) redbeard  (1000)        0 2023-08-01 21:44:04.118498 intrinio-sdk-6.25.0/intrinio_sdk.egg-info/
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)      698 2023-08-01 21:44:04.000000 intrinio-sdk-6.25.0/intrinio_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    27307 2023-08-01 21:44:04.000000 intrinio-sdk-6.25.0/intrinio_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)        1 2023-08-01 21:44:04.000000 intrinio-sdk-6.25.0/intrinio_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)       64 2023-08-01 21:44:04.000000 intrinio-sdk-6.25.0/intrinio_sdk.egg-info/requires.txt
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)       18 2023-08-01 21:44:04.000000 intrinio-sdk-6.25.0/intrinio_sdk.egg-info/top_level.txt
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)       38 2023-08-01 21:44:04.222494 intrinio-sdk-6.25.0/setup.cfg
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1844 2023-08-01 21:03:10.000000 intrinio-sdk-6.25.0/setup.py
+drwxr-xr-x   0 redbeard  (1000) redbeard  (1000)        0 2023-08-01 21:44:04.218495 intrinio-sdk-6.25.0/test/
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)        0 2023-08-01 21:03:10.000000 intrinio-sdk-6.25.0/test/__init__.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1562 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_accumulation_distribution_index_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1442 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_bulk_download_links.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1374 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_companies.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1424 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_companies_search.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1416 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_company_answers.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1416 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_company_filings.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1456 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_company_fundamentals.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1474 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_company_historical_data.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1564 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_company_insider_transaction_filings.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1392 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_company_news.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1432 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_company_recognize.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1440 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_company_securities.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1498 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_company_shares_outstanding.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1368 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_data_tags.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1418 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_data_tags_search.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1524 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_economic_index_historical_data.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1424 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_economic_indices.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1474 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_economic_indices_search.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1400 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_esg_companies.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1598 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_esg_company_comprehensive_rating_history.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1492 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_esg_company_rating_history.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1376 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_esg_latest.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1482 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_esg_latest_comprehensive.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1336 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_et_fs.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1392 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_etf_holdings.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1408 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_filing_answers.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1448 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_filing_fundamentals.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1392 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_filing_notes.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1442 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_filing_notes_search.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1358 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_filings.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1424 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_forex_currencies.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1384 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_forex_pairs.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1392 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_forex_prices.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1416 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_historical_data.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1482 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_initial_public_offerings.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1506 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_insider_transaction_filings.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1414 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_municipalities.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1488 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_municipalitiy_financials.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1334 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_news.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1400 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_option_prices.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1358 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_options.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1400 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_options_chain.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1426 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_options_chain_eod.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1466 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_options_chain_realtime.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1448 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_options_expirations.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1466 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_options_price_realtime.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1516 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_options_prices_batch_realtime.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1434 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_options_prices_eod.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1424 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_options_realtime.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1466 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_options_stats_realtime.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1416 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_options_tickers.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1482 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_options_unusual_activity.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1548 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_owner_insider_transaction_filings.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1514 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_owner_institutional_holdings.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1350 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_owners.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1448 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_reported_financials.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1382 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_securities.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1432 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_securities_search.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1604 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_security_accumulation_distribution_index.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1574 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_security_average_daily_trading_volume.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1556 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_security_average_directional_index.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1500 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_security_average_true_range.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1506 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_security_awesome_oscillator.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1482 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_security_bollinger_bands.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1500 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_security_chaikin_money_flow.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1540 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_security_commodity_channel_index.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1564 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_security_detrended_price_oscillator.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1490 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_security_donchian_channel.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1484 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_security_ease_of_movement.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1450 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_security_force_index.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1482 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_security_historical_data.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1500 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_security_ichimoku_kinko_hyo.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1546 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_security_institutional_ownership.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1482 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_security_interval_prices.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1482 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_security_intraday_prices.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1482 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_security_keltner_channel.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1476 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_security_know_sure_thing.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1442 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_security_mass_index.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1484 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_security_money_flow_index.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1646 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_security_moving_average_convergence_divergence.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1524 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_security_negative_volume_index.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1492 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_security_on_balance_volume.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1526 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_security_on_balance_volume_mean.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1540 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_security_relative_strength_index.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1524 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_security_simple_moving_average.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1530 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_security_stochastic_oscillator.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1540 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_security_stock_price_adjustments.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1458 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_security_stock_prices.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1564 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_security_triple_exponential_average.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1508 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_security_true_strength_index.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1514 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_security_ultimate_oscillator.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1500 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_security_volume_price_trend.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1582 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_security_volume_weighted_average_price.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1490 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_security_vortex_indicator.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1442 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_security_williams_r.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1524 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_security_zacks_analyst_ratings.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1590 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_security_zacks_analyst_ratings_snapshot.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1508 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_security_zacks_eps_surprises.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1524 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_security_zacks_sales_surprises.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1484 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_sic_index_historical_data.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1384 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_sic_indices.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1434 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_sic_indices_search.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1480 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_standardized_financials.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1562 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_standardized_financials_dimensions.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1566 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_stock_exchange_realtime_stock_prices.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1490 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_stock_exchange_securities.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1582 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_stock_exchange_stock_price_adjustments.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1500 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_stock_exchange_stock_prices.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1416 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_stock_exchanges.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1550 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_stock_market_index_historical_data.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1450 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_stock_market_indices.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1500 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_stock_market_indices_search.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1458 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_zacks_analyst_ratings.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1442 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_zacks_eps_estimates.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1460 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_zacks_eps_growth_rates.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1442 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_zacks_eps_surprises.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1434 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_zacks_etf_holdings.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1580 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_zacks_institutional_holding_companies.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1556 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_zacks_institutional_holding_owners.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1514 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_zacks_institutional_holdings.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1502 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_zacks_long_term_growth_rates.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1458 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_zacks_sales_surprises.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1524 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_api_response_zacks_target_price_consensuses.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1532 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_average_daily_trading_volume_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1514 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_average_directional_index_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1458 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_average_true_range_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1464 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_awesome_oscillator_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1440 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_bollinger_bands_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1350 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_bulk_download_links.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1366 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_bulk_download_summary.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1310 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_bulk_downloads_api.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1458 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_chaikin_money_flow_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1498 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_commodity_channel_index_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1266 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_company.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     4107 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_company_api.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1316 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_company_filing.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1440 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_company_initial_public_offering.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1300 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_company_news.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1358 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_company_news_summary.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1406 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_company_shares_outstanding.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1324 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_company_summary.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1444 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_data_point_api.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1268 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_data_tag.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1559 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_data_tag_api.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1326 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_data_tag_summary.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1522 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_detrended_price_oscillator_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1324 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_dividend_record.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1448 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_donchian_channel_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1324 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_earnings_record.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1442 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_ease_of_movement_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1316 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_economic_index.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1374 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_economic_index_summary.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1934 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_esg_api.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1350 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_esg_company_summary.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1390 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_esg_comprehensive_rating.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1482 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_esg_comprehensive_rating_with_company.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1284 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_esg_rating.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1376 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_esg_rating_with_company.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1924 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_et_fs_api.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1234 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_etf.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1308 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_etf_analytics.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1292 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_etf_holding.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1276 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_etf_stats.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1292 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_etf_summary.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1258 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_filing.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     2673 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_filing_api.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1292 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_filing_note.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1342 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_filing_note_filing.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1350 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_filing_note_summary.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1316 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_filing_summary.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1408 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_force_index_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1558 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_forex_api.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1316 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_forex_currency.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1284 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_forex_pair.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1292 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_forex_price.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1298 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_fundamental.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1356 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_fundamental_summary.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     2223 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_fundamentals_api.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1324 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_historical_data.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1314 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_historical_data_api.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1458 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_ichimoku_kinko_hyo_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     4422 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_index_api.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1356 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_insider_transaction.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1406 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_insider_transaction_filing.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1431 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_insider_transaction_filings_api.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1372 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_institutional_holding.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1388 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_institutional_ownership.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1358 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_intraday_stock_price.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1440 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_keltner_channel_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1434 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_know_sure_thing_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1400 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_mass_index_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1442 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_money_flow_index_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1604 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_moving_average_convergence_divergence_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1306 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_municipality.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1648 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_municipality_api.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1380 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_municipality_financial.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1482 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_negative_volume_index_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1484 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_on_balance_volume_mean_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1450 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_on_balance_volume_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1258 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_option.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1300 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_option_chain.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1326 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_option_chain_eod.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1366 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_option_chain_realtime.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1366 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_option_contracts_list.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1284 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_option_eod.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1382 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_option_factors_realtime.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1324 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_option_interval.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1366 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_option_interval_mover.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1432 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_option_intervals_movers_result.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1382 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_option_intervals_result.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1300 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_option_price.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1408 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_option_price_batch_realtime.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1326 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_option_price_eod.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1366 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_option_price_realtime.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1324 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_option_realtime.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1366 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_option_snapshot_group.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1382 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_option_snapshots_result.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1366 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_option_stats_realtime.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1358 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_option_unusual_trade.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     5109 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_options_api.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1250 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_owner.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1308 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_owner_summary.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1918 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_owners_api.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1358 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_realtime_stock_price.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1424 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_realtime_stock_price_security.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1498 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_relative_strength_index_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1348 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_reported_financial.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1422 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_reported_financial_dimension.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1300 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_reported_tag.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1274 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_security.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)    10454 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_security_api.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1382 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_security_interval_mover.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1448 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_security_intervals_movers_result.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1408 2023-08-01 16:57:17.000000 intrinio-sdk-6.25.0/test/test_security_replay_file_result.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1374 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_security_screen_clause.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1366 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_security_screen_group.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1374 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_security_screen_result.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1408 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_security_screen_result_data.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1382 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_security_snapshot_group.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1398 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_security_snapshots_result.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1332 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_security_summary.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1324 2023-08-01 16:57:17.000000 intrinio-sdk-6.25.0/test/test_security_trades.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1374 2023-08-01 16:57:17.000000 intrinio-sdk-6.25.0/test/test_security_trades_result.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1276 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_sic_index.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1482 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_simple_moving_average_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1380 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_standardized_financial.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1462 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_standardized_financials_dimension.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1488 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_stochastic_oscillator_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1316 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_stock_exchange.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     2236 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_stock_exchange_api.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1342 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_stock_market_index.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1400 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_stock_market_index_summary.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1292 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_stock_price.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1374 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_stock_price_adjustment.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1432 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_stock_price_adjustment_summary.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1358 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_stock_price_interval.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1350 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_stock_price_summary.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     6812 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_technical_api.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1356 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_technical_indicator.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1342 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_thea_entity_answer.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1358 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_thea_source_document.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1522 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_triple_exponential_average_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1466 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_true_strength_index_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1472 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_ultimate_oscillator_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1458 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_volume_price_trend_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1466 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_volume_weighted_average_price_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1448 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_vortex_indicator_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1400 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_williams_r_technical_value.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1358 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_zacks_analyst_rating.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1424 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_zacks_analyst_rating_snapshot.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1416 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_zacks_analyst_rating_summary.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     3094 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_zacks_api.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1342 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_zacks_eps_estimate.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1360 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_zacks_eps_growth_rate.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1342 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_zacks_eps_surprise.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1400 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_zacks_eps_surprise_summary.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1334 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_zacks_etf_holding.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1414 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_zacks_institutional_holding.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1522 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_zacks_institutional_holding_company_detail.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1530 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_zacks_institutional_holding_company_summary.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1554 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_zacks_institutional_holding_historical_summary.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1506 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_zacks_institutional_holding_owner_detail.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1514 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_zacks_institutional_holding_owner_summary.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1402 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_zacks_long_term_growth_rate.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1358 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_zacks_sales_surprise.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1416 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_zacks_sales_surprise_summary.py
+-rw-r--r--   0 redbeard  (1000) redbeard  (1000)     1416 2023-08-01 16:57:13.000000 intrinio-sdk-6.25.0/test/test_zacks_target_price_consensus.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/configuration.py` & `intrinio-sdk-6.25.0/intrinio_sdk/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
@@ -241,10 +241,10 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 2.43.6\n"\
-               "SDK Package Version: 6.24.1".\
+               "Version of the API: 2.45.0\n"\
+               "SDK Package Version: 6.25.0".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/rest.py` & `intrinio-sdk-6.25.0/intrinio_sdk/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/__init__.py` & `intrinio-sdk-6.25.0/intrinio_sdk/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # flake8: noqa
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/zacks_target_price_consensus.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/zacks_target_price_consensus.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_zacks_sales_surprises.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_zacks_sales_surprises.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/detrended_price_oscillator_technical_value.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/detrended_price_oscillator_technical_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/zacks_sales_surprise_summary.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/zacks_sales_surprise_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_options.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_municipalities.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_municipalities.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_williams_r.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_williams_r.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/forex_currency.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/forex_currency.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/zacks_institutional_holding_company_detail.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/zacks_institutional_holding_company_detail.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_vortex_indicator.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_vortex_indicator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_awesome_oscillator.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_awesome_oscillator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_securities_search.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_securities_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_company_filings.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_company_filings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_filing_notes.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_filing_notes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/williams_r_technical_value.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/williams_r_technical_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_options_stats_realtime.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_options_stats_realtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/security_summary.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/security_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/stock_price_adjustment.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/stock_price_adjustment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_options_prices_batch_realtime.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_options_prices_batch_realtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_options_chain.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_options_chain.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_standardized_financials.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_standardized_financials.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/stock_market_index_summary.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/stock_market_index_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_sic_index_historical_data.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_sic_index_historical_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_company_news.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_company_news.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/option_unusual_trade.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/option_unusual_trade.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_data_tags_search.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_data_tags_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/institutional_holding.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/institutional_holding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_company_recognize.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_company_recognize.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_economic_indices_search.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_economic_indices_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/zacks_analyst_rating_summary.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/zacks_analyst_rating_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/etf_stats.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/etf_stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/standardized_financials_dimension.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/standardized_financials_dimension.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/zacks_long_term_growth_rate.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/zacks_long_term_growth_rate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_company_securities.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_company_securities.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/company.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/company.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_zacks_eps_growth_rates.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_zacks_eps_growth_rates.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/company_news.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/company_news.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/etf_analytics.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/etf_analytics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/reported_financial.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/reported_financial.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/municipality.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/municipality.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/company_filing.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/company_filing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/company_shares_outstanding.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/company_shares_outstanding.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_zacks_analyst_ratings.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_zacks_analyst_ratings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_filing_notes_search.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_filing_notes_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/force_index_technical_value.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/force_index_technical_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_economic_index_historical_data.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_economic_index_historical_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/commodity_channel_index_technical_value.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/commodity_channel_index_technical_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_company_answers.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_company_answers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_zacks_eps_surprises.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_zacks_eps_surprises.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_company_historical_data.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_company_historical_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/option_interval_mover.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/option_interval_mover.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/moving_average_convergence_divergence_technical_value.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/moving_average_convergence_divergence_technical_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_forex_prices.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_forex_prices.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_options_chain_realtime.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_options_chain_realtime.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/zacks_institutional_holding_owner_summary.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/zacks_institutional_holding_owner_summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/option.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/option.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/stock_price_summary.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/stock_price_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/filing_summary.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/filing_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/forex_price.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/forex_price.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_volume_weighted_average_price.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_volume_weighted_average_price.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/zacks_analyst_rating_snapshot.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/zacks_analyst_rating_snapshot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_ichimoku_kinko_hyo.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_ichimoku_kinko_hyo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/volume_weighted_average_price_value.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/volume_weighted_average_price_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/option_chain_eod.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/option_chain_eod.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/bulk_download_links.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/bulk_download_links.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_volume_price_trend.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_volume_price_trend.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/security_trades.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/security_trades.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/etf_holding.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/etf_holding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/simple_moving_average_technical_value.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/simple_moving_average_technical_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_options_unusual_activity.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_options_unusual_activity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/zacks_institutional_holding_company_summary.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/zacks_institutional_holding_company_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_stock_exchange_securities.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_stock_exchange_securities.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_stock_exchange_stock_price_adjustments.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_stock_exchange_stock_price_adjustments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_keltner_channel.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_keltner_channel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_stock_prices.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_stock_prices.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_stochastic_oscillator.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_stochastic_oscillator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/ichimoku_kinko_hyo_technical_value.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/ichimoku_kinko_hyo_technical_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_stock_market_index_historical_data.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_stock_market_index_historical_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/company_initial_public_offering.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/company_initial_public_offering.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/esg_company_summary.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/esg_company_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/etf.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/etf.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 000001d0: 5d28 6874 7470 733a 2f2f 696e 7472 696e  ](https://intrin
 000001e0: 696f 2e63 6f6d 2920 616e 6420 636c 6963  io.com) and clic
 000001f0: 6b20 6f6e 2074 6865 2063 6861 7420 6963  k on the chat ic
 00000200: 6f6e 2069 6e20 7468 6520 6c6f 7765 7220  on in the lower 
 00000210: 7269 6768 7420 636f 726e 6572 2e20 2023  right corner.  #
 00000220: 206e 6f71 613a 2045 3530 310a 0a20 2020   noqa: E501..   
 00000230: 204f 7065 6e41 5049 2073 7065 6320 7665   OpenAPI spec ve
-00000240: 7273 696f 6e3a 2032 2e34 332e 360a 2020  rsion: 2.43.6.  
+00000240: 7273 696f 6e3a 2032 2e34 352e 300a 2020  rsion: 2.45.0.  
 00000250: 2020 0a20 2020 2047 656e 6572 6174 6564    .    Generated
 00000260: 2062 793a 2068 7474 7073 3a2f 2f67 6974   by: https://git
 00000270: 6875 622e 636f 6d2f 7377 6167 6765 722d  hub.com/swagger-
 00000280: 6170 692f 7377 6167 6765 722d 636f 6465  api/swagger-code
 00000290: 6765 6e2e 6769 740a 2222 220a 0a0a 696d  gen.git."""...im
 000002a0: 706f 7274 2070 7072 696e 740a 696d 706f  port pprint.impo
 000002b0: 7274 2072 6520 2023 206e 6f71 613a 2046  rt re  # noqa: F
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_average_directional_index.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_average_directional_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_ease_of_movement.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_ease_of_movement.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/stock_price.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/stock_price.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/owner_summary.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/owner_summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/zacks_etf_holding.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/zacks_etf_holding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/keltner_channel_technical_value.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/keltner_channel_technical_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/vortex_indicator_technical_value.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/vortex_indicator_technical_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/security_interval_mover.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/security_interval_mover.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/intraday_stock_price.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/intraday_stock_price.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/stock_price_interval.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/stock_price_interval.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/option_stats_realtime.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/option_stats_realtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/security.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/security.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_zacks_etf_holdings.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_zacks_etf_holdings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/filing.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/filing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/true_strength_index_technical_value.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/true_strength_index_technical_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/dividend_record.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/dividend_record.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/average_daily_trading_volume_technical_value.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/average_daily_trading_volume_technical_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/zacks_analyst_rating.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/zacks_analyst_rating.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_companies.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_companies.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/option_chain.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/option_chain.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/security_intervals_movers_result.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/security_intervals_movers_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/zacks_institutional_holding_historical_summary.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/zacks_institutional_holding_historical_summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_zacks_institutional_holding_owners.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_zacks_institutional_holding_owners.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_companies_search.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_companies_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/security_screen_clause.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/security_screen_clause.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/security_screen_result_data.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/security_screen_result_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/awesome_oscillator_technical_value.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/awesome_oscillator_technical_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/option_realtime.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/option_realtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/filing_note.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/filing_note.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/__init__.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/accumulation_distribution_index_technical_value.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/accumulation_distribution_index_technical_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_news.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_news.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_ultimate_oscillator.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_ultimate_oscillator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/option_contracts_list.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/option_contracts_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/economic_index_summary.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/economic_index_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/option_interval.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/option_interval.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_relative_strength_index.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_relative_strength_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_esg_companies.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_esg_companies.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/technical_indicator.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/technical_indicator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/option_chain_realtime.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/option_chain_realtime.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/esg_rating_with_company.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/esg_rating_with_company.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/owner.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/owner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/historical_data.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/historical_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_insider_transaction_filings.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_insider_transaction_filings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_average_true_range.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_average_true_range.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_esg_company_comprehensive_rating_history.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_esg_company_comprehensive_rating_history.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/esg_comprehensive_rating.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/esg_comprehensive_rating.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/zacks_eps_surprise.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/zacks_eps_surprise.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_zacks_eps_surprises.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_zacks_eps_surprises.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_options_tickers.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_options_tickers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/filing_note_filing.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/filing_note_filing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/standardized_financial.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/standardized_financial.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_company_insider_transaction_filings.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_company_insider_transaction_filings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/esg_rating.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/esg_rating.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_reported_financials.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_reported_financials.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_chaikin_money_flow.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_chaikin_money_flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/zacks_eps_estimate.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/zacks_eps_estimate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/option_price_batch_realtime.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/option_price_batch_realtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_municipalitiy_financials.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_municipalitiy_financials.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/option_factors_realtime.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/option_factors_realtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/on_balance_volume_mean_technical_value.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/on_balance_volume_mean_technical_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_detrended_price_oscillator.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_detrended_price_oscillator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/thea_entity_answer.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/thea_entity_answer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_securities.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_securities.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/data_tag.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/data_tag.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_data_tags.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_data_tags.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/etf_summary.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/etf_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_historical_data.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_historical_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_etf_holdings.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_etf_holdings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/money_flow_index_technical_value.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/money_flow_index_technical_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_interval_prices.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_interval_prices.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_accumulation_distribution_index.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_accumulation_distribution_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/zacks_eps_growth_rate.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/zacks_eps_growth_rate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_stock_price_adjustments.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_stock_price_adjustments.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_filing_answers.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_filing_answers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_options_prices_eod.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_options_prices_eod.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/stock_market_index.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/stock_market_index.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/on_balance_volume_technical_value.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/on_balance_volume_technical_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/insider_transaction.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/insider_transaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/relative_strength_index_technical_value.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/relative_strength_index_technical_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/option_price_eod.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/option_price_eod.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_intraday_prices.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_intraday_prices.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
@@ -226,15 +226,15 @@
         """Sets the source of this ApiResponseSecurityIntradayPrices.
 
         The source of the data  # noqa: E501
 
         :param source: The source of this ApiResponseSecurityIntradayPrices.  # noqa: E501
         :type: str
         """
-        allowed_values = ["iex", "bats"]  # noqa: E501
+        allowed_values = ["realtime", "delayed", "nasdaq_basic"]  # noqa: E501
         if source not in allowed_values:
             raise ValueError(
                 "Invalid value for `source` ({0}), must be one of {1}"  # noqa: E501
                 .format(source, allowed_values)
             )
 
         self._source = source
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/zacks_institutional_holding.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/zacks_institutional_holding.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_et_fs.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_et_fs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_zacks_institutional_holding_companies.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_zacks_institutional_holding_companies.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/volume_price_trend_technical_value.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/volume_price_trend_technical_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/esg_comprehensive_rating_with_company.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/esg_comprehensive_rating_with_company.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_stock_exchanges.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_stock_exchanges.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/zacks_institutional_holding_owner_detail.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/zacks_institutional_holding_owner_detail.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/security_screen_group.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/security_screen_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_money_flow_index.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_money_flow_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_forex_currencies.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_forex_currencies.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_forex_pairs.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_forex_pairs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_know_sure_thing.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_know_sure_thing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_esg_latest_comprehensive.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_esg_latest_comprehensive.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_commodity_channel_index.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_commodity_channel_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/insider_transaction_filing.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/insider_transaction_filing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_zacks_sales_surprises.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_zacks_sales_surprises.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/security_snapshot_group.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/security_snapshot_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_institutional_ownership.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_institutional_ownership.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_owners.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_owners.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/donchian_channel_technical_value.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/donchian_channel_technical_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_simple_moving_average.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_simple_moving_average.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_stock_market_indices_search.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_stock_market_indices_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_filing_fundamentals.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_filing_fundamentals.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_stock_exchange_stock_prices.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_stock_exchange_stock_prices.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/forex_pair.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/forex_pair.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/security_replay_file_result.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/security_replay_file_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_esg_company_rating_history.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_esg_company_rating_history.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_zacks_target_price_consensuses.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_zacks_target_price_consensuses.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/average_true_range_technical_value.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/average_true_range_technical_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_bollinger_bands.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_bollinger_bands.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_initial_public_offerings.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_initial_public_offerings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_sic_indices_search.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_sic_indices_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/security_trades_result.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/security_trades_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_options_expirations.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_options_expirations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/security_screen_result.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/security_screen_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/know_sure_thing_technical_value.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/know_sure_thing_technical_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/chaikin_money_flow_technical_value.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/chaikin_money_flow_technical_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_historical_data.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_historical_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_economic_indices.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_economic_indices.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/zacks_eps_surprise_summary.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/zacks_eps_surprise_summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_on_balance_volume.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_on_balance_volume.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_zacks_analyst_ratings.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_zacks_analyst_ratings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_stock_exchange_realtime_stock_prices.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_stock_exchange_realtime_stock_prices.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/ease_of_movement_technical_value.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/ease_of_movement_technical_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/bulk_download_summary.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/bulk_download_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_force_index.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_force_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_zacks_institutional_holdings.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_zacks_institutional_holdings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_stock_market_indices.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_stock_market_indices.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_esg_latest.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_esg_latest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/realtime_stock_price_security.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/realtime_stock_price_security.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_options_price_realtime.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_options_price_realtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_owner_insider_transaction_filings.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_owner_insider_transaction_filings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_filings.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_filings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/negative_volume_index_technical_value.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/negative_volume_index_technical_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/sic_index.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/sic_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/security_snapshots_result.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/security_snapshots_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/institutional_ownership.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/institutional_ownership.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/data_tag_summary.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/data_tag_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/company_news_summary.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/company_news_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/option_intervals_movers_result.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/option_intervals_movers_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_donchian_channel.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_donchian_channel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_bulk_download_links.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_bulk_download_links.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_option_prices.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_option_prices.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/option_price.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/option_price.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_standardized_financials_dimensions.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_standardized_financials_dimensions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_zacks_eps_estimates.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_zacks_eps_estimates.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_options_realtime.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_options_realtime.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/company_summary.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/company_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_options_chain_eod.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_options_chain_eod.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_moving_average_convergence_divergence.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_moving_average_convergence_divergence.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/realtime_stock_price.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/realtime_stock_price.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_company_fundamentals.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_company_fundamentals.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/average_directional_index_technical_value.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/average_directional_index_technical_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/stock_exchange.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/stock_exchange.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_sic_indices.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_sic_indices.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/fundamental.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/fundamental.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/economic_index.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/economic_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_negative_volume_index.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_negative_volume_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/filing_note_summary.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/filing_note_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/option_price_realtime.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/option_price_realtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/mass_index_technical_value.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/mass_index_technical_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/option_eod.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/option_eod.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_true_strength_index.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_true_strength_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/ultimate_oscillator_technical_value.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/ultimate_oscillator_technical_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_owner_institutional_holdings.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_owner_institutional_holdings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_zacks_analyst_ratings_snapshot.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_zacks_analyst_ratings_snapshot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/zacks_sales_surprise.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/zacks_sales_surprise.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/option_snapshots_result.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/option_snapshots_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/option_intervals_result.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/option_intervals_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/fundamental_summary.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/fundamental_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/reported_tag.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/reported_tag.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_triple_exponential_average.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_triple_exponential_average.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_zacks_long_term_growth_rates.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_zacks_long_term_growth_rates.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/bollinger_bands_technical_value.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/bollinger_bands_technical_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/reported_financial_dimension.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/reported_financial_dimension.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/thea_source_document.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/thea_source_document.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/stock_price_adjustment_summary.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/stock_price_adjustment_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/municipality_financial.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/municipality_financial.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_mass_index.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_mass_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_on_balance_volume_mean.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_on_balance_volume_mean.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_company_shares_outstanding.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_company_shares_outstanding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/stochastic_oscillator_technical_value.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/stochastic_oscillator_technical_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/earnings_record.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/earnings_record.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/option_snapshot_group.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/option_snapshot_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/triple_exponential_average_technical_value.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/triple_exponential_average_technical_value.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/models/api_response_security_average_daily_trading_volume.py` & `intrinio-sdk-6.25.0/intrinio_sdk/models/api_response_security_average_daily_trading_volume.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/api/data_point_api.py` & `intrinio-sdk-6.25.0/intrinio_sdk/api/data_point_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/api/index_api.py` & `intrinio-sdk-6.25.0/intrinio_sdk/api/index_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/api/owners_api.py` & `intrinio-sdk-6.25.0/intrinio_sdk/api/owners_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/api/et_fs_api.py` & `intrinio-sdk-6.25.0/intrinio_sdk/api/et_fs_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/api/company_api.py` & `intrinio-sdk-6.25.0/intrinio_sdk/api/company_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/api/municipality_api.py` & `intrinio-sdk-6.25.0/intrinio_sdk/api/municipality_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/api/__init__.py` & `intrinio-sdk-6.25.0/intrinio_sdk/api/__init__.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/api/security_api.py` & `intrinio-sdk-6.25.0/intrinio_sdk/api/security_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 000001d0: 5d28 6874 7470 733a 2f2f 696e 7472 696e  ](https://intrin
 000001e0: 696f 2e63 6f6d 2920 616e 6420 636c 6963  io.com) and clic
 000001f0: 6b20 6f6e 2074 6865 2063 6861 7420 6963  k on the chat ic
 00000200: 6f6e 2069 6e20 7468 6520 6c6f 7765 7220  on in the lower 
 00000210: 7269 6768 7420 636f 726e 6572 2e20 2023  right corner.  #
 00000220: 206e 6f71 613a 2045 3530 310a 0a20 2020   noqa: E501..   
 00000230: 204f 7065 6e41 5049 2073 7065 6320 7665   OpenAPI spec ve
-00000240: 7273 696f 6e3a 2032 2e34 332e 360a 2020  rsion: 2.43.6.  
+00000240: 7273 696f 6e3a 2032 2e34 352e 300a 2020  rsion: 2.45.0.  
 00000250: 2020 0a20 2020 2047 656e 6572 6174 6564    .    Generated
 00000260: 2062 793a 2068 7474 7073 3a2f 2f67 6974   by: https://git
 00000270: 6875 622e 636f 6d2f 7377 6167 6765 722d  hub.com/swagger-
 00000280: 6170 692f 7377 6167 6765 722d 636f 6465  api/swagger-code
 00000290: 6765 6e2e 6769 740a 2222 220a 0a0a 6672  gen.git."""...fr
 000002a0: 6f6d 205f 5f66 7574 7572 655f 5f20 696d  om __future__ im
 000002b0: 706f 7274 2061 6273 6f6c 7574 655f 696d  port absolute_im
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/api/technical_api.py` & `intrinio-sdk-6.25.0/intrinio_sdk/api/technical_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/api/options_api.py` & `intrinio-sdk-6.25.0/intrinio_sdk/api/options_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
@@ -235,14 +235,16 @@
         asynchronous HTTP request, please pass async=True
         >>> thread = api.get_option_strikes_realtime(symbol, strike, _async=True)
         >>> result = thread.get()
 
         :param async bool
         :param str symbol: The option symbol, corresponding to the underlying security. (required)
         :param float strike: The strike price of the option contract. This will return options contracts with strike price equal to this price. (required)
+        :param str stock_price_source: Source for underlying price for calculating Greeks.
+        :param str model: Model for calculating Greek values. Default is black_scholes.
         :return: ApiResponseOptionsChainRealtime
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async'):
             return self.get_option_strikes_realtime_with_http_info(symbol, strike, **kwargs)  # noqa: E501
@@ -258,20 +260,22 @@
         asynchronous HTTP request, please pass async=True
         >>> thread = api.get_option_strikes_realtime_with_http_info(symbol, strike, _async=True)
         >>> result = thread.get()
 
         :param async bool
         :param str symbol: The option symbol, corresponding to the underlying security. (required)
         :param float strike: The strike price of the option contract. This will return options contracts with strike price equal to this price. (required)
+        :param str stock_price_source: Source for underlying price for calculating Greeks.
+        :param str model: Model for calculating Greek values. Default is black_scholes.
         :return: ApiResponseOptionsChainRealtime
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['symbol', 'strike']  # noqa: E501
+        all_params = ['symbol', 'strike', 'stock_price_source', 'model']  # noqa: E501
         all_params.append('async')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -296,14 +300,18 @@
         path_params = {}
         if 'symbol' in params:
             path_params['symbol'] = params['symbol']  # noqa: E501
         if 'strike' in params:
             path_params['strike'] = params['strike']  # noqa: E501
 
         query_params = []
+        if 'stock_price_source' in params:
+            query_params.append(('stock_price_source', params['stock_price_source']))  # noqa: E501
+        if 'model' in params:
+            query_params.append(('model', params['model']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -864,14 +872,16 @@
         :param float strike_greater_than: The strike price of the option contract. This will return options contracts with strike prices greater than this price.
         :param float strike_less_than: The strike price of the option contract. This will return options contracts with strike prices less than this price.
         :param float volume_greater_than: The volume of the option contract. This will return options contracts with volumes greater than this amount.
         :param float volume_less_than: The volume of the option contract. This will return options contracts with volumes less than this amout.
         :param float open_interest_greater_than: The open interest of the option contract. This will return options contracts with open interest greater than this amount.
         :param float open_interest_less_than: The open interest of the option contract. This will return options contracts with open interest less than this amount.
         :param str moneyness: The moneyness of the options contracts to return. 'all' will return all options contracts. 'in_the_money' will return options contracts that are in the money (call options with strike prices below the current price, put options with strike prices above the current price). 'out_of_they_money' will return options contracts that are out of the money (call options with strike prices above the current price, put options with strike prices below the current price). 'near_the_money' will return options contracts that are $0.50 or less away from being in the money.  Requires subscription to realtime stock price data.
+        :param str stock_price_source: Source for underlying price for calculating Greeks.
+        :param str model: Model for calculating Greek values. Default is black_scholes.
         :return: ApiResponseOptionsChainRealtime
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async'):
             return self.get_options_chain_realtime_with_http_info(symbol, expiration, **kwargs)  # noqa: E501
@@ -897,20 +907,22 @@
         :param float strike_greater_than: The strike price of the option contract. This will return options contracts with strike prices greater than this price.
         :param float strike_less_than: The strike price of the option contract. This will return options contracts with strike prices less than this price.
         :param float volume_greater_than: The volume of the option contract. This will return options contracts with volumes greater than this amount.
         :param float volume_less_than: The volume of the option contract. This will return options contracts with volumes less than this amout.
         :param float open_interest_greater_than: The open interest of the option contract. This will return options contracts with open interest greater than this amount.
         :param float open_interest_less_than: The open interest of the option contract. This will return options contracts with open interest less than this amount.
         :param str moneyness: The moneyness of the options contracts to return. 'all' will return all options contracts. 'in_the_money' will return options contracts that are in the money (call options with strike prices below the current price, put options with strike prices above the current price). 'out_of_they_money' will return options contracts that are out of the money (call options with strike prices above the current price, put options with strike prices below the current price). 'near_the_money' will return options contracts that are $0.50 or less away from being in the money.  Requires subscription to realtime stock price data.
+        :param str stock_price_source: Source for underlying price for calculating Greeks.
+        :param str model: Model for calculating Greek values. Default is black_scholes.
         :return: ApiResponseOptionsChainRealtime
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['symbol', 'expiration', 'source', 'type', 'strike', 'strike_greater_than', 'strike_less_than', 'volume_greater_than', 'volume_less_than', 'open_interest_greater_than', 'open_interest_less_than', 'moneyness']  # noqa: E501
+        all_params = ['symbol', 'expiration', 'source', 'type', 'strike', 'strike_greater_than', 'strike_less_than', 'volume_greater_than', 'volume_less_than', 'open_interest_greater_than', 'open_interest_less_than', 'moneyness', 'stock_price_source', 'model']  # noqa: E501
         all_params.append('async')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -955,14 +967,18 @@
             query_params.append(('volume_less_than', params['volume_less_than']))  # noqa: E501
         if 'open_interest_greater_than' in params:
             query_params.append(('open_interest_greater_than', params['open_interest_greater_than']))  # noqa: E501
         if 'open_interest_less_than' in params:
             query_params.append(('open_interest_less_than', params['open_interest_less_than']))  # noqa: E501
         if 'moneyness' in params:
             query_params.append(('moneyness', params['moneyness']))  # noqa: E501
+        if 'stock_price_source' in params:
+            query_params.append(('stock_price_source', params['stock_price_source']))  # noqa: E501
+        if 'model' in params:
+            query_params.append(('model', params['model']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -1718,14 +1734,16 @@
         asynchronous HTTP request, please pass async=True
         >>> thread = api.get_options_prices_batch_realtime(body, _async=True)
         >>> result = thread.get()
 
         :param async bool
         :param OptionContractsList body: The contract symbols for which to return options prices for. (required)
         :param str source: Realtime or 15-minute delayed contracts.
+        :param str stock_price_source: Source for underlying price for calculating Greeks.
+        :param str model: Model for calculating Greek values. Default is black_scholes.
         :return: ApiResponseOptionsPricesBatchRealtime
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async'):
             return self.get_options_prices_batch_realtime_with_http_info(body, **kwargs)  # noqa: E501
@@ -1741,20 +1759,22 @@
         asynchronous HTTP request, please pass async=True
         >>> thread = api.get_options_prices_batch_realtime_with_http_info(body, _async=True)
         >>> result = thread.get()
 
         :param async bool
         :param OptionContractsList body: The contract symbols for which to return options prices for. (required)
         :param str source: Realtime or 15-minute delayed contracts.
+        :param str stock_price_source: Source for underlying price for calculating Greeks.
+        :param str model: Model for calculating Greek values. Default is black_scholes.
         :return: ApiResponseOptionsPricesBatchRealtime
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['body', 'source']  # noqa: E501
+        all_params = ['body', 'source', 'stock_price_source', 'model']  # noqa: E501
         all_params.append('async')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -1773,14 +1793,18 @@
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
         if 'source' in params:
             query_params.append(('source', params['source']))  # noqa: E501
+        if 'stock_price_source' in params:
+            query_params.append(('stock_price_source', params['stock_price_source']))  # noqa: E501
+        if 'model' in params:
+            query_params.append(('model', params['model']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -1916,14 +1940,16 @@
         asynchronous HTTP request, please pass async=True
         >>> thread = api.get_options_prices_realtime(identifier, _async=True)
         >>> result = thread.get()
 
         :param async bool
         :param str identifier: The Intrinio ID or code of the options contract to request prices for. (required)
         :param str source: Realtime or 15-minute delayed contracts.
+        :param str stock_price_source: Source for underlying price for calculating Greeks.
+        :param str model: Model for calculating Greek values. Default is black_scholes.
         :return: ApiResponseOptionsPriceRealtime
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async'):
             return self.get_options_prices_realtime_with_http_info(identifier, **kwargs)  # noqa: E501
@@ -1939,20 +1965,22 @@
         asynchronous HTTP request, please pass async=True
         >>> thread = api.get_options_prices_realtime_with_http_info(identifier, _async=True)
         >>> result = thread.get()
 
         :param async bool
         :param str identifier: The Intrinio ID or code of the options contract to request prices for. (required)
         :param str source: Realtime or 15-minute delayed contracts.
+        :param str stock_price_source: Source for underlying price for calculating Greeks.
+        :param str model: Model for calculating Greek values. Default is black_scholes.
         :return: ApiResponseOptionsPriceRealtime
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['identifier', 'source']  # noqa: E501
+        all_params = ['identifier', 'source', 'stock_price_source', 'model']  # noqa: E501
         all_params.append('async')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -1973,14 +2001,18 @@
         path_params = {}
         if 'identifier' in params:
             path_params['identifier'] = params['identifier']  # noqa: E501
 
         query_params = []
         if 'source' in params:
             query_params.append(('source', params['source']))  # noqa: E501
+        if 'stock_price_source' in params:
+            query_params.append(('stock_price_source', params['stock_price_source']))  # noqa: E501
+        if 'model' in params:
+            query_params.append(('model', params['model']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/api/insider_transaction_filings_api.py` & `intrinio-sdk-6.25.0/intrinio_sdk/api/insider_transaction_filings_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/api/historical_data_api.py` & `intrinio-sdk-6.25.0/intrinio_sdk/api/historical_data_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/api/fundamentals_api.py` & `intrinio-sdk-6.25.0/intrinio_sdk/api/fundamentals_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/api/stock_exchange_api.py` & `intrinio-sdk-6.25.0/intrinio_sdk/api/stock_exchange_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/api/filing_api.py` & `intrinio-sdk-6.25.0/intrinio_sdk/api/filing_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/api/data_tag_api.py` & `intrinio-sdk-6.25.0/intrinio_sdk/api/data_tag_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/api/forex_api.py` & `intrinio-sdk-6.25.0/intrinio_sdk/api/forex_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/api/zacks_api.py` & `intrinio-sdk-6.25.0/intrinio_sdk/api/zacks_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/api/bulk_downloads_api.py` & `intrinio-sdk-6.25.0/intrinio_sdk/api/bulk_downloads_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/api/esg_api.py` & `intrinio-sdk-6.25.0/intrinio_sdk/api/esg_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk/api_client.py` & `intrinio-sdk-6.25.0/intrinio_sdk/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import datetime
@@ -72,15 +72,15 @@
         self.pool = ThreadPool()
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Swagger-Codegen/6.24.1/python'
+        self.user_agent = 'Swagger-Codegen/6.25.0/python'
 
     def __del__(self):
         self.pool.close()
         self.pool.join()
 
     @property
     def user_agent(self):
```

### Comparing `intrinio-sdk-6.24.1/PKG-INFO` & `intrinio-sdk-6.25.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: intrinio-sdk
-Version: 6.24.1
+Version: 6.25.0
 Summary: Intrinio API
 Home-page: https://github.com/intrinio/python-sdk
-Author: UNKNOWN
-Author-email: UNKNOWN
-License: UNKNOWN
-Description:     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
-            
+Author-email: 
 Keywords: Swagger,Intrinio API
-Platform: UNKNOWN
+
+    Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
+
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk.egg-info/PKG-INFO` & `intrinio-sdk-6.25.0/intrinio_sdk.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: intrinio-sdk
-Version: 6.24.1
+Version: 6.25.0
 Summary: Intrinio API
 Home-page: https://github.com/intrinio/python-sdk
-Author: UNKNOWN
-Author-email: UNKNOWN
-License: UNKNOWN
-Description:     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
-            
+Author-email: 
 Keywords: Swagger,Intrinio API
-Platform: UNKNOWN
+
+    Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
+
```

### Comparing `intrinio-sdk-6.24.1/intrinio_sdk.egg-info/SOURCES.txt` & `intrinio-sdk-6.25.0/intrinio_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_etf_holding.py` & `intrinio-sdk-6.25.0/test/test_etf_holding.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_security_commodity_channel_index.py` & `intrinio-sdk-6.25.0/test/test_api_response_security_commodity_channel_index.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_security_ichimoku_kinko_hyo.py` & `intrinio-sdk-6.25.0/test/test_api_response_security_ichimoku_kinko_hyo.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_zacks_analyst_ratings.py` & `intrinio-sdk-6.25.0/test/test_api_response_zacks_analyst_ratings.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_security_institutional_ownership.py` & `intrinio-sdk-6.25.0/test/test_api_response_security_institutional_ownership.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_company_securities.py` & `intrinio-sdk-6.25.0/test/test_api_response_company_securities.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_option_price.py` & `intrinio-sdk-6.25.0/test/test_option_price.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_sic_index.py` & `intrinio-sdk-6.25.0/test/test_sic_index.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_stock_exchange_stock_price_adjustments.py` & `intrinio-sdk-6.25.0/test/test_api_response_stock_exchange_stock_price_adjustments.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_etf.py` & `intrinio-sdk-6.25.0/test/test_etf.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_filing_notes_search.py` & `intrinio-sdk-6.25.0/test/test_api_response_filing_notes_search.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_option_factors_realtime.py` & `intrinio-sdk-6.25.0/test/test_option_factors_realtime.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_zacks_eps_growth_rates.py` & `intrinio-sdk-6.25.0/test/test_api_response_zacks_eps_growth_rates.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_data_tag_summary.py` & `intrinio-sdk-6.25.0/test/test_data_tag_summary.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_options_chain_eod.py` & `intrinio-sdk-6.25.0/test/test_api_response_options_chain_eod.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_company.py` & `intrinio-sdk-6.25.0/test/test_company.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_zacks_eps_surprises.py` & `intrinio-sdk-6.25.0/test/test_api_response_zacks_eps_surprises.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_options_chain_realtime.py` & `intrinio-sdk-6.25.0/test/test_api_response_options_chain_realtime.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_forex_currencies.py` & `intrinio-sdk-6.25.0/test/test_api_response_forex_currencies.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_esg_company_summary.py` & `intrinio-sdk-6.25.0/test/test_esg_company_summary.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_sic_indices.py` & `intrinio-sdk-6.25.0/test/test_api_response_sic_indices.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_mass_index_technical_value.py` & `intrinio-sdk-6.25.0/test/test_mass_index_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_stock_price.py` & `intrinio-sdk-6.25.0/test/test_stock_price.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_security.py` & `intrinio-sdk-6.25.0/test/test_security.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_security_stock_price_adjustments.py` & `intrinio-sdk-6.25.0/test/test_api_response_security_stock_price_adjustments.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_bulk_download_links.py` & `intrinio-sdk-6.25.0/test/test_bulk_download_links.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_etf_analytics.py` & `intrinio-sdk-6.25.0/test/test_etf_analytics.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_esg_rating_with_company.py` & `intrinio-sdk-6.25.0/test/test_esg_rating_with_company.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_volume_weighted_average_price_value.py` & `intrinio-sdk-6.25.0/test/test_volume_weighted_average_price_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_filings.py` & `intrinio-sdk-6.25.0/test/test_api_response_filings.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_security_trades_result.py` & `intrinio-sdk-6.25.0/test/test_security_trades_result.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_option_intervals_movers_result.py` & `intrinio-sdk-6.25.0/test/test_option_intervals_movers_result.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_esg_company_comprehensive_rating_history.py` & `intrinio-sdk-6.25.0/test/test_api_response_esg_company_comprehensive_rating_history.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_security_screen_result.py` & `intrinio-sdk-6.25.0/test/test_security_screen_result.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_security_interval_mover.py` & `intrinio-sdk-6.25.0/test/test_security_interval_mover.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_company_api.py` & `intrinio-sdk-6.25.0/test/test_company_api.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_option_snapshot_group.py` & `intrinio-sdk-6.25.0/test/test_option_snapshot_group.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_security_screen_result_data.py` & `intrinio-sdk-6.25.0/test/test_security_screen_result_data.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_stochastic_oscillator_technical_value.py` & `intrinio-sdk-6.25.0/test/test_stochastic_oscillator_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_filing_note.py` & `intrinio-sdk-6.25.0/test/test_filing_note.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_sic_index_historical_data.py` & `intrinio-sdk-6.25.0/test/test_api_response_sic_index_historical_data.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_security_williams_r.py` & `intrinio-sdk-6.25.0/test/test_api_response_security_williams_r.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_security_zacks_eps_surprises.py` & `intrinio-sdk-6.25.0/test/test_api_response_security_zacks_eps_surprises.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_stock_price_adjustment_summary.py` & `intrinio-sdk-6.25.0/test/test_stock_price_adjustment_summary.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_options_stats_realtime.py` & `intrinio-sdk-6.25.0/test/test_api_response_options_stats_realtime.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_security_detrended_price_oscillator.py` & `intrinio-sdk-6.25.0/test/test_api_response_security_detrended_price_oscillator.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_reported_tag.py` & `intrinio-sdk-6.25.0/test/test_reported_tag.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_option_prices.py` & `intrinio-sdk-6.25.0/test/test_api_response_option_prices.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_company_insider_transaction_filings.py` & `intrinio-sdk-6.25.0/test/test_api_response_company_insider_transaction_filings.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_security_stochastic_oscillator.py` & `intrinio-sdk-6.25.0/test/test_api_response_security_stochastic_oscillator.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_economic_index.py` & `intrinio-sdk-6.25.0/test/test_economic_index.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_realtime_stock_price_security.py` & `intrinio-sdk-6.25.0/test/test_realtime_stock_price_security.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_option_eod.py` & `intrinio-sdk-6.25.0/test/test_option_eod.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_stock_exchange.py` & `intrinio-sdk-6.25.0/test/test_stock_exchange.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_etf_holdings.py` & `intrinio-sdk-6.25.0/test/test_api_response_etf_holdings.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_technical_indicator.py` & `intrinio-sdk-6.25.0/test/test_technical_indicator.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_bulk_downloads_api.py` & `intrinio-sdk-6.25.0/test/test_bulk_downloads_api.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_data_tags.py` & `intrinio-sdk-6.25.0/test/test_api_response_data_tags.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_reported_financial_dimension.py` & `intrinio-sdk-6.25.0/test/test_reported_financial_dimension.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_security_awesome_oscillator.py` & `intrinio-sdk-6.25.0/test/test_api_response_security_awesome_oscillator.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_zacks_institutional_holding_company_summary.py` & `intrinio-sdk-6.25.0/test/test_zacks_institutional_holding_company_summary.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_economic_indices.py` & `intrinio-sdk-6.25.0/test/test_api_response_economic_indices.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_standardized_financials_dimensions.py` & `intrinio-sdk-6.25.0/test/test_api_response_standardized_financials_dimensions.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_security_ultimate_oscillator.py` & `intrinio-sdk-6.25.0/test/test_api_response_security_ultimate_oscillator.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_option_price_realtime.py` & `intrinio-sdk-6.25.0/test/test_option_price_realtime.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_option_price_batch_realtime.py` & `intrinio-sdk-6.25.0/test/test_option_price_batch_realtime.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_owner_insider_transaction_filings.py` & `intrinio-sdk-6.25.0/test/test_api_response_owner_insider_transaction_filings.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_security_vortex_indicator.py` & `intrinio-sdk-6.25.0/test/test_api_response_security_vortex_indicator.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_security_chaikin_money_flow.py` & `intrinio-sdk-6.25.0/test/test_api_response_security_chaikin_money_flow.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_security_intervals_movers_result.py` & `intrinio-sdk-6.25.0/test/test_security_intervals_movers_result.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_municipalities.py` & `intrinio-sdk-6.25.0/test/test_api_response_municipalities.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_historical_data.py` & `intrinio-sdk-6.25.0/test/test_api_response_historical_data.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_security_screen_group.py` & `intrinio-sdk-6.25.0/test/test_security_screen_group.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_realtime_stock_price.py` & `intrinio-sdk-6.25.0/test/test_realtime_stock_price.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_security_zacks_analyst_ratings_snapshot.py` & `intrinio-sdk-6.25.0/test/test_api_response_security_zacks_analyst_ratings_snapshot.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_security_know_sure_thing.py` & `intrinio-sdk-6.25.0/test/test_api_response_security_know_sure_thing.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_esg_latest_comprehensive.py` & `intrinio-sdk-6.25.0/test/test_api_response_esg_latest_comprehensive.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_insider_transaction_filings.py` & `intrinio-sdk-6.25.0/test/test_api_response_insider_transaction_filings.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_technical_api.py` & `intrinio-sdk-6.25.0/test/test_technical_api.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_security_intraday_prices.py` & `intrinio-sdk-6.25.0/test/test_api_response_security_intraday_prices.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_security_average_true_range.py` & `intrinio-sdk-6.25.0/test/test_api_response_security_average_true_range.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_municipality_financial.py` & `intrinio-sdk-6.25.0/test/test_municipality_financial.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_on_balance_volume_mean_technical_value.py` & `intrinio-sdk-6.25.0/test/test_on_balance_volume_mean_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_zacks_sales_surprise.py` & `intrinio-sdk-6.25.0/test/test_zacks_sales_surprise.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_esg_comprehensive_rating_with_company.py` & `intrinio-sdk-6.25.0/test/test_esg_comprehensive_rating_with_company.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_zacks_eps_surprise_summary.py` & `intrinio-sdk-6.25.0/test/test_zacks_eps_surprise_summary.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_et_fs.py` & `intrinio-sdk-6.25.0/test/test_api_response_et_fs.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_economic_index_historical_data.py` & `intrinio-sdk-6.25.0/test/test_api_response_economic_index_historical_data.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_awesome_oscillator_technical_value.py` & `intrinio-sdk-6.25.0/test/test_awesome_oscillator_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_security_interval_prices.py` & `intrinio-sdk-6.25.0/test/test_api_response_security_interval_prices.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_security_on_balance_volume_mean.py` & `intrinio-sdk-6.25.0/test/test_api_response_security_on_balance_volume_mean.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_options_realtime.py` & `intrinio-sdk-6.25.0/test/test_api_response_options_realtime.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_zacks_eps_growth_rate.py` & `intrinio-sdk-6.25.0/test/test_zacks_eps_growth_rate.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_stock_market_index.py` & `intrinio-sdk-6.25.0/test/test_stock_market_index.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_thea_entity_answer.py` & `intrinio-sdk-6.25.0/test/test_thea_entity_answer.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_stock_exchanges.py` & `intrinio-sdk-6.25.0/test/test_api_response_stock_exchanges.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_standardized_financials_dimension.py` & `intrinio-sdk-6.25.0/test/test_standardized_financials_dimension.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_reported_financials.py` & `intrinio-sdk-6.25.0/test/test_api_response_reported_financials.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_earnings_record.py` & `intrinio-sdk-6.25.0/test/test_earnings_record.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_zacks_api.py` & `intrinio-sdk-6.25.0/test/test_zacks_api.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_option_price_eod.py` & `intrinio-sdk-6.25.0/test/test_option_price_eod.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_thea_source_document.py` & `intrinio-sdk-6.25.0/test/test_thea_source_document.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_moving_average_convergence_divergence_technical_value.py` & `intrinio-sdk-6.25.0/test/test_moving_average_convergence_divergence_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_fundamentals_api.py` & `intrinio-sdk-6.25.0/test/test_fundamentals_api.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_zacks_long_term_growth_rate.py` & `intrinio-sdk-6.25.0/test/test_zacks_long_term_growth_rate.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_owner_summary.py` & `intrinio-sdk-6.25.0/test/test_owner_summary.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_commodity_channel_index_technical_value.py` & `intrinio-sdk-6.25.0/test/test_commodity_channel_index_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_stock_price_summary.py` & `intrinio-sdk-6.25.0/test/test_stock_price_summary.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_insider_transaction_filing.py` & `intrinio-sdk-6.25.0/test/test_insider_transaction_filing.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_security_stock_prices.py` & `intrinio-sdk-6.25.0/test/test_api_response_security_stock_prices.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_negative_volume_index_technical_value.py` & `intrinio-sdk-6.25.0/test/test_negative_volume_index_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_security_ease_of_movement.py` & `intrinio-sdk-6.25.0/test/test_api_response_security_ease_of_movement.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_ichimoku_kinko_hyo_technical_value.py` & `intrinio-sdk-6.25.0/test/test_ichimoku_kinko_hyo_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_zacks_institutional_holding_owner_summary.py` & `intrinio-sdk-6.25.0/test/test_zacks_institutional_holding_owner_summary.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_data_tag_api.py` & `intrinio-sdk-6.25.0/test/test_data_tag_api.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_bulk_download_summary.py` & `intrinio-sdk-6.25.0/test/test_bulk_download_summary.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_triple_exponential_average_technical_value.py` & `intrinio-sdk-6.25.0/test/test_triple_exponential_average_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_company_news_summary.py` & `intrinio-sdk-6.25.0/test/test_company_news_summary.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_company_initial_public_offering.py` & `intrinio-sdk-6.25.0/test/test_company_initial_public_offering.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_security_historical_data.py` & `intrinio-sdk-6.25.0/test/test_api_response_security_historical_data.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_forex_pairs.py` & `intrinio-sdk-6.25.0/test/test_api_response_forex_pairs.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_filing_api.py` & `intrinio-sdk-6.25.0/test/test_filing_api.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_stock_exchange_securities.py` & `intrinio-sdk-6.25.0/test/test_api_response_stock_exchange_securities.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_keltner_channel_technical_value.py` & `intrinio-sdk-6.25.0/test/test_keltner_channel_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_security_snapshots_result.py` & `intrinio-sdk-6.25.0/test/test_security_snapshots_result.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_stock_exchange_api.py` & `intrinio-sdk-6.25.0/test/test_stock_exchange_api.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_vortex_indicator_technical_value.py` & `intrinio-sdk-6.25.0/test/test_vortex_indicator_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_force_index_technical_value.py` & `intrinio-sdk-6.25.0/test/test_force_index_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_initial_public_offerings.py` & `intrinio-sdk-6.25.0/test/test_api_response_initial_public_offerings.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_forex_api.py` & `intrinio-sdk-6.25.0/test/test_forex_api.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_security_volume_price_trend.py` & `intrinio-sdk-6.25.0/test/test_api_response_security_volume_price_trend.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_forex_price.py` & `intrinio-sdk-6.25.0/test/test_forex_price.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_zacks_etf_holdings.py` & `intrinio-sdk-6.25.0/test/test_api_response_zacks_etf_holdings.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_company_summary.py` & `intrinio-sdk-6.25.0/test/test_company_summary.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_forex_pair.py` & `intrinio-sdk-6.25.0/test/test_forex_pair.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_security_bollinger_bands.py` & `intrinio-sdk-6.25.0/test/test_api_response_security_bollinger_bands.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_security_zacks_sales_surprises.py` & `intrinio-sdk-6.25.0/test/test_api_response_security_zacks_sales_surprises.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_security_volume_weighted_average_price.py` & `intrinio-sdk-6.25.0/test/test_api_response_security_volume_weighted_average_price.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_true_strength_index_technical_value.py` & `intrinio-sdk-6.25.0/test/test_true_strength_index_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_options_prices_batch_realtime.py` & `intrinio-sdk-6.25.0/test/test_api_response_options_prices_batch_realtime.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_zacks_institutional_holding_owners.py` & `intrinio-sdk-6.25.0/test/test_api_response_zacks_institutional_holding_owners.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_filing_fundamentals.py` & `intrinio-sdk-6.25.0/test/test_api_response_filing_fundamentals.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_donchian_channel_technical_value.py` & `intrinio-sdk-6.25.0/test/test_donchian_channel_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_esg_comprehensive_rating.py` & `intrinio-sdk-6.25.0/test/test_esg_comprehensive_rating.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_forex_prices.py` & `intrinio-sdk-6.25.0/test/test_api_response_forex_prices.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_option_intervals_result.py` & `intrinio-sdk-6.25.0/test/test_option_intervals_result.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_option_stats_realtime.py` & `intrinio-sdk-6.25.0/test/test_option_stats_realtime.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_accumulation_distribution_index_technical_value.py` & `intrinio-sdk-6.25.0/test/test_accumulation_distribution_index_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_sic_indices_search.py` & `intrinio-sdk-6.25.0/test/test_api_response_sic_indices_search.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_average_true_range_technical_value.py` & `intrinio-sdk-6.25.0/test/test_average_true_range_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_options_expirations.py` & `intrinio-sdk-6.25.0/test/test_api_response_options_expirations.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_know_sure_thing_technical_value.py` & `intrinio-sdk-6.25.0/test/test_know_sure_thing_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_detrended_price_oscillator_technical_value.py` & `intrinio-sdk-6.25.0/test/test_detrended_price_oscillator_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_etf_stats.py` & `intrinio-sdk-6.25.0/test/test_etf_stats.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_data_tags_search.py` & `intrinio-sdk-6.25.0/test/test_api_response_data_tags_search.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_esg_companies.py` & `intrinio-sdk-6.25.0/test/test_api_response_esg_companies.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_ease_of_movement_technical_value.py` & `intrinio-sdk-6.25.0/test/test_ease_of_movement_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_security_keltner_channel.py` & `intrinio-sdk-6.25.0/test/test_api_response_security_keltner_channel.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_owners_api.py` & `intrinio-sdk-6.25.0/test/test_owners_api.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_chaikin_money_flow_technical_value.py` & `intrinio-sdk-6.25.0/test/test_chaikin_money_flow_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_options_unusual_activity.py` & `intrinio-sdk-6.25.0/test/test_api_response_options_unusual_activity.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_simple_moving_average_technical_value.py` & `intrinio-sdk-6.25.0/test/test_simple_moving_average_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_security_negative_volume_index.py` & `intrinio-sdk-6.25.0/test/test_api_response_security_negative_volume_index.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_options_price_realtime.py` & `intrinio-sdk-6.25.0/test/test_api_response_options_price_realtime.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_option_snapshots_result.py` & `intrinio-sdk-6.25.0/test/test_option_snapshots_result.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_zacks_institutional_holding_company_detail.py` & `intrinio-sdk-6.25.0/test/test_zacks_institutional_holding_company_detail.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_stock_market_indices_search.py` & `intrinio-sdk-6.25.0/test/test_api_response_stock_market_indices_search.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_stock_exchange_stock_prices.py` & `intrinio-sdk-6.25.0/test/test_api_response_stock_exchange_stock_prices.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_security_average_daily_trading_volume.py` & `intrinio-sdk-6.25.0/test/test_api_response_security_average_daily_trading_volume.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_company_fundamentals.py` & `intrinio-sdk-6.25.0/test/test_api_response_company_fundamentals.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_security_triple_exponential_average.py` & `intrinio-sdk-6.25.0/test/test_api_response_security_triple_exponential_average.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_zacks_eps_surprise.py` & `intrinio-sdk-6.25.0/test/test_zacks_eps_surprise.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_esg_rating.py` & `intrinio-sdk-6.25.0/test/test_esg_rating.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_filing_note_filing.py` & `intrinio-sdk-6.25.0/test/test_filing_note_filing.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_municipalitiy_financials.py` & `intrinio-sdk-6.25.0/test/test_api_response_municipalitiy_financials.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_company_news.py` & `intrinio-sdk-6.25.0/test/test_api_response_company_news.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_stock_price_adjustment.py` & `intrinio-sdk-6.25.0/test/test_stock_price_adjustment.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_zacks_eps_estimate.py` & `intrinio-sdk-6.25.0/test/test_zacks_eps_estimate.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_zacks_long_term_growth_rates.py` & `intrinio-sdk-6.25.0/test/test_api_response_zacks_long_term_growth_rates.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_zacks_institutional_holding_owner_detail.py` & `intrinio-sdk-6.25.0/test/test_zacks_institutional_holding_owner_detail.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_money_flow_index_technical_value.py` & `intrinio-sdk-6.25.0/test/test_money_flow_index_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_options.py` & `intrinio-sdk-6.25.0/test/test_api_response_options.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_fundamental.py` & `intrinio-sdk-6.25.0/test/test_fundamental.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_fundamental_summary.py` & `intrinio-sdk-6.25.0/test/test_fundamental_summary.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_security_average_directional_index.py` & `intrinio-sdk-6.25.0/test/test_api_response_security_average_directional_index.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_options_prices_eod.py` & `intrinio-sdk-6.25.0/test/test_api_response_options_prices_eod.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_stock_market_index_historical_data.py` & `intrinio-sdk-6.25.0/test/test_api_response_stock_market_index_historical_data.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_municipality_api.py` & `intrinio-sdk-6.25.0/test/test_municipality_api.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_company_shares_outstanding.py` & `intrinio-sdk-6.25.0/test/test_api_response_company_shares_outstanding.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_security_money_flow_index.py` & `intrinio-sdk-6.25.0/test/test_api_response_security_money_flow_index.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_average_directional_index_technical_value.py` & `intrinio-sdk-6.25.0/test/test_average_directional_index_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_option_chain_realtime.py` & `intrinio-sdk-6.25.0/test/test_option_chain_realtime.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_option_contracts_list.py` & `intrinio-sdk-6.25.0/test/test_option_contracts_list.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_security_api.py` & `intrinio-sdk-6.25.0/test/test_security_api.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_zacks_analyst_rating_snapshot.py` & `intrinio-sdk-6.25.0/test/test_zacks_analyst_rating_snapshot.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_zacks_sales_surprises.py` & `intrinio-sdk-6.25.0/test/test_api_response_zacks_sales_surprises.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_institutional_ownership.py` & `intrinio-sdk-6.25.0/test/test_institutional_ownership.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_security_true_strength_index.py` & `intrinio-sdk-6.25.0/test/test_api_response_security_true_strength_index.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_options_tickers.py` & `intrinio-sdk-6.25.0/test/test_api_response_options_tickers.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_owner_institutional_holdings.py` & `intrinio-sdk-6.25.0/test/test_api_response_owner_institutional_holdings.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_insider_transaction_filings_api.py` & `intrinio-sdk-6.25.0/test/test_insider_transaction_filings_api.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_filing_notes.py` & `intrinio-sdk-6.25.0/test/test_api_response_filing_notes.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_option_unusual_trade.py` & `intrinio-sdk-6.25.0/test/test_option_unusual_trade.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_option_chain.py` & `intrinio-sdk-6.25.0/test/test_option_chain.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_volume_price_trend_technical_value.py` & `intrinio-sdk-6.25.0/test/test_volume_price_trend_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_filing_note_summary.py` & `intrinio-sdk-6.25.0/test/test_filing_note_summary.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_option.py` & `intrinio-sdk-6.25.0/test/test_option.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_zacks_target_price_consensus.py` & `intrinio-sdk-6.25.0/test/test_zacks_target_price_consensus.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_etf_summary.py` & `intrinio-sdk-6.25.0/test/test_etf_summary.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_company_historical_data.py` & `intrinio-sdk-6.25.0/test/test_api_response_company_historical_data.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_relative_strength_index_technical_value.py` & `intrinio-sdk-6.25.0/test/test_relative_strength_index_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_zacks_sales_surprise_summary.py` & `intrinio-sdk-6.25.0/test/test_zacks_sales_surprise_summary.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_option_realtime.py` & `intrinio-sdk-6.25.0/test/test_option_realtime.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_stock_market_indices.py` & `intrinio-sdk-6.25.0/test/test_api_response_stock_market_indices.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_institutional_holding.py` & `intrinio-sdk-6.25.0/test/test_institutional_holding.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_owners.py` & `intrinio-sdk-6.25.0/test/test_api_response_owners.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_option_interval.py` & `intrinio-sdk-6.25.0/test/test_option_interval.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_security_force_index.py` & `intrinio-sdk-6.25.0/test/test_api_response_security_force_index.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_security_zacks_analyst_ratings.py` & `intrinio-sdk-6.25.0/test/test_api_response_security_zacks_analyst_ratings.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_filing_answers.py` & `intrinio-sdk-6.25.0/test/test_api_response_filing_answers.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_data_tag.py` & `intrinio-sdk-6.25.0/test/test_data_tag.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_insider_transaction.py` & `intrinio-sdk-6.25.0/test/test_insider_transaction.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_standardized_financial.py` & `intrinio-sdk-6.25.0/test/test_standardized_financial.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_stock_exchange_realtime_stock_prices.py` & `intrinio-sdk-6.25.0/test/test_api_response_stock_exchange_realtime_stock_prices.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_options_api.py` & `intrinio-sdk-6.25.0/test/test_options_api.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_company_filings.py` & `intrinio-sdk-6.25.0/test/test_api_response_company_filings.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_ultimate_oscillator_technical_value.py` & `intrinio-sdk-6.25.0/test/test_ultimate_oscillator_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_company_recognize.py` & `intrinio-sdk-6.25.0/test/test_api_response_company_recognize.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_esg_latest.py` & `intrinio-sdk-6.25.0/test/test_api_response_esg_latest.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_esg_api.py` & `intrinio-sdk-6.25.0/test/test_esg_api.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_zacks_institutional_holding.py` & `intrinio-sdk-6.25.0/test/test_zacks_institutional_holding.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_security_screen_clause.py` & `intrinio-sdk-6.25.0/test/test_security_screen_clause.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_company_shares_outstanding.py` & `intrinio-sdk-6.25.0/test/test_company_shares_outstanding.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_bollinger_bands_technical_value.py` & `intrinio-sdk-6.25.0/test/test_bollinger_bands_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_historical_data.py` & `intrinio-sdk-6.25.0/test/test_historical_data.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_security_summary.py` & `intrinio-sdk-6.25.0/test/test_security_summary.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_security_mass_index.py` & `intrinio-sdk-6.25.0/test/test_api_response_security_mass_index.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_securities_search.py` & `intrinio-sdk-6.25.0/test/test_api_response_securities_search.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_forex_currency.py` & `intrinio-sdk-6.25.0/test/test_forex_currency.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_economic_index_summary.py` & `intrinio-sdk-6.25.0/test/test_economic_index_summary.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_security_simple_moving_average.py` & `intrinio-sdk-6.25.0/test/test_api_response_security_simple_moving_average.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_filing.py` & `intrinio-sdk-6.25.0/test/test_filing.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_zacks_etf_holding.py` & `intrinio-sdk-6.25.0/test/test_zacks_etf_holding.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_zacks_target_price_consensuses.py` & `intrinio-sdk-6.25.0/test/test_api_response_zacks_target_price_consensuses.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_security_trades.py` & `intrinio-sdk-6.25.0/test/test_security_trades.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_zacks_analyst_rating_summary.py` & `intrinio-sdk-6.25.0/test/test_zacks_analyst_rating_summary.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_et_fs_api.py` & `intrinio-sdk-6.25.0/test/test_et_fs_api.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_zacks_institutional_holding_historical_summary.py` & `intrinio-sdk-6.25.0/test/test_zacks_institutional_holding_historical_summary.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_security_accumulation_distribution_index.py` & `intrinio-sdk-6.25.0/test/test_api_response_security_accumulation_distribution_index.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_news.py` & `intrinio-sdk-6.25.0/test/test_api_response_news.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_data_point_api.py` & `intrinio-sdk-6.25.0/test/test_data_point_api.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_security_on_balance_volume.py` & `intrinio-sdk-6.25.0/test/test_api_response_security_on_balance_volume.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_security_replay_file_result.py` & `intrinio-sdk-6.25.0/test/test_security_replay_file_result.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_standardized_financials.py` & `intrinio-sdk-6.25.0/test/test_api_response_standardized_financials.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_stock_market_index_summary.py` & `intrinio-sdk-6.25.0/test/test_stock_market_index_summary.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_security_moving_average_convergence_divergence.py` & `intrinio-sdk-6.25.0/test/test_api_response_security_moving_average_convergence_divergence.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_filing_summary.py` & `intrinio-sdk-6.25.0/test/test_filing_summary.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_zacks_institutional_holdings.py` & `intrinio-sdk-6.25.0/test/test_api_response_zacks_institutional_holdings.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_security_snapshot_group.py` & `intrinio-sdk-6.25.0/test/test_security_snapshot_group.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_options_chain.py` & `intrinio-sdk-6.25.0/test/test_api_response_options_chain.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_option_interval_mover.py` & `intrinio-sdk-6.25.0/test/test_option_interval_mover.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_companies_search.py` & `intrinio-sdk-6.25.0/test/test_api_response_companies_search.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_economic_indices_search.py` & `intrinio-sdk-6.25.0/test/test_api_response_economic_indices_search.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_companies.py` & `intrinio-sdk-6.25.0/test/test_api_response_companies.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_on_balance_volume_technical_value.py` & `intrinio-sdk-6.25.0/test/test_on_balance_volume_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_esg_company_rating_history.py` & `intrinio-sdk-6.25.0/test/test_api_response_esg_company_rating_history.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_company_answers.py` & `intrinio-sdk-6.25.0/test/test_api_response_company_answers.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_intraday_stock_price.py` & `intrinio-sdk-6.25.0/test/test_intraday_stock_price.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_reported_financial.py` & `intrinio-sdk-6.25.0/test/test_reported_financial.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_security_relative_strength_index.py` & `intrinio-sdk-6.25.0/test/test_api_response_security_relative_strength_index.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_bulk_download_links.py` & `intrinio-sdk-6.25.0/test/test_api_response_bulk_download_links.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_index_api.py` & `intrinio-sdk-6.25.0/test/test_index_api.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_stock_price_interval.py` & `intrinio-sdk-6.25.0/test/test_stock_price_interval.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_williams_r_technical_value.py` & `intrinio-sdk-6.25.0/test/test_williams_r_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_average_daily_trading_volume_technical_value.py` & `intrinio-sdk-6.25.0/test/test_average_daily_trading_volume_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_company_news.py` & `intrinio-sdk-6.25.0/test/test_company_news.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_securities.py` & `intrinio-sdk-6.25.0/test/test_api_response_securities.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_option_chain_eod.py` & `intrinio-sdk-6.25.0/test/test_option_chain_eod.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_zacks_institutional_holding_companies.py` & `intrinio-sdk-6.25.0/test/test_api_response_zacks_institutional_holding_companies.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_municipality.py` & `intrinio-sdk-6.25.0/test/test_municipality.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_security_donchian_channel.py` & `intrinio-sdk-6.25.0/test/test_api_response_security_donchian_channel.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_company_filing.py` & `intrinio-sdk-6.25.0/test/test_company_filing.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_historical_data_api.py` & `intrinio-sdk-6.25.0/test/test_historical_data_api.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_zacks_analyst_rating.py` & `intrinio-sdk-6.25.0/test/test_zacks_analyst_rating.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_owner.py` & `intrinio-sdk-6.25.0/test/test_owner.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_api_response_zacks_eps_estimates.py` & `intrinio-sdk-6.25.0/test/test_api_response_zacks_eps_estimates.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/test/test_dividend_record.py` & `intrinio-sdk-6.25.0/test/test_dividend_record.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.24.1/README.md` & `intrinio-sdk-6.25.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Intrinio Python SDK
 
 To get an API key, [sign up here](https://intrinio.com/).
 
 Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.
 
-- API version: 2.43.6
-- Package version: 6.24.1
+- API version: 2.45.0
+- Package version: 6.25.0
 
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation
```

### Comparing `intrinio-sdk-6.24.1/setup.py` & `intrinio-sdk-6.25.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.43.6
+    OpenAPI spec version: 2.45.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "intrinio-sdk"
-VERSION = "6.24.1"
+VERSION = "6.25.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

