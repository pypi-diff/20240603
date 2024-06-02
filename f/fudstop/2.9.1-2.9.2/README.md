# Comparing `tmp/fudstop-2.9.1.tar.gz` & `tmp/fudstop-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fudstop-2.9.1.tar", last modified: Sat Jun  1 22:42:55 2024, max compression
+gzip compressed data, was "fudstop-2.9.2.tar", last modified: Sat Jun  1 22:52:08 2024, max compression
```

## Comparing `fudstop-2.9.1.tar` & `fudstop-2.9.2.tar`

### file list

```diff
@@ -1,378 +1,378 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.931745 fudstop-2.9.1/
--rw-rw-rw-   0        0        0     7616 2024-06-01 22:42:55.930745 fudstop-2.9.1/PKG-INFO
--rw-rw-rw-   0        0        0     2341 2024-01-05 23:27:36.000000 fudstop-2.9.1/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.729014 fudstop-2.9.1/app/
--rw-rw-rw-   0        0        0    43348 2024-01-23 23:29:23.000000 fudstop-2.9.1/app/__init__.py
--rw-rw-rw-   0        0        0     4011 2024-01-12 03:32:55.000000 fudstop-2.9.1/app/fetcher.py
--rw-rw-rw-   0        0        0    17884 2024-01-12 06:07:09.000000 fudstop-2.9.1/app/fudstop_info.py
--rw-rw-rw-   0        0        0    38553 2024-01-12 03:47:25.000000 fudstop-2.9.1/app/helpers.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.733018 fudstop-2.9.1/fudstop/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.755015 fudstop-2.9.1/fudstop/_markets/
--rw-rw-rw-   0        0        0     1327 2024-01-18 15:18:48.000000 fudstop-2.9.1/fudstop/_markets/__init__.py
--rw-rw-rw-   0        0        0     2440 2024-02-22 04:18:16.000000 fudstop-2.9.1/fudstop/_markets/analyzers.py
--rw-rw-rw-   0        0        0    67237 2024-02-07 15:09:55.000000 fudstop-2.9.1/fudstop/_markets/embeddings.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.759014 fudstop-2.9.1/fudstop/_markets/finished/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:49:02.000000 fudstop-2.9.1/fudstop/_markets/finished/__init__.py
--rw-rw-rw-   0        0        0    25622 2024-01-21 19:47:09.000000 fudstop-2.9.1/fudstop/_markets/finished/db_manager.py
--rw-rw-rw-   0        0        0     2530 2023-10-12 23:34:06.000000 fudstop-2.9.1/fudstop/_markets/finished/economic_data.py
--rw-rw-rw-   0        0        0    53472 2024-02-11 04:30:33.000000 fudstop-2.9.1/fudstop/_markets/finished/master_class.py
--rw-rw-rw-   0        0        0     9940 2024-01-25 21:35:47.000000 fudstop-2.9.1/fudstop/_markets/finished/td9_states.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.761015 fudstop-2.9.1/fudstop/_markets/list_sets/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/_markets/list_sets/__init__.py
--rw-rw-rw-   0        0        0    92394 2024-02-22 03:17:43.000000 fudstop-2.9.1/fudstop/_markets/list_sets/dicts.py
--rw-rw-rw-   0        0        0    88831 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/_markets/list_sets/saved_tickers.py
--rw-rw-rw-   0        0        0   125429 2024-01-17 16:34:32.000000 fudstop-2.9.1/fudstop/_markets/list_sets/ticker_lists.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.767015 fudstop-2.9.1/fudstop/_markets/market_handlers/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/_markets/market_handlers/__init__.py
--rw-rw-rw-   0        0        0     1265 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/_markets/market_handlers/cfg.py
--rw-rw-rw-   0        0        0     1491 2024-01-09 04:43:27.000000 fudstop-2.9.1/fudstop/_markets/market_handlers/crypto.py
--rw-rw-rw-   0        0        0    17424 2024-02-12 18:43:10.000000 fudstop-2.9.1/fudstop/_markets/market_handlers/database_.py
--rw-rw-rw-   0        0        0      768 2024-01-09 05:02:23.000000 fudstop-2.9.1/fudstop/_markets/market_handlers/forex.py
--rw-rw-rw-   0        0        0     1770 2024-01-08 17:15:06.000000 fudstop-2.9.1/fudstop/_markets/market_handlers/indices.py
--rw-rw-rw-   0        0        0   762960 2024-01-11 23:53:54.000000 fudstop-2.9.1/fudstop/_markets/market_handlers/list_sets.py
--rw-rw-rw-   0        0        0    13155 2024-01-11 17:06:04.000000 fudstop-2.9.1/fudstop/_markets/market_handlers/options.py
--rw-rw-rw-   0        0        0     3929 2024-01-09 21:38:56.000000 fudstop-2.9.1/fudstop/_markets/market_handlers/stocks.py
--rw-rw-rw-   0        0        0     1166 2024-01-12 17:40:54.000000 fudstop-2.9.1/fudstop/_markets/monitor.py
--rw-rw-rw-   0        0        0    31105 2024-02-12 14:30:27.000000 fudstop-2.9.1/fudstop/_markets/multimarkets.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.767015 fudstop-2.9.1/fudstop/_markets/plotting/
--rw-rw-rw-   0        0        0     1814 2024-01-13 01:48:40.000000 fudstop-2.9.1/fudstop/_markets/plotting/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.769014 fudstop-2.9.1/fudstop/_markets/reference_markets/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/_markets/reference_markets/__init__.py
--rw-rw-rw-   0        0        0     1400 2024-01-08 00:31:15.000000 fudstop-2.9.1/fudstop/_markets/reference_markets/conditional_scans.py
--rw-rw-rw-   0        0        0     8389 2024-01-10 04:38:30.000000 fudstop-2.9.1/fudstop/_markets/reference_markets/reference_market.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.777015 fudstop-2.9.1/fudstop/_markets/scripts/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/_markets/scripts/__init__.py
--rw-rw-rw-   0        0        0      846 2024-01-20 18:45:32.000000 fudstop-2.9.1/fudstop/_markets/scripts/all_polygon_options.py
--rw-rw-rw-   0        0        0      683 2024-01-07 06:56:40.000000 fudstop-2.9.1/fudstop/_markets/scripts/all_webull_options.py
--rw-rw-rw-   0        0        0     1208 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/_markets/scripts/generation.py
--rw-rw-rw-   0        0        0     1351 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/_markets/scripts/million_dollar_trades.py
--rw-rw-rw-   0        0        0     1533 2024-01-18 14:58:07.000000 fudstop-2.9.1/fudstop/_markets/scripts/option_scripts.py
--rw-rw-rw-   0        0        0    20845 2024-01-20 18:50:03.000000 fudstop-2.9.1/fudstop/_markets/scripts/options_market.py
--rw-rw-rw-   0        0        0     2961 2024-01-11 18:09:48.000000 fudstop-2.9.1/fudstop/_markets/scripts/options_volume_analysis.py
--rw-rw-rw-   0        0        0     1942 2024-01-11 18:07:34.000000 fudstop-2.9.1/fudstop/_markets/scripts/rsi_2_4_8.py
--rw-rw-rw-   0        0        0     2172 2024-01-24 23:43:15.000000 fudstop-2.9.1/fudstop/_markets/scripts/rsi_screener.py
--rw-rw-rw-   0        0        0     1197 2024-01-20 05:06:57.000000 fudstop-2.9.1/fudstop/_markets/scripts/ssr_scanner.py
--rw-rw-rw-   0        0        0     7315 2024-01-23 17:20:40.000000 fudstop-2.9.1/fudstop/_markets/scripts/stock_market.py
--rw-rw-rw-   0        0        0     6271 2024-01-12 19:46:21.000000 fudstop-2.9.1/fudstop/_markets/scripts/td9_states.py
--rw-rw-rw-   0        0        0    14287 2024-02-06 18:37:20.000000 fudstop-2.9.1/fudstop/_markets/scripts/universal_snapshot.py
--rw-rw-rw-   0        0        0    13782 2024-01-25 20:46:06.000000 fudstop-2.9.1/fudstop/_markets/stock_market.py
--rw-rw-rw-   0        0        0     1893 2024-01-10 18:26:30.000000 fudstop-2.9.1/fudstop/_markets/webhook_dicts.py
--rw-rw-rw-   0        0        0    14911 2024-01-06 18:40:07.000000 fudstop-2.9.1/fudstop/all_helpers.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.778015 fudstop-2.9.1/fudstop/apis/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.779014 fudstop-2.9.1/fudstop/apis/_asyncpg/
--rw-rw-rw-   0        0        0        0 2024-02-29 20:06:59.000000 fudstop-2.9.1/fudstop/apis/_asyncpg/__init__.py
--rw-rw-rw-   0        0        0    15085 2024-04-14 15:28:27.000000 fudstop-2.9.1/fudstop/apis/_asyncpg/asyncpg_sdk.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.780014 fudstop-2.9.1/fudstop/apis/_datetime/
--rw-rw-rw-   0        0        0        0 2024-02-29 20:06:52.000000 fudstop-2.9.1/fudstop/apis/_datetime/__init__.py
--rw-rw-rw-   0        0        0     3440 2024-04-14 23:10:42.000000 fudstop-2.9.1/fudstop/apis/_datetime/datetime_sdk.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.783015 fudstop-2.9.1/fudstop/apis/_openai/
--rw-rw-rw-   0        0        0        0 2024-01-07 17:40:15.000000 fudstop-2.9.1/fudstop/apis/_openai/__init__.py
--rw-rw-rw-   0        0        0     4824 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/_openai/agent.py
--rw-rw-rw-   0        0        0     7552 2024-03-07 23:34:16.000000 fudstop-2.9.1/fudstop/apis/_openai/openai_sdk.py
--rw-rw-rw-   0        0        0    27388 2024-02-25 03:36:21.000000 fudstop-2.9.1/fudstop/apis/_openai/tools_shcema.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.784014 fudstop-2.9.1/fudstop/apis/_pandas/
--rw-rw-rw-   0        0        0        0 2024-02-29 20:42:25.000000 fudstop-2.9.1/fudstop/apis/_pandas/__init__.py
--rw-rw-rw-   0        0        0      226 2024-02-29 20:44:07.000000 fudstop-2.9.1/fudstop/apis/_pandas/pandas_sdk.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.785014 fudstop-2.9.1/fudstop/apis/_selenium/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/_selenium/__init__.py
--rw-rw-rw-   0        0        0     1863 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/_selenium/selenium_sdk.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.786014 fudstop-2.9.1/fudstop/apis/alphaquery/
--rw-rw-rw-   0        0        0        0 2024-04-13 21:58:49.000000 fudstop-2.9.1/fudstop/apis/alphaquery/__init__.py
--rw-rw-rw-   0        0        0     3639 2024-04-13 22:04:47.000000 fudstop-2.9.1/fudstop/apis/alphaquery/alpha_sdk.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.787014 fudstop-2.9.1/fudstop/apis/alphaquery/models/
--rw-rw-rw-   0        0        0        0 2024-04-13 21:58:58.000000 fudstop-2.9.1/fudstop/apis/alphaquery/models/__init__.py
--rw-rw-rw-   0        0        0       41 2024-04-13 21:59:36.000000 fudstop-2.9.1/fudstop/apis/alphaquery/models/alpha_models.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.788015 fudstop-2.9.1/fudstop/apis/caselaw/
--rw-rw-rw-   0        0        0        0 2024-05-09 17:36:00.000000 fudstop-2.9.1/fudstop/apis/caselaw/__init__.py
--rw-rw-rw-   0        0        0     3199 2024-05-09 18:13:57.000000 fudstop-2.9.1/fudstop/apis/caselaw/caselaw_models.py
--rw-rw-rw-   0        0        0     1709 2024-05-09 18:18:24.000000 fudstop-2.9.1/fudstop/apis/caselaw/caselaw_sdk.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.791015 fudstop-2.9.1/fudstop/apis/cfr/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/cfr/__init__.py
--rw-rw-rw-   0        0        0     3742 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/cfr/cfr_2.0.py
--rw-rw-rw-   0        0        0       87 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/cfr/cfr_helpers.py
--rw-rw-rw-   0        0        0     7590 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/cfr/cfr_sdk.py
--rw-rw-rw-   0        0        0     2525 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/cfr/title_12.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.793015 fudstop-2.9.1/fudstop/apis/datalink/
--rw-rw-rw-   0        0        0        0 2024-03-25 21:17:59.000000 fudstop-2.9.1/fudstop/apis/datalink/__init__.py
--rw-rw-rw-   0        0        0     2661 2024-03-27 07:04:34.000000 fudstop-2.9.1/fudstop/apis/datalink/datalink_sdk.py
--rw-rw-rw-   0        0        0     2609 2024-03-25 21:32:23.000000 fudstop-2.9.1/fudstop/apis/datalink/models.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.794014 fudstop-2.9.1/fudstop/apis/discord_/
--rw-rw-rw-   0        0        0     4430 2024-01-08 04:14:36.000000 fudstop-2.9.1/fudstop/apis/discord_/__init__.py
--rw-rw-rw-   0        0        0    12863 2024-02-23 01:28:51.000000 fudstop-2.9.1/fudstop/apis/discord_/discord_sdk.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.796014 fudstop-2.9.1/fudstop/apis/discord_/models/
--rw-rw-rw-   0        0        0        0 2024-01-18 14:52:13.000000 fudstop-2.9.1/fudstop/apis/discord_/models/__init__.py
--rw-rw-rw-   0        0        0     5431 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/discord_/models/application_commands.py
--rw-rw-rw-   0        0        0     2767 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/discord_/models/search.py
--rw-rw-rw-   0        0        0     1101 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/discord_/models/webhooks.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.798014 fudstop-2.9.1/fudstop/apis/earnings_whisper/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/earnings_whisper/__init__.py
--rw-rw-rw-   0        0        0    12823 2024-03-25 21:47:38.000000 fudstop-2.9.1/fudstop/apis/earnings_whisper/ew_models.py
--rw-rw-rw-   0        0        0     4016 2024-03-25 21:44:18.000000 fudstop-2.9.1/fudstop/apis/earnings_whisper/ew_sdk.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.799013 fudstop-2.9.1/fudstop/apis/fastcase/
--rw-rw-rw-   0        0        0        0 2024-04-14 15:00:18.000000 fudstop-2.9.1/fudstop/apis/fastcase/__init__.py
--rw-rw-rw-   0        0        0     6212 2024-05-02 15:37:07.000000 fudstop-2.9.1/fudstop/apis/fastcase/fastcase_sdk.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.801015 fudstop-2.9.1/fudstop/apis/fed_print/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/fed_print/__init__.py
--rw-rw-rw-   0        0        0     2908 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/fed_print/fed_print_sync.py
--rw-rw-rw-   0        0        0     5322 2024-02-24 20:29:40.000000 fudstop-2.9.1/fudstop/apis/fed_print/fedprint_models.py
--rw-rw-rw-   0        0        0     3354 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/fed_print/fedprint_sdk.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.803013 fudstop-2.9.1/fudstop/apis/federal_register/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/federal_register/__init__.py
--rw-rw-rw-   0        0        0     3075 2024-02-25 17:21:39.000000 fudstop-2.9.1/fudstop/apis/federal_register/fed_register_sdk.py
--rw-rw-rw-   0        0        0     2924 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/federal_register/fed_register_sync.py
--rw-rw-rw-   0        0        0     2904 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/federal_register/register_models.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.805015 fudstop-2.9.1/fudstop/apis/gexbot/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/gexbot/__init__.py
--rw-rw-rw-   0        0        0     4095 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/gexbot/gexbot.py
--rw-rw-rw-   0        0        0     4139 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/gexbot/models.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.806016 fudstop-2.9.1/fudstop/apis/gpts/
--rw-rw-rw-   0        0        0      231 2024-01-08 03:41:52.000000 fudstop-2.9.1/fudstop/apis/gpts/DiscoAI.py
--rw-rw-rw-   0        0        0        2 2024-01-08 03:38:45.000000 fudstop-2.9.1/fudstop/apis/gpts/__init__.py
--rw-rw-rw-   0        0        0    36326 2024-05-01 23:15:01.000000 fudstop-2.9.1/fudstop/apis/helpers.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.808014 fudstop-2.9.1/fudstop/apis/master/
--rw-rw-rw-   0        0        0        0 2024-02-25 05:43:46.000000 fudstop-2.9.1/fudstop/apis/master/__init__.py
--rw-rw-rw-   0        0        0     1459 2024-02-25 09:02:57.000000 fudstop-2.9.1/fudstop/apis/master/master_helpers.py
--rw-rw-rw-   0        0        0    29960 2024-02-25 19:23:31.000000 fudstop-2.9.1/fudstop/apis/master/master_sdk.py
--rw-rw-rw-   0        0        0    34633 2024-02-25 09:11:27.000000 fudstop-2.9.1/fudstop/apis/master/tools.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.811019 fudstop-2.9.1/fudstop/apis/misc/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/misc/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.812018 fudstop-2.9.1/fudstop/apis/misc/models/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/misc/models/__init__.py
--rw-rw-rw-   0        0        0      249 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/misc/models/unsplash_models.py
--rw-rw-rw-   0        0        0     2204 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/misc/models/weather_models.py
--rw-rw-rw-   0        0        0      869 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/misc/unsplash.py
--rw-rw-rw-   0        0        0     1790 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/misc/weather.py
--rw-rw-rw-   0        0        0      294 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/misc/weather_helpers.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.814018 fudstop-2.9.1/fudstop/apis/nasdaq/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/nasdaq/__init__.py
--rw-rw-rw-   0        0        0     4200 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/nasdaq/nasdaq_lists.py
--rw-rw-rw-   0        0        0    12177 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/nasdaq/nasdaq_sdk.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.815017 fudstop-2.9.1/fudstop/apis/newyork_fed/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/newyork_fed/__init__.py
--rw-rw-rw-   0        0        0    14970 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/newyork_fed/models.py
--rw-rw-rw-   0        0        0    22750 2024-03-27 00:32:52.000000 fudstop-2.9.1/fudstop/apis/newyork_fed/newyork_fed_sdk.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.817018 fudstop-2.9.1/fudstop/apis/occ/
--rw-rw-rw-   0        0        0        0 2024-01-12 03:42:31.000000 fudstop-2.9.1/fudstop/apis/occ/__init__.py
--rw-rw-rw-   0        0        0    30622 2024-05-19 05:08:45.000000 fudstop-2.9.1/fudstop/apis/occ/occ_models.py
--rw-rw-rw-   0        0        0    14163 2024-05-29 23:33:52.000000 fudstop-2.9.1/fudstop/apis/occ/occ_sdk.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.819016 fudstop-2.9.1/fudstop/apis/ofr/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/ofr/__init__.py
--rw-rw-rw-   0        0        0    37577 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/ofr/ofr_list_sets.py
--rw-rw-rw-   0        0        0     5462 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/ofr/ofr_sdk.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.821018 fudstop-2.9.1/fudstop/apis/oic/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/oic/__init__.py
--rw-rw-rw-   0        0        0    16116 2024-01-07 16:09:24.000000 fudstop-2.9.1/fudstop/apis/oic/async_oic_sdk.py
--rw-rw-rw-   0        0        0    11292 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/oic/oic_models.py
--rw-rw-rw-   0        0        0     4938 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/oic/oic_sdk.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.826233 fudstop-2.9.1/fudstop/apis/polygonio/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/polygonio/__init__.py
--rw-rw-rw-   0        0        0    31100 2024-05-27 03:23:49.000000 fudstop-2.9.1/fudstop/apis/polygonio/async_polygon_sdk.py
--rw-rw-rw-   0        0        0     2368 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/polygonio/db_polygon.py
--rw-rw-rw-   0        0        0    47011 2024-01-10 15:38:01.000000 fudstop-2.9.1/fudstop/apis/polygonio/mapping.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.831233 fudstop-2.9.1/fudstop/apis/polygonio/models/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/polygonio/models/__init__.py
--rw-rw-rw-   0        0        0     1330 2024-04-13 19:03:08.000000 fudstop-2.9.1/fudstop/apis/polygonio/models/aggregates.py
--rw-rw-rw-   0        0        0     1319 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/polygonio/models/company_info.py
--rw-rw-rw-   0        0        0     4295 2024-04-14 23:13:19.000000 fudstop-2.9.1/fudstop/apis/polygonio/models/gainers_losers.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.833234 fudstop-2.9.1/fudstop/apis/polygonio/models/option_models/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/polygonio/models/option_models/__init__.py
--rw-rw-rw-   0        0        0     5734 2024-01-12 15:43:51.000000 fudstop-2.9.1/fudstop/apis/polygonio/models/option_models/option_snapshot.py
--rw-rw-rw-   0        0        0     7043 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/polygonio/models/option_models/universal_option.py
--rw-rw-rw-   0        0        0    58850 2024-05-23 05:30:03.000000 fudstop-2.9.1/fudstop/apis/polygonio/models/option_models/universal_snapshot.py
--rw-rw-rw-   0        0        0     7964 2024-05-25 04:33:35.000000 fudstop-2.9.1/fudstop/apis/polygonio/models/technicals.py
--rw-rw-rw-   0        0        0     2271 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/polygonio/models/ticker_news.py
--rw-rw-rw-   0        0        0     3801 2024-01-07 01:51:36.000000 fudstop-2.9.1/fudstop/apis/polygonio/models/ticker_snapshot.py
--rw-rw-rw-   0        0        0     5787 2024-01-21 19:53:33.000000 fudstop-2.9.1/fudstop/apis/polygonio/models/trades.py
--rw-rw-rw-   0        0        0    13162 2024-06-01 18:36:58.000000 fudstop-2.9.1/fudstop/apis/polygonio/polygon_database.py
--rw-rw-rw-   0        0        0    41160 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/polygonio/polygon_helpers.py
--rw-rw-rw-   0        0        0    71525 2024-05-23 05:18:46.000000 fudstop-2.9.1/fudstop/apis/polygonio/polygon_options.py
--rw-rw-rw-   0        0        0     3692 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/polygonio/polygon_sync.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.835233 fudstop-2.9.1/fudstop/apis/polygonio/scripts/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/polygonio/scripts/__init__.py
--rw-rw-rw-   0        0        0     2267 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/polygonio/scripts/daily_aggregates.py
--rw-rw-rw-   0        0        0     1716 2024-02-04 09:29:32.000000 fudstop-2.9.1/fudstop/apis/polygonio/scripts/rsi.py
--rw-rw-rw-   0        0        0     9164 2024-03-01 01:05:43.000000 fudstop-2.9.1/fudstop/apis/polygonio/technicals.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.837233 fudstop-2.9.1/fudstop/apis/rapid/
--rw-rw-rw-   0        0        0        0 2024-05-08 03:47:05.000000 fudstop-2.9.1/fudstop/apis/rapid/__init__.py
--rw-rw-rw-   0        0        0     8348 2024-05-08 05:03:43.000000 fudstop-2.9.1/fudstop/apis/rapid/rapid_models.py
--rw-rw-rw-   0        0        0     3188 2024-05-08 04:36:56.000000 fudstop-2.9.1/fudstop/apis/rapid/rapid_sdk.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.840233 fudstop-2.9.1/fudstop/apis/rss/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/rss/__init__.py
--rw-rw-rw-   0        0        0      736 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/rss/rss_helpers.py
--rw-rw-rw-   0        0        0     1497 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/rss/rss_models.py
--rw-rw-rw-   0        0        0    10360 2024-01-11 18:07:47.000000 fudstop-2.9.1/fudstop/apis/rss/rss_sdk.py
--rw-rw-rw-   0        0        0    10203 2024-01-11 18:07:47.000000 fudstop-2.9.1/fudstop/apis/rss/snyc_rss.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.841234 fudstop-2.9.1/fudstop/apis/sec/
--rw-rw-rw-   0        0        0        0 2024-02-29 20:06:34.000000 fudstop-2.9.1/fudstop/apis/sec/__init__.py
--rw-rw-rw-   0        0        0     8441 2024-02-29 22:33:02.000000 fudstop-2.9.1/fudstop/apis/sec/sec_sdk.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.842234 fudstop-2.9.1/fudstop/apis/stocksera_/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/stocksera_/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.851235 fudstop-2.9.1/fudstop/apis/stocksera_/models/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/stocksera_/models/__init__.py
--rw-rw-rw-   0        0        0      487 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/stocksera_/models/borrowed_shares.py
--rw-rw-rw-   0        0        0      827 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/stocksera_/models/daily_treasury.py
--rw-rw-rw-   0        0        0      747 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/stocksera_/models/ftds.py
--rw-rw-rw-   0        0        0      871 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/stocksera_/models/highest_shorted.py
--rw-rw-rw-   0        0        0      813 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/stocksera_/models/inflation.py
--rw-rw-rw-   0        0        0     1062 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/stocksera_/models/insider_trades.py
--rw-rw-rw-   0        0        0      667 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/stocksera_/models/jim_cramer.py
--rw-rw-rw-   0        0        0      850 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/stocksera_/models/jobless_claims.py
--rw-rw-rw-   0        0        0     1043 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/stocksera_/models/low_float.py
--rw-rw-rw-   0        0        0      660 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/stocksera_/models/market_news.py
--rw-rw-rw-   0        0        0    21824 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/stocksera_/models/models.py
--rw-rw-rw-   0        0        0      676 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/stocksera_/models/news_sentiment.py
--rw-rw-rw-   0        0        0      693 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/stocksera_/models/retail_sales.py
--rw-rw-rw-   0        0        0      708 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/stocksera_/models/reverse_repo.py
--rw-rw-rw-   0        0        0      777 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/stocksera_/models/sec_filings.py
--rw-rw-rw-   0        0        0      789 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/stocksera_/models/short_volume.py
--rw-rw-rw-   0        0        0    19676 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/stocksera_/stocksera_.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.853234 fudstop-2.9.1/fudstop/apis/treasury/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/treasury/__init__.py
--rw-rw-rw-   0        0        0    10964 2024-01-20 19:15:58.000000 fudstop-2.9.1/fudstop/apis/treasury/treasury_models.py
--rw-rw-rw-   0        0        0    10281 2024-01-20 19:16:09.000000 fudstop-2.9.1/fudstop/apis/treasury/treasury_sdk.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.855235 fudstop-2.9.1/fudstop/apis/udio/
--rw-rw-rw-   0        0        0        0 2024-05-04 04:08:21.000000 fudstop-2.9.1/fudstop/apis/udio/__init__.py
--rw-rw-rw-   0        0        0     4605 2024-05-04 04:20:04.000000 fudstop-2.9.1/fudstop/apis/udio/imps.py
--rw-rw-rw-   0        0        0     2130 2024-05-04 05:03:43.000000 fudstop-2.9.1/fudstop/apis/udio/udio_sdk.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.864234 fudstop-2.9.1/fudstop/apis/webull/
--rw-rw-rw-   0        0        0     4945 2024-01-15 22:06:39.000000 fudstop-2.9.1/fudstop/apis/webull/__init__.py
--rw-rw-rw-   0        0        0    12127 2024-01-23 03:47:19.000000 fudstop-2.9.1/fudstop/apis/webull/database_manager.py
--rw-rw-rw-   0        0        0     2732 2024-01-11 18:10:25.000000 fudstop-2.9.1/fudstop/apis/webull/get_volume_analysis.py
--rw-rw-rw-   0        0        0    10628 2024-01-11 18:10:17.000000 fudstop-2.9.1/fudstop/apis/webull/modal.py
--rw-rw-rw-   0        0        0     5320 2024-01-10 21:10:43.000000 fudstop-2.9.1/fudstop/apis/webull/opt_modal.py
--rw-rw-rw-   0        0        0     4916 2024-06-01 20:48:50.000000 fudstop-2.9.1/fudstop/apis/webull/option_data.py
--rw-rw-rw-   0        0        0     9390 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/webull/options.py
--rw-rw-rw-   0        0        0     6520 2024-05-15 23:10:46.000000 fudstop-2.9.1/fudstop/apis/webull/screener_models.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.874234 fudstop-2.9.1/fudstop/apis/webull/trade_models/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/webull/trade_models/__init__.py
--rw-rw-rw-   0        0        0     2030 2024-02-18 21:14:42.000000 fudstop-2.9.1/fudstop/apis/webull/trade_models/analyst_ratings.py
--rw-rw-rw-   0        0        0    15033 2024-05-31 23:04:35.000000 fudstop-2.9.1/fudstop/apis/webull/trade_models/capital_flow.py
--rw-rw-rw-   0        0        0     2147 2024-02-24 19:57:32.000000 fudstop-2.9.1/fudstop/apis/webull/trade_models/company_brief.py
--rw-rw-rw-   0        0        0     2235 2024-01-23 05:04:58.000000 fudstop-2.9.1/fudstop/apis/webull/trade_models/cost_distribution.py
--rw-rw-rw-   0        0        0     1053 2024-02-18 19:14:15.000000 fudstop-2.9.1/fudstop/apis/webull/trade_models/etf_holdings.py
--rw-rw-rw-   0        0        0     1727 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/webull/trade_models/events.py
--rw-rw-rw-   0        0        0    19884 2024-02-18 19:14:03.000000 fudstop-2.9.1/fudstop/apis/webull/trade_models/financials.py
--rw-rw-rw-   0        0        0     3780 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/webull/trade_models/forecast_evaluator.py
--rw-rw-rw-   0        0        0     3500 2024-02-18 18:48:35.000000 fudstop-2.9.1/fudstop/apis/webull/trade_models/institutional_holdings.py
--rw-rw-rw-   0        0        0     1335 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/webull/trade_models/news.py
--rw-rw-rw-   0        0        0     2235 2024-05-14 22:42:18.000000 fudstop-2.9.1/fudstop/apis/webull/trade_models/order_flow.py
--rw-rw-rw-   0        0        0     1195 2024-03-01 01:13:55.000000 fudstop-2.9.1/fudstop/apis/webull/trade_models/price_streamer.py
--rw-rw-rw-   0        0        0      601 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/webull/trade_models/short_interest.py
--rw-rw-rw-   0        0        0     4714 2024-04-29 02:51:39.000000 fudstop-2.9.1/fudstop/apis/webull/trade_models/stock_quote.py
--rw-rw-rw-   0        0        0    11042 2024-03-07 17:43:34.000000 fudstop-2.9.1/fudstop/apis/webull/trade_models/ticker_query.py
--rw-rw-rw-   0        0        0     1314 2024-01-13 16:23:06.000000 fudstop-2.9.1/fudstop/apis/webull/trade_models/volume_analysis.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.875234 fudstop-2.9.1/fudstop/apis/webull/trader_models/
--rw-rw-rw-   0        0        0        0 2024-04-23 22:21:57.000000 fudstop-2.9.1/fudstop/apis/webull/trader_models/__init__.py
--rw-rw-rw-   0        0        0    39759 2024-04-28 00:01:42.000000 fudstop-2.9.1/fudstop/apis/webull/trader_models/trader_models.py
--rw-rw-rw-   0        0        0    13181 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/webull/webull_helpers.py
--rw-rw-rw-   0        0        0    12274 2024-02-25 06:46:04.000000 fudstop-2.9.1/fudstop/apis/webull/webull_markets.py
--rw-rw-rw-   0        0        0    17501 2024-06-01 19:46:46.000000 fudstop-2.9.1/fudstop/apis/webull/webull_option_screener.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.878233 fudstop-2.9.1/fudstop/apis/webull/webull_options/
--rw-rw-rw-   0        0        0        0 2024-01-06 17:03:12.000000 fudstop-2.9.1/fudstop/apis/webull/webull_options/__init__.py
--rw-rw-rw-   0        0        0    15129 2024-01-06 17:03:12.000000 fudstop-2.9.1/fudstop/apis/webull/webull_options/helpers.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.879233 fudstop-2.9.1/fudstop/apis/webull/webull_options/models/
--rw-rw-rw-   0        0        0        0 2024-01-06 17:03:12.000000 fudstop-2.9.1/fudstop/apis/webull/webull_options/models/__init__.py
--rw-rw-rw-   0        0        0    36853 2024-02-06 07:52:04.000000 fudstop-2.9.1/fudstop/apis/webull/webull_options/models/db_manager.py
--rw-rw-rw-   0        0        0    23420 2024-04-23 23:48:07.000000 fudstop-2.9.1/fudstop/apis/webull/webull_options/models/options_data.py
--rw-rw-rw-   0        0        0    47807 2024-06-01 21:40:11.000000 fudstop-2.9.1/fudstop/apis/webull/webull_options/webull_options.py
--rw-rw-rw-   0        0        0      957 2024-02-06 07:52:33.000000 fudstop-2.9.1/fudstop/apis/webull/webull_options/webull_trader.py
--rw-rw-rw-   0        0        0    35666 2024-01-21 19:47:41.000000 fudstop-2.9.1/fudstop/apis/webull/webull_options.py
--rw-rw-rw-   0        0        0    14292 2024-06-01 19:10:13.000000 fudstop-2.9.1/fudstop/apis/webull/webull_paper_trader.py
--rw-rw-rw-   0        0        0     9106 2024-01-18 22:00:22.000000 fudstop-2.9.1/fudstop/apis/webull/webull_parsing.py
--rw-rw-rw-   0        0        0     7309 2024-05-15 23:18:59.000000 fudstop-2.9.1/fudstop/apis/webull/webull_trader.py
--rw-rw-rw-   0        0        0    32001 2024-05-31 22:58:27.000000 fudstop-2.9.1/fudstop/apis/webull/webull_trading.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.881235 fudstop-2.9.1/fudstop/apis/whale/
--rw-rw-rw-   0        0        0        0 2024-03-27 06:54:53.000000 fudstop-2.9.1/fudstop/apis/whale/__init__.py
--rw-rw-rw-   0        0        0    42102 2024-03-27 21:07:42.000000 fudstop-2.9.1/fudstop/apis/whale/whale_models.py
--rw-rw-rw-   0        0        0     7065 2024-03-27 21:07:56.000000 fudstop-2.9.1/fudstop/apis/whale/whale_sdk.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.882234 fudstop-2.9.1/fudstop/apis/y_finance/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/apis/y_finance/__init__.py
--rw-rw-rw-   0        0        0     9028 2024-02-18 15:18:29.000000 fudstop-2.9.1/fudstop/apis/y_finance/yf_sdk.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.883233 fudstop-2.9.1/fudstop/database_/
--rw-rw-rw-   0        0        0    66479 2024-02-18 06:41:46.000000 fudstop-2.9.1/fudstop/database_/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.886234 fudstop-2.9.1/fudstop/discord_/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/discord_/__init__.py
--rw-rw-rw-   0        0        0     2191 2024-01-11 18:10:55.000000 fudstop-2.9.1/fudstop/discord_/autocomp.py
--rw-rw-rw-   0        0        0    63312 2024-05-30 22:08:03.000000 fudstop-2.9.1/fudstop/discord_/bot.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.887233 fudstop-2.9.1/fudstop/discord_/bot_menus/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/discord_/bot_menus/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.889234 fudstop-2.9.1/fudstop/discord_/bot_menus/modals/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/discord_/bot_menus/modals/__init__.py
--rw-rw-rw-   0        0        0     2226 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/discord_/bot_menus/modals/dalle_modal.py
--rw-rw-rw-   0        0        0    13054 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/discord_/bot_menus/modals/options_modal.py
--rw-rw-rw-   0        0        0     3597 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/discord_/bot_menus/pagination.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.902234 fudstop-2.9.1/fudstop/discord_/cogs/
--rw-rw-rw-   0        0        0     4305 2024-01-07 18:05:54.000000 fudstop-2.9.1/fudstop/discord_/cogs/__init__.py
--rw-rw-rw-   0        0        0    20340 2024-01-06 18:32:34.000000 fudstop-2.9.1/fudstop/discord_/cogs/accounting.py
--rw-rw-rw-   0        0        0    11559 2024-01-06 18:29:35.000000 fudstop-2.9.1/fudstop/discord_/cogs/assistant.py
--rw-rw-rw-   0        0        0    11795 2024-02-06 17:49:34.000000 fudstop-2.9.1/fudstop/discord_/cogs/database.py
--rw-rw-rw-   0        0        0    12937 2024-01-11 18:07:47.000000 fudstop-2.9.1/fudstop/discord_/cogs/earnings.py
--rw-rw-rw-   0        0        0     2104 2024-01-06 18:30:08.000000 fudstop-2.9.1/fudstop/discord_/cogs/fed_print.py
--rw-rw-rw-   0        0        0     4463 2024-01-11 18:16:25.000000 fudstop-2.9.1/fudstop/discord_/cogs/filter.py
--rw-rw-rw-   0        0        0    34896 2024-01-11 18:17:51.000000 fudstop-2.9.1/fudstop/discord_/cogs/fiscal_service.py
--rw-rw-rw-   0        0        0     4482 2024-01-07 16:10:05.000000 fudstop-2.9.1/fudstop/discord_/cogs/gex.py
--rw-rw-rw-   0        0        0     6390 2024-02-07 19:46:50.000000 fudstop-2.9.1/fudstop/discord_/cogs/gpt.py
--rw-rw-rw-   0        0        0     3906 2024-02-17 21:04:28.000000 fudstop-2.9.1/fudstop/discord_/cogs/ibrs.py
--rw-rw-rw-   0        0        0     2313 2024-01-06 18:31:02.000000 fudstop-2.9.1/fudstop/discord_/cogs/main_view.py
--rw-rw-rw-   0        0        0    29489 2024-04-06 03:42:15.000000 fudstop-2.9.1/fudstop/discord_/cogs/options.py
--rw-rw-rw-   0        0        0     3827 2024-01-11 18:16:07.000000 fudstop-2.9.1/fudstop/discord_/cogs/plays.py
--rw-rw-rw-   0        0        0     3428 2024-01-06 18:35:15.000000 fudstop-2.9.1/fudstop/discord_/cogs/register.py
--rw-rw-rw-   0        0        0     3800 2024-01-06 18:31:37.000000 fudstop-2.9.1/fudstop/discord_/cogs/spx.py
--rw-rw-rw-   0        0        0     9302 2024-01-11 18:15:53.000000 fudstop-2.9.1/fudstop/discord_/cogs/strategy.py
--rw-rw-rw-   0        0        0     2776 2024-01-06 18:31:52.000000 fudstop-2.9.1/fudstop/discord_/cogs/ta.py
--rw-rw-rw-   0        0        0     3071 2024-01-06 18:32:00.000000 fudstop-2.9.1/fudstop/discord_/cogs/weather.py
--rw-rw-rw-   0        0        0     1346 2024-01-06 18:32:07.000000 fudstop-2.9.1/fudstop/discord_/cogs/webull.py
--rw-rw-rw-   0        0        0    11097 2024-01-06 18:32:21.000000 fudstop-2.9.1/fudstop/discord_/cogs/yfin.py
--rw-rw-rw-   0        0        0     1843 2024-01-14 21:57:53.000000 fudstop-2.9.1/fudstop/discord_/database_getter.py
--rw-rw-rw-   0        0        0     6337 2024-01-11 18:07:47.000000 fudstop-2.9.1/fudstop/discord_/discord_rsi.py
--rw-rw-rw-   0        0        0     3697 2024-01-06 18:23:33.000000 fudstop-2.9.1/fudstop/discord_/embeddings.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.913237 fudstop-2.9.1/fudstop/examples/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/examples/__init__.py
--rw-rw-rw-   0        0        0     1134 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/examples/ecfr_test.py
--rw-rw-rw-   0        0        0      178 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/examples/fed_print_test.py
--rw-rw-rw-   0        0        0      237 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/examples/fed_reg_test.py
--rw-rw-rw-   0        0        0      258 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/examples/nasdaq_test.py
--rw-rw-rw-   0        0        0      181 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/examples/newyork_fed_test.py
--rw-rw-rw-   0        0        0     3793 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/examples/ofr_test.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.920238 fudstop-2.9.1/fudstop/examples/polygonio/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/examples/polygonio/__init__.py
--rw-rw-rw-   0        0        0     1392 2024-01-11 18:07:47.000000 fudstop-2.9.1/fudstop/examples/polygonio/aggregates_second.py
--rw-rw-rw-   0        0        0      709 2024-01-11 18:07:47.000000 fudstop-2.9.1/fudstop/examples/polygonio/company_info.py
--rw-rw-rw-   0        0        0     2345 2024-01-07 23:40:02.000000 fudstop-2.9.1/fudstop/examples/polygonio/get_all_options.py
--rw-rw-rw-   0        0        0      379 2024-01-11 18:07:47.000000 fudstop-2.9.1/fudstop/examples/polygonio/get_all_tickers.py
--rw-rw-rw-   0        0        0      611 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/examples/polygonio/get_near_the_money.py
--rw-rw-rw-   0        0        0     2307 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/examples/polygonio/get_option_aggs.py
--rw-rw-rw-   0        0        0     1190 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/examples/polygonio/get_option_rsi.py
--rw-rw-rw-   0        0        0     3751 2024-01-06 00:03:40.000000 fudstop-2.9.1/fudstop/examples/polygonio/get_option_trades.py
--rw-rw-rw-   0        0        0     2409 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/examples/polygonio/get_ticker_aggs.py
--rw-rw-rw-   0        0        0      683 2024-01-11 18:07:47.000000 fudstop-2.9.1/fudstop/examples/polygonio/market_news.py
--rw-rw-rw-   0        0        0     1305 2024-01-11 18:07:47.000000 fudstop-2.9.1/fudstop/examples/polygonio/polygon_test.py
--rw-rw-rw-   0        0        0     1134 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/examples/scripty.py
--rw-rw-rw-   0        0        0     1871 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/examples/stocksera_test.py
--rw-rw-rw-   0        0        0      776 2024-01-06 17:35:55.000000 fudstop-2.9.1/fudstop/examples/test.py
--rw-rw-rw-   0        0        0     2721 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/examples/test_gex.py
--rw-rw-rw-   0        0        0      284 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/examples/test_insert.py
--rw-rw-rw-   0        0        0     2255 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/examples/test_openai.py
--rw-rw-rw-   0        0        0      698 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/examples/test_opts.py
--rw-rw-rw-   0        0        0      637 2024-05-30 22:08:03.000000 fudstop-2.9.1/fudstop/examples/test_screener.py
--rw-rw-rw-   0        0        0     4324 2024-01-11 18:10:12.000000 fudstop-2.9.1/fudstop/examples/test_sec.py
--rw-rw-rw-   0        0        0     1758 2024-01-11 18:11:03.000000 fudstop-2.9.1/fudstop/examples/test_webull.py
--rw-rw-rw-   0        0        0        0 2024-01-08 17:00:41.000000 fudstop-2.9.1/fudstop/examples/tests_discord.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.922238 fudstop-2.9.1/fudstop/examples/webull/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/examples/webull/__init__.py
--rw-rw-rw-   0        0        0      805 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/examples/webull/markets_example.py
--rw-rw-rw-   0        0        0     2439 2024-01-05 23:27:36.000000 fudstop-2.9.1/fudstop/examples/webull/trade_example.py
--rw-rw-rw-   0        0        0     7753 2024-01-11 18:14:32.000000 fudstop-2.9.1/fudstop/options_filter.py
--rw-rw-rw-   0        0        0    21800 2024-01-11 18:09:07.000000 fudstop-2.9.1/fudstop/plots.py
--rw-rw-rw-   0        0        0    15233 2024-01-11 18:14:18.000000 fudstop-2.9.1/fudstop/schema.py
--rw-rw-rw-   0        0        0      490 2024-02-04 05:36:05.000000 fudstop-2.9.1/fudstop/wet.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:42:55.751013 fudstop-2.9.1/fudstop.egg-info/
--rw-rw-rw-   0        0        0     7616 2024-06-01 22:42:55.000000 fudstop-2.9.1/fudstop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    11843 2024-06-01 22:42:55.000000 fudstop-2.9.1/fudstop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 22:42:55.000000 fudstop-2.9.1/fudstop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     4026 2024-06-01 22:42:55.000000 fudstop-2.9.1/fudstop.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-06-01 22:42:55.000000 fudstop-2.9.1/fudstop.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 22:42:55.931745 fudstop-2.9.1/setup.cfg
--rw-rw-rw-   0        0        0      363 2024-06-01 22:42:38.000000 fudstop-2.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.266527 fudstop-2.9.2/
+-rw-rw-rw-   0        0        0     7616 2024-06-01 22:52:08.265526 fudstop-2.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2341 2024-01-05 23:27:36.000000 fudstop-2.9.2/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.115383 fudstop-2.9.2/app/
+-rw-rw-rw-   0        0        0    43348 2024-01-23 23:29:23.000000 fudstop-2.9.2/app/__init__.py
+-rw-rw-rw-   0        0        0     4011 2024-01-12 03:32:55.000000 fudstop-2.9.2/app/fetcher.py
+-rw-rw-rw-   0        0        0    17884 2024-01-12 06:07:09.000000 fudstop-2.9.2/app/fudstop_info.py
+-rw-rw-rw-   0        0        0    38553 2024-01-12 03:47:25.000000 fudstop-2.9.2/app/helpers.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.119383 fudstop-2.9.2/fudstop/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.125384 fudstop-2.9.2/fudstop/_markets/
+-rw-rw-rw-   0        0        0     1327 2024-01-18 15:18:48.000000 fudstop-2.9.2/fudstop/_markets/__init__.py
+-rw-rw-rw-   0        0        0     2440 2024-02-22 04:18:16.000000 fudstop-2.9.2/fudstop/_markets/analyzers.py
+-rw-rw-rw-   0        0        0    67237 2024-02-07 15:09:55.000000 fudstop-2.9.2/fudstop/_markets/embeddings.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.128383 fudstop-2.9.2/fudstop/_markets/finished/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:49:02.000000 fudstop-2.9.2/fudstop/_markets/finished/__init__.py
+-rw-rw-rw-   0        0        0    25622 2024-01-21 19:47:09.000000 fudstop-2.9.2/fudstop/_markets/finished/db_manager.py
+-rw-rw-rw-   0        0        0     2530 2023-10-12 23:34:06.000000 fudstop-2.9.2/fudstop/_markets/finished/economic_data.py
+-rw-rw-rw-   0        0        0    53472 2024-02-11 04:30:33.000000 fudstop-2.9.2/fudstop/_markets/finished/master_class.py
+-rw-rw-rw-   0        0        0     9960 2024-06-01 22:49:43.000000 fudstop-2.9.2/fudstop/_markets/finished/td9_states.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.130384 fudstop-2.9.2/fudstop/_markets/list_sets/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/_markets/list_sets/__init__.py
+-rw-rw-rw-   0        0        0    92394 2024-02-22 03:17:43.000000 fudstop-2.9.2/fudstop/_markets/list_sets/dicts.py
+-rw-rw-rw-   0        0        0    88831 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/_markets/list_sets/saved_tickers.py
+-rw-rw-rw-   0        0        0   125429 2024-01-17 16:34:32.000000 fudstop-2.9.2/fudstop/_markets/list_sets/ticker_lists.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.135388 fudstop-2.9.2/fudstop/_markets/market_handlers/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/_markets/market_handlers/__init__.py
+-rw-rw-rw-   0        0        0     1265 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/_markets/market_handlers/cfg.py
+-rw-rw-rw-   0        0        0     1491 2024-01-09 04:43:27.000000 fudstop-2.9.2/fudstop/_markets/market_handlers/crypto.py
+-rw-rw-rw-   0        0        0    17424 2024-02-12 18:43:10.000000 fudstop-2.9.2/fudstop/_markets/market_handlers/database_.py
+-rw-rw-rw-   0        0        0      768 2024-01-09 05:02:23.000000 fudstop-2.9.2/fudstop/_markets/market_handlers/forex.py
+-rw-rw-rw-   0        0        0     1770 2024-01-08 17:15:06.000000 fudstop-2.9.2/fudstop/_markets/market_handlers/indices.py
+-rw-rw-rw-   0        0        0   762960 2024-01-11 23:53:54.000000 fudstop-2.9.2/fudstop/_markets/market_handlers/list_sets.py
+-rw-rw-rw-   0        0        0    13155 2024-01-11 17:06:04.000000 fudstop-2.9.2/fudstop/_markets/market_handlers/options.py
+-rw-rw-rw-   0        0        0     3929 2024-01-09 21:38:56.000000 fudstop-2.9.2/fudstop/_markets/market_handlers/stocks.py
+-rw-rw-rw-   0        0        0     1166 2024-01-12 17:40:54.000000 fudstop-2.9.2/fudstop/_markets/monitor.py
+-rw-rw-rw-   0        0        0    31105 2024-02-12 14:30:27.000000 fudstop-2.9.2/fudstop/_markets/multimarkets.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.135388 fudstop-2.9.2/fudstop/_markets/plotting/
+-rw-rw-rw-   0        0        0     1814 2024-01-13 01:48:40.000000 fudstop-2.9.2/fudstop/_markets/plotting/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.137388 fudstop-2.9.2/fudstop/_markets/reference_markets/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/_markets/reference_markets/__init__.py
+-rw-rw-rw-   0        0        0     1400 2024-01-08 00:31:15.000000 fudstop-2.9.2/fudstop/_markets/reference_markets/conditional_scans.py
+-rw-rw-rw-   0        0        0     8389 2024-01-10 04:38:30.000000 fudstop-2.9.2/fudstop/_markets/reference_markets/reference_market.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.144388 fudstop-2.9.2/fudstop/_markets/scripts/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/_markets/scripts/__init__.py
+-rw-rw-rw-   0        0        0      846 2024-01-20 18:45:32.000000 fudstop-2.9.2/fudstop/_markets/scripts/all_polygon_options.py
+-rw-rw-rw-   0        0        0      703 2024-06-01 22:50:21.000000 fudstop-2.9.2/fudstop/_markets/scripts/all_webull_options.py
+-rw-rw-rw-   0        0        0     1208 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/_markets/scripts/generation.py
+-rw-rw-rw-   0        0        0     1351 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/_markets/scripts/million_dollar_trades.py
+-rw-rw-rw-   0        0        0     1533 2024-01-18 14:58:07.000000 fudstop-2.9.2/fudstop/_markets/scripts/option_scripts.py
+-rw-rw-rw-   0        0        0    20865 2024-06-01 22:49:57.000000 fudstop-2.9.2/fudstop/_markets/scripts/options_market.py
+-rw-rw-rw-   0        0        0     2961 2024-01-11 18:09:48.000000 fudstop-2.9.2/fudstop/_markets/scripts/options_volume_analysis.py
+-rw-rw-rw-   0        0        0     1942 2024-01-11 18:07:34.000000 fudstop-2.9.2/fudstop/_markets/scripts/rsi_2_4_8.py
+-rw-rw-rw-   0        0        0     2172 2024-01-24 23:43:15.000000 fudstop-2.9.2/fudstop/_markets/scripts/rsi_screener.py
+-rw-rw-rw-   0        0        0     1197 2024-01-20 05:06:57.000000 fudstop-2.9.2/fudstop/_markets/scripts/ssr_scanner.py
+-rw-rw-rw-   0        0        0     7315 2024-01-23 17:20:40.000000 fudstop-2.9.2/fudstop/_markets/scripts/stock_market.py
+-rw-rw-rw-   0        0        0     6271 2024-01-12 19:46:21.000000 fudstop-2.9.2/fudstop/_markets/scripts/td9_states.py
+-rw-rw-rw-   0        0        0    14287 2024-02-06 18:37:20.000000 fudstop-2.9.2/fudstop/_markets/scripts/universal_snapshot.py
+-rw-rw-rw-   0        0        0    13782 2024-01-25 20:46:06.000000 fudstop-2.9.2/fudstop/_markets/stock_market.py
+-rw-rw-rw-   0        0        0     1893 2024-01-10 18:26:30.000000 fudstop-2.9.2/fudstop/_markets/webhook_dicts.py
+-rw-rw-rw-   0        0        0    14911 2024-01-06 18:40:07.000000 fudstop-2.9.2/fudstop/all_helpers.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.145388 fudstop-2.9.2/fudstop/apis/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.146387 fudstop-2.9.2/fudstop/apis/_asyncpg/
+-rw-rw-rw-   0        0        0        0 2024-02-29 20:06:59.000000 fudstop-2.9.2/fudstop/apis/_asyncpg/__init__.py
+-rw-rw-rw-   0        0        0    15085 2024-04-14 15:28:27.000000 fudstop-2.9.2/fudstop/apis/_asyncpg/asyncpg_sdk.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.146387 fudstop-2.9.2/fudstop/apis/_datetime/
+-rw-rw-rw-   0        0        0        0 2024-02-29 20:06:52.000000 fudstop-2.9.2/fudstop/apis/_datetime/__init__.py
+-rw-rw-rw-   0        0        0     3440 2024-04-14 23:10:42.000000 fudstop-2.9.2/fudstop/apis/_datetime/datetime_sdk.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.148436 fudstop-2.9.2/fudstop/apis/_openai/
+-rw-rw-rw-   0        0        0        0 2024-01-07 17:40:15.000000 fudstop-2.9.2/fudstop/apis/_openai/__init__.py
+-rw-rw-rw-   0        0        0     4824 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/_openai/agent.py
+-rw-rw-rw-   0        0        0     7552 2024-03-07 23:34:16.000000 fudstop-2.9.2/fudstop/apis/_openai/openai_sdk.py
+-rw-rw-rw-   0        0        0    27388 2024-02-25 03:36:21.000000 fudstop-2.9.2/fudstop/apis/_openai/tools_shcema.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.149437 fudstop-2.9.2/fudstop/apis/_pandas/
+-rw-rw-rw-   0        0        0        0 2024-02-29 20:42:25.000000 fudstop-2.9.2/fudstop/apis/_pandas/__init__.py
+-rw-rw-rw-   0        0        0      226 2024-02-29 20:44:07.000000 fudstop-2.9.2/fudstop/apis/_pandas/pandas_sdk.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.150436 fudstop-2.9.2/fudstop/apis/_selenium/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/_selenium/__init__.py
+-rw-rw-rw-   0        0        0     1863 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/_selenium/selenium_sdk.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.151436 fudstop-2.9.2/fudstop/apis/alphaquery/
+-rw-rw-rw-   0        0        0        0 2024-04-13 21:58:49.000000 fudstop-2.9.2/fudstop/apis/alphaquery/__init__.py
+-rw-rw-rw-   0        0        0     3639 2024-04-13 22:04:47.000000 fudstop-2.9.2/fudstop/apis/alphaquery/alpha_sdk.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.152436 fudstop-2.9.2/fudstop/apis/alphaquery/models/
+-rw-rw-rw-   0        0        0        0 2024-04-13 21:58:58.000000 fudstop-2.9.2/fudstop/apis/alphaquery/models/__init__.py
+-rw-rw-rw-   0        0        0       41 2024-04-13 21:59:36.000000 fudstop-2.9.2/fudstop/apis/alphaquery/models/alpha_models.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.153436 fudstop-2.9.2/fudstop/apis/caselaw/
+-rw-rw-rw-   0        0        0        0 2024-05-09 17:36:00.000000 fudstop-2.9.2/fudstop/apis/caselaw/__init__.py
+-rw-rw-rw-   0        0        0     3199 2024-05-09 18:13:57.000000 fudstop-2.9.2/fudstop/apis/caselaw/caselaw_models.py
+-rw-rw-rw-   0        0        0     1709 2024-05-09 18:18:24.000000 fudstop-2.9.2/fudstop/apis/caselaw/caselaw_sdk.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.155436 fudstop-2.9.2/fudstop/apis/cfr/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/cfr/__init__.py
+-rw-rw-rw-   0        0        0     3742 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/cfr/cfr_2.0.py
+-rw-rw-rw-   0        0        0       87 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/cfr/cfr_helpers.py
+-rw-rw-rw-   0        0        0     7590 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/cfr/cfr_sdk.py
+-rw-rw-rw-   0        0        0     2525 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/cfr/title_12.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.157437 fudstop-2.9.2/fudstop/apis/datalink/
+-rw-rw-rw-   0        0        0        0 2024-03-25 21:17:59.000000 fudstop-2.9.2/fudstop/apis/datalink/__init__.py
+-rw-rw-rw-   0        0        0     2661 2024-03-27 07:04:34.000000 fudstop-2.9.2/fudstop/apis/datalink/datalink_sdk.py
+-rw-rw-rw-   0        0        0     2609 2024-03-25 21:32:23.000000 fudstop-2.9.2/fudstop/apis/datalink/models.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.158436 fudstop-2.9.2/fudstop/apis/discord_/
+-rw-rw-rw-   0        0        0     4430 2024-01-08 04:14:36.000000 fudstop-2.9.2/fudstop/apis/discord_/__init__.py
+-rw-rw-rw-   0        0        0    12863 2024-02-23 01:28:51.000000 fudstop-2.9.2/fudstop/apis/discord_/discord_sdk.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.159436 fudstop-2.9.2/fudstop/apis/discord_/models/
+-rw-rw-rw-   0        0        0        0 2024-01-18 14:52:13.000000 fudstop-2.9.2/fudstop/apis/discord_/models/__init__.py
+-rw-rw-rw-   0        0        0     5431 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/discord_/models/application_commands.py
+-rw-rw-rw-   0        0        0     2767 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/discord_/models/search.py
+-rw-rw-rw-   0        0        0     1101 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/discord_/models/webhooks.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.160436 fudstop-2.9.2/fudstop/apis/earnings_whisper/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/earnings_whisper/__init__.py
+-rw-rw-rw-   0        0        0    12823 2024-03-25 21:47:38.000000 fudstop-2.9.2/fudstop/apis/earnings_whisper/ew_models.py
+-rw-rw-rw-   0        0        0     4016 2024-03-25 21:44:18.000000 fudstop-2.9.2/fudstop/apis/earnings_whisper/ew_sdk.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.161436 fudstop-2.9.2/fudstop/apis/fastcase/
+-rw-rw-rw-   0        0        0        0 2024-04-14 15:00:18.000000 fudstop-2.9.2/fudstop/apis/fastcase/__init__.py
+-rw-rw-rw-   0        0        0     6212 2024-05-02 15:37:07.000000 fudstop-2.9.2/fudstop/apis/fastcase/fastcase_sdk.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.163436 fudstop-2.9.2/fudstop/apis/fed_print/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/fed_print/__init__.py
+-rw-rw-rw-   0        0        0     2908 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/fed_print/fed_print_sync.py
+-rw-rw-rw-   0        0        0     5322 2024-02-24 20:29:40.000000 fudstop-2.9.2/fudstop/apis/fed_print/fedprint_models.py
+-rw-rw-rw-   0        0        0     3354 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/fed_print/fedprint_sdk.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.165437 fudstop-2.9.2/fudstop/apis/federal_register/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/federal_register/__init__.py
+-rw-rw-rw-   0        0        0     3075 2024-02-25 17:21:39.000000 fudstop-2.9.2/fudstop/apis/federal_register/fed_register_sdk.py
+-rw-rw-rw-   0        0        0     2924 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/federal_register/fed_register_sync.py
+-rw-rw-rw-   0        0        0     2904 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/federal_register/register_models.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.166437 fudstop-2.9.2/fudstop/apis/gexbot/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/gexbot/__init__.py
+-rw-rw-rw-   0        0        0     4095 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/gexbot/gexbot.py
+-rw-rw-rw-   0        0        0     4139 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/gexbot/models.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.167436 fudstop-2.9.2/fudstop/apis/gpts/
+-rw-rw-rw-   0        0        0      231 2024-01-08 03:41:52.000000 fudstop-2.9.2/fudstop/apis/gpts/DiscoAI.py
+-rw-rw-rw-   0        0        0        2 2024-01-08 03:38:45.000000 fudstop-2.9.2/fudstop/apis/gpts/__init__.py
+-rw-rw-rw-   0        0        0    36326 2024-05-01 23:15:01.000000 fudstop-2.9.2/fudstop/apis/helpers.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.169436 fudstop-2.9.2/fudstop/apis/master/
+-rw-rw-rw-   0        0        0        0 2024-02-25 05:43:46.000000 fudstop-2.9.2/fudstop/apis/master/__init__.py
+-rw-rw-rw-   0        0        0     1459 2024-02-25 09:02:57.000000 fudstop-2.9.2/fudstop/apis/master/master_helpers.py
+-rw-rw-rw-   0        0        0    29980 2024-06-01 22:49:47.000000 fudstop-2.9.2/fudstop/apis/master/master_sdk.py
+-rw-rw-rw-   0        0        0    34633 2024-02-25 09:11:27.000000 fudstop-2.9.2/fudstop/apis/master/tools.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.171435 fudstop-2.9.2/fudstop/apis/misc/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/misc/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.172436 fudstop-2.9.2/fudstop/apis/misc/models/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/misc/models/__init__.py
+-rw-rw-rw-   0        0        0      249 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/misc/models/unsplash_models.py
+-rw-rw-rw-   0        0        0     2204 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/misc/models/weather_models.py
+-rw-rw-rw-   0        0        0      869 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/misc/unsplash.py
+-rw-rw-rw-   0        0        0     1790 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/misc/weather.py
+-rw-rw-rw-   0        0        0      294 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/misc/weather_helpers.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.173436 fudstop-2.9.2/fudstop/apis/nasdaq/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/nasdaq/__init__.py
+-rw-rw-rw-   0        0        0     4200 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/nasdaq/nasdaq_lists.py
+-rw-rw-rw-   0        0        0    12177 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/nasdaq/nasdaq_sdk.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.175436 fudstop-2.9.2/fudstop/apis/newyork_fed/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/newyork_fed/__init__.py
+-rw-rw-rw-   0        0        0    14970 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/newyork_fed/models.py
+-rw-rw-rw-   0        0        0    22750 2024-03-27 00:32:52.000000 fudstop-2.9.2/fudstop/apis/newyork_fed/newyork_fed_sdk.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.176436 fudstop-2.9.2/fudstop/apis/occ/
+-rw-rw-rw-   0        0        0        0 2024-01-12 03:42:31.000000 fudstop-2.9.2/fudstop/apis/occ/__init__.py
+-rw-rw-rw-   0        0        0    30622 2024-05-19 05:08:45.000000 fudstop-2.9.2/fudstop/apis/occ/occ_models.py
+-rw-rw-rw-   0        0        0    14163 2024-05-29 23:33:52.000000 fudstop-2.9.2/fudstop/apis/occ/occ_sdk.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.177435 fudstop-2.9.2/fudstop/apis/ofr/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/ofr/__init__.py
+-rw-rw-rw-   0        0        0    37577 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/ofr/ofr_list_sets.py
+-rw-rw-rw-   0        0        0     5462 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/ofr/ofr_sdk.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.179435 fudstop-2.9.2/fudstop/apis/oic/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/oic/__init__.py
+-rw-rw-rw-   0        0        0    16116 2024-01-07 16:09:24.000000 fudstop-2.9.2/fudstop/apis/oic/async_oic_sdk.py
+-rw-rw-rw-   0        0        0    11292 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/oic/oic_models.py
+-rw-rw-rw-   0        0        0     4938 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/oic/oic_sdk.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.183436 fudstop-2.9.2/fudstop/apis/polygonio/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/polygonio/__init__.py
+-rw-rw-rw-   0        0        0    31100 2024-05-27 03:23:49.000000 fudstop-2.9.2/fudstop/apis/polygonio/async_polygon_sdk.py
+-rw-rw-rw-   0        0        0     2368 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/polygonio/db_polygon.py
+-rw-rw-rw-   0        0        0    47011 2024-01-10 15:38:01.000000 fudstop-2.9.2/fudstop/apis/polygonio/mapping.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.187437 fudstop-2.9.2/fudstop/apis/polygonio/models/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/polygonio/models/__init__.py
+-rw-rw-rw-   0        0        0     1330 2024-04-13 19:03:08.000000 fudstop-2.9.2/fudstop/apis/polygonio/models/aggregates.py
+-rw-rw-rw-   0        0        0     1319 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/polygonio/models/company_info.py
+-rw-rw-rw-   0        0        0     4295 2024-04-14 23:13:19.000000 fudstop-2.9.2/fudstop/apis/polygonio/models/gainers_losers.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.189436 fudstop-2.9.2/fudstop/apis/polygonio/models/option_models/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/polygonio/models/option_models/__init__.py
+-rw-rw-rw-   0        0        0     5734 2024-01-12 15:43:51.000000 fudstop-2.9.2/fudstop/apis/polygonio/models/option_models/option_snapshot.py
+-rw-rw-rw-   0        0        0     7043 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/polygonio/models/option_models/universal_option.py
+-rw-rw-rw-   0        0        0    58850 2024-05-23 05:30:03.000000 fudstop-2.9.2/fudstop/apis/polygonio/models/option_models/universal_snapshot.py
+-rw-rw-rw-   0        0        0     7964 2024-05-25 04:33:35.000000 fudstop-2.9.2/fudstop/apis/polygonio/models/technicals.py
+-rw-rw-rw-   0        0        0     2271 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/polygonio/models/ticker_news.py
+-rw-rw-rw-   0        0        0     3801 2024-01-07 01:51:36.000000 fudstop-2.9.2/fudstop/apis/polygonio/models/ticker_snapshot.py
+-rw-rw-rw-   0        0        0     5787 2024-01-21 19:53:33.000000 fudstop-2.9.2/fudstop/apis/polygonio/models/trades.py
+-rw-rw-rw-   0        0        0    13162 2024-06-01 18:36:58.000000 fudstop-2.9.2/fudstop/apis/polygonio/polygon_database.py
+-rw-rw-rw-   0        0        0    41160 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/polygonio/polygon_helpers.py
+-rw-rw-rw-   0        0        0    71525 2024-05-23 05:18:46.000000 fudstop-2.9.2/fudstop/apis/polygonio/polygon_options.py
+-rw-rw-rw-   0        0        0     3692 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/polygonio/polygon_sync.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.190436 fudstop-2.9.2/fudstop/apis/polygonio/scripts/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/polygonio/scripts/__init__.py
+-rw-rw-rw-   0        0        0     2267 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/polygonio/scripts/daily_aggregates.py
+-rw-rw-rw-   0        0        0     1716 2024-02-04 09:29:32.000000 fudstop-2.9.2/fudstop/apis/polygonio/scripts/rsi.py
+-rw-rw-rw-   0        0        0     9164 2024-03-01 01:05:43.000000 fudstop-2.9.2/fudstop/apis/polygonio/technicals.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.191435 fudstop-2.9.2/fudstop/apis/rapid/
+-rw-rw-rw-   0        0        0        0 2024-05-08 03:47:05.000000 fudstop-2.9.2/fudstop/apis/rapid/__init__.py
+-rw-rw-rw-   0        0        0     8348 2024-05-08 05:03:43.000000 fudstop-2.9.2/fudstop/apis/rapid/rapid_models.py
+-rw-rw-rw-   0        0        0     3188 2024-05-08 04:36:56.000000 fudstop-2.9.2/fudstop/apis/rapid/rapid_sdk.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.194437 fudstop-2.9.2/fudstop/apis/rss/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/rss/__init__.py
+-rw-rw-rw-   0        0        0      736 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/rss/rss_helpers.py
+-rw-rw-rw-   0        0        0     1497 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/rss/rss_models.py
+-rw-rw-rw-   0        0        0    10360 2024-01-11 18:07:47.000000 fudstop-2.9.2/fudstop/apis/rss/rss_sdk.py
+-rw-rw-rw-   0        0        0    10203 2024-01-11 18:07:47.000000 fudstop-2.9.2/fudstop/apis/rss/snyc_rss.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.194437 fudstop-2.9.2/fudstop/apis/sec/
+-rw-rw-rw-   0        0        0        0 2024-02-29 20:06:34.000000 fudstop-2.9.2/fudstop/apis/sec/__init__.py
+-rw-rw-rw-   0        0        0     8441 2024-02-29 22:33:02.000000 fudstop-2.9.2/fudstop/apis/sec/sec_sdk.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.195437 fudstop-2.9.2/fudstop/apis/stocksera_/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/stocksera_/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.203436 fudstop-2.9.2/fudstop/apis/stocksera_/models/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/stocksera_/models/__init__.py
+-rw-rw-rw-   0        0        0      487 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/stocksera_/models/borrowed_shares.py
+-rw-rw-rw-   0        0        0      827 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/stocksera_/models/daily_treasury.py
+-rw-rw-rw-   0        0        0      747 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/stocksera_/models/ftds.py
+-rw-rw-rw-   0        0        0      871 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/stocksera_/models/highest_shorted.py
+-rw-rw-rw-   0        0        0      813 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/stocksera_/models/inflation.py
+-rw-rw-rw-   0        0        0     1062 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/stocksera_/models/insider_trades.py
+-rw-rw-rw-   0        0        0      667 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/stocksera_/models/jim_cramer.py
+-rw-rw-rw-   0        0        0      850 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/stocksera_/models/jobless_claims.py
+-rw-rw-rw-   0        0        0     1043 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/stocksera_/models/low_float.py
+-rw-rw-rw-   0        0        0      660 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/stocksera_/models/market_news.py
+-rw-rw-rw-   0        0        0    21824 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/stocksera_/models/models.py
+-rw-rw-rw-   0        0        0      676 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/stocksera_/models/news_sentiment.py
+-rw-rw-rw-   0        0        0      693 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/stocksera_/models/retail_sales.py
+-rw-rw-rw-   0        0        0      708 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/stocksera_/models/reverse_repo.py
+-rw-rw-rw-   0        0        0      777 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/stocksera_/models/sec_filings.py
+-rw-rw-rw-   0        0        0      789 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/stocksera_/models/short_volume.py
+-rw-rw-rw-   0        0        0    19676 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/stocksera_/stocksera_.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.204436 fudstop-2.9.2/fudstop/apis/treasury/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/treasury/__init__.py
+-rw-rw-rw-   0        0        0    10964 2024-01-20 19:15:58.000000 fudstop-2.9.2/fudstop/apis/treasury/treasury_models.py
+-rw-rw-rw-   0        0        0    10281 2024-01-20 19:16:09.000000 fudstop-2.9.2/fudstop/apis/treasury/treasury_sdk.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.206436 fudstop-2.9.2/fudstop/apis/udio/
+-rw-rw-rw-   0        0        0        0 2024-05-04 04:08:21.000000 fudstop-2.9.2/fudstop/apis/udio/__init__.py
+-rw-rw-rw-   0        0        0     4605 2024-05-04 04:20:04.000000 fudstop-2.9.2/fudstop/apis/udio/imps.py
+-rw-rw-rw-   0        0        0     2130 2024-05-04 05:03:43.000000 fudstop-2.9.2/fudstop/apis/udio/udio_sdk.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.213436 fudstop-2.9.2/fudstop/apis/webull/
+-rw-rw-rw-   0        0        0     4945 2024-01-15 22:06:39.000000 fudstop-2.9.2/fudstop/apis/webull/__init__.py
+-rw-rw-rw-   0        0        0    12127 2024-01-23 03:47:19.000000 fudstop-2.9.2/fudstop/apis/webull/database_manager.py
+-rw-rw-rw-   0        0        0     2732 2024-01-11 18:10:25.000000 fudstop-2.9.2/fudstop/apis/webull/get_volume_analysis.py
+-rw-rw-rw-   0        0        0    10628 2024-01-11 18:10:17.000000 fudstop-2.9.2/fudstop/apis/webull/modal.py
+-rw-rw-rw-   0        0        0     5320 2024-01-10 21:10:43.000000 fudstop-2.9.2/fudstop/apis/webull/opt_modal.py
+-rw-rw-rw-   0        0        0     4916 2024-06-01 20:48:50.000000 fudstop-2.9.2/fudstop/apis/webull/option_data.py
+-rw-rw-rw-   0        0        0     9390 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/webull/options.py
+-rw-rw-rw-   0        0        0     6520 2024-05-15 23:10:46.000000 fudstop-2.9.2/fudstop/apis/webull/screener_models.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.221437 fudstop-2.9.2/fudstop/apis/webull/trade_models/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/webull/trade_models/__init__.py
+-rw-rw-rw-   0        0        0     2030 2024-02-18 21:14:42.000000 fudstop-2.9.2/fudstop/apis/webull/trade_models/analyst_ratings.py
+-rw-rw-rw-   0        0        0    15033 2024-05-31 23:04:35.000000 fudstop-2.9.2/fudstop/apis/webull/trade_models/capital_flow.py
+-rw-rw-rw-   0        0        0     2147 2024-02-24 19:57:32.000000 fudstop-2.9.2/fudstop/apis/webull/trade_models/company_brief.py
+-rw-rw-rw-   0        0        0     2235 2024-01-23 05:04:58.000000 fudstop-2.9.2/fudstop/apis/webull/trade_models/cost_distribution.py
+-rw-rw-rw-   0        0        0     1053 2024-02-18 19:14:15.000000 fudstop-2.9.2/fudstop/apis/webull/trade_models/etf_holdings.py
+-rw-rw-rw-   0        0        0     1727 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/webull/trade_models/events.py
+-rw-rw-rw-   0        0        0    19884 2024-02-18 19:14:03.000000 fudstop-2.9.2/fudstop/apis/webull/trade_models/financials.py
+-rw-rw-rw-   0        0        0     3780 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/webull/trade_models/forecast_evaluator.py
+-rw-rw-rw-   0        0        0     3500 2024-02-18 18:48:35.000000 fudstop-2.9.2/fudstop/apis/webull/trade_models/institutional_holdings.py
+-rw-rw-rw-   0        0        0     1335 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/webull/trade_models/news.py
+-rw-rw-rw-   0        0        0     2235 2024-05-14 22:42:18.000000 fudstop-2.9.2/fudstop/apis/webull/trade_models/order_flow.py
+-rw-rw-rw-   0        0        0     1195 2024-03-01 01:13:55.000000 fudstop-2.9.2/fudstop/apis/webull/trade_models/price_streamer.py
+-rw-rw-rw-   0        0        0      601 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/webull/trade_models/short_interest.py
+-rw-rw-rw-   0        0        0     4714 2024-04-29 02:51:39.000000 fudstop-2.9.2/fudstop/apis/webull/trade_models/stock_quote.py
+-rw-rw-rw-   0        0        0    11042 2024-03-07 17:43:34.000000 fudstop-2.9.2/fudstop/apis/webull/trade_models/ticker_query.py
+-rw-rw-rw-   0        0        0     1314 2024-01-13 16:23:06.000000 fudstop-2.9.2/fudstop/apis/webull/trade_models/volume_analysis.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.222436 fudstop-2.9.2/fudstop/apis/webull/trader_models/
+-rw-rw-rw-   0        0        0        0 2024-04-23 22:21:57.000000 fudstop-2.9.2/fudstop/apis/webull/trader_models/__init__.py
+-rw-rw-rw-   0        0        0    39759 2024-04-28 00:01:42.000000 fudstop-2.9.2/fudstop/apis/webull/trader_models/trader_models.py
+-rw-rw-rw-   0        0        0    13181 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/webull/webull_helpers.py
+-rw-rw-rw-   0        0        0    12274 2024-02-25 06:46:04.000000 fudstop-2.9.2/fudstop/apis/webull/webull_markets.py
+-rw-rw-rw-   0        0        0    17501 2024-06-01 19:46:46.000000 fudstop-2.9.2/fudstop/apis/webull/webull_option_screener.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.224435 fudstop-2.9.2/fudstop/apis/webull/webull_options/
+-rw-rw-rw-   0        0        0        0 2024-01-06 17:03:12.000000 fudstop-2.9.2/fudstop/apis/webull/webull_options/__init__.py
+-rw-rw-rw-   0        0        0    15129 2024-01-06 17:03:12.000000 fudstop-2.9.2/fudstop/apis/webull/webull_options/helpers.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.225437 fudstop-2.9.2/fudstop/apis/webull/webull_options/models/
+-rw-rw-rw-   0        0        0        0 2024-01-06 17:03:12.000000 fudstop-2.9.2/fudstop/apis/webull/webull_options/models/__init__.py
+-rw-rw-rw-   0        0        0    36853 2024-02-06 07:52:04.000000 fudstop-2.9.2/fudstop/apis/webull/webull_options/models/db_manager.py
+-rw-rw-rw-   0        0        0    23420 2024-04-23 23:48:07.000000 fudstop-2.9.2/fudstop/apis/webull/webull_options/models/options_data.py
+-rw-rw-rw-   0        0        0    47807 2024-06-01 21:40:11.000000 fudstop-2.9.2/fudstop/apis/webull/webull_options/webull_options.py
+-rw-rw-rw-   0        0        0      957 2024-02-06 07:52:33.000000 fudstop-2.9.2/fudstop/apis/webull/webull_options/webull_trader.py
+-rw-rw-rw-   0        0        0    35666 2024-01-21 19:47:41.000000 fudstop-2.9.2/fudstop/apis/webull/webull_options.py
+-rw-rw-rw-   0        0        0    14292 2024-06-01 19:10:13.000000 fudstop-2.9.2/fudstop/apis/webull/webull_paper_trader.py
+-rw-rw-rw-   0        0        0     9106 2024-01-18 22:00:22.000000 fudstop-2.9.2/fudstop/apis/webull/webull_parsing.py
+-rw-rw-rw-   0        0        0     7309 2024-05-15 23:18:59.000000 fudstop-2.9.2/fudstop/apis/webull/webull_trader.py
+-rw-rw-rw-   0        0        0    32001 2024-05-31 22:58:27.000000 fudstop-2.9.2/fudstop/apis/webull/webull_trading.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.226436 fudstop-2.9.2/fudstop/apis/whale/
+-rw-rw-rw-   0        0        0        0 2024-03-27 06:54:53.000000 fudstop-2.9.2/fudstop/apis/whale/__init__.py
+-rw-rw-rw-   0        0        0    42102 2024-03-27 21:07:42.000000 fudstop-2.9.2/fudstop/apis/whale/whale_models.py
+-rw-rw-rw-   0        0        0     7065 2024-03-27 21:07:56.000000 fudstop-2.9.2/fudstop/apis/whale/whale_sdk.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.227435 fudstop-2.9.2/fudstop/apis/y_finance/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/apis/y_finance/__init__.py
+-rw-rw-rw-   0        0        0     9028 2024-02-18 15:18:29.000000 fudstop-2.9.2/fudstop/apis/y_finance/yf_sdk.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.228436 fudstop-2.9.2/fudstop/database_/
+-rw-rw-rw-   0        0        0    66479 2024-02-18 06:41:46.000000 fudstop-2.9.2/fudstop/database_/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.230436 fudstop-2.9.2/fudstop/discord_/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/discord_/__init__.py
+-rw-rw-rw-   0        0        0     2191 2024-01-11 18:10:55.000000 fudstop-2.9.2/fudstop/discord_/autocomp.py
+-rw-rw-rw-   0        0        0    63312 2024-05-30 22:08:03.000000 fudstop-2.9.2/fudstop/discord_/bot.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.231437 fudstop-2.9.2/fudstop/discord_/bot_menus/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/discord_/bot_menus/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.233440 fudstop-2.9.2/fudstop/discord_/bot_menus/modals/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/discord_/bot_menus/modals/__init__.py
+-rw-rw-rw-   0        0        0     2226 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/discord_/bot_menus/modals/dalle_modal.py
+-rw-rw-rw-   0        0        0    13054 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/discord_/bot_menus/modals/options_modal.py
+-rw-rw-rw-   0        0        0     3597 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/discord_/bot_menus/pagination.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.243440 fudstop-2.9.2/fudstop/discord_/cogs/
+-rw-rw-rw-   0        0        0     4305 2024-01-07 18:05:54.000000 fudstop-2.9.2/fudstop/discord_/cogs/__init__.py
+-rw-rw-rw-   0        0        0    20340 2024-01-06 18:32:34.000000 fudstop-2.9.2/fudstop/discord_/cogs/accounting.py
+-rw-rw-rw-   0        0        0    11559 2024-01-06 18:29:35.000000 fudstop-2.9.2/fudstop/discord_/cogs/assistant.py
+-rw-rw-rw-   0        0        0    11795 2024-02-06 17:49:34.000000 fudstop-2.9.2/fudstop/discord_/cogs/database.py
+-rw-rw-rw-   0        0        0    12937 2024-01-11 18:07:47.000000 fudstop-2.9.2/fudstop/discord_/cogs/earnings.py
+-rw-rw-rw-   0        0        0     2104 2024-01-06 18:30:08.000000 fudstop-2.9.2/fudstop/discord_/cogs/fed_print.py
+-rw-rw-rw-   0        0        0     4483 2024-06-01 22:49:52.000000 fudstop-2.9.2/fudstop/discord_/cogs/filter.py
+-rw-rw-rw-   0        0        0    34896 2024-01-11 18:17:51.000000 fudstop-2.9.2/fudstop/discord_/cogs/fiscal_service.py
+-rw-rw-rw-   0        0        0     4482 2024-01-07 16:10:05.000000 fudstop-2.9.2/fudstop/discord_/cogs/gex.py
+-rw-rw-rw-   0        0        0     6390 2024-02-07 19:46:50.000000 fudstop-2.9.2/fudstop/discord_/cogs/gpt.py
+-rw-rw-rw-   0        0        0     3906 2024-02-17 21:04:28.000000 fudstop-2.9.2/fudstop/discord_/cogs/ibrs.py
+-rw-rw-rw-   0        0        0     2313 2024-01-06 18:31:02.000000 fudstop-2.9.2/fudstop/discord_/cogs/main_view.py
+-rw-rw-rw-   0        0        0    29489 2024-04-06 03:42:15.000000 fudstop-2.9.2/fudstop/discord_/cogs/options.py
+-rw-rw-rw-   0        0        0     3847 2024-06-01 22:50:04.000000 fudstop-2.9.2/fudstop/discord_/cogs/plays.py
+-rw-rw-rw-   0        0        0     3428 2024-01-06 18:35:15.000000 fudstop-2.9.2/fudstop/discord_/cogs/register.py
+-rw-rw-rw-   0        0        0     3800 2024-01-06 18:31:37.000000 fudstop-2.9.2/fudstop/discord_/cogs/spx.py
+-rw-rw-rw-   0        0        0     9322 2024-06-01 22:50:57.000000 fudstop-2.9.2/fudstop/discord_/cogs/strategy.py
+-rw-rw-rw-   0        0        0     2776 2024-01-06 18:31:52.000000 fudstop-2.9.2/fudstop/discord_/cogs/ta.py
+-rw-rw-rw-   0        0        0     3071 2024-01-06 18:32:00.000000 fudstop-2.9.2/fudstop/discord_/cogs/weather.py
+-rw-rw-rw-   0        0        0     1346 2024-01-06 18:32:07.000000 fudstop-2.9.2/fudstop/discord_/cogs/webull.py
+-rw-rw-rw-   0        0        0    11097 2024-01-06 18:32:21.000000 fudstop-2.9.2/fudstop/discord_/cogs/yfin.py
+-rw-rw-rw-   0        0        0     1843 2024-01-14 21:57:53.000000 fudstop-2.9.2/fudstop/discord_/database_getter.py
+-rw-rw-rw-   0        0        0     6337 2024-01-11 18:07:47.000000 fudstop-2.9.2/fudstop/discord_/discord_rsi.py
+-rw-rw-rw-   0        0        0     3697 2024-01-06 18:23:33.000000 fudstop-2.9.2/fudstop/discord_/embeddings.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.251526 fudstop-2.9.2/fudstop/examples/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/examples/__init__.py
+-rw-rw-rw-   0        0        0     1134 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/examples/ecfr_test.py
+-rw-rw-rw-   0        0        0      178 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/examples/fed_print_test.py
+-rw-rw-rw-   0        0        0      237 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/examples/fed_reg_test.py
+-rw-rw-rw-   0        0        0      258 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/examples/nasdaq_test.py
+-rw-rw-rw-   0        0        0      181 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/examples/newyork_fed_test.py
+-rw-rw-rw-   0        0        0     3793 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/examples/ofr_test.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.256526 fudstop-2.9.2/fudstop/examples/polygonio/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/examples/polygonio/__init__.py
+-rw-rw-rw-   0        0        0     1392 2024-01-11 18:07:47.000000 fudstop-2.9.2/fudstop/examples/polygonio/aggregates_second.py
+-rw-rw-rw-   0        0        0      709 2024-01-11 18:07:47.000000 fudstop-2.9.2/fudstop/examples/polygonio/company_info.py
+-rw-rw-rw-   0        0        0     2345 2024-01-07 23:40:02.000000 fudstop-2.9.2/fudstop/examples/polygonio/get_all_options.py
+-rw-rw-rw-   0        0        0      379 2024-01-11 18:07:47.000000 fudstop-2.9.2/fudstop/examples/polygonio/get_all_tickers.py
+-rw-rw-rw-   0        0        0      611 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/examples/polygonio/get_near_the_money.py
+-rw-rw-rw-   0        0        0     2307 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/examples/polygonio/get_option_aggs.py
+-rw-rw-rw-   0        0        0     1190 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/examples/polygonio/get_option_rsi.py
+-rw-rw-rw-   0        0        0     3751 2024-01-06 00:03:40.000000 fudstop-2.9.2/fudstop/examples/polygonio/get_option_trades.py
+-rw-rw-rw-   0        0        0     2409 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/examples/polygonio/get_ticker_aggs.py
+-rw-rw-rw-   0        0        0      683 2024-01-11 18:07:47.000000 fudstop-2.9.2/fudstop/examples/polygonio/market_news.py
+-rw-rw-rw-   0        0        0     1305 2024-01-11 18:07:47.000000 fudstop-2.9.2/fudstop/examples/polygonio/polygon_test.py
+-rw-rw-rw-   0        0        0     1134 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/examples/scripty.py
+-rw-rw-rw-   0        0        0     1871 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/examples/stocksera_test.py
+-rw-rw-rw-   0        0        0      776 2024-01-06 17:35:55.000000 fudstop-2.9.2/fudstop/examples/test.py
+-rw-rw-rw-   0        0        0     2721 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/examples/test_gex.py
+-rw-rw-rw-   0        0        0      284 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/examples/test_insert.py
+-rw-rw-rw-   0        0        0     2255 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/examples/test_openai.py
+-rw-rw-rw-   0        0        0      698 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/examples/test_opts.py
+-rw-rw-rw-   0        0        0      637 2024-05-30 22:08:03.000000 fudstop-2.9.2/fudstop/examples/test_screener.py
+-rw-rw-rw-   0        0        0     4324 2024-01-11 18:10:12.000000 fudstop-2.9.2/fudstop/examples/test_sec.py
+-rw-rw-rw-   0        0        0     1758 2024-01-11 18:11:03.000000 fudstop-2.9.2/fudstop/examples/test_webull.py
+-rw-rw-rw-   0        0        0        0 2024-01-08 17:00:41.000000 fudstop-2.9.2/fudstop/examples/tests_discord.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.258526 fudstop-2.9.2/fudstop/examples/webull/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/examples/webull/__init__.py
+-rw-rw-rw-   0        0        0      805 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/examples/webull/markets_example.py
+-rw-rw-rw-   0        0        0     2439 2024-01-05 23:27:36.000000 fudstop-2.9.2/fudstop/examples/webull/trade_example.py
+-rw-rw-rw-   0        0        0     7773 2024-06-01 22:49:37.000000 fudstop-2.9.2/fudstop/options_filter.py
+-rw-rw-rw-   0        0        0    21800 2024-01-11 18:09:07.000000 fudstop-2.9.2/fudstop/plots.py
+-rw-rw-rw-   0        0        0    15253 2024-06-01 22:50:09.000000 fudstop-2.9.2/fudstop/schema.py
+-rw-rw-rw-   0        0        0      490 2024-02-04 05:36:05.000000 fudstop-2.9.2/fudstop/wet.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:08.121383 fudstop-2.9.2/fudstop.egg-info/
+-rw-rw-rw-   0        0        0     7616 2024-06-01 22:52:07.000000 fudstop-2.9.2/fudstop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    11843 2024-06-01 22:52:08.000000 fudstop-2.9.2/fudstop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 22:52:07.000000 fudstop-2.9.2/fudstop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     4026 2024-06-01 22:52:07.000000 fudstop-2.9.2/fudstop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-06-01 22:52:07.000000 fudstop-2.9.2/fudstop.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 22:52:08.266527 fudstop-2.9.2/setup.cfg
+-rw-rw-rw-   0        0        0      363 2024-06-01 22:51:58.000000 fudstop-2.9.2/setup.py
```

### Comparing `fudstop-2.9.1/PKG-INFO` & `fudstop-2.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fudstop
-Version: 2.9.1
+Version: 2.9.2
 Requires-Dist: absl-py==2.0.0
 Requires-Dist: aiofiles==23.2.1
 Requires-Dist: aiohttp==3.9.5
 Requires-Dist: aiosignal==1.3.1
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: anyio==3.7.1
 Requires-Dist: appdirs==1.4.4
```

### Comparing `fudstop-2.9.1/README.md` & `fudstop-2.9.2/README.md`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/app/__init__.py` & `fudstop-2.9.2/app/__init__.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/app/fetcher.py` & `fudstop-2.9.2/app/fetcher.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/app/fudstop_info.py` & `fudstop-2.9.2/app/fudstop_info.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/app/helpers.py` & `fudstop-2.9.2/app/helpers.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/_markets/__init__.py` & `fudstop-2.9.2/fudstop/_markets/__init__.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/_markets/analyzers.py` & `fudstop-2.9.2/fudstop/_markets/analyzers.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/_markets/embeddings.py` & `fudstop-2.9.2/fudstop/_markets/embeddings.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/_markets/finished/db_manager.py` & `fudstop-2.9.2/fudstop/_markets/finished/db_manager.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/_markets/finished/economic_data.py` & `fudstop-2.9.2/fudstop/_markets/finished/economic_data.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/_markets/finished/master_class.py` & `fudstop-2.9.2/fudstop/_markets/finished/master_class.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/_markets/finished/td9_states.py` & `fudstop-2.9.2/fudstop/_markets/finished/td9_states.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import aiohttp
 import asyncio
 import pandas as pd
 from apis.helpers import calculate_countdown, calculate_setup
 from aiohttp.client_exceptions import ClientConnectorError, ClientOSError
 import aiohttp
 from asyncio import Semaphore
-from webull_options.webull_options import WebullOptions
+from fudstop.apis.webull.webull_options.webull_options import WebullOptions
 from db_manager import DbManager as DatabaseManager
 sema = Semaphore(10)
 db = DatabaseManager(host='localhost', port=5432, user='chuck', password='fud', database='markets')
 wb_opts = WebullOptions(user='chuck', database='markets')
 fudstop_logo = os.environ.get('fudstop_logo')
 min1_td9 = os.environ.get("min1_td9")
 min5_td9 = os.environ.get("min5_td9")
```

### Comparing `fudstop-2.9.1/fudstop/_markets/list_sets/dicts.py` & `fudstop-2.9.2/fudstop/_markets/list_sets/dicts.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/_markets/list_sets/saved_tickers.py` & `fudstop-2.9.2/fudstop/_markets/list_sets/saved_tickers.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/_markets/list_sets/ticker_lists.py` & `fudstop-2.9.2/fudstop/_markets/list_sets/ticker_lists.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/_markets/market_handlers/cfg.py` & `fudstop-2.9.2/fudstop/_markets/market_handlers/cfg.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/_markets/market_handlers/crypto.py` & `fudstop-2.9.2/fudstop/_markets/market_handlers/crypto.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/_markets/market_handlers/database_.py` & `fudstop-2.9.2/fudstop/_markets/market_handlers/database_.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/_markets/market_handlers/forex.py` & `fudstop-2.9.2/fudstop/_markets/market_handlers/forex.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/_markets/market_handlers/indices.py` & `fudstop-2.9.2/fudstop/_markets/market_handlers/indices.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/_markets/market_handlers/list_sets.py` & `fudstop-2.9.2/fudstop/_markets/market_handlers/list_sets.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/_markets/market_handlers/options.py` & `fudstop-2.9.2/fudstop/_markets/market_handlers/options.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/_markets/market_handlers/stocks.py` & `fudstop-2.9.2/fudstop/_markets/market_handlers/stocks.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/_markets/monitor.py` & `fudstop-2.9.2/fudstop/_markets/monitor.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/_markets/multimarkets.py` & `fudstop-2.9.2/fudstop/_markets/multimarkets.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/_markets/plotting/__init__.py` & `fudstop-2.9.2/fudstop/_markets/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/_markets/reference_markets/conditional_scans.py` & `fudstop-2.9.2/fudstop/_markets/reference_markets/conditional_scans.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/_markets/reference_markets/reference_market.py` & `fudstop-2.9.2/fudstop/_markets/reference_markets/reference_market.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/_markets/scripts/all_polygon_options.py` & `fudstop-2.9.2/fudstop/_markets/scripts/all_polygon_options.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/_markets/scripts/all_webull_options.py` & `fudstop-2.9.2/fudstop/_markets/scripts/all_webull_options.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 load_dotenv()
 import sys
 from pathlib import Path
 # Add the project directory to the sys.path
 project_dir = str(Path(__file__).resolve().parents[1])
 if project_dir not in sys.path:
     sys.path.append(project_dir)
-from webull_options.webull_options import WebullOptions
+from fudstop.apis.webull.webull_options.webull_options import WebullOptions
 
 db = WebullOptions(database='markets', user='chuck')
 
 
 
 import asyncio
```

### Comparing `fudstop-2.9.1/fudstop/_markets/scripts/generation.py` & `fudstop-2.9.2/fudstop/_markets/scripts/generation.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/_markets/scripts/million_dollar_trades.py` & `fudstop-2.9.2/fudstop/_markets/scripts/million_dollar_trades.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/_markets/scripts/option_scripts.py` & `fudstop-2.9.2/fudstop/_markets/scripts/option_scripts.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/_markets/scripts/options_market.py` & `fudstop-2.9.2/fudstop/_markets/scripts/options_market.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from dotenv import load_dotenv
 load_dotenv()
 from discord_webhook import AsyncDiscordWebhook, DiscordEmbed
 from _markets.webhook_dicts import option_conditions_hooks
 from _markets.embeddings import sized_trade_embed, specials_embed_2, dip_specials_embed, index_surge_embed, dip_specials_embed_2_super, theta_resistant_embed
 from polygon.websocket import WebSocketClient, WebSocketMessage, Market, Feed
 from apis.polygonio.polygon_options import PolygonOptions
-from webull_options.webull_options import WebullOptions
+from fudstop.apis.webull.webull_options.webull_options import WebullOptions
 
 
 
 from _markets.list_sets.dicts import hex_color_dict as hex_colors
 
 from apis.polygonio.polygon_database import PolygonDatabase
 import asyncio
```

### Comparing `fudstop-2.9.1/fudstop/_markets/scripts/options_volume_analysis.py` & `fudstop-2.9.2/fudstop/_markets/scripts/options_volume_analysis.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/_markets/scripts/rsi_2_4_8.py` & `fudstop-2.9.2/fudstop/_markets/scripts/rsi_2_4_8.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/_markets/scripts/rsi_screener.py` & `fudstop-2.9.2/fudstop/_markets/scripts/rsi_screener.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/_markets/scripts/ssr_scanner.py` & `fudstop-2.9.2/fudstop/_markets/scripts/ssr_scanner.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/_markets/scripts/stock_market.py` & `fudstop-2.9.2/fudstop/_markets/scripts/stock_market.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/_markets/scripts/td9_states.py` & `fudstop-2.9.2/fudstop/_markets/scripts/td9_states.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/_markets/scripts/universal_snapshot.py` & `fudstop-2.9.2/fudstop/_markets/scripts/universal_snapshot.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/_markets/stock_market.py` & `fudstop-2.9.2/fudstop/_markets/stock_market.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/_markets/webhook_dicts.py` & `fudstop-2.9.2/fudstop/_markets/webhook_dicts.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/all_helpers.py` & `fudstop-2.9.2/fudstop/all_helpers.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/_asyncpg/asyncpg_sdk.py` & `fudstop-2.9.2/fudstop/apis/_asyncpg/asyncpg_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/_datetime/datetime_sdk.py` & `fudstop-2.9.2/fudstop/apis/_datetime/datetime_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/_openai/agent.py` & `fudstop-2.9.2/fudstop/apis/_openai/agent.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/_openai/openai_sdk.py` & `fudstop-2.9.2/fudstop/apis/_openai/openai_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/_openai/tools_shcema.py` & `fudstop-2.9.2/fudstop/apis/_openai/tools_shcema.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/_selenium/selenium_sdk.py` & `fudstop-2.9.2/fudstop/apis/_selenium/selenium_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/alphaquery/alpha_sdk.py` & `fudstop-2.9.2/fudstop/apis/alphaquery/alpha_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/caselaw/caselaw_models.py` & `fudstop-2.9.2/fudstop/apis/caselaw/caselaw_models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/caselaw/caselaw_sdk.py` & `fudstop-2.9.2/fudstop/apis/caselaw/caselaw_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/cfr/cfr_2.0.py` & `fudstop-2.9.2/fudstop/apis/cfr/cfr_2.0.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/cfr/cfr_sdk.py` & `fudstop-2.9.2/fudstop/apis/cfr/cfr_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/cfr/title_12.py` & `fudstop-2.9.2/fudstop/apis/cfr/title_12.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/datalink/datalink_sdk.py` & `fudstop-2.9.2/fudstop/apis/datalink/datalink_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/datalink/models.py` & `fudstop-2.9.2/fudstop/apis/datalink/models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/discord_/__init__.py` & `fudstop-2.9.2/fudstop/apis/discord_/__init__.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/discord_/discord_sdk.py` & `fudstop-2.9.2/fudstop/apis/discord_/discord_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/discord_/models/application_commands.py` & `fudstop-2.9.2/fudstop/apis/discord_/models/application_commands.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/discord_/models/search.py` & `fudstop-2.9.2/fudstop/apis/discord_/models/search.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/discord_/models/webhooks.py` & `fudstop-2.9.2/fudstop/apis/discord_/models/webhooks.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/earnings_whisper/ew_models.py` & `fudstop-2.9.2/fudstop/apis/earnings_whisper/ew_models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/earnings_whisper/ew_sdk.py` & `fudstop-2.9.2/fudstop/apis/earnings_whisper/ew_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/fastcase/fastcase_sdk.py` & `fudstop-2.9.2/fudstop/apis/fastcase/fastcase_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/fed_print/fed_print_sync.py` & `fudstop-2.9.2/fudstop/apis/fed_print/fed_print_sync.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/fed_print/fedprint_models.py` & `fudstop-2.9.2/fudstop/apis/fed_print/fedprint_models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/fed_print/fedprint_sdk.py` & `fudstop-2.9.2/fudstop/apis/fed_print/fedprint_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/federal_register/fed_register_sdk.py` & `fudstop-2.9.2/fudstop/apis/federal_register/fed_register_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/federal_register/fed_register_sync.py` & `fudstop-2.9.2/fudstop/apis/federal_register/fed_register_sync.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/federal_register/register_models.py` & `fudstop-2.9.2/fudstop/apis/federal_register/register_models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/gexbot/gexbot.py` & `fudstop-2.9.2/fudstop/apis/gexbot/gexbot.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/gexbot/models.py` & `fudstop-2.9.2/fudstop/apis/gexbot/models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/helpers.py` & `fudstop-2.9.2/fudstop/apis/helpers.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/master/master_helpers.py` & `fudstop-2.9.2/fudstop/apis/master/master_helpers.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/master/master_sdk.py` & `fudstop-2.9.2/fudstop/apis/master/master_sdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from apis.webull.webull_markets import WebullMarkets
 from apis.occ.occ_sdk import occSDK
 from apis.newyork_fed.newyork_fed_sdk import FedNewyork
 from apis.fed_print.fedprint_sdk import FedPrint
 from apis.earnings_whisper.ew_sdk import EarningsWhisper
 from apis.federal_register.fed_register_sdk import FedRegisterSDK
 from apis.treasury.treasury_sdk import Treasury
-from webull_options.webull_options import WebullOptions
+from fudstop.apis.webull.webull_options.webull_options import WebullOptions
 from datetime import datetime, timedelta
 from openai import OpenAI
 import httpx
 import asyncio
 from datetime import date, datetime
 etf_list = pd.read_csv('etf_list.csv')
 class CustomJSONEncoder(json.JSONEncoder):
```

### Comparing `fudstop-2.9.1/fudstop/apis/master/tools.py` & `fudstop-2.9.2/fudstop/apis/master/tools.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/misc/models/weather_models.py` & `fudstop-2.9.2/fudstop/apis/misc/models/weather_models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/misc/unsplash.py` & `fudstop-2.9.2/fudstop/apis/misc/unsplash.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/misc/weather.py` & `fudstop-2.9.2/fudstop/apis/misc/weather.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/nasdaq/nasdaq_lists.py` & `fudstop-2.9.2/fudstop/apis/nasdaq/nasdaq_lists.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/nasdaq/nasdaq_sdk.py` & `fudstop-2.9.2/fudstop/apis/nasdaq/nasdaq_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/newyork_fed/models.py` & `fudstop-2.9.2/fudstop/apis/newyork_fed/models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/newyork_fed/newyork_fed_sdk.py` & `fudstop-2.9.2/fudstop/apis/newyork_fed/newyork_fed_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/occ/occ_models.py` & `fudstop-2.9.2/fudstop/apis/occ/occ_models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/occ/occ_sdk.py` & `fudstop-2.9.2/fudstop/apis/occ/occ_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/ofr/ofr_list_sets.py` & `fudstop-2.9.2/fudstop/apis/ofr/ofr_list_sets.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/ofr/ofr_sdk.py` & `fudstop-2.9.2/fudstop/apis/ofr/ofr_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/oic/async_oic_sdk.py` & `fudstop-2.9.2/fudstop/apis/oic/async_oic_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/oic/oic_models.py` & `fudstop-2.9.2/fudstop/apis/oic/oic_models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/oic/oic_sdk.py` & `fudstop-2.9.2/fudstop/apis/oic/oic_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/polygonio/async_polygon_sdk.py` & `fudstop-2.9.2/fudstop/apis/polygonio/async_polygon_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/polygonio/db_polygon.py` & `fudstop-2.9.2/fudstop/apis/polygonio/db_polygon.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/polygonio/mapping.py` & `fudstop-2.9.2/fudstop/apis/polygonio/mapping.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/polygonio/models/aggregates.py` & `fudstop-2.9.2/fudstop/apis/polygonio/models/aggregates.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/polygonio/models/company_info.py` & `fudstop-2.9.2/fudstop/apis/polygonio/models/company_info.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/polygonio/models/gainers_losers.py` & `fudstop-2.9.2/fudstop/apis/polygonio/models/gainers_losers.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/polygonio/models/option_models/option_snapshot.py` & `fudstop-2.9.2/fudstop/apis/polygonio/models/option_models/option_snapshot.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/polygonio/models/option_models/universal_option.py` & `fudstop-2.9.2/fudstop/apis/polygonio/models/option_models/universal_option.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/polygonio/models/option_models/universal_snapshot.py` & `fudstop-2.9.2/fudstop/apis/polygonio/models/option_models/universal_snapshot.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/polygonio/models/technicals.py` & `fudstop-2.9.2/fudstop/apis/polygonio/models/technicals.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/polygonio/models/ticker_news.py` & `fudstop-2.9.2/fudstop/apis/polygonio/models/ticker_news.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/polygonio/models/ticker_snapshot.py` & `fudstop-2.9.2/fudstop/apis/polygonio/models/ticker_snapshot.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/polygonio/models/trades.py` & `fudstop-2.9.2/fudstop/apis/polygonio/models/trades.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/polygonio/polygon_database.py` & `fudstop-2.9.2/fudstop/apis/polygonio/polygon_database.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/polygonio/polygon_helpers.py` & `fudstop-2.9.2/fudstop/apis/polygonio/polygon_helpers.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/polygonio/polygon_options.py` & `fudstop-2.9.2/fudstop/apis/polygonio/polygon_options.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/polygonio/polygon_sync.py` & `fudstop-2.9.2/fudstop/apis/polygonio/polygon_sync.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/polygonio/scripts/daily_aggregates.py` & `fudstop-2.9.2/fudstop/apis/polygonio/scripts/daily_aggregates.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/polygonio/scripts/rsi.py` & `fudstop-2.9.2/fudstop/apis/polygonio/scripts/rsi.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/polygonio/technicals.py` & `fudstop-2.9.2/fudstop/apis/polygonio/technicals.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/rapid/rapid_models.py` & `fudstop-2.9.2/fudstop/apis/rapid/rapid_models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/rapid/rapid_sdk.py` & `fudstop-2.9.2/fudstop/apis/rapid/rapid_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/rss/rss_helpers.py` & `fudstop-2.9.2/fudstop/apis/rss/rss_helpers.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/rss/rss_models.py` & `fudstop-2.9.2/fudstop/apis/rss/rss_models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/rss/rss_sdk.py` & `fudstop-2.9.2/fudstop/apis/rss/rss_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/rss/snyc_rss.py` & `fudstop-2.9.2/fudstop/apis/rss/snyc_rss.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/sec/sec_sdk.py` & `fudstop-2.9.2/fudstop/apis/sec/sec_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/stocksera_/models/daily_treasury.py` & `fudstop-2.9.2/fudstop/apis/stocksera_/models/daily_treasury.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/stocksera_/models/ftds.py` & `fudstop-2.9.2/fudstop/apis/stocksera_/models/ftds.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/stocksera_/models/highest_shorted.py` & `fudstop-2.9.2/fudstop/apis/stocksera_/models/highest_shorted.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/stocksera_/models/inflation.py` & `fudstop-2.9.2/fudstop/apis/stocksera_/models/inflation.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/stocksera_/models/insider_trades.py` & `fudstop-2.9.2/fudstop/apis/stocksera_/models/insider_trades.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/stocksera_/models/jim_cramer.py` & `fudstop-2.9.2/fudstop/apis/stocksera_/models/jim_cramer.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/stocksera_/models/jobless_claims.py` & `fudstop-2.9.2/fudstop/apis/stocksera_/models/jobless_claims.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/stocksera_/models/low_float.py` & `fudstop-2.9.2/fudstop/apis/stocksera_/models/low_float.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/stocksera_/models/market_news.py` & `fudstop-2.9.2/fudstop/apis/stocksera_/models/market_news.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/stocksera_/models/models.py` & `fudstop-2.9.2/fudstop/apis/stocksera_/models/models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/stocksera_/models/news_sentiment.py` & `fudstop-2.9.2/fudstop/apis/stocksera_/models/news_sentiment.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/stocksera_/models/retail_sales.py` & `fudstop-2.9.2/fudstop/apis/stocksera_/models/retail_sales.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/stocksera_/models/reverse_repo.py` & `fudstop-2.9.2/fudstop/apis/stocksera_/models/reverse_repo.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/stocksera_/models/sec_filings.py` & `fudstop-2.9.2/fudstop/apis/stocksera_/models/sec_filings.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/stocksera_/models/short_volume.py` & `fudstop-2.9.2/fudstop/apis/stocksera_/models/short_volume.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/stocksera_/stocksera_.py` & `fudstop-2.9.2/fudstop/apis/stocksera_/stocksera_.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/treasury/treasury_models.py` & `fudstop-2.9.2/fudstop/apis/treasury/treasury_models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/treasury/treasury_sdk.py` & `fudstop-2.9.2/fudstop/apis/treasury/treasury_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/udio/imps.py` & `fudstop-2.9.2/fudstop/apis/udio/imps.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/udio/udio_sdk.py` & `fudstop-2.9.2/fudstop/apis/udio/udio_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/webull/__init__.py` & `fudstop-2.9.2/fudstop/apis/webull/__init__.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/webull/database_manager.py` & `fudstop-2.9.2/fudstop/apis/webull/database_manager.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/webull/get_volume_analysis.py` & `fudstop-2.9.2/fudstop/apis/webull/get_volume_analysis.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/webull/modal.py` & `fudstop-2.9.2/fudstop/apis/webull/modal.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/webull/opt_modal.py` & `fudstop-2.9.2/fudstop/apis/webull/opt_modal.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/webull/option_data.py` & `fudstop-2.9.2/fudstop/apis/webull/option_data.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/webull/options.py` & `fudstop-2.9.2/fudstop/apis/webull/options.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/webull/screener_models.py` & `fudstop-2.9.2/fudstop/apis/webull/screener_models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/webull/trade_models/analyst_ratings.py` & `fudstop-2.9.2/fudstop/apis/webull/trade_models/analyst_ratings.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/webull/trade_models/capital_flow.py` & `fudstop-2.9.2/fudstop/apis/webull/trade_models/capital_flow.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/webull/trade_models/company_brief.py` & `fudstop-2.9.2/fudstop/apis/webull/trade_models/company_brief.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/webull/trade_models/cost_distribution.py` & `fudstop-2.9.2/fudstop/apis/webull/trade_models/cost_distribution.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/webull/trade_models/etf_holdings.py` & `fudstop-2.9.2/fudstop/apis/webull/trade_models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/webull/trade_models/events.py` & `fudstop-2.9.2/fudstop/apis/webull/trade_models/events.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/webull/trade_models/financials.py` & `fudstop-2.9.2/fudstop/apis/webull/trade_models/financials.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/webull/trade_models/forecast_evaluator.py` & `fudstop-2.9.2/fudstop/apis/webull/trade_models/forecast_evaluator.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/webull/trade_models/institutional_holdings.py` & `fudstop-2.9.2/fudstop/apis/webull/trade_models/institutional_holdings.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/webull/trade_models/news.py` & `fudstop-2.9.2/fudstop/apis/webull/trade_models/news.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/webull/trade_models/order_flow.py` & `fudstop-2.9.2/fudstop/apis/webull/trade_models/order_flow.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/webull/trade_models/price_streamer.py` & `fudstop-2.9.2/fudstop/apis/webull/trade_models/price_streamer.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/webull/trade_models/short_interest.py` & `fudstop-2.9.2/fudstop/apis/webull/trade_models/short_interest.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/webull/trade_models/stock_quote.py` & `fudstop-2.9.2/fudstop/apis/webull/trade_models/stock_quote.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/webull/trade_models/ticker_query.py` & `fudstop-2.9.2/fudstop/apis/webull/trade_models/ticker_query.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/webull/trade_models/volume_analysis.py` & `fudstop-2.9.2/fudstop/apis/webull/trade_models/volume_analysis.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/webull/trader_models/trader_models.py` & `fudstop-2.9.2/fudstop/apis/webull/trader_models/trader_models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/webull/webull_helpers.py` & `fudstop-2.9.2/fudstop/apis/webull/webull_helpers.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/webull/webull_markets.py` & `fudstop-2.9.2/fudstop/apis/webull/webull_markets.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/webull/webull_option_screener.py` & `fudstop-2.9.2/fudstop/apis/webull/webull_option_screener.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/webull/webull_options/helpers.py` & `fudstop-2.9.2/fudstop/apis/webull/webull_options/helpers.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/webull/webull_options/models/db_manager.py` & `fudstop-2.9.2/fudstop/apis/webull/webull_options/models/db_manager.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/webull/webull_options/models/options_data.py` & `fudstop-2.9.2/fudstop/apis/webull/webull_options/models/options_data.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/webull/webull_options/webull_options.py` & `fudstop-2.9.2/fudstop/apis/webull/webull_options/webull_options.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/webull/webull_options/webull_trader.py` & `fudstop-2.9.2/fudstop/apis/webull/webull_options/webull_trader.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/webull/webull_options.py` & `fudstop-2.9.2/fudstop/apis/webull/webull_options.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/webull/webull_paper_trader.py` & `fudstop-2.9.2/fudstop/apis/webull/webull_paper_trader.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/webull/webull_parsing.py` & `fudstop-2.9.2/fudstop/apis/webull/webull_parsing.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/webull/webull_trader.py` & `fudstop-2.9.2/fudstop/apis/webull/webull_trader.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/webull/webull_trading.py` & `fudstop-2.9.2/fudstop/apis/webull/webull_trading.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/whale/whale_models.py` & `fudstop-2.9.2/fudstop/apis/whale/whale_models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/whale/whale_sdk.py` & `fudstop-2.9.2/fudstop/apis/whale/whale_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/apis/y_finance/yf_sdk.py` & `fudstop-2.9.2/fudstop/apis/y_finance/yf_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/database_/__init__.py` & `fudstop-2.9.2/fudstop/database_/__init__.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/discord_/autocomp.py` & `fudstop-2.9.2/fudstop/discord_/autocomp.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/discord_/bot.py` & `fudstop-2.9.2/fudstop/discord_/bot.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/discord_/bot_menus/modals/dalle_modal.py` & `fudstop-2.9.2/fudstop/discord_/bot_menus/modals/dalle_modal.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/discord_/bot_menus/modals/options_modal.py` & `fudstop-2.9.2/fudstop/discord_/bot_menus/modals/options_modal.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/discord_/bot_menus/pagination.py` & `fudstop-2.9.2/fudstop/discord_/bot_menus/pagination.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/discord_/cogs/__init__.py` & `fudstop-2.9.2/fudstop/discord_/cogs/__init__.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/discord_/cogs/accounting.py` & `fudstop-2.9.2/fudstop/discord_/cogs/accounting.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/discord_/cogs/assistant.py` & `fudstop-2.9.2/fudstop/discord_/cogs/assistant.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/discord_/cogs/database.py` & `fudstop-2.9.2/fudstop/discord_/cogs/database.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/discord_/cogs/earnings.py` & `fudstop-2.9.2/fudstop/discord_/cogs/earnings.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/discord_/cogs/fed_print.py` & `fudstop-2.9.2/fudstop/discord_/cogs/fed_print.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/discord_/cogs/filter.py` & `fudstop-2.9.2/fudstop/discord_/cogs/filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 import asyncpg
 from dotenv import load_dotenv
 from datetime import datetime
 from tabulate import tabulate
 from schema import run_conversation, tools
 from options_filter import FilterView, FilterMenu
-from webull_options.webull_options import WebullOptions
+from fudstop.apis.webull.webull_options.webull_options import WebullOptions
 load_dotenv()
 
 
 
 class FilterCog(commands.Cog):
     def __init__(self, bot):
         self.bot=bot
```

### Comparing `fudstop-2.9.1/fudstop/discord_/cogs/fiscal_service.py` & `fudstop-2.9.2/fudstop/discord_/cogs/fiscal_service.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/discord_/cogs/gex.py` & `fudstop-2.9.2/fudstop/discord_/cogs/gex.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/discord_/cogs/gpt.py` & `fudstop-2.9.2/fudstop/discord_/cogs/gpt.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/discord_/cogs/ibrs.py` & `fudstop-2.9.2/fudstop/discord_/cogs/ibrs.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/discord_/cogs/main_view.py` & `fudstop-2.9.2/fudstop/discord_/cogs/main_view.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/discord_/cogs/options.py` & `fudstop-2.9.2/fudstop/discord_/cogs/options.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/discord_/cogs/plays.py` & `fudstop-2.9.2/fudstop/discord_/cogs/plays.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 load_dotenv()
 import disnake
 from disnake.ext import commands
 from tabulate import tabulate
 import pandas as pd
 from apis.polygonio.polygon_options import PolygonOptions
 from apis.polygonio.polygon_database import PolygonDatabase
-from webull_options.webull_options import WebullOptions
+from fudstop.apis.webull.webull_options.webull_options import WebullOptions
 import datetime
 from discord_.bot_menus.pagination import AlertMenus
 
 wb_opts = WebullOptions(database='markets', user='chuck')
 db = PolygonDatabase(user='chuck', database='charlie', host='localhost', port=5432, password='fud')
 opts = PolygonOptions(user='chuck', database='charlie', host='localhost', port=5432, password='fud')
```

### Comparing `fudstop-2.9.1/fudstop/discord_/cogs/register.py` & `fudstop-2.9.2/fudstop/discord_/cogs/register.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/discord_/cogs/spx.py` & `fudstop-2.9.2/fudstop/discord_/cogs/spx.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/discord_/cogs/strategy.py` & `fudstop-2.9.2/fudstop/discord_/cogs/strategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import disnake
 from disnake.ext import commands
 import pandas as pd
 from tabulate import tabulate
-from webull_options.webull_options import WebullOptions
+from fudstop.apis.webull.webull_options.webull_options import WebullOptions
 from discord_.bot_menus.pagination import AlertMenus
 import os
 
 from dotenv import load_dotenv
 load_dotenv()
 theta_em = "<a:_:1047010360554704977>"
 gamma_em = "<a:_:1190024505700134973>"
```

### Comparing `fudstop-2.9.1/fudstop/discord_/cogs/ta.py` & `fudstop-2.9.2/fudstop/discord_/cogs/ta.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/discord_/cogs/weather.py` & `fudstop-2.9.2/fudstop/discord_/cogs/weather.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/discord_/cogs/webull.py` & `fudstop-2.9.2/fudstop/discord_/cogs/webull.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/discord_/cogs/yfin.py` & `fudstop-2.9.2/fudstop/discord_/cogs/yfin.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/discord_/database_getter.py` & `fudstop-2.9.2/fudstop/discord_/database_getter.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/discord_/discord_rsi.py` & `fudstop-2.9.2/fudstop/discord_/discord_rsi.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/discord_/embeddings.py` & `fudstop-2.9.2/fudstop/discord_/embeddings.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/examples/ecfr_test.py` & `fudstop-2.9.2/fudstop/examples/ecfr_test.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/examples/ofr_test.py` & `fudstop-2.9.2/fudstop/examples/ofr_test.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/examples/polygonio/aggregates_second.py` & `fudstop-2.9.2/fudstop/examples/polygonio/aggregates_second.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/examples/polygonio/company_info.py` & `fudstop-2.9.2/fudstop/examples/polygonio/company_info.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/examples/polygonio/get_all_options.py` & `fudstop-2.9.2/fudstop/examples/polygonio/get_all_options.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/examples/polygonio/get_near_the_money.py` & `fudstop-2.9.2/fudstop/examples/polygonio/get_near_the_money.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/examples/polygonio/get_option_aggs.py` & `fudstop-2.9.2/fudstop/examples/polygonio/get_option_aggs.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/examples/polygonio/get_option_rsi.py` & `fudstop-2.9.2/fudstop/examples/polygonio/get_option_rsi.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/examples/polygonio/get_option_trades.py` & `fudstop-2.9.2/fudstop/examples/polygonio/get_option_trades.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/examples/polygonio/get_ticker_aggs.py` & `fudstop-2.9.2/fudstop/examples/polygonio/get_ticker_aggs.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/examples/polygonio/market_news.py` & `fudstop-2.9.2/fudstop/examples/polygonio/market_news.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/examples/polygonio/polygon_test.py` & `fudstop-2.9.2/fudstop/examples/polygonio/polygon_test.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/examples/scripty.py` & `fudstop-2.9.2/fudstop/examples/scripty.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/examples/stocksera_test.py` & `fudstop-2.9.2/fudstop/examples/stocksera_test.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/examples/test.py` & `fudstop-2.9.2/fudstop/examples/test.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/examples/test_gex.py` & `fudstop-2.9.2/fudstop/examples/test_gex.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/examples/test_openai.py` & `fudstop-2.9.2/fudstop/examples/test_openai.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/examples/test_opts.py` & `fudstop-2.9.2/fudstop/examples/test_opts.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/examples/test_screener.py` & `fudstop-2.9.2/fudstop/examples/test_screener.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/examples/test_sec.py` & `fudstop-2.9.2/fudstop/examples/test_sec.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/examples/test_webull.py` & `fudstop-2.9.2/fudstop/examples/test_webull.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/examples/webull/markets_example.py` & `fudstop-2.9.2/fudstop/examples/webull/markets_example.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/examples/webull/trade_example.py` & `fudstop-2.9.2/fudstop/examples/webull/trade_example.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/options_filter.py` & `fudstop-2.9.2/fudstop/options_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import disnake
 from disnake import TextInputStyle
 from disnake.ext import commands
 import pandas as pd
 from typing import List
-from webull_options.webull_options import WebullOptions
+from fudstop.apis.webull.webull_options.webull_options import WebullOptions
 import os
 from tabulate import tabulate
 
 from discord_.bot_menus.pagination import AlertMenus
 
 
 from dotenv import load_dotenv
```

### Comparing `fudstop-2.9.1/fudstop/plots.py` & `fudstop-2.9.2/fudstop/plots.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop/schema.py` & `fudstop-2.9.2/fudstop/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from openai import OpenAI
 import os
 import asyncio
-from webull_options.webull_options import WebullOptions
+from fudstop.apis.webull.webull_options.webull_options import WebullOptions
 import json
 from dotenv import load_dotenv
 load_dotenv()
 import datetime
 client = OpenAI(api_key=os.environ.get('YOUR_OPENAI_KEY'))
 sdk = WebullOptions(database='markets', user='postgres')
 def serialize_record(record):
```

### Comparing `fudstop-2.9.1/fudstop.egg-info/PKG-INFO` & `fudstop-2.9.2/fudstop.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fudstop
-Version: 2.9.1
+Version: 2.9.2
 Requires-Dist: absl-py==2.0.0
 Requires-Dist: aiofiles==23.2.1
 Requires-Dist: aiohttp==3.9.5
 Requires-Dist: aiosignal==1.3.1
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: anyio==3.7.1
 Requires-Dist: appdirs==1.4.4
```

### Comparing `fudstop-2.9.1/fudstop.egg-info/SOURCES.txt` & `fudstop-2.9.2/fudstop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fudstop-2.9.1/fudstop.egg-info/requires.txt` & `fudstop-2.9.2/fudstop.egg-info/requires.txt`

 * *Files identical despite different names*

