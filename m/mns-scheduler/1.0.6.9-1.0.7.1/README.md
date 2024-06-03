# Comparing `tmp/mns-scheduler-1.0.6.9.tar.gz` & `tmp/mns-scheduler-1.0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mns-scheduler-1.0.6.9.tar", last modified: Thu May 30 14:24:52 2024, max compression
+gzip compressed data, was "mns-scheduler-1.0.7.1.tar", last modified: Mon Jun  3 08:41:47 2024, max compression
```

## Comparing `mns-scheduler-1.0.6.9.tar` & `mns-scheduler-1.0.7.1.tar`

### file list

```diff
@@ -1,134 +1,144 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 14:24:52.918992 mns-scheduler-1.0.6.9/
--rw-rw-rw-   0        0        0       62 2024-05-30 14:24:52.917994 mns-scheduler-1.0.6.9/PKG-INFO
--rw-rw-rw-   0        0        0     1357 2023-12-16 03:56:24.000000 mns-scheduler-1.0.6.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 14:24:52.871120 mns-scheduler-1.0.6.9/mns_scheduler/
--rw-rw-rw-   0        0        0      165 2024-05-20 12:48:16.000000 mns-scheduler-1.0.6.9/mns_scheduler/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:24:52.873114 mns-scheduler-1.0.6.9/mns_scheduler/backup/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.6.9/mns_scheduler/backup/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:24:52.874111 mns-scheduler-1.0.6.9/mns_scheduler/backup/app/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.6.9/mns_scheduler/backup/app/__init__.py
--rw-rw-rw-   0        0        0     5148 2024-04-27 03:55:36.000000 mns-scheduler-1.0.6.9/mns_scheduler/backup/app/ths_new_concept_sync_app.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:24:52.876106 mns-scheduler-1.0.6.9/mns_scheduler/backup/em/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.6.9/mns_scheduler/backup/em/__init__.py
--rw-rw-rw-   0        0        0     4992 2024-04-27 03:55:36.000000 mns-scheduler-1.0.6.9/mns_scheduler/backup/em/em_new_concept_his_sync.py
--rw-rw-rw-   0        0        0     7083 2024-04-27 03:55:36.000000 mns-scheduler-1.0.6.9/mns_scheduler/backup/em/em_new_concept_sync_common_api.py
--rw-rw-rw-   0        0        0     2334 2024-04-27 03:55:36.000000 mns-scheduler-1.0.6.9/mns_scheduler/backup/em/em_new_concept_sync_web.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:24:52.877104 mns-scheduler-1.0.6.9/mns_scheduler/backup/wen_cai/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.6.9/mns_scheduler/backup/wen_cai/__init__.py
--rw-rw-rw-   0        0        0     1747 2024-04-27 03:55:36.000000 mns-scheduler-1.0.6.9/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:24:52.878101 mns-scheduler-1.0.6.9/mns_scheduler/big_deal/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.9/mns_scheduler/big_deal/__init__.py
--rw-rw-rw-   0        0        0     4555 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.9/mns_scheduler/big_deal/ths_big_deal_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:24:52.880096 mns-scheduler-1.0.6.9/mns_scheduler/company_info/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.9/mns_scheduler/company_info/__init__.py
--rw-rw-rw-   0        0        0    14306 2024-05-17 08:56:50.000000 mns-scheduler-1.0.6.9/mns_scheduler/company_info/company_constant_data.py
--rw-rw-rw-   0        0        0    22727 2024-05-24 07:13:02.000000 mns-scheduler-1.0.6.9/mns_scheduler/company_info/company_info_sync_api.py
--rw-rw-rw-   0        0        0     1993 2024-05-17 07:32:00.000000 mns-scheduler-1.0.6.9/mns_scheduler/company_info/de_list_stock_service.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:24:52.881093 mns-scheduler-1.0.6.9/mns_scheduler/concept/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.9/mns_scheduler/concept/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:24:52.882090 mns-scheduler-1.0.6.9/mns_scheduler/concept/clean/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.9/mns_scheduler/concept/clean/__init__.py
--rw-rw-rw-   0        0        0     4512 2024-05-09 14:49:14.000000 mns-scheduler-1.0.6.9/mns_scheduler/concept/clean/kpl_concept_clean_api.py
--rw-rw-rw-   0        0        0     5907 2024-05-09 07:47:40.000000 mns-scheduler-1.0.6.9/mns_scheduler/concept/clean/ths_concept_clean_api.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:24:52.883087 mns-scheduler-1.0.6.9/mns_scheduler/concept/ths/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.9/mns_scheduler/concept/ths/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:24:52.884085 mns-scheduler-1.0.6.9/mns_scheduler/concept/ths/common/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.9/mns_scheduler/concept/ths/common/__init__.py
--rw-rw-rw-   0        0        0     6724 2024-04-30 12:29:06.000000 mns-scheduler-1.0.6.9/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
--rw-rw-rw-   0        0        0     4460 2024-04-30 09:34:23.000000 mns-scheduler-1.0.6.9/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:24:52.886080 mns-scheduler-1.0.6.9/mns_scheduler/concept/ths/sync_new_index/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.6.9/mns_scheduler/concept/ths/sync_new_index/__init__.py
--rw-rw-rw-   0        0        0     5315 2024-05-29 04:39:42.000000 mns-scheduler-1.0.6.9/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py
--rw-rw-rw-   0        0        0     3990 2024-05-29 13:06:57.000000 mns-scheduler-1.0.6.9/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:24:52.887081 mns-scheduler-1.0.6.9/mns_scheduler/concept/ths/update_concept_info/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.6.9/mns_scheduler/concept/ths/update_concept_info/__init__.py
--rw-rw-rw-   0        0        0     1928 2024-04-27 03:55:36.000000 mns-scheduler-1.0.6.9/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py
--rw-rw-rw-   0        0        0     8764 2024-04-27 03:55:36.000000 mns-scheduler-1.0.6.9/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:24:52.889077 mns-scheduler-1.0.6.9/mns_scheduler/db/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.9/mns_scheduler/db/__init__.py
--rw-rw-rw-   0        0        0     3952 2024-05-29 07:44:21.000000 mns-scheduler-1.0.6.9/mns_scheduler/db/col_move_service.py
--rw-rw-rw-   0        0        0      747 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.9/mns_scheduler/db/db_status.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:24:52.890071 mns-scheduler-1.0.6.9/mns_scheduler/dt/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.9/mns_scheduler/dt/__init__.py
--rw-rw-rw-   0        0        0     3466 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.9/mns_scheduler/dt/stock_dt_pool_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:24:52.893068 mns-scheduler-1.0.6.9/mns_scheduler/finance/
--rw-rw-rw-   0        0        0      163 2024-05-15 14:37:41.000000 mns-scheduler-1.0.6.9/mns_scheduler/finance/__init__.py
--rw-rw-rw-   0        0        0    19437 2024-05-16 00:08:00.000000 mns-scheduler-1.0.6.9/mns_scheduler/finance/em_financial_asset_liability_sync_service_api.py
--rw-rw-rw-   0        0        0    14145 2024-05-16 00:05:34.000000 mns-scheduler-1.0.6.9/mns_scheduler/finance/em_financial_profit_sync_service_api.py
--rw-rw-rw-   0        0        0     2471 2024-05-16 08:53:00.000000 mns-scheduler-1.0.6.9/mns_scheduler/finance/finance_common_api.py
--rw-rw-rw-   0        0        0    10561 2024-05-16 09:27:25.000000 mns-scheduler-1.0.6.9/mns_scheduler/finance/financial_high_risk_stock_clean_service_api.py
--rw-rw-rw-   0        0        0     5042 2024-05-16 09:27:25.000000 mns-scheduler-1.0.6.9/mns_scheduler/finance/sync_financial_report_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:24:52.894063 mns-scheduler-1.0.6.9/mns_scheduler/finance/test/
--rw-rw-rw-   0        0        0      163 2024-05-16 01:05:27.000000 mns-scheduler-1.0.6.9/mns_scheduler/finance/test/__init__.py
--rw-rw-rw-   0        0        0     1304 2024-05-16 06:04:02.000000 mns-scheduler-1.0.6.9/mns_scheduler/finance/test/fix_blask_list.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:24:52.895057 mns-scheduler-1.0.6.9/mns_scheduler/hk/
--rw-rw-rw-   0        0        0      163 2024-05-16 07:31:10.000000 mns-scheduler-1.0.6.9/mns_scheduler/hk/__init__.py
--rw-rw-rw-   0        0        0     3661 2024-05-17 08:14:15.000000 mns-scheduler-1.0.6.9/mns_scheduler/hk/hk_company_info_sync_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:24:52.896060 mns-scheduler-1.0.6.9/mns_scheduler/irm/
--rw-rw-rw-   0        0        0      163 2024-05-20 12:48:16.000000 mns-scheduler-1.0.6.9/mns_scheduler/irm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:24:52.898048 mns-scheduler-1.0.6.9/mns_scheduler/irm/api/
--rw-rw-rw-   0        0        0      163 2024-05-24 14:59:41.000000 mns-scheduler-1.0.6.9/mns_scheduler/irm/api/__init__.py
--rw-rw-rw-   0        0        0     4931 2024-05-24 22:45:39.000000 mns-scheduler-1.0.6.9/mns_scheduler/irm/api/sh_stock_sns_sse_info_api.py
--rw-rw-rw-   0        0        0     6199 2024-05-25 08:40:25.000000 mns-scheduler-1.0.6.9/mns_scheduler/irm/api/sz_stock_sns_sse_info_api.py
--rw-rw-rw-   0        0        0     9712 2024-05-30 14:20:13.000000 mns-scheduler-1.0.6.9/mns_scheduler/irm/stock_irm_cninfo_service.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:24:52.898048 mns-scheduler-1.0.6.9/mns_scheduler/k_line/
--rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.9/mns_scheduler/k_line/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:24:52.900042 mns-scheduler-1.0.6.9/mns_scheduler/k_line/clean/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.9/mns_scheduler/k_line/clean/__init__.py
--rw-rw-rw-   0        0        0    22262 2024-05-23 09:26:20.000000 mns-scheduler-1.0.6.9/mns_scheduler/k_line/clean/k_line_info_clean_impl.py
--rw-rw-rw-   0        0        0     8118 2024-05-23 15:00:37.000000 mns-scheduler-1.0.6.9/mns_scheduler/k_line/clean/k_line_info_clean_service.py
--rw-rw-rw-   0        0        0     2628 2024-05-23 15:06:42.000000 mns-scheduler-1.0.6.9/mns_scheduler/k_line/clean/recent_hot_stocks_clean_service.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:24:52.901040 mns-scheduler-1.0.6.9/mns_scheduler/k_line/sync/
--rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.9/mns_scheduler/k_line/sync/__init__.py
--rw-rw-rw-   0        0        0     5652 2024-05-11 03:27:17.000000 mns-scheduler-1.0.6.9/mns_scheduler/k_line/sync/daily_week_month_line_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:24:52.902037 mns-scheduler-1.0.6.9/mns_scheduler/kpl/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.9/mns_scheduler/kpl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:24:52.902037 mns-scheduler-1.0.6.9/mns_scheduler/kpl/selection/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.9/mns_scheduler/kpl/selection/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:24:52.904032 mns-scheduler-1.0.6.9/mns_scheduler/kpl/selection/index/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.9/mns_scheduler/kpl/selection/index/__init__.py
--rw-rw-rw-   0        0        0     4748 2024-05-09 13:26:15.000000 mns-scheduler-1.0.6.9/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py
--rw-rw-rw-   0        0        0     8016 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.9/mns_scheduler/kpl/selection/index/sync_best_choose_index.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:24:52.904032 mns-scheduler-1.0.6.9/mns_scheduler/kpl/selection/symbol/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.9/mns_scheduler/kpl/selection/symbol/__init__.py
--rw-rw-rw-   0        0        0     4679 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.9/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:24:52.906026 mns-scheduler-1.0.6.9/mns_scheduler/kpl/selection/total/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.9/mns_scheduler/kpl/selection/total/__init__.py
--rw-rw-rw-   0        0        0    10461 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.9/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:24:52.907024 mns-scheduler-1.0.6.9/mns_scheduler/lhb/
--rw-rw-rw-   0        0        0      163 2024-05-22 07:47:25.000000 mns-scheduler-1.0.6.9/mns_scheduler/lhb/__init__.py
--rw-rw-rw-   0        0        0      641 2024-05-22 07:52:36.000000 mns-scheduler-1.0.6.9/mns_scheduler/lhb/stock_lhb_sync_service.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:24:52.908021 mns-scheduler-1.0.6.9/mns_scheduler/real_time/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.9/mns_scheduler/real_time/__init__.py
--rw-rw-rw-   0        0        0     1066 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.9/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py
--rw-rw-rw-   0        0        0     9491 2024-05-29 15:14:09.000000 mns-scheduler-1.0.6.9/mns_scheduler/real_time/realtime_quotes_now_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:24:52.910016 mns-scheduler-1.0.6.9/mns_scheduler/risk/
--rw-rw-rw-   0        0        0      163 2024-05-22 07:47:47.000000 mns-scheduler-1.0.6.9/mns_scheduler/risk/__init__.py
--rw-rw-rw-   0        0        0     5086 2024-05-17 13:05:26.000000 mns-scheduler-1.0.6.9/mns_scheduler/risk/register_and_investigate_stock_sync_api.py
--rw-rw-rw-   0        0        0      871 2024-05-18 01:43:32.000000 mns-scheduler-1.0.6.9/mns_scheduler/risk/stock_equity_mortgage_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:24:52.912010 mns-scheduler-1.0.6.9/mns_scheduler/trade/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.9/mns_scheduler/trade/__init__.py
--rw-rw-rw-   0        0        0      377 2024-04-28 03:16:51.000000 mns-scheduler-1.0.6.9/mns_scheduler/trade/auto_ipo_buy_api.py
--rw-rw-rw-   0        0        0     4423 2024-04-28 08:59:05.000000 mns-scheduler-1.0.6.9/mns_scheduler/trade/auto_sell_service_api.py
--rw-rw-rw-   0        0        0     2739 2024-04-28 08:08:30.000000 mns-scheduler-1.0.6.9/mns_scheduler/trade/sync_position_api.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:24:52.913008 mns-scheduler-1.0.6.9/mns_scheduler/zb/
--rw-rw-rw-   0        0        0      165 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.9/mns_scheduler/zb/__init__.py
--rw-rw-rw-   0        0        0     1936 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.9/mns_scheduler/zb/stock_zb_pool_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:24:52.916000 mns-scheduler-1.0.6.9/mns_scheduler/zt/
--rw-rw-rw-   0        0        0     1641 2024-05-22 03:34:21.000000 mns-scheduler-1.0.6.9/mns_scheduler/zt/__init__.py
--rw-rw-rw-   0        0        0     4015 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.9/mns_scheduler/zt/export_open_data_to_excel.py
--rw-rw-rw-   0        0        0    17525 2024-05-29 09:53:47.000000 mns-scheduler-1.0.6.9/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py
--rw-rw-rw-   0        0        0    21283 2024-05-29 09:53:47.000000 mns-scheduler-1.0.6.9/mns_scheduler/zt/today_high_chg_pool_sync_api.py
--rw-rw-rw-   0        0        0    10916 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.9/mns_scheduler/zt/zt_five_boards_sync_api.py
--rw-rw-rw-   0        0        0     7604 2024-05-18 00:16:23.000000 mns-scheduler-1.0.6.9/mns_scheduler/zt/zt_pool_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:24:52.916996 mns-scheduler-1.0.6.9/mns_scheduler/zz_task/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.9/mns_scheduler/zz_task/__init__.py
--rw-rw-rw-   0        0        0    16850 2024-05-29 13:46:49.000000 mns-scheduler-1.0.6.9/mns_scheduler/zz_task/data_sync_task.py
--rw-rw-rw-   0        0        0      932 2024-04-22 00:53:06.000000 mns-scheduler-1.0.6.9/mns_scheduler/zz_task/sync_realtime_quotes_task.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:24:52.917994 mns-scheduler-1.0.6.9/mns_scheduler.egg-info/
--rw-rw-rw-   0        0        0       62 2024-05-30 14:24:52.000000 mns-scheduler-1.0.6.9/mns_scheduler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4351 2024-05-30 14:24:52.000000 mns-scheduler-1.0.6.9/mns_scheduler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 14:24:52.000000 mns-scheduler-1.0.6.9/mns_scheduler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-30 14:24:52.000000 mns-scheduler-1.0.6.9/mns_scheduler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 14:24:52.918992 mns-scheduler-1.0.6.9/setup.cfg
--rw-rw-rw-   0        0        0      212 2024-05-30 14:21:05.000000 mns-scheduler-1.0.6.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:41:47.479046 mns-scheduler-1.0.7.1/
+-rw-rw-rw-   0        0        0       62 2024-06-03 08:41:47.478048 mns-scheduler-1.0.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1357 2023-12-16 03:56:24.000000 mns-scheduler-1.0.7.1/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 08:41:47.428182 mns-scheduler-1.0.7.1/mns_scheduler/
+-rw-rw-rw-   0        0        0      165 2024-05-20 12:48:16.000000 mns-scheduler-1.0.7.1/mns_scheduler/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:41:47.430177 mns-scheduler-1.0.7.1/mns_scheduler/backup/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.7.1/mns_scheduler/backup/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:41:47.431174 mns-scheduler-1.0.7.1/mns_scheduler/backup/app/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.7.1/mns_scheduler/backup/app/__init__.py
+-rw-rw-rw-   0        0        0     5148 2024-04-27 03:55:36.000000 mns-scheduler-1.0.7.1/mns_scheduler/backup/app/ths_new_concept_sync_app.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:41:47.433168 mns-scheduler-1.0.7.1/mns_scheduler/backup/em/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.7.1/mns_scheduler/backup/em/__init__.py
+-rw-rw-rw-   0        0        0     4992 2024-04-27 03:55:36.000000 mns-scheduler-1.0.7.1/mns_scheduler/backup/em/em_new_concept_his_sync.py
+-rw-rw-rw-   0        0        0     7083 2024-04-27 03:55:36.000000 mns-scheduler-1.0.7.1/mns_scheduler/backup/em/em_new_concept_sync_common_api.py
+-rw-rw-rw-   0        0        0     2334 2024-04-27 03:55:36.000000 mns-scheduler-1.0.7.1/mns_scheduler/backup/em/em_new_concept_sync_web.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:41:47.434166 mns-scheduler-1.0.7.1/mns_scheduler/backup/wen_cai/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.7.1/mns_scheduler/backup/wen_cai/__init__.py
+-rw-rw-rw-   0        0        0     1747 2024-04-27 03:55:36.000000 mns-scheduler-1.0.7.1/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:41:47.435163 mns-scheduler-1.0.7.1/mns_scheduler/big_deal/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.7.1/mns_scheduler/big_deal/__init__.py
+-rw-rw-rw-   0        0        0     4555 2024-04-22 00:53:06.000000 mns-scheduler-1.0.7.1/mns_scheduler/big_deal/ths_big_deal_sync.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:41:47.438156 mns-scheduler-1.0.7.1/mns_scheduler/company_info/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.7.1/mns_scheduler/company_info/__init__.py
+-rw-rw-rw-   0        0        0    14306 2024-05-17 08:56:50.000000 mns-scheduler-1.0.7.1/mns_scheduler/company_info/company_constant_data.py
+-rw-rw-rw-   0        0        0    22727 2024-05-24 07:13:02.000000 mns-scheduler-1.0.7.1/mns_scheduler/company_info/company_info_sync_api.py
+-rw-rw-rw-   0        0        0     1993 2024-05-17 07:32:00.000000 mns-scheduler-1.0.7.1/mns_scheduler/company_info/de_list_stock_service.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:41:47.438156 mns-scheduler-1.0.7.1/mns_scheduler/concept/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.7.1/mns_scheduler/concept/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:41:47.439152 mns-scheduler-1.0.7.1/mns_scheduler/concept/clean/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.7.1/mns_scheduler/concept/clean/__init__.py
+-rw-rw-rw-   0        0        0     4512 2024-05-09 14:49:14.000000 mns-scheduler-1.0.7.1/mns_scheduler/concept/clean/kpl_concept_clean_api.py
+-rw-rw-rw-   0        0        0     5907 2024-05-09 07:47:40.000000 mns-scheduler-1.0.7.1/mns_scheduler/concept/clean/ths_concept_clean_api.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:41:47.440150 mns-scheduler-1.0.7.1/mns_scheduler/concept/ths/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.7.1/mns_scheduler/concept/ths/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:41:47.441147 mns-scheduler-1.0.7.1/mns_scheduler/concept/ths/common/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.7.1/mns_scheduler/concept/ths/common/__init__.py
+-rw-rw-rw-   0        0        0     6724 2024-04-30 12:29:06.000000 mns-scheduler-1.0.7.1/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
+-rw-rw-rw-   0        0        0     4460 2024-04-30 09:34:23.000000 mns-scheduler-1.0.7.1/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:41:47.443141 mns-scheduler-1.0.7.1/mns_scheduler/concept/ths/sync_new_index/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.7.1/mns_scheduler/concept/ths/sync_new_index/__init__.py
+-rw-rw-rw-   0        0        0     5315 2024-05-29 04:39:42.000000 mns-scheduler-1.0.7.1/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py
+-rw-rw-rw-   0        0        0     3990 2024-05-29 13:06:57.000000 mns-scheduler-1.0.7.1/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:41:47.445136 mns-scheduler-1.0.7.1/mns_scheduler/concept/ths/update_concept_info/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.7.1/mns_scheduler/concept/ths/update_concept_info/__init__.py
+-rw-rw-rw-   0        0        0     1928 2024-04-27 03:55:36.000000 mns-scheduler-1.0.7.1/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py
+-rw-rw-rw-   0        0        0     8852 2024-05-30 15:46:48.000000 mns-scheduler-1.0.7.1/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:41:47.446134 mns-scheduler-1.0.7.1/mns_scheduler/db/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.7.1/mns_scheduler/db/__init__.py
+-rw-rw-rw-   0        0        0     3952 2024-05-29 07:44:21.000000 mns-scheduler-1.0.7.1/mns_scheduler/db/col_move_service.py
+-rw-rw-rw-   0        0        0      747 2024-04-22 00:53:06.000000 mns-scheduler-1.0.7.1/mns_scheduler/db/db_status.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:41:47.447131 mns-scheduler-1.0.7.1/mns_scheduler/dt/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.7.1/mns_scheduler/dt/__init__.py
+-rw-rw-rw-   0        0        0     3466 2024-04-22 00:53:06.000000 mns-scheduler-1.0.7.1/mns_scheduler/dt/stock_dt_pool_sync.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:41:47.450123 mns-scheduler-1.0.7.1/mns_scheduler/finance/
+-rw-rw-rw-   0        0        0      163 2024-05-15 14:37:41.000000 mns-scheduler-1.0.7.1/mns_scheduler/finance/__init__.py
+-rw-rw-rw-   0        0        0    19437 2024-05-16 00:08:00.000000 mns-scheduler-1.0.7.1/mns_scheduler/finance/em_financial_asset_liability_sync_service_api.py
+-rw-rw-rw-   0        0        0    14145 2024-05-16 00:05:34.000000 mns-scheduler-1.0.7.1/mns_scheduler/finance/em_financial_profit_sync_service_api.py
+-rw-rw-rw-   0        0        0     2471 2024-05-16 08:53:00.000000 mns-scheduler-1.0.7.1/mns_scheduler/finance/finance_common_api.py
+-rw-rw-rw-   0        0        0    10561 2024-05-16 09:27:25.000000 mns-scheduler-1.0.7.1/mns_scheduler/finance/financial_high_risk_stock_clean_service_api.py
+-rw-rw-rw-   0        0        0     5042 2024-05-16 09:27:25.000000 mns-scheduler-1.0.7.1/mns_scheduler/finance/sync_financial_report_service_api.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:41:47.451121 mns-scheduler-1.0.7.1/mns_scheduler/finance/test/
+-rw-rw-rw-   0        0        0      163 2024-05-16 01:05:27.000000 mns-scheduler-1.0.7.1/mns_scheduler/finance/test/__init__.py
+-rw-rw-rw-   0        0        0     1304 2024-05-16 06:04:02.000000 mns-scheduler-1.0.7.1/mns_scheduler/finance/test/fix_blask_list.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:41:47.452118 mns-scheduler-1.0.7.1/mns_scheduler/hk/
+-rw-rw-rw-   0        0        0      163 2024-05-16 07:31:10.000000 mns-scheduler-1.0.7.1/mns_scheduler/hk/__init__.py
+-rw-rw-rw-   0        0        0     3661 2024-05-17 08:14:15.000000 mns-scheduler-1.0.7.1/mns_scheduler/hk/hk_company_info_sync_service_api.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:41:47.453115 mns-scheduler-1.0.7.1/mns_scheduler/irm/
+-rw-rw-rw-   0        0        0      163 2024-05-20 12:48:16.000000 mns-scheduler-1.0.7.1/mns_scheduler/irm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:41:47.455110 mns-scheduler-1.0.7.1/mns_scheduler/irm/api/
+-rw-rw-rw-   0        0        0      163 2024-05-24 14:59:41.000000 mns-scheduler-1.0.7.1/mns_scheduler/irm/api/__init__.py
+-rw-rw-rw-   0        0        0     4931 2024-05-24 22:45:39.000000 mns-scheduler-1.0.7.1/mns_scheduler/irm/api/sh_stock_sns_sse_info_api.py
+-rw-rw-rw-   0        0        0     6199 2024-05-25 08:40:25.000000 mns-scheduler-1.0.7.1/mns_scheduler/irm/api/sz_stock_sns_sse_info_api.py
+-rw-rw-rw-   0        0        0     9712 2024-05-30 14:20:13.000000 mns-scheduler-1.0.7.1/mns_scheduler/irm/stock_irm_cninfo_service.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:41:47.455110 mns-scheduler-1.0.7.1/mns_scheduler/k_line/
+-rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.7.1/mns_scheduler/k_line/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:41:47.457104 mns-scheduler-1.0.7.1/mns_scheduler/k_line/clean/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.7.1/mns_scheduler/k_line/clean/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:41:47.458102 mns-scheduler-1.0.7.1/mns_scheduler/k_line/clean/daily/
+-rw-rw-rw-   0        0        0      163 2024-06-03 08:41:02.000000 mns-scheduler-1.0.7.1/mns_scheduler/k_line/clean/daily/__init__.py
+-rw-rw-rw-   0        0        0    18257 2024-06-03 08:41:02.000000 mns-scheduler-1.0.7.1/mns_scheduler/k_line/clean/daily/daily_k_line_clean_common_service.py
+-rw-rw-rw-   0        0        0     6132 2024-06-03 08:41:02.000000 mns-scheduler-1.0.7.1/mns_scheduler/k_line/clean/daily/daily_k_line_service.py
+-rw-rw-rw-   0        0        0     1238 2024-06-03 08:41:02.000000 mns-scheduler-1.0.7.1/mns_scheduler/k_line/clean/k_line_info_clean_impl.py
+-rw-rw-rw-   0        0        0     8384 2024-06-03 08:41:02.000000 mns-scheduler-1.0.7.1/mns_scheduler/k_line/clean/k_line_info_clean_task.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:41:47.459099 mns-scheduler-1.0.7.1/mns_scheduler/k_line/clean/week_month/
+-rw-rw-rw-   0        0        0      163 2024-06-03 08:41:02.000000 mns-scheduler-1.0.7.1/mns_scheduler/k_line/clean/week_month/__init__.py
+-rw-rw-rw-   0        0        0     4862 2024-06-03 08:41:02.000000 mns-scheduler-1.0.7.1/mns_scheduler/k_line/clean/week_month/normal_week_month_k_line_service.py
+-rw-rw-rw-   0        0        0     2044 2024-06-03 08:41:02.000000 mns-scheduler-1.0.7.1/mns_scheduler/k_line/clean/week_month/sub_new_week_month_k_line_service.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:41:47.460096 mns-scheduler-1.0.7.1/mns_scheduler/k_line/hot_stocks/
+-rw-rw-rw-   0        0        0      163 2024-06-03 08:41:02.000000 mns-scheduler-1.0.7.1/mns_scheduler/k_line/hot_stocks/__init__.py
+-rw-rw-rw-   0        0        0     2628 2024-06-03 08:41:02.000000 mns-scheduler-1.0.7.1/mns_scheduler/k_line/hot_stocks/recent_hot_stocks_clean_service.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:41:47.461094 mns-scheduler-1.0.7.1/mns_scheduler/k_line/sync/
+-rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.7.1/mns_scheduler/k_line/sync/__init__.py
+-rw-rw-rw-   0        0        0     5652 2024-05-11 03:27:17.000000 mns-scheduler-1.0.7.1/mns_scheduler/k_line/sync/daily_week_month_line_sync.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:41:47.462091 mns-scheduler-1.0.7.1/mns_scheduler/kpl/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.7.1/mns_scheduler/kpl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:41:47.462091 mns-scheduler-1.0.7.1/mns_scheduler/kpl/selection/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.7.1/mns_scheduler/kpl/selection/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:41:47.463089 mns-scheduler-1.0.7.1/mns_scheduler/kpl/selection/index/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.7.1/mns_scheduler/kpl/selection/index/__init__.py
+-rw-rw-rw-   0        0        0     4748 2024-05-09 13:26:15.000000 mns-scheduler-1.0.7.1/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py
+-rw-rw-rw-   0        0        0     8016 2024-04-22 00:53:06.000000 mns-scheduler-1.0.7.1/mns_scheduler/kpl/selection/index/sync_best_choose_index.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:41:47.464086 mns-scheduler-1.0.7.1/mns_scheduler/kpl/selection/symbol/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.7.1/mns_scheduler/kpl/selection/symbol/__init__.py
+-rw-rw-rw-   0        0        0     4679 2024-04-22 00:53:06.000000 mns-scheduler-1.0.7.1/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:41:47.465083 mns-scheduler-1.0.7.1/mns_scheduler/kpl/selection/total/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.7.1/mns_scheduler/kpl/selection/total/__init__.py
+-rw-rw-rw-   0        0        0    10461 2024-04-22 00:53:06.000000 mns-scheduler-1.0.7.1/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:41:47.466081 mns-scheduler-1.0.7.1/mns_scheduler/lhb/
+-rw-rw-rw-   0        0        0      163 2024-05-22 07:47:25.000000 mns-scheduler-1.0.7.1/mns_scheduler/lhb/__init__.py
+-rw-rw-rw-   0        0        0      641 2024-05-22 07:52:36.000000 mns-scheduler-1.0.7.1/mns_scheduler/lhb/stock_lhb_sync_service.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:41:47.468076 mns-scheduler-1.0.7.1/mns_scheduler/real_time/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.7.1/mns_scheduler/real_time/__init__.py
+-rw-rw-rw-   0        0        0     1066 2024-04-22 00:53:06.000000 mns-scheduler-1.0.7.1/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py
+-rw-rw-rw-   0        0        0     9491 2024-05-29 15:14:09.000000 mns-scheduler-1.0.7.1/mns_scheduler/real_time/realtime_quotes_now_sync.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:41:47.469072 mns-scheduler-1.0.7.1/mns_scheduler/risk/
+-rw-rw-rw-   0        0        0      163 2024-05-22 07:47:47.000000 mns-scheduler-1.0.7.1/mns_scheduler/risk/__init__.py
+-rw-rw-rw-   0        0        0     5086 2024-05-17 13:05:26.000000 mns-scheduler-1.0.7.1/mns_scheduler/risk/register_and_investigate_stock_sync_api.py
+-rw-rw-rw-   0        0        0      871 2024-05-18 01:43:32.000000 mns-scheduler-1.0.7.1/mns_scheduler/risk/stock_equity_mortgage_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:41:47.471068 mns-scheduler-1.0.7.1/mns_scheduler/trade/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.7.1/mns_scheduler/trade/__init__.py
+-rw-rw-rw-   0        0        0      377 2024-04-28 03:16:51.000000 mns-scheduler-1.0.7.1/mns_scheduler/trade/auto_ipo_buy_api.py
+-rw-rw-rw-   0        0        0     4423 2024-04-28 08:59:05.000000 mns-scheduler-1.0.7.1/mns_scheduler/trade/auto_sell_service_api.py
+-rw-rw-rw-   0        0        0     2739 2024-04-28 08:08:30.000000 mns-scheduler-1.0.7.1/mns_scheduler/trade/sync_position_api.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:41:47.472064 mns-scheduler-1.0.7.1/mns_scheduler/zb/
+-rw-rw-rw-   0        0        0      165 2024-04-22 00:53:06.000000 mns-scheduler-1.0.7.1/mns_scheduler/zb/__init__.py
+-rw-rw-rw-   0        0        0     1936 2024-04-22 00:53:06.000000 mns-scheduler-1.0.7.1/mns_scheduler/zb/stock_zb_pool_sync.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:41:47.476054 mns-scheduler-1.0.7.1/mns_scheduler/zt/
+-rw-rw-rw-   0        0        0     1641 2024-05-22 03:34:21.000000 mns-scheduler-1.0.7.1/mns_scheduler/zt/__init__.py
+-rw-rw-rw-   0        0        0     4015 2024-04-22 00:53:06.000000 mns-scheduler-1.0.7.1/mns_scheduler/zt/export_open_data_to_excel.py
+-rw-rw-rw-   0        0        0    17525 2024-05-29 09:53:47.000000 mns-scheduler-1.0.7.1/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py
+-rw-rw-rw-   0        0        0    21283 2024-05-29 09:53:47.000000 mns-scheduler-1.0.7.1/mns_scheduler/zt/today_high_chg_pool_sync_api.py
+-rw-rw-rw-   0        0        0    10916 2024-04-22 00:53:06.000000 mns-scheduler-1.0.7.1/mns_scheduler/zt/zt_five_boards_sync_api.py
+-rw-rw-rw-   0        0        0     7604 2024-05-18 00:16:23.000000 mns-scheduler-1.0.7.1/mns_scheduler/zt/zt_pool_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:41:47.477051 mns-scheduler-1.0.7.1/mns_scheduler/zz_task/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.7.1/mns_scheduler/zz_task/__init__.py
+-rw-rw-rw-   0        0        0    16847 2024-06-03 08:41:02.000000 mns-scheduler-1.0.7.1/mns_scheduler/zz_task/data_sync_task.py
+-rw-rw-rw-   0        0        0      932 2024-04-22 00:53:06.000000 mns-scheduler-1.0.7.1/mns_scheduler/zz_task/sync_realtime_quotes_task.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:41:47.478048 mns-scheduler-1.0.7.1/mns_scheduler.egg-info/
+-rw-rw-rw-   0        0        0       62 2024-06-03 08:41:47.000000 mns-scheduler-1.0.7.1/mns_scheduler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4768 2024-06-03 08:41:47.000000 mns-scheduler-1.0.7.1/mns_scheduler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 08:41:47.000000 mns-scheduler-1.0.7.1/mns_scheduler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-06-03 08:41:47.000000 mns-scheduler-1.0.7.1/mns_scheduler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-03 08:41:47.479046 mns-scheduler-1.0.7.1/setup.cfg
+-rw-rw-rw-   0        0        0      212 2024-06-03 08:41:14.000000 mns-scheduler-1.0.7.1/setup.py
```

### Comparing `mns-scheduler-1.0.6.9/README.md` & `mns-scheduler-1.0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/backup/app/ths_new_concept_sync_app.py` & `mns-scheduler-1.0.7.1/mns_scheduler/backup/app/ths_new_concept_sync_app.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/backup/em/em_new_concept_his_sync.py` & `mns-scheduler-1.0.7.1/mns_scheduler/backup/em/em_new_concept_his_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/backup/em/em_new_concept_sync_common_api.py` & `mns-scheduler-1.0.7.1/mns_scheduler/backup/em/em_new_concept_sync_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/backup/em/em_new_concept_sync_web.py` & `mns-scheduler-1.0.7.1/mns_scheduler/backup/em/em_new_concept_sync_web.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py` & `mns-scheduler-1.0.7.1/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/big_deal/ths_big_deal_sync.py` & `mns-scheduler-1.0.7.1/mns_scheduler/big_deal/ths_big_deal_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/company_info/company_constant_data.py` & `mns-scheduler-1.0.7.1/mns_scheduler/company_info/company_constant_data.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/company_info/company_info_sync_api.py` & `mns-scheduler-1.0.7.1/mns_scheduler/company_info/company_info_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/company_info/de_list_stock_service.py` & `mns-scheduler-1.0.7.1/mns_scheduler/company_info/de_list_stock_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/concept/clean/kpl_concept_clean_api.py` & `mns-scheduler-1.0.7.1/mns_scheduler/concept/clean/kpl_concept_clean_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/concept/clean/ths_concept_clean_api.py` & `mns-scheduler-1.0.7.1/mns_scheduler/concept/clean/ths_concept_clean_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py` & `mns-scheduler-1.0.7.1/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py` & `mns-scheduler-1.0.7.1/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py` & `mns-scheduler-1.0.7.1/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py` & `mns-scheduler-1.0.7.1/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py` & `mns-scheduler-1.0.7.1/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py` & `mns-scheduler-1.0.7.1/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,16 +34,16 @@
 
 
 # 同步新概念到详情表中
 # @async_fun
 def sync_new_concept_to_ths_detail(symbol_add_new_concept_df, str_day, str_now_time):
     for new_concept_one in symbol_add_new_concept_df.itertuples():
         try:
-            concept_code = new_concept_one.concept_code
-            query = {'web_concept_code': int(concept_code)}
+            web_concept_code = new_concept_one.concept_code
+            query = {'web_concept_code': int(web_concept_code)}
             ths_concept_list = mongodb_util.find_query_data('ths_concept_list', query)
             if data_frame_util.is_empty(ths_concept_list):
                 logger.error("无此同花顺概念:{}", new_concept_one.title)
             else:
                 concept_code = list(ths_concept_list['symbol'])[0]
                 concept_name = list(ths_concept_list['name'])[0]
                 ths_concept_sync_common_api.save_ths_concept_detail(symbol_add_new_concept_df,
@@ -91,15 +91,16 @@
             symbol_ths_concept_all_df = pd.DataFrame(ths_concept_json)
             if data_frame_util.is_empty(symbol_ths_concept_all_df):
                 continue
 
             now_date = datetime.now()
             # 开盘交易前不同步 资源开销过大
             if date_handle_util.is_close_time(now_date):
-                ths_concept_update_common_api.update_ths_concept_choose_reason(symbol_ths_concept_all_df, stock_one.symbol)
+                ths_concept_update_common_api.update_ths_concept_choose_reason(symbol_ths_concept_all_df,
+                                                                               stock_one.symbol)
 
             str_day = now_date.strftime('%Y-%m-%d')
             str_now_date = now_date.strftime('%Y-%m-%d %H:%M:%S')
             symbol_ths_concept_all_df.loc[:, 'str_day'] = str_day
             symbol_ths_concept_all_df.loc[:, 'str_now_date'] = str_now_date
             symbol_ths_concept_all_df.loc[:, 'symbol'] = stock_one.symbol
             symbol_ths_concept_all_df.loc[:, 'name'] = stock_one.name
```

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/db/col_move_service.py` & `mns-scheduler-1.0.7.1/mns_scheduler/db/col_move_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/db/db_status.py` & `mns-scheduler-1.0.7.1/mns_scheduler/db/db_status.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/dt/stock_dt_pool_sync.py` & `mns-scheduler-1.0.7.1/mns_scheduler/dt/stock_dt_pool_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/finance/em_financial_asset_liability_sync_service_api.py` & `mns-scheduler-1.0.7.1/mns_scheduler/finance/em_financial_asset_liability_sync_service_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/finance/em_financial_profit_sync_service_api.py` & `mns-scheduler-1.0.7.1/mns_scheduler/finance/em_financial_profit_sync_service_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/finance/finance_common_api.py` & `mns-scheduler-1.0.7.1/mns_scheduler/finance/finance_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/finance/financial_high_risk_stock_clean_service_api.py` & `mns-scheduler-1.0.7.1/mns_scheduler/finance/financial_high_risk_stock_clean_service_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/finance/sync_financial_report_service_api.py` & `mns-scheduler-1.0.7.1/mns_scheduler/finance/sync_financial_report_service_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/finance/test/fix_blask_list.py` & `mns-scheduler-1.0.7.1/mns_scheduler/finance/test/fix_blask_list.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/hk/hk_company_info_sync_service_api.py` & `mns-scheduler-1.0.7.1/mns_scheduler/hk/hk_company_info_sync_service_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/irm/api/sh_stock_sns_sse_info_api.py` & `mns-scheduler-1.0.7.1/mns_scheduler/irm/api/sh_stock_sns_sse_info_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/irm/api/sz_stock_sns_sse_info_api.py` & `mns-scheduler-1.0.7.1/mns_scheduler/irm/api/sz_stock_sns_sse_info_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/irm/stock_irm_cninfo_service.py` & `mns-scheduler-1.0.7.1/mns_scheduler/irm/stock_irm_cninfo_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/k_line/clean/k_line_info_clean_impl.py` & `mns-scheduler-1.0.7.1/mns_scheduler/k_line/clean/daily/daily_k_line_clean_common_service.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,181 +1,22 @@
 import sys
 import os
 
 file_path = os.path.abspath(__file__)
-end = file_path.index('mns') + 17
+end = file_path.index('mns') + 16
 project_path = file_path[0:end]
 sys.path.append(project_path)
-
-import mns_common.utils.data_frame_util as data_frame_util
 import pandas as pd
-from mns_common.db.MongodbUtil import MongodbUtil
-import mns_common.utils.date_handle_util as date_handle_util
 import mns_common.component.k_line.patterns.k_line_patterns_service_api as k_line_patterns_service
-import mns_common.component.k_line.clean.sh_small_normal_zt_k_line_check_api as sh_small_normal_zt_k_line_check_api
-import mns_common.component.classify.symbol_classify_api as symbol_classify_api
-import mns_common.component.k_line.common.k_line_common_service_api as k_line_common_service_api
-import mns_scheduler.k_line.clean.recent_hot_stocks_clean_service as recent_hot_stocks_clean_service
-
-mongodb_util = MongodbUtil('27017')
-# 排除最近10天有三个连板的股票
-EXCLUDE_DAYS = 10
-
-MAX_CONTINUE_BOARDS = 3
-
-
-# 日线 周线 月线 成交量  筹码信息
-def calculate_k_line_info(str_day, symbol, diff_days):
-    k_line_info = pd.DataFrame([[
-        str_day,
-        symbol, diff_days]],
-        columns=['str_day',
-                 'symbol',
-                 'diff_days'
-                 ])
-    k_line_info = handle_month_line(k_line_info, str_day, symbol)
-    k_line_info = handle_week_line(k_line_info, str_day, symbol)
-    k_line_info = handle_day_line(k_line_info, str_day, symbol)
-    return k_line_info
-
-
-# 处理月线
-def handle_month_line(k_line_info, str_day, symbol):
-    month_begin_day = str_day[0:7] + '-01'
-    query = {"symbol": symbol,
-             'date': {"$lt": date_handle_util.no_slash_date(month_begin_day)}}
-    stock_hfq_monthly = mongodb_util.descend_query(query, 'stock_qfq_monthly', 'date', 2)
-    month_num = stock_hfq_monthly.shape[0]
-    k_line_info['month_num'] = month_num
-    if month_num > 0:
-        k_line_info['sum_month'] = round(sum(stock_hfq_monthly['chg']), 2)
-    else:
-        k_line_info['sum_month'] = 0
-
-    if month_num == 0:
-        k_line_info['month01'] = 0
-        k_line_info['month02'] = 0
-        k_line_info['month01_date'] = '19890729'
-        k_line_info['month02_date'] = '19890729'
-    elif month_num == 1:
-        k_line_info['month01'] = stock_hfq_monthly.iloc[0].chg
-        k_line_info['month02'] = 0
-        k_line_info['month01_date'] = stock_hfq_monthly.iloc[0].date
-        k_line_info['month02_date'] = '19890729'
-    elif month_num == 2:
-        k_line_info['month01'] = stock_hfq_monthly.iloc[0].chg
-        k_line_info['month02'] = stock_hfq_monthly.iloc[1].chg
-        k_line_info['month01_date'] = stock_hfq_monthly.iloc[0].date
-        k_line_info['month02_date'] = stock_hfq_monthly.iloc[1].date
-
-    return k_line_info
-
-
-# 处理周线
-def handle_week_line(k_line_info, str_day, symbol):
-    month_begin_day = str_day[0:7] + '-01'
-    query = {"symbol": symbol,
-             '$and': [{'date': {"$gte": date_handle_util.no_slash_date(month_begin_day)}},
-                      {'date': {"$lt": date_handle_util.no_slash_date(str_day)}}]}
-    stock_hfq_weekly = mongodb_util.find_query_data('stock_qfq_weekly', query)
-    week_num = stock_hfq_weekly.shape[0]
-    if week_num > 0:
-        stock_hfq_weekly = stock_hfq_weekly.sort_values(by=['date'], ascending=False)
-        k_line_info['sum_week'] = round(sum(stock_hfq_weekly['chg']), 2)
-    else:
-        k_line_info['sum_week'] = 0
-    k_line_info['week_num'] = week_num
-    if week_num == 1:
-        k_line_info['week01'] = stock_hfq_weekly.iloc[0].chg
-        k_line_info['week02'] = 0
-        k_line_info['week03'] = 0
-        k_line_info['week04'] = 0
-    elif week_num == 2:
-        k_line_info['week01'] = stock_hfq_weekly.iloc[0].chg
-        k_line_info['week02'] = stock_hfq_weekly.iloc[1].chg
-        k_line_info['week03'] = 0
-        k_line_info['week04'] = 0
-    elif week_num == 3:
-        k_line_info['week01'] = stock_hfq_weekly.iloc[0].chg
-        k_line_info['week02'] = stock_hfq_weekly.iloc[1].chg
-        k_line_info['week03'] = stock_hfq_weekly.iloc[2].chg
-        k_line_info['week04'] = 0
-    elif week_num >= 4:
-        k_line_info['week01'] = stock_hfq_weekly.iloc[0].chg
-        k_line_info['week02'] = stock_hfq_weekly.iloc[1].chg
-        k_line_info['week03'] = stock_hfq_weekly.iloc[2].chg
-        k_line_info['week04'] = stock_hfq_weekly.iloc[3].chg
-    elif week_num == 0:
-        k_line_info['week01'] = 0
-        k_line_info['week02'] = 0
-        k_line_info['week03'] = 0
-        k_line_info['week04'] = 0
-        k_line_info['week_last_day'] = month_begin_day
-        k_line_info['sum_week'] = 0
-        return k_line_info
-    stock_hfq_weekly = stock_hfq_weekly.sort_values(by=['date'], ascending=False)
-    stock_hfq_weekly_last = stock_hfq_weekly.iloc[0:1]
-    k_line_info['week_last_day'] = list(stock_hfq_weekly_last['date'])[0]
-
-    return k_line_info
-
-
-# 处理日线
-def handle_day_line(k_line_info, str_day, symbol):
-    deal_days = k_line_common_service_api.get_deal_days(str_day, symbol)
-
-    # 取五天刚好包含一周 todo 选择60天的历史记录
-    # 当天没有k线数据时 进行同步
-    query = {"symbol": symbol, 'date': {"$lt": date_handle_util.no_slash_date(str_day)}}
-    stock_qfq_daily = mongodb_util.descend_query(query, 'stock_qfq_daily', 'date', 60)
-    if stock_qfq_daily.shape[0] == 0:
-        return k_line_info
-    k_line_info = init_day_line_data(k_line_info, stock_qfq_daily)
-    k_line_info = calculate_30_day_max_chg(stock_qfq_daily, k_line_info)
-
-    stock_qfq_daily = calculate_exchange_avg_param(stock_qfq_daily)
-    stock_qfq_daily_one = stock_qfq_daily.iloc[0:1]
-    stock_qfq_daily_one = set_k_line_patterns(stock_qfq_daily_one.copy())
-    stock_qfq_daily_one = set_history_list(stock_qfq_daily_one.copy(), stock_qfq_daily.copy())
-    k_line_info = k_line_field_fix(k_line_info.copy(), stock_qfq_daily_one.copy())
-
-    k_line_info.loc[:, 'deal_days'] = deal_days
-
-    k_line_info.loc[k_line_info['deal_days'] > 5, 'sum_five_chg'] = k_line_info['daily01'] \
-                                                                    + k_line_info['daily02'] \
-                                                                    + k_line_info['daily03'] \
-                                                                    + k_line_info['daily04'] \
-                                                                    + k_line_info['daily05']
-    k_line_info.loc[k_line_info['deal_days'] <= 5, 'sum_five_chg'] = 0
-
-    # 计算开盘涨幅
-    k_line_info = calculate_open_chg(stock_qfq_daily, k_line_info)
-    # 排除最近有三板以上的股票
-    k_line_info = check_recent_zt_stock(str_day, k_line_info)
-    # 计算 昨日最高点到开盘涨幅差值 and   # 昨日最高点到当日收盘涨幅之间的差值
-    k_line_info = calculate_chg_diff_value(k_line_info)
-
-    recent_hot_stocks_clean_service.calculate_recent_hot_stocks(stock_qfq_daily, symbol, str_day)
 
-    return k_line_info
-
-
-# 计算涨幅差值
-def calculate_chg_diff_value(result):
-    # 昨日最高点到开盘涨幅差值
-    result['diff_chg_from_open_last'] = round(
-        result['max_chg_last'] - result['open_chg_last'], 2)
-
-    # 昨日最高点到当日收盘涨幅之间的差值
-    result['diff_chg_high_last'] = round(
-        result['max_chg_last'] - result['chg_last'], 2)
-
-    return result
+# 计算五日线之和交易天数最小值
+MIN_DEAL_DAYS = 6
 
 
+# 初始化数据
 def init_day_line_data(k_line_info, stock_qfq_daily):
     daily_num = stock_qfq_daily.shape[0]
     if daily_num == 0:
         k_line_info['max_chg_daily01'] = 0
         k_line_info['daily01'] = 0
         k_line_info['daily02'] = 0
         k_line_info['daily03'] = 0
@@ -212,28 +53,75 @@
     elif daily_num >= 5:
         k_line_info['max_chg_daily01'] = stock_qfq_daily.iloc[0].max_chg
         k_line_info['daily01'] = stock_qfq_daily.iloc[0].chg
         k_line_info['daily02'] = stock_qfq_daily.iloc[1].chg
         k_line_info['daily03'] = stock_qfq_daily.iloc[2].chg
         k_line_info['daily04'] = stock_qfq_daily.iloc[3].chg
         k_line_info['daily05'] = stock_qfq_daily.iloc[4].chg
+    k_line_info.loc[:, 'exclude'] = False
+    # 30日最大涨幅
+    k_line_info.loc[:, 'amount_level_last'] = 0
+    k_line_info.loc[:, 'exchange_last'] = 0
+    k_line_info.loc[:, 'exchange_mean_last'] = 0
+    k_line_info.loc[:, 'exchange_mean_last_02'] = 0
+    k_line_info.loc[:, 'exchange_difference_last'] = 0
+    k_line_info.loc[:, 'exchange_chg_percent_last'] = 0
+    k_line_info.loc[:, 'pct_chg_mean_last'] = 0
+    k_line_info.loc[:, 'pct_chg_difference_last'] = 0
+    k_line_info.loc[:, 'close_difference_five_last'] = 0
+    k_line_info.loc[:, 'close_difference_ten_last'] = 0
+    k_line_info.loc[:, 'close_difference_twenty_last'] = 0
+    k_line_info.loc[:, 'close_difference_thirty_last'] = 0
+    k_line_info.loc[:, 'close_difference_sixty_last'] = 0
+    k_line_info.loc[:, 'pct_chg_last'] = 0
+    k_line_info.loc[:, 'max_chg_last'] = 0
+    k_line_info.loc[:, 'chg_last'] = 0
+    k_line_info.loc[:, 'close_last'] = 0
+    k_line_info.loc[:, 'high_last'] = 0
+    k_line_info.loc[:, 'low_last'] = 0
+
+    k_line_info.loc[:, 'avg_five_last'] = 0
+    k_line_info.loc[:, 'avg_ten_last'] = 0
+    k_line_info.loc[:, 'avg_twenty_last'] = 0
+    k_line_info.loc[:, 'avg_thirty_last'] = 0
+    k_line_info.loc[:, 'avg_sixty_last'] = 0
+
+    k_line_info.loc[:, 'std_amount_ten'] = 0
+    k_line_info.loc[:, 'mean_amount_ten'] = 0
+    k_line_info.loc[:, 'std_amount_thirty'] = 0
+    k_line_info.loc[:, 'mean_amount_thirty'] = 0
+
+    k_line_info.loc[:, 'std_amount_sixty'] = 0
+    k_line_info.loc[:, 'mean_amount_sixty'] = 0
+
+    k_line_info.loc[:, 'sum_five_chg'] = 0
+
+    k_line_info.loc[:, 'open_chg_last'] = 0
+
+    k_line_info.loc[:, 'before_close'] = 0
+
+    k_line_info.loc[:, 'diff_max_chg_from_open_last'] = 0
+
+    k_line_info.loc[:, 'diff_max_chg_from_close_last'] = 0
+
+    k_line_info.loc[:, 'diff_close_from_open_last'] = 0
 
     return k_line_info
 
 
 # 计算30天最大涨幅
 def calculate_30_day_max_chg(stock_qfq_daily, k_line_info):
+    # 取30天的交易k线
     stock_qfq_daily_30 = stock_qfq_daily.iloc[0:29]
 
     deal_days = stock_qfq_daily_30.shape[0]
 
-    if stock_qfq_daily_30.shape[0] < 30:
+    if deal_days < 30:
         stock_qfq_daily_30 = stock_qfq_daily_30[0: deal_days - 1]
-    if stock_qfq_daily_30.shape[0] == 0:
-        k_line_info['max_chg_30'] = 0
+    if deal_days == 0:
         return k_line_info
 
     stock_qfq_daily_30['date_time'] = pd.to_datetime(stock_qfq_daily_30['date'])
     # 找出最高点和最低点的行
     max_row = stock_qfq_daily_30[stock_qfq_daily_30['high'] == stock_qfq_daily_30['high'].max()]
     min_row = stock_qfq_daily_30[stock_qfq_daily_30['low'] == stock_qfq_daily_30['low'].min()]
 
@@ -245,34 +133,35 @@
     max_chg_30 = round((max_high - min_low) * 100 / min_low, 2)
     if date_of_max_high < date_of_min_low:
         max_chg_30 = -max_chg_30
     k_line_info['max_chg_30'] = max_chg_30
     return k_line_info
 
 
-# 计算平均值
-def calculate_exchange_avg_param(stock_qfq_daily):
+# 计算换手平均值 k线 5 10 20 30 60均线
+def calculate_exchange_and_k_line_avg_param(stock_qfq_daily):
     stock_qfq_daily = stock_qfq_daily.sort_values(by=['date'], ascending=True)
 
-    # exchange
-    # 计算每个日期的前10天的均值
+    # 计算每个日期前10天的换手均值
     stock_qfq_daily['exchange_mean'] = round(
         stock_qfq_daily['exchange'].rolling(window=10, min_periods=1).mean(), 2)
 
     # stock_qfq_daily['exchange_mean_ewm'] = round(
     #     stock_qfq_daily['exchange'].ewm(span=10).mean(), 2)
 
     stock_qfq_daily['exchange_mean_yesterday'] = stock_qfq_daily['exchange_mean']
 
     # 昨日平均值 向当前移位
     stock_qfq_daily['exchange_mean_yesterday'] = stock_qfq_daily['exchange_mean_yesterday'].shift(1)
 
+    # 今天换手相对于[昨日平均十日换手]的差值
     stock_qfq_daily['exchange_difference'] = round(
         stock_qfq_daily['exchange'] - stock_qfq_daily['exchange_mean_yesterday'], 2)
 
+    # 今天换手相对于[昨日平均十日换手]的倍数
     stock_qfq_daily['exchange_chg_percent'] = round(
         stock_qfq_daily['exchange'] / stock_qfq_daily['exchange_mean_yesterday'], 2)
 
     # pct_chg
 
     # 计算每个日期的前10天的均值
     stock_qfq_daily['pct_chg_mean'] = round(stock_qfq_daily['pct_chg'].rolling(window=10, min_periods=1).mean(),
@@ -301,15 +190,15 @@
     stock_qfq_daily['avg_thirty'] = round(stock_qfq_daily['close'].rolling(window=30, min_periods=1).mean(),
                                           2)
 
     # 计算六十日均线
     stock_qfq_daily['avg_sixty'] = round(stock_qfq_daily['close'].rolling(window=60, min_periods=1).mean(),
                                          2)
 
-    # 与均线差值
+    # 收盘价格与均线差值
     stock_qfq_daily['close_difference_five'] = round(
         100 * (stock_qfq_daily['close'] - stock_qfq_daily['avg_five']) / stock_qfq_daily['close'],
         2)
 
     stock_qfq_daily['close_difference_ten'] = round(
         100 * (stock_qfq_daily['close'] - stock_qfq_daily['avg_ten']) / stock_qfq_daily['close'],
         2)
@@ -368,14 +257,29 @@
     ]]
     stock_qfq_daily = stock_qfq_daily.sort_values(by=['date'], ascending=False)
     stock_qfq_daily = stock_qfq_daily.fillna(0)
 
     return stock_qfq_daily
 
 
+# 设置当天k线形态 下一个交易日判断当前交易日k线形态
+def set_k_line_patterns(stock_qfq_daily_one):
+    open = list(stock_qfq_daily_one['open'])[0]
+    close = list(stock_qfq_daily_one['close'])[0]
+    high = list(stock_qfq_daily_one['high'])[0]
+    low = list(stock_qfq_daily_one['low'])[0]
+    max_chg = list(stock_qfq_daily_one['max_chg'])[0]
+    chg = list(stock_qfq_daily_one['chg'])[0]
+
+    k_line_pattern = k_line_patterns_service.k_line_patterns_classify(open, close, high, low, max_chg, chg)
+    stock_qfq_daily_one.loc[:, 'k_line_pattern'] = k_line_pattern.value
+    return stock_qfq_daily_one
+
+
+# 设置历史k线列表
 def set_history_list(stock_qfq_daily_one, stock_qfq_daily):
     stock_qfq_daily = stock_qfq_daily[[
         "date",
         "exchange",
         "exchange_mean",
         "exchange_mean_yesterday",
         "exchange_difference",
@@ -405,17 +309,17 @@
     std_amount_thirty = 0
     mean_amount_thirty = 0
     std_amount_sixty = 0
     mean_amount_sixty = 0
 
     if daily_num >= 10:
         stock_qfq_daily_ten = stock_qfq_daily.iloc[0:10]
-        # 计算 amount 的标准差
+        # 计算 10日 amount 的标准差
         std_amount_ten = round(stock_qfq_daily_ten['amount_level'].std(), 2)
-        # 计算 amount 的平均值
+        # 计算 10日amount 的平均值
         mean_amount_ten = round(stock_qfq_daily_ten['amount_level'].mean(), 2)
 
     if daily_num >= 30:
         stock_qfq_daily_thirty = stock_qfq_daily.iloc[0:30]
         # 计算 amount 的标准差
         std_amount_thirty = round(stock_qfq_daily_thirty['amount_level'].std(), 2)
         # 计算 amount 的平均值
@@ -434,30 +338,16 @@
     stock_qfq_daily_one.loc[:, 'mean_amount_thirty'] = mean_amount_thirty
     stock_qfq_daily_one.loc[:, 'std_amount_sixty'] = std_amount_sixty
     stock_qfq_daily_one.loc[:, 'mean_amount_sixty'] = mean_amount_sixty
 
     return stock_qfq_daily_one
 
 
-# k线形态
-def set_k_line_patterns(stock_qfq_daily_one):
-    open = list(stock_qfq_daily_one['open'])[0]
-    close = list(stock_qfq_daily_one['close'])[0]
-    high = list(stock_qfq_daily_one['high'])[0]
-    low = list(stock_qfq_daily_one['low'])[0]
-    max_chg = list(stock_qfq_daily_one['max_chg'])[0]
-    chg = list(stock_qfq_daily_one['chg'])[0]
-
-    k_line_pattern = k_line_patterns_service.k_line_patterns_classify(open, close, high, low, max_chg, chg)
-    stock_qfq_daily_one.loc[:, 'k_line_pattern'] = k_line_pattern.value
-    return stock_qfq_daily_one
-
-
-# 字段选择
-def k_line_field_fix(k_line_info, stock_qfq_daily_one):
+# 修改字段名称
+def k_line_field_fix_name(k_line_info, stock_qfq_daily_one):
     k_line_info['classification'] = stock_qfq_daily_one['classification']
     k_line_info['amount_level_last'] = stock_qfq_daily_one['amount_level']
     k_line_info['name'] = stock_qfq_daily_one['name']
     k_line_info['exchange_last'] = stock_qfq_daily_one['exchange']
     k_line_info['exchange_mean_last'] = stock_qfq_daily_one['exchange_mean']
     k_line_info['exchange_mean_last_02'] = stock_qfq_daily_one['exchange_mean_yesterday']
     k_line_info['exchange_difference_last'] = stock_qfq_daily_one['exchange_difference']
@@ -493,30 +383,52 @@
     k_line_info['mean_amount_sixty'] = stock_qfq_daily_one['mean_amount_sixty']
     k_line_info['k_line_pattern'] = stock_qfq_daily_one['k_line_pattern']
     k_line_info['history_data'] = stock_qfq_daily_one['history_data']
 
     return k_line_info
 
 
-# 计算开盘涨幅
+# 设置五日k线和
+def set_sum_five_chg(k_line_info, deal_days):
+    k_line_info.loc[:, 'deal_days'] = deal_days
+    # 排除上市第一天的k线
+    k_line_info.loc[k_line_info['deal_days'] >= MIN_DEAL_DAYS, 'sum_five_chg'] = k_line_info['daily01'] \
+                                                                                 + k_line_info['daily02'] \
+                                                                                 + k_line_info['daily03'] \
+                                                                                 + k_line_info['daily04'] \
+                                                                                 + k_line_info['daily05']
+    k_line_info.loc[k_line_info['deal_days'] < MIN_DEAL_DAYS, 'sum_five_chg'] = 0
+
+    return k_line_info
+
+
+# 计算当前交易日开盘时的涨幅
 def calculate_open_chg(stock_qfq_daily, k_line_info):
     # 新股
     if stock_qfq_daily.shape[0] == 1:
         k_line_info['open_chg_last'] = k_line_info['daily01']
     else:
         # 获取前一个交易日的收盘价格
         k_line_info['before_close'] = round(
             k_line_info['close_last'] / (1 + k_line_info['daily01'] * 0.01), 2)
         k_line_info['open_chg_last'] = round((k_line_info['open_last'] / k_line_info['before_close'] - 1) * 100, 2)
     return k_line_info
 
 
-# 排除最近10个交易日有三板以上的股票
-def check_recent_zt_stock(str_day, k_line_info):
-    k_line_info.loc[:, 'exclude'] = False
-    k_line_info = symbol_classify_api.set_stock_type(k_line_info)
-    k_line_info_sh = symbol_classify_api.choose_sh_symbol(k_line_info)
-    if data_frame_util.is_empty(k_line_info_sh):
-        return k_line_info
-    else:
-        k_line_info_sh = sh_small_normal_zt_k_line_check_api.recent_day_zt_check(k_line_info_sh.copy())
-        return k_line_info_sh
+# 计算涨幅差值
+# 昨日最高点到开盘涨幅差值
+# 昨日最高点到当日收盘涨幅之间的差值
+# 昨日收盘到当日开盘涨幅之间的差值
+def calculate_chg_diff_value(result):
+    # 昨日最高点到开盘涨幅差值
+    result['diff_max_chg_from_open_last'] = round(
+        result['max_chg_last'] - result['open_chg_last'], 2)
+
+    # 昨日最高点到当日收盘涨幅之间的差值
+    result['diff_max_chg_from_close_last'] = round(
+        result['max_chg_last'] - result['chg_last'], 2)
+
+    # 昨日最高点到当日收盘涨幅之间的差值
+    result['diff_close_from_open_last'] = round(
+        result['chg_last'] - result['open_chg_last'], 2)
+
+    return result
```

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/k_line/clean/k_line_info_clean_service.py` & `mns-scheduler-1.0.7.1/mns_scheduler/k_line/clean/k_line_info_clean_task.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import threading
 import mns_common.component.trade_date.trade_date_common_service_api as trade_date_common_service_api
 import mns_common.component.common_service_fun_api as common_service_fun_api
 import mns_scheduler.k_line.sync.daily_week_month_line_sync as daily_week_month_line_sync_api
 import mns_scheduler.k_line.clean.k_line_info_clean_impl as k_line_info_clean_impl
 import mns_common.utils.data_frame_util as data_frame_util
 import mns_common.component.company.company_common_service_api as company_common_service_api
+
 K_LINE_CLEAN_DB_NAME = 'k_line_clean_fail_name'
 
 # 定义一个全局锁，用于保护 result 变量的访问
 result_lock = threading.Lock()
 # 初始化 result 变量为一个空的 Pandas DataFrame
 result = pd.DataFrame()
 # 分页大小
@@ -32,14 +33,15 @@
 def sync_k_line_info_task(str_day):
     # 创建索引
     create_k_line_index()
 
     last_trade_day = trade_date_common_service_api.get_last_trade_day(str_day)
     query = {'date': date_handle_util.no_slash_date(last_trade_day)}
     count = mongodb_util.count(query, 'stock_qfq_daily')
+    # 当天没有k线数据时 进行同步
     if count == 0:
         daily_week_month_line_sync_api.sync_all_daily_data('daily', 'qfq', 'stock_qfq_daily', str_day,
                                                            None)
     sync_k_line_info(str_day, None)
 
 
 def sync_k_line_info(str_day, symbol_list):
@@ -86,15 +88,18 @@
     if data_frame_util.is_not_empty(k_line_fail_df):
         fail_data_df = real_time_quotes_now.loc[real_time_quotes_now['symbol'].isin(k_line_fail_df['symbol'])]
         single_threaded_sync_task(fail_data_df, str_day, 88)
 
 
 # 多线程同步任务
 def multi_threaded_k_line_sync(str_day):
+    # 退市代码
+    de_list_company_symbols = company_common_service_api.get_de_list_company()
     real_time_quotes_now = east_money_stock_api.get_real_time_quotes_all_stocks()
+    real_time_quotes_now = real_time_quotes_now.loc[~(real_time_quotes_now['symbol'].isin(de_list_company_symbols))]
 
     # 将list_date列中的所有NaN值设置为99990909
     real_time_quotes_now['list_date'].fillna(20990909.0, inplace=True)
 
     # 将日期数值转换为日期时间格式
     real_time_quotes_now['list_date_01'] = pd.to_datetime(real_time_quotes_now['list_date'], format='%Y%m%d')
 
@@ -180,10 +185,10 @@
             sync_k_line_info_task(trade_data_one.trade_date)
             logger.info("清洗数据到:{}", trade_data_one.trade_date)
         except BaseException as e:
             logger.error("发生异常:{},{}", trade_data_one.trade_date, e)
 
 
 if __name__ == '__main__':
-    sync_k_line_info("2024-05-24", None)
+    sync_k_line_info("2024-06-03", None)
     # clean_history_data()
     # sync_k_line_info("2023-12-22")
```

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/k_line/clean/recent_hot_stocks_clean_service.py` & `mns-scheduler-1.0.7.1/mns_scheduler/k_line/hot_stocks/recent_hot_stocks_clean_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/k_line/sync/daily_week_month_line_sync.py` & `mns-scheduler-1.0.7.1/mns_scheduler/k_line/sync/daily_week_month_line_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py` & `mns-scheduler-1.0.7.1/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/kpl/selection/index/sync_best_choose_index.py` & `mns-scheduler-1.0.7.1/mns_scheduler/kpl/selection/index/sync_best_choose_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py` & `mns-scheduler-1.0.7.1/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py` & `mns-scheduler-1.0.7.1/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/lhb/stock_lhb_sync_service.py` & `mns-scheduler-1.0.7.1/mns_scheduler/lhb/stock_lhb_sync_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py` & `mns-scheduler-1.0.7.1/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/real_time/realtime_quotes_now_sync.py` & `mns-scheduler-1.0.7.1/mns_scheduler/real_time/realtime_quotes_now_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/risk/register_and_investigate_stock_sync_api.py` & `mns-scheduler-1.0.7.1/mns_scheduler/risk/register_and_investigate_stock_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/risk/stock_equity_mortgage_sync_api.py` & `mns-scheduler-1.0.7.1/mns_scheduler/risk/stock_equity_mortgage_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/trade/auto_sell_service_api.py` & `mns-scheduler-1.0.7.1/mns_scheduler/trade/auto_sell_service_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/trade/sync_position_api.py` & `mns-scheduler-1.0.7.1/mns_scheduler/trade/sync_position_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/zb/stock_zb_pool_sync.py` & `mns-scheduler-1.0.7.1/mns_scheduler/zb/stock_zb_pool_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/zt/__init__.py` & `mns-scheduler-1.0.7.1/mns_scheduler/zt/__init__.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/zt/export_open_data_to_excel.py` & `mns-scheduler-1.0.7.1/mns_scheduler/zt/export_open_data_to_excel.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py` & `mns-scheduler-1.0.7.1/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/zt/today_high_chg_pool_sync_api.py` & `mns-scheduler-1.0.7.1/mns_scheduler/zt/today_high_chg_pool_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/zt/zt_five_boards_sync_api.py` & `mns-scheduler-1.0.7.1/mns_scheduler/zt/zt_five_boards_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/zt/zt_pool_sync_api.py` & `mns-scheduler-1.0.7.1/mns_scheduler/zt/zt_pool_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/zz_task/data_sync_task.py` & `mns-scheduler-1.0.7.1/mns_scheduler/zz_task/data_sync_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import mns_scheduler.db.db_status as db_status_api
 import mns_scheduler.big_deal.ths_big_deal_sync as ths_big_deal_sync_api
 import mns_scheduler.zt.realtime_quotes_now_zt_kc_sync as realtime_quotes_now_zt_kc_sync_api
 import mns_scheduler.zt.export_open_data_to_excel as export_open_data_to_excel_api
 import mns_scheduler.zt.zt_five_boards_sync_api as zt_five_boards_sync_api
 import mns_scheduler.zt.zt_pool_sync_api as zt_pool_sync_api
 import mns_scheduler.zt.today_high_chg_pool_sync_api as today_high_chg_pool_sync_api
-import mns_scheduler.k_line.clean.k_line_info_clean_service as k_line_info_clean_service
+import mns_scheduler.k_line.clean.k_line_info_clean_task as k_line_info_clean_service
 import mns_scheduler.concept.clean.ths_concept_clean_api as ths_concept_choose_api
 import mns_common.api.em.east_money_stock_gdfx_free_top_10_api as east_money_stock_gdfx_free_top_10_api
 import \
     mns_scheduler.concept.ths.update_concept_info.sync_one_concept_all_symbols_api as sync_one_concept_all_symbols_api
 import \
     mns_scheduler.concept.ths.update_concept_info.sync_one_symbol_all_concepts_api as sync_one_symbol_all_concepts_api
 import mns_scheduler.concept.ths.sync_new_index.sync_ths_new_concept_by_web_api as sync_ths_new_concept_by_web_api
```

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler/zz_task/sync_realtime_quotes_task.py` & `mns-scheduler-1.0.7.1/mns_scheduler/zz_task/sync_realtime_quotes_task.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.6.9/mns_scheduler.egg-info/SOURCES.txt` & `mns-scheduler-1.0.7.1/mns_scheduler.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -53,16 +53,23 @@
 mns_scheduler/irm/stock_irm_cninfo_service.py
 mns_scheduler/irm/api/__init__.py
 mns_scheduler/irm/api/sh_stock_sns_sse_info_api.py
 mns_scheduler/irm/api/sz_stock_sns_sse_info_api.py
 mns_scheduler/k_line/__init__.py
 mns_scheduler/k_line/clean/__init__.py
 mns_scheduler/k_line/clean/k_line_info_clean_impl.py
-mns_scheduler/k_line/clean/k_line_info_clean_service.py
-mns_scheduler/k_line/clean/recent_hot_stocks_clean_service.py
+mns_scheduler/k_line/clean/k_line_info_clean_task.py
+mns_scheduler/k_line/clean/daily/__init__.py
+mns_scheduler/k_line/clean/daily/daily_k_line_clean_common_service.py
+mns_scheduler/k_line/clean/daily/daily_k_line_service.py
+mns_scheduler/k_line/clean/week_month/__init__.py
+mns_scheduler/k_line/clean/week_month/normal_week_month_k_line_service.py
+mns_scheduler/k_line/clean/week_month/sub_new_week_month_k_line_service.py
+mns_scheduler/k_line/hot_stocks/__init__.py
+mns_scheduler/k_line/hot_stocks/recent_hot_stocks_clean_service.py
 mns_scheduler/k_line/sync/__init__.py
 mns_scheduler/k_line/sync/daily_week_month_line_sync.py
 mns_scheduler/kpl/__init__.py
 mns_scheduler/kpl/selection/__init__.py
 mns_scheduler/kpl/selection/index/__init__.py
 mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py
 mns_scheduler/kpl/selection/index/sync_best_choose_index.py
```

