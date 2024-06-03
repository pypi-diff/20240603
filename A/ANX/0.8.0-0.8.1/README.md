# Comparing `tmp/ANX-0.8.0.tar.gz` & `tmp/ANX-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ANX-0.8.0.tar", last modified: Thu May 23 07:49:20 2024, max compression
+gzip compressed data, was "ANX-0.8.1.tar", last modified: Mon Jun  3 09:50:01 2024, max compression
```

## Comparing `ANX-0.8.0.tar` & `ANX-0.8.1.tar`

### file list

```diff
@@ -1,166 +1,166 @@
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.837765 ANX-0.8.0/
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.803773 ANX-0.8.0/ANX.egg-info/
--rw-r--r--   0 1a         (501) staff       (20)      125 2024-05-23 07:49:20.000000 ANX-0.8.0/ANX.egg-info/PKG-INFO
--rw-r--r--   0 1a         (501) staff       (20)     4882 2024-05-23 07:49:20.000000 ANX-0.8.0/ANX.egg-info/SOURCES.txt
--rw-r--r--   0 1a         (501) staff       (20)        1 2024-05-23 07:49:20.000000 ANX-0.8.0/ANX.egg-info/dependency_links.txt
--rw-r--r--   0 1a         (501) staff       (20)      108 2024-05-23 07:49:20.000000 ANX-0.8.0/ANX.egg-info/requires.txt
--rw-r--r--   0 1a         (501) staff       (20)       10 2024-05-23 07:49:20.000000 ANX-0.8.0/ANX.egg-info/top_level.txt
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.804326 ANX-0.8.0/AndroidQQ/
--rw-r--r--   0 1a         (501) staff       (20)    34971 2024-05-23 07:48:15.000000 ANX-0.8.0/AndroidQQ/Android.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.804689 ANX-0.8.0/AndroidQQ/Echo/
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/Echo/Tcp.py
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/Echo/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     4522 2024-05-15 01:55:22.000000 ANX-0.8.0/AndroidQQ/Tcp.py
--rw-r--r--   0 1a         (501) staff       (20)       71 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.807541 ANX-0.8.0/AndroidQQ/http/
--rw-r--r--   0 1a         (501) staff       (20)     2195 2024-04-08 06:23:23.000000 ANX-0.8.0/AndroidQQ/http/ClientKey.py
--rw-r--r--   0 1a         (501) staff       (20)      138 2024-04-08 05:21:16.000000 ANX-0.8.0/AndroidQQ/http/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     2009 2024-04-08 05:37:11.000000 ANX-0.8.0/AndroidQQ/http/accounts.py
--rw-r--r--   0 1a         (501) staff       (20)      820 2024-04-08 05:31:10.000000 ANX-0.8.0/AndroidQQ/http/cip.py
--rw-r--r--   0 1a         (501) staff       (20)     4061 2024-04-08 05:46:08.000000 ANX-0.8.0/AndroidQQ/http/friends.py
--rw-r--r--   0 1a         (501) staff       (20)     4734 2024-05-19 23:14:02.000000 ANX-0.8.0/AndroidQQ/http/game_credit.py
--rw-r--r--   0 1a         (501) staff       (20)      422 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/http/headers.py
--rw-r--r--   0 1a         (501) staff       (20)     7243 2024-04-25 09:25:24.000000 ANX-0.8.0/AndroidQQ/http/level.py
--rw-r--r--   0 1a         (501) staff       (20)    11548 2024-04-25 09:27:50.000000 ANX-0.8.0/AndroidQQ/http/music.py
--rw-r--r--   0 1a         (501) staff       (20)     1499 2024-04-08 05:42:12.000000 ANX-0.8.0/AndroidQQ/http/qqsignin.py
--rw-r--r--   0 1a         (501) staff       (20)     1325 2024-04-08 05:50:32.000000 ANX-0.8.0/AndroidQQ/http/weishi.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.807762 ANX-0.8.0/AndroidQQ/im/
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/im/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.807852 ANX-0.8.0/AndroidQQ/im/oidb/
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.808189 ANX-0.8.0/AndroidQQ/im/oidb/OidbSvc_0xc96/
--rw-r--r--   0 1a         (501) staff       (20)     2797 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/im/oidb/OidbSvc_0xc96/OidbSvc_0xc96_pb2.py
--rw-r--r--   0 1a         (501) staff       (20)       34 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/im/oidb/OidbSvc_0xc96/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/im/oidb/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.808710 ANX-0.8.0/AndroidQQ/im/oidb/cmd0x88d/
--rw-r--r--   0 1a         (501) staff       (20)       30 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/im/oidb/cmd0x88d/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     2139 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/im/oidb/cmd0x88d/oidb_0x88d_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.810253 ANX-0.8.0/AndroidQQ/im/oidb/cmd0x922/
--rw-r--r--   0 1a         (501) staff       (20)     1343 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/im/oidb/cmd0x922/PushInfo_pb2.py
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/im/oidb/cmd0x922/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1542 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/im/oidb/cmd0x922/cmd0x922_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.810772 ANX-0.8.0/AndroidQQ/im/oidb/cmd0xeb8/
--rw-r--r--   0 1a         (501) staff       (20)       28 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/im/oidb/cmd0xeb8/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1872 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/im/oidb/cmd0xeb8/cmd0xeb8_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.811313 ANX-0.8.0/AndroidQQ/im/oidb/oidb_0xc05/
--rw-r--r--   0 1a         (501) staff       (20)       30 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/im/oidb/oidb_0xc05/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     2603 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/im/oidb/oidb_0xc05/oidb_0xc05_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.811830 ANX-0.8.0/AndroidQQ/im/oidb/oidb_sso/
--rw-r--r--   0 1a         (501) staff       (20)       27 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/im/oidb/oidb_sso/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1468 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/im/oidb/oidb_sso/oidb_sso_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.812397 ANX-0.8.0/AndroidQQ/im/oidb/qqconnect/
--rw-r--r--   0 1a         (501) staff       (20)       29 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/im/oidb/qqconnect/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     2618 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/im/oidb/qqconnect/qqconnect_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.813382 ANX-0.8.0/AndroidQQ/im/oidb/scanlogin/
--rw-r--r--   0 1a         (501) staff       (20)       29 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/im/oidb/scanlogin/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1385 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/im/oidb/scanlogin/scanlogin_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.813683 ANX-0.8.0/AndroidQQ/log/
--rw-r--r--   0 1a         (501) staff       (20)       33 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/log/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.817493 ANX-0.8.0/AndroidQQ/pack/
--rw-r--r--   0 1a         (501) staff       (20)      395 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/pack/Heartbeat_Alive.py
--rw-r--r--   0 1a         (501) staff       (20)      872 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/pack/MQUpdateSvc_com_qq_ti_web_scanlogin.py
--rw-r--r--   0 1a         (501) staff       (20)      733 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/pack/MQUpdateSvc_com_qq_vip_zb_web_OidbSvc_0xdfa_0.py
--rw-r--r--   0 1a         (501) staff       (20)     1368 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/pack/OidbSvc_0x88d_1.py
--rw-r--r--   0 1a         (501) staff       (20)      986 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/pack/OidbSvc_0xc05.py
--rw-r--r--   0 1a         (501) staff       (20)     1141 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/pack/OidbSvc_0xc96.py
--rw-r--r--   0 1a         (501) staff       (20)      872 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/pack/OidbSvc_0xeb8.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.819100 ANX-0.8.0/AndroidQQ/pack/SQQzoneSvc/
--rw-r--r--   0 1a         (501) staff       (20)       94 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/pack/SQQzoneSvc/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1124 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/pack/SQQzoneSvc/delUgc.py
--rw-r--r--   0 1a         (501) staff       (20)     2637 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/pack/SQQzoneSvc/like.py
--rw-r--r--   0 1a         (501) staff       (20)     2631 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/pack/SQQzoneSvc/publishmood.py
--rw-r--r--   0 1a         (501) staff       (20)     2152 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/pack/SQQzoneSvc/shuoshuo.py
--rw-r--r--   0 1a         (501) staff       (20)     1116 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/pack/StatSvc_register.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.819512 ANX-0.8.0/AndroidQQ/pack/SummaryCard/
--rw-r--r--   0 1a         (501) staff       (20)     1349 2024-03-07 10:14:41.000000 ANX-0.8.0/AndroidQQ/pack/SummaryCard/ReqSummaryCard.py
--rw-r--r--   0 1a         (501) staff       (20)       29 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/pack/SummaryCard/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)      402 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/pack/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1383 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/pack/friendlist.py
--rw-r--r--   0 1a         (501) staff       (20)      543 2024-03-06 13:46:02.000000 ANX-0.8.0/AndroidQQ/pack/test.py
--rw-r--r--   0 1a         (501) staff       (20)    46467 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/pack/trpc_metaverse_mob_proxy_svr_MobProxy_SsoHandle.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.820230 ANX-0.8.0/AndroidQQ/proto/
--rw-r--r--   0 1a         (501) staff       (20)     4301 2024-02-12 04:07:38.000000 ANX-0.8.0/AndroidQQ/proto/IM_r_pb2.py
--rw-r--r--   0 1a         (501) staff       (20)       67 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/proto/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1308 2023-10-29 17:25:21.000000 ANX-0.8.0/AndroidQQ/proto/wtlogin_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.822502 ANX-0.8.0/AndroidQQ/struct/
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.823667 ANX-0.8.0/AndroidQQ/struct/Avatarlnfo/
--rw-r--r--   0 1a         (501) staff       (20)      444 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/Avatarlnfo/DestQQHeadInfo.py
--rw-r--r--   0 1a         (501) staff       (20)     1061 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/Avatarlnfo/QQHeadInfo.py
--rw-r--r--   0 1a         (501) staff       (20)      853 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/Avatarlnfo/QQHeadUrlReq.py
--rw-r--r--   0 1a         (501) staff       (20)      673 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/Avatarlnfo/QQHeadUrlResp.py
--rw-r--r--   0 1a         (501) staff       (20)     1028 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/Avatarlnfo/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)      894 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/MessageSvc.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.824183 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_COMM/
--rw-r--r--   0 1a         (501) staff       (20)      373 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_COMM/UgcRightInfo.py
--rw-r--r--   0 1a         (501) staff       (20)       28 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_COMM/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.827431 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_FEEDS/
--rw-r--r--   0 1a         (501) staff       (20)       70 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_FEEDS/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     3064 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_comm.py
--rw-r--r--   0 1a         (501) staff       (20)     1565 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_operation.py
--rw-r--r--   0 1a         (501) staff       (20)      565 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_userinfo.py
--rw-r--r--   0 1a         (501) staff       (20)      895 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_req.py
--rw-r--r--   0 1a         (501) staff       (20)     1789 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_rsp.py
--rw-r--r--   0 1a         (501) staff       (20)      451 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_FEEDS/s_arkshare.py
--rw-r--r--   0 1a         (501) staff       (20)      673 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_FEEDS/s_outshare.py
--rw-r--r--   0 1a         (501) staff       (20)      728 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_FEEDS/s_picurl.py
--rw-r--r--   0 1a         (501) staff       (20)      249 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_FEEDS/s_user.py
--rw-r--r--   0 1a         (501) staff       (20)     1163 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_FEEDS/single_feed.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.829812 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_OPERATION/
--rw-r--r--   0 1a         (501) staff       (20)      479 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_OPERATION/Source.py
--rw-r--r--   0 1a         (501) staff       (20)      187 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_OPERATION/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)      656 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_OPERATION/cmshow_active_result.py
--rw-r--r--   0 1a         (501) staff       (20)     1161 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_delugc_req.py
--rw-r--r--   0 1a         (501) staff       (20)     1300 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_req.py
--rw-r--r--   0 1a         (501) staff       (20)      560 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_rsp.py
--rw-r--r--   0 1a         (501) staff       (20)     3031 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_publishmood_req.py
--rw-r--r--   0 1a         (501) staff       (20)      503 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_publishmood_rsp.py
--rw-r--r--   0 1a         (501) staff       (20)      594 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/OidbSvc.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.832938 ANX-0.8.0/AndroidQQ/struct/QMF_PROTOCAL/
--rw-r--r--   0 1a         (501) staff       (20)      504 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/QMF_PROTOCAL/QmfBusiControl.py
--rw-r--r--   0 1a         (501) staff       (20)      630 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/QMF_PROTOCAL/QmfClientIpInfo.py
--rw-r--r--   0 1a         (501) staff       (20)      714 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/QMF_PROTOCAL/QmfDownstream.py
--rw-r--r--   0 1a         (501) staff       (20)      526 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/QMF_PROTOCAL/QmfTokenInfo.py
--rw-r--r--   0 1a         (501) staff       (20)     1180 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/QMF_PROTOCAL/QmfUpstream.py
--rw-r--r--   0 1a         (501) staff       (20)      489 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/QMF_PROTOCAL/RetryInfo.py
--rw-r--r--   0 1a         (501) staff       (20)       87 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/QMF_PROTOCAL/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.833278 ANX-0.8.0/AndroidQQ/struct/QQService/
--rw-r--r--   0 1a         (501) staff       (20)     1112 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/QQService/SvcReqGetDevLoginInfo.py
--rw-r--r--   0 1a         (501) staff       (20)      878 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/QQService/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1043 2024-05-10 20:44:20.000000 ANX-0.8.0/AndroidQQ/struct/StatSvc.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.834214 ANX-0.8.0/AndroidQQ/struct/SummaryCard/
--rw-r--r--   0 1a         (501) staff       (20)     2861 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/SummaryCard/ReqSummaryCard.py
--rw-r--r--   0 1a         (501) staff       (20)      493 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/SummaryCard/UserLocaleInfo.py
--rw-r--r--   0 1a         (501) staff       (20)       61 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/SummaryCard/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)    15568 2024-03-05 18:40:23.000000 ANX-0.8.0/AndroidQQ/struct/Tlv.py
--rw-r--r--   0 1a         (501) staff       (20)     4784 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/Tlv_res.py
--rw-r--r--   0 1a         (501) staff       (20)      131 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.834701 ANX-0.8.0/AndroidQQ/struct/cooperation/
--rw-r--r--   0 1a         (501) staff       (20)       23 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/cooperation/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.835225 ANX-0.8.0/AndroidQQ/struct/cooperation/qzone/
--rw-r--r--   0 1a         (501) staff       (20)     4558 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/cooperation/qzone/WNSStream.py
--rw-r--r--   0 1a         (501) staff       (20)       26 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/cooperation/qzone/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.835514 ANX-0.8.0/AndroidQQ/struct/feedcomponent/
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/feedcomponent/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1482 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/feedcomponent/model.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.835889 ANX-0.8.0/AndroidQQ/struct/friendlist/
--rw-r--r--   0 1a         (501) staff       (20)     2842 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/friendlist/AddFriendReq.py
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/friendlist/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     7428 2024-03-07 10:14:48.000000 ANX-0.8.0/AndroidQQ/struct/head.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.836317 ANX-0.8.0/AndroidQQ/struct/push/
--rw-r--r--   0 1a         (501) staff       (20)     3536 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/push/SvcReqRegister.py
--rw-r--r--   0 1a         (501) staff       (20)     2084 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/push/SvcRespRegister.py
--rw-r--r--   0 1a         (501) staff       (20)       31 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/push/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)    27313 2024-03-05 18:40:23.000000 ANX-0.8.0/AndroidQQ/struct/wtlogin.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.837132 ANX-0.8.0/AndroidQQ/utils/
--rw-r--r--   0 1a         (501) staff       (20)       20 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/utils/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)      523 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/utils/build_device.py
--rw-r--r--   0 1a         (501) staff       (20)     1140 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/utils/ecdh.py
--rw-r--r--   0 1a         (501) staff       (20)     1379 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/utils/sso_server.py
--rw-r--r--   0 1a         (501) staff       (20)      735 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/utils/tool.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.837295 ANX-0.8.0/AndroidQQ/wlogin_sdk/
--rw-r--r--   0 1a         (501) staff       (20)       25 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/wlogin_sdk/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.837443 ANX-0.8.0/AndroidQQ/wlogin_sdk/request/
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/wlogin_sdk/request/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)      125 2024-05-23 07:49:20.837611 ANX-0.8.0/PKG-INFO
--rw-r--r--   0 1a         (501) staff       (20)       34 2023-08-04 12:41:32.000000 ANX-0.8.0/README.md
--rw-r--r--   0 1a         (501) staff       (20)       38 2024-05-23 07:49:20.837818 ANX-0.8.0/setup.cfg
--rw-r--r--   0 1a         (501) staff       (20)      601 2024-05-23 07:49:04.000000 ANX-0.8.0/setup.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-06-03 09:50:01.238156 ANX-0.8.1/
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-06-03 09:50:01.204946 ANX-0.8.1/ANX.egg-info/
+-rw-r--r--   0 1a         (501) staff       (20)      125 2024-06-03 09:50:01.000000 ANX-0.8.1/ANX.egg-info/PKG-INFO
+-rw-r--r--   0 1a         (501) staff       (20)     4882 2024-06-03 09:50:01.000000 ANX-0.8.1/ANX.egg-info/SOURCES.txt
+-rw-r--r--   0 1a         (501) staff       (20)        1 2024-06-03 09:50:01.000000 ANX-0.8.1/ANX.egg-info/dependency_links.txt
+-rw-r--r--   0 1a         (501) staff       (20)      108 2024-06-03 09:50:01.000000 ANX-0.8.1/ANX.egg-info/requires.txt
+-rw-r--r--   0 1a         (501) staff       (20)       10 2024-06-03 09:50:01.000000 ANX-0.8.1/ANX.egg-info/top_level.txt
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-06-03 09:50:01.205559 ANX-0.8.1/AndroidQQ/
+-rw-r--r--   0 1a         (501) staff       (20)    35460 2024-06-03 09:48:37.000000 ANX-0.8.1/AndroidQQ/Android.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-06-03 09:50:01.205888 ANX-0.8.1/AndroidQQ/Echo/
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/Echo/Tcp.py
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/Echo/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     4522 2024-05-15 01:55:22.000000 ANX-0.8.1/AndroidQQ/Tcp.py
+-rw-r--r--   0 1a         (501) staff       (20)       71 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-06-03 09:50:01.209041 ANX-0.8.1/AndroidQQ/http/
+-rw-r--r--   0 1a         (501) staff       (20)     2195 2024-04-08 06:23:23.000000 ANX-0.8.1/AndroidQQ/http/ClientKey.py
+-rw-r--r--   0 1a         (501) staff       (20)      138 2024-04-08 05:21:16.000000 ANX-0.8.1/AndroidQQ/http/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     2009 2024-04-08 05:37:11.000000 ANX-0.8.1/AndroidQQ/http/accounts.py
+-rw-r--r--   0 1a         (501) staff       (20)      820 2024-04-08 05:31:10.000000 ANX-0.8.1/AndroidQQ/http/cip.py
+-rw-r--r--   0 1a         (501) staff       (20)     4061 2024-04-08 05:46:08.000000 ANX-0.8.1/AndroidQQ/http/friends.py
+-rw-r--r--   0 1a         (501) staff       (20)     4734 2024-05-19 23:14:02.000000 ANX-0.8.1/AndroidQQ/http/game_credit.py
+-rw-r--r--   0 1a         (501) staff       (20)      422 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/http/headers.py
+-rw-r--r--   0 1a         (501) staff       (20)     7243 2024-04-25 09:25:24.000000 ANX-0.8.1/AndroidQQ/http/level.py
+-rw-r--r--   0 1a         (501) staff       (20)    11548 2024-04-25 09:27:50.000000 ANX-0.8.1/AndroidQQ/http/music.py
+-rw-r--r--   0 1a         (501) staff       (20)     1499 2024-04-08 05:42:12.000000 ANX-0.8.1/AndroidQQ/http/qqsignin.py
+-rw-r--r--   0 1a         (501) staff       (20)     1325 2024-04-08 05:50:32.000000 ANX-0.8.1/AndroidQQ/http/weishi.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-06-03 09:50:01.209293 ANX-0.8.1/AndroidQQ/im/
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/im/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-06-03 09:50:01.209389 ANX-0.8.1/AndroidQQ/im/oidb/
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-06-03 09:50:01.209753 ANX-0.8.1/AndroidQQ/im/oidb/OidbSvc_0xc96/
+-rw-r--r--   0 1a         (501) staff       (20)     2797 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/im/oidb/OidbSvc_0xc96/OidbSvc_0xc96_pb2.py
+-rw-r--r--   0 1a         (501) staff       (20)       34 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/im/oidb/OidbSvc_0xc96/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/im/oidb/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-06-03 09:50:01.210365 ANX-0.8.1/AndroidQQ/im/oidb/cmd0x88d/
+-rw-r--r--   0 1a         (501) staff       (20)       30 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/im/oidb/cmd0x88d/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     2139 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/im/oidb/cmd0x88d/oidb_0x88d_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-06-03 09:50:01.211396 ANX-0.8.1/AndroidQQ/im/oidb/cmd0x922/
+-rw-r--r--   0 1a         (501) staff       (20)     1343 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/im/oidb/cmd0x922/PushInfo_pb2.py
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/im/oidb/cmd0x922/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1542 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/im/oidb/cmd0x922/cmd0x922_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-06-03 09:50:01.211886 ANX-0.8.1/AndroidQQ/im/oidb/cmd0xeb8/
+-rw-r--r--   0 1a         (501) staff       (20)       28 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/im/oidb/cmd0xeb8/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1872 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/im/oidb/cmd0xeb8/cmd0xeb8_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-06-03 09:50:01.212352 ANX-0.8.1/AndroidQQ/im/oidb/oidb_0xc05/
+-rw-r--r--   0 1a         (501) staff       (20)       30 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/im/oidb/oidb_0xc05/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     2603 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/im/oidb/oidb_0xc05/oidb_0xc05_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-06-03 09:50:01.212803 ANX-0.8.1/AndroidQQ/im/oidb/oidb_sso/
+-rw-r--r--   0 1a         (501) staff       (20)       27 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/im/oidb/oidb_sso/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1468 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/im/oidb/oidb_sso/oidb_sso_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-06-03 09:50:01.213267 ANX-0.8.1/AndroidQQ/im/oidb/qqconnect/
+-rw-r--r--   0 1a         (501) staff       (20)       29 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/im/oidb/qqconnect/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     2618 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/im/oidb/qqconnect/qqconnect_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-06-03 09:50:01.213896 ANX-0.8.1/AndroidQQ/im/oidb/scanlogin/
+-rw-r--r--   0 1a         (501) staff       (20)       29 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/im/oidb/scanlogin/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1385 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/im/oidb/scanlogin/scanlogin_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-06-03 09:50:01.214214 ANX-0.8.1/AndroidQQ/log/
+-rw-r--r--   0 1a         (501) staff       (20)       33 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/log/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-06-03 09:50:01.217548 ANX-0.8.1/AndroidQQ/pack/
+-rw-r--r--   0 1a         (501) staff       (20)      395 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/pack/Heartbeat_Alive.py
+-rw-r--r--   0 1a         (501) staff       (20)      872 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/pack/MQUpdateSvc_com_qq_ti_web_scanlogin.py
+-rw-r--r--   0 1a         (501) staff       (20)      733 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/pack/MQUpdateSvc_com_qq_vip_zb_web_OidbSvc_0xdfa_0.py
+-rw-r--r--   0 1a         (501) staff       (20)     1368 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/pack/OidbSvc_0x88d_1.py
+-rw-r--r--   0 1a         (501) staff       (20)      986 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/pack/OidbSvc_0xc05.py
+-rw-r--r--   0 1a         (501) staff       (20)     1141 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/pack/OidbSvc_0xc96.py
+-rw-r--r--   0 1a         (501) staff       (20)      872 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/pack/OidbSvc_0xeb8.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-06-03 09:50:01.219120 ANX-0.8.1/AndroidQQ/pack/SQQzoneSvc/
+-rw-r--r--   0 1a         (501) staff       (20)       94 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/pack/SQQzoneSvc/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1124 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/pack/SQQzoneSvc/delUgc.py
+-rw-r--r--   0 1a         (501) staff       (20)     2637 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/pack/SQQzoneSvc/like.py
+-rw-r--r--   0 1a         (501) staff       (20)     2639 2024-06-03 09:34:21.000000 ANX-0.8.1/AndroidQQ/pack/SQQzoneSvc/publishmood.py
+-rw-r--r--   0 1a         (501) staff       (20)     2152 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/pack/SQQzoneSvc/shuoshuo.py
+-rw-r--r--   0 1a         (501) staff       (20)     1116 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/pack/StatSvc_register.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-06-03 09:50:01.219613 ANX-0.8.1/AndroidQQ/pack/SummaryCard/
+-rw-r--r--   0 1a         (501) staff       (20)     1349 2024-03-07 10:14:41.000000 ANX-0.8.1/AndroidQQ/pack/SummaryCard/ReqSummaryCard.py
+-rw-r--r--   0 1a         (501) staff       (20)       29 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/pack/SummaryCard/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)      402 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/pack/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1383 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/pack/friendlist.py
+-rw-r--r--   0 1a         (501) staff       (20)      543 2024-03-06 13:46:02.000000 ANX-0.8.1/AndroidQQ/pack/test.py
+-rw-r--r--   0 1a         (501) staff       (20)    46467 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/pack/trpc_metaverse_mob_proxy_svr_MobProxy_SsoHandle.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-06-03 09:50:01.220325 ANX-0.8.1/AndroidQQ/proto/
+-rw-r--r--   0 1a         (501) staff       (20)     4301 2024-02-12 04:07:38.000000 ANX-0.8.1/AndroidQQ/proto/IM_r_pb2.py
+-rw-r--r--   0 1a         (501) staff       (20)       67 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/proto/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1308 2023-10-29 17:25:21.000000 ANX-0.8.1/AndroidQQ/proto/wtlogin_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-06-03 09:50:01.222540 ANX-0.8.1/AndroidQQ/struct/
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-06-03 09:50:01.224562 ANX-0.8.1/AndroidQQ/struct/Avatarlnfo/
+-rw-r--r--   0 1a         (501) staff       (20)      444 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/Avatarlnfo/DestQQHeadInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)     1061 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/Avatarlnfo/QQHeadInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)      853 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/Avatarlnfo/QQHeadUrlReq.py
+-rw-r--r--   0 1a         (501) staff       (20)      673 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/Avatarlnfo/QQHeadUrlResp.py
+-rw-r--r--   0 1a         (501) staff       (20)     1028 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/Avatarlnfo/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)      894 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/MessageSvc.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-06-03 09:50:01.225103 ANX-0.8.1/AndroidQQ/struct/NS_MOBILE_COMM/
+-rw-r--r--   0 1a         (501) staff       (20)      373 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/NS_MOBILE_COMM/UgcRightInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)       28 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/NS_MOBILE_COMM/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-06-03 09:50:01.228448 ANX-0.8.1/AndroidQQ/struct/NS_MOBILE_FEEDS/
+-rw-r--r--   0 1a         (501) staff       (20)       70 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/NS_MOBILE_FEEDS/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     3064 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_comm.py
+-rw-r--r--   0 1a         (501) staff       (20)     1565 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_operation.py
+-rw-r--r--   0 1a         (501) staff       (20)      565 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_userinfo.py
+-rw-r--r--   0 1a         (501) staff       (20)      895 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_req.py
+-rw-r--r--   0 1a         (501) staff       (20)     1789 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_rsp.py
+-rw-r--r--   0 1a         (501) staff       (20)      451 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/NS_MOBILE_FEEDS/s_arkshare.py
+-rw-r--r--   0 1a         (501) staff       (20)      673 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/NS_MOBILE_FEEDS/s_outshare.py
+-rw-r--r--   0 1a         (501) staff       (20)      728 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/NS_MOBILE_FEEDS/s_picurl.py
+-rw-r--r--   0 1a         (501) staff       (20)      249 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/NS_MOBILE_FEEDS/s_user.py
+-rw-r--r--   0 1a         (501) staff       (20)     1163 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/NS_MOBILE_FEEDS/single_feed.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-06-03 09:50:01.230862 ANX-0.8.1/AndroidQQ/struct/NS_MOBILE_OPERATION/
+-rw-r--r--   0 1a         (501) staff       (20)      479 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/NS_MOBILE_OPERATION/Source.py
+-rw-r--r--   0 1a         (501) staff       (20)      187 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/NS_MOBILE_OPERATION/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)      656 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/NS_MOBILE_OPERATION/cmshow_active_result.py
+-rw-r--r--   0 1a         (501) staff       (20)     1161 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_delugc_req.py
+-rw-r--r--   0 1a         (501) staff       (20)     1300 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_req.py
+-rw-r--r--   0 1a         (501) staff       (20)      560 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_rsp.py
+-rw-r--r--   0 1a         (501) staff       (20)     3031 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_publishmood_req.py
+-rw-r--r--   0 1a         (501) staff       (20)      503 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_publishmood_rsp.py
+-rw-r--r--   0 1a         (501) staff       (20)      594 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/OidbSvc.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-06-03 09:50:01.233584 ANX-0.8.1/AndroidQQ/struct/QMF_PROTOCAL/
+-rw-r--r--   0 1a         (501) staff       (20)      504 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/QMF_PROTOCAL/QmfBusiControl.py
+-rw-r--r--   0 1a         (501) staff       (20)      630 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/QMF_PROTOCAL/QmfClientIpInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)      714 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/QMF_PROTOCAL/QmfDownstream.py
+-rw-r--r--   0 1a         (501) staff       (20)      526 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/QMF_PROTOCAL/QmfTokenInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)     1180 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/QMF_PROTOCAL/QmfUpstream.py
+-rw-r--r--   0 1a         (501) staff       (20)      489 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/QMF_PROTOCAL/RetryInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)       87 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/QMF_PROTOCAL/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-06-03 09:50:01.233922 ANX-0.8.1/AndroidQQ/struct/QQService/
+-rw-r--r--   0 1a         (501) staff       (20)     1112 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/QQService/SvcReqGetDevLoginInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)      878 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/QQService/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1043 2024-05-10 20:44:20.000000 ANX-0.8.1/AndroidQQ/struct/StatSvc.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-06-03 09:50:01.234618 ANX-0.8.1/AndroidQQ/struct/SummaryCard/
+-rw-r--r--   0 1a         (501) staff       (20)     2861 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/SummaryCard/ReqSummaryCard.py
+-rw-r--r--   0 1a         (501) staff       (20)      493 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/SummaryCard/UserLocaleInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)       61 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/SummaryCard/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)    15568 2024-03-05 18:40:23.000000 ANX-0.8.1/AndroidQQ/struct/Tlv.py
+-rw-r--r--   0 1a         (501) staff       (20)     4784 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/Tlv_res.py
+-rw-r--r--   0 1a         (501) staff       (20)      131 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-06-03 09:50:01.235448 ANX-0.8.1/AndroidQQ/struct/cooperation/
+-rw-r--r--   0 1a         (501) staff       (20)       23 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/cooperation/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-06-03 09:50:01.235879 ANX-0.8.1/AndroidQQ/struct/cooperation/qzone/
+-rw-r--r--   0 1a         (501) staff       (20)     4558 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/cooperation/qzone/WNSStream.py
+-rw-r--r--   0 1a         (501) staff       (20)       26 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/cooperation/qzone/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-06-03 09:50:01.236111 ANX-0.8.1/AndroidQQ/struct/feedcomponent/
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/feedcomponent/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1482 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/feedcomponent/model.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-06-03 09:50:01.236382 ANX-0.8.1/AndroidQQ/struct/friendlist/
+-rw-r--r--   0 1a         (501) staff       (20)     2842 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/friendlist/AddFriendReq.py
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/friendlist/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     7428 2024-03-07 10:14:48.000000 ANX-0.8.1/AndroidQQ/struct/head.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-06-03 09:50:01.236756 ANX-0.8.1/AndroidQQ/struct/push/
+-rw-r--r--   0 1a         (501) staff       (20)     3536 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/push/SvcReqRegister.py
+-rw-r--r--   0 1a         (501) staff       (20)     2084 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/push/SvcRespRegister.py
+-rw-r--r--   0 1a         (501) staff       (20)       31 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/struct/push/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)    27313 2024-03-05 18:40:23.000000 ANX-0.8.1/AndroidQQ/struct/wtlogin.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-06-03 09:50:01.237508 ANX-0.8.1/AndroidQQ/utils/
+-rw-r--r--   0 1a         (501) staff       (20)       20 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/utils/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)      523 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/utils/build_device.py
+-rw-r--r--   0 1a         (501) staff       (20)     1140 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/utils/ecdh.py
+-rw-r--r--   0 1a         (501) staff       (20)     1379 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/utils/sso_server.py
+-rw-r--r--   0 1a         (501) staff       (20)      735 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/utils/tool.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-06-03 09:50:01.237639 ANX-0.8.1/AndroidQQ/wlogin_sdk/
+-rw-r--r--   0 1a         (501) staff       (20)       25 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/wlogin_sdk/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-06-03 09:50:01.237792 ANX-0.8.1/AndroidQQ/wlogin_sdk/request/
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.8.1/AndroidQQ/wlogin_sdk/request/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)      125 2024-06-03 09:50:01.237987 ANX-0.8.1/PKG-INFO
+-rw-r--r--   0 1a         (501) staff       (20)       34 2023-08-04 12:41:32.000000 ANX-0.8.1/README.md
+-rw-r--r--   0 1a         (501) staff       (20)       38 2024-06-03 09:50:01.238206 ANX-0.8.1/setup.cfg
+-rw-r--r--   0 1a         (501) staff       (20)      601 2024-06-03 09:49:55.000000 ANX-0.8.1/setup.py
```

### Comparing `ANX-0.8.0/ANX.egg-info/SOURCES.txt` & `ANX-0.8.1/ANX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/Android.py` & `ANX-0.8.1/AndroidQQ/Android.py`

 * *Files 2% similar despite different names*

```diff
@@ -386,15 +386,15 @@
 
         return self.tcp_task(req_func, rsp_func)
 
     def no_tail_login(self):
         """无尾登录包"""
 
         def req_func(info):
-            return OidbSvc_0x88d_1(info, 849829771)
+            return OidbSvc_0x88d_1(info, 1042249288)
 
         return self.tcp_task(req_func, OidbSvc_0x88d_1_rep)
 
     def scan_Login(self, service_type: int, token: str):
         """扫码登录/辅助验证"""
 
         def req_func(info):
@@ -876,18 +876,32 @@
         self.get_lv_task()
 
     def lv_continuous_login(self):
 
         self.get_summary_card()
         self.get_lv_task()
 
-    def lv_Qzone(self, content='当遇到你时，大脑连上CSGO都会掉帧。'):
+    def lv_Qzone(self, content=None):
         """空间任务"""
+        content_list = [
+            ' 小荷才露尖尖角，早有蜻蜓立上头',
+            ' 有三秋桂子，十里荷花',
+            ' 藕花珠缀，犹似汗凝妆',
+            ' 一缕清香，一缕淡香',
+            ' 接天莲叶无穷碧，映日荷花别样红',
+            '能不能停下来，看看那个满眼泪花奔向你的我。',
+            '承诺常常很像蝴蝶，美丽的盘旋后就不见了。'
+        ]
+        random_content = random.choice(content_list)
+        if not content:
+            content = random_content
+
+        logger.info(f'空间任务内容：{content}')
         try:
-            rsp = self.Qzone_publishmood(content)['response']
+            rsp = self.Qzone_publishmood(content).get('response', {})
             tid = rsp.get('Busi', {}).get('tid', '')
             self.get_qq_level()
             self.Qzone_delUgc(tid)
             task = self.refresh_task('2').get('response', {}).get('task', {})
             if not task:
                 return Box(status=False, message='刷新任务异常')
             button_text = task.get('button_text')
@@ -909,15 +923,15 @@
         rsp = self.no_tail_login()
         status = rsp['status']
         if status != 0:
             return Box(status=False, message=rsp['message'])
 
         task_functions = {
             '连续登录QQ': self.lv_continuous_login,
-            '发布一条空间说说': self.lv_Qzone,
+            '发布一条空间说说': lambda: self.lv_Qzone(content=zone_content),
             '去日签卡打一次卡': self.lv_clock_in,
             '去QQ音乐听歌30分钟+0.5天': self.lv_music,
             '加一位好友': self.lv_Friend,
             '去超级QQ秀更新装扮并保存': self.lv_cm_show,
             '去微视APP看视频': self.lv_weishi,
         }
 
@@ -927,23 +941,18 @@
 
             if task_name == '去QQ音乐听歌30分钟+0.5天' and not lv_music:
                 logger.info(f'{self.info.uin}跳过音乐')
                 continue  # 如果任务是'去QQ音乐听歌30分钟+0.5天'并且设置为不可选执行，则跳过执行
             is_done = task_status.get(task_name, {}).get('is_done', None)
             if not is_done:
                 logger.info(f'{self.info.uin}执行{task_name}')
-
-                if task_name == '发布一条空间说说':
-                    function(content=zone_content)
-                else:
-                    function()
-
+                function()
                 execute_task = True
 
-        level = self.get_summary_card()['response']['5']
+        level = self.get_summary_card().get('response', {}).get('5', 0)
         if execute_task:
             task_status = self.get_lv_task_status(True)
 
         done_count = task_status.get('done_count', None)
         logger.info(f'{self.info.uin}已完成任务数量{done_count}')
         return Box(status=True, level=level, done_count=done_count, task_status=task_status)
```

### Comparing `ANX-0.8.0/AndroidQQ/Tcp.py` & `ANX-0.8.1/AndroidQQ/Tcp.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/http/ClientKey.py` & `ANX-0.8.1/AndroidQQ/http/ClientKey.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/http/accounts.py` & `ANX-0.8.1/AndroidQQ/http/accounts.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/http/cip.py` & `ANX-0.8.1/AndroidQQ/http/cip.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/http/friends.py` & `ANX-0.8.1/AndroidQQ/http/friends.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/http/game_credit.py` & `ANX-0.8.1/AndroidQQ/http/game_credit.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/http/level.py` & `ANX-0.8.1/AndroidQQ/http/level.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/http/music.py` & `ANX-0.8.1/AndroidQQ/http/music.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/http/qqsignin.py` & `ANX-0.8.1/AndroidQQ/http/qqsignin.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/http/weishi.py` & `ANX-0.8.1/AndroidQQ/http/weishi.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/im/oidb/OidbSvc_0xc96/OidbSvc_0xc96_pb2.py` & `ANX-0.8.1/AndroidQQ/im/oidb/OidbSvc_0xc96/OidbSvc_0xc96_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/im/oidb/cmd0x88d/oidb_0x88d_pb2.py` & `ANX-0.8.1/AndroidQQ/im/oidb/cmd0x88d/oidb_0x88d_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/im/oidb/cmd0x922/PushInfo_pb2.py` & `ANX-0.8.1/AndroidQQ/im/oidb/cmd0x922/PushInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/im/oidb/cmd0x922/cmd0x922_pb2.py` & `ANX-0.8.1/AndroidQQ/im/oidb/cmd0x922/cmd0x922_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/im/oidb/cmd0xeb8/cmd0xeb8_pb2.py` & `ANX-0.8.1/AndroidQQ/im/oidb/cmd0xeb8/cmd0xeb8_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/im/oidb/oidb_0xc05/oidb_0xc05_pb2.py` & `ANX-0.8.1/AndroidQQ/im/oidb/oidb_0xc05/oidb_0xc05_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/im/oidb/oidb_sso/oidb_sso_pb2.py` & `ANX-0.8.1/AndroidQQ/im/oidb/oidb_sso/oidb_sso_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/im/oidb/qqconnect/qqconnect_pb2.py` & `ANX-0.8.1/AndroidQQ/im/oidb/qqconnect/qqconnect_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/im/oidb/scanlogin/scanlogin_pb2.py` & `ANX-0.8.1/AndroidQQ/im/oidb/scanlogin/scanlogin_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/pack/MQUpdateSvc_com_qq_ti_web_scanlogin.py` & `ANX-0.8.1/AndroidQQ/pack/MQUpdateSvc_com_qq_ti_web_scanlogin.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/pack/MQUpdateSvc_com_qq_vip_zb_web_OidbSvc_0xdfa_0.py` & `ANX-0.8.1/AndroidQQ/pack/MQUpdateSvc_com_qq_vip_zb_web_OidbSvc_0xdfa_0.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/pack/OidbSvc_0x88d_1.py` & `ANX-0.8.1/AndroidQQ/pack/OidbSvc_0x88d_1.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/pack/OidbSvc_0xc05.py` & `ANX-0.8.1/AndroidQQ/pack/OidbSvc_0xc05.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/pack/OidbSvc_0xc96.py` & `ANX-0.8.1/AndroidQQ/pack/OidbSvc_0xc96.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/pack/OidbSvc_0xeb8.py` & `ANX-0.8.1/AndroidQQ/pack/OidbSvc_0xeb8.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/pack/SQQzoneSvc/delUgc.py` & `ANX-0.8.1/AndroidQQ/pack/SQQzoneSvc/delUgc.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/pack/SQQzoneSvc/like.py` & `ANX-0.8.1/AndroidQQ/pack/SQQzoneSvc/like.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/pack/SQQzoneSvc/publishmood.py` & `ANX-0.8.1/AndroidQQ/pack/SQQzoneSvc/publishmood.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
     Upstream = createQmfUpstream(info, 1, Buffer, 'QzoneNewService.publishmood')
     Buffer = PackHead_QMF(info, 'SQQzoneSvc.publishmood', Upstream)
 
     return Buffer
 
 
-def SQQzoneSvc_publishmood_rsp(buffer: bytes):
+def SQQzoneSvc_publishmood_rsp(buffer: bytes) -> dict:
     rsp_Buffer, msg, ret = UnQmfDownstream(buffer, 'publishmood', 'NS_MOBILE_OPERATION.operation_publishmood_rsp')
 
     if rsp_Buffer == b'':
         return {'Busi': {}, 'msg': msg, 'ret': ret}
     like_rsp = JceReader(rsp_Buffer).read_object(operation_publishmood_rsp)
     return {'Busi': like_rsp.to_dict(), 'msg': msg, 'ret': ret}
```

### Comparing `ANX-0.8.0/AndroidQQ/pack/SQQzoneSvc/shuoshuo.py` & `ANX-0.8.1/AndroidQQ/pack/SQQzoneSvc/shuoshuo.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/pack/StatSvc_register.py` & `ANX-0.8.1/AndroidQQ/pack/StatSvc_register.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/pack/SummaryCard/ReqSummaryCard.py` & `ANX-0.8.1/AndroidQQ/pack/SummaryCard/ReqSummaryCard.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/pack/friendlist.py` & `ANX-0.8.1/AndroidQQ/pack/friendlist.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/pack/test.py` & `ANX-0.8.1/AndroidQQ/pack/test.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/pack/trpc_metaverse_mob_proxy_svr_MobProxy_SsoHandle.py` & `ANX-0.8.1/AndroidQQ/pack/trpc_metaverse_mob_proxy_svr_MobProxy_SsoHandle.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/proto/IM_r_pb2.py` & `ANX-0.8.1/AndroidQQ/proto/IM_r_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/proto/wtlogin_pb2.py` & `ANX-0.8.1/AndroidQQ/proto/wtlogin_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/struct/Avatarlnfo/QQHeadInfo.py` & `ANX-0.8.1/AndroidQQ/struct/Avatarlnfo/QQHeadInfo.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/struct/Avatarlnfo/QQHeadUrlReq.py` & `ANX-0.8.1/AndroidQQ/struct/Avatarlnfo/QQHeadUrlReq.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/struct/Avatarlnfo/QQHeadUrlResp.py` & `ANX-0.8.1/AndroidQQ/struct/Avatarlnfo/QQHeadUrlResp.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/struct/Avatarlnfo/__init__.py` & `ANX-0.8.1/AndroidQQ/struct/Avatarlnfo/__init__.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/struct/MessageSvc.py` & `ANX-0.8.1/AndroidQQ/struct/MessageSvc.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_comm.py` & `ANX-0.8.1/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_comm.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_operation.py` & `ANX-0.8.1/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_operation.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_userinfo.py` & `ANX-0.8.1/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_userinfo.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_req.py` & `ANX-0.8.1/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_req.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_rsp.py` & `ANX-0.8.1/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_rsp.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_FEEDS/s_outshare.py` & `ANX-0.8.1/AndroidQQ/struct/NS_MOBILE_FEEDS/s_outshare.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_FEEDS/s_picurl.py` & `ANX-0.8.1/AndroidQQ/struct/NS_MOBILE_FEEDS/s_picurl.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_FEEDS/single_feed.py` & `ANX-0.8.1/AndroidQQ/struct/NS_MOBILE_FEEDS/single_feed.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_OPERATION/cmshow_active_result.py` & `ANX-0.8.1/AndroidQQ/struct/NS_MOBILE_OPERATION/cmshow_active_result.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_delugc_req.py` & `ANX-0.8.1/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_delugc_req.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_req.py` & `ANX-0.8.1/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_req.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_rsp.py` & `ANX-0.8.1/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_rsp.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_publishmood_req.py` & `ANX-0.8.1/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_publishmood_req.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/struct/OidbSvc.py` & `ANX-0.8.1/AndroidQQ/struct/OidbSvc.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/struct/QMF_PROTOCAL/QmfClientIpInfo.py` & `ANX-0.8.1/AndroidQQ/struct/QMF_PROTOCAL/QmfClientIpInfo.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/struct/QMF_PROTOCAL/QmfDownstream.py` & `ANX-0.8.1/AndroidQQ/struct/QMF_PROTOCAL/QmfDownstream.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/struct/QMF_PROTOCAL/QmfTokenInfo.py` & `ANX-0.8.1/AndroidQQ/struct/QMF_PROTOCAL/QmfTokenInfo.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/struct/QMF_PROTOCAL/QmfUpstream.py` & `ANX-0.8.1/AndroidQQ/struct/QMF_PROTOCAL/QmfUpstream.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/struct/QQService/SvcReqGetDevLoginInfo.py` & `ANX-0.8.1/AndroidQQ/struct/QQService/SvcReqGetDevLoginInfo.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/struct/QQService/__init__.py` & `ANX-0.8.1/AndroidQQ/struct/QQService/__init__.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/struct/StatSvc.py` & `ANX-0.8.1/AndroidQQ/struct/StatSvc.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/struct/SummaryCard/ReqSummaryCard.py` & `ANX-0.8.1/AndroidQQ/struct/SummaryCard/ReqSummaryCard.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/struct/Tlv.py` & `ANX-0.8.1/AndroidQQ/struct/Tlv.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/struct/Tlv_res.py` & `ANX-0.8.1/AndroidQQ/struct/Tlv_res.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/struct/cooperation/qzone/WNSStream.py` & `ANX-0.8.1/AndroidQQ/struct/cooperation/qzone/WNSStream.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/struct/feedcomponent/model.py` & `ANX-0.8.1/AndroidQQ/struct/feedcomponent/model.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/struct/friendlist/AddFriendReq.py` & `ANX-0.8.1/AndroidQQ/struct/friendlist/AddFriendReq.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/struct/head.py` & `ANX-0.8.1/AndroidQQ/struct/head.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/struct/push/SvcReqRegister.py` & `ANX-0.8.1/AndroidQQ/struct/push/SvcReqRegister.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/struct/push/SvcRespRegister.py` & `ANX-0.8.1/AndroidQQ/struct/push/SvcRespRegister.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/struct/wtlogin.py` & `ANX-0.8.1/AndroidQQ/struct/wtlogin.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/utils/build_device.py` & `ANX-0.8.1/AndroidQQ/utils/build_device.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/utils/ecdh.py` & `ANX-0.8.1/AndroidQQ/utils/ecdh.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/utils/sso_server.py` & `ANX-0.8.1/AndroidQQ/utils/sso_server.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/AndroidQQ/utils/tool.py` & `ANX-0.8.1/AndroidQQ/utils/tool.py`

 * *Files identical despite different names*

### Comparing `ANX-0.8.0/setup.py` & `ANX-0.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 setuptools.setup(
     name='ANX',
-    version='0.8.0',
+    version='0.8.1',
     url='https://github.com/grayrail000/AndroidQQ',
     packages=setuptools.find_packages(exclude=["tests", "tests.*"]),
     license='',
     author='1x',
     author_email='',
     description='',
     install_requires=[
```

