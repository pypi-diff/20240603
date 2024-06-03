# Comparing `tmp/edri-2024.4.1.tar.gz` & `tmp/edri-2024.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edri-2024.4.1.tar", last modified: Tue Apr  2 09:52:49 2024, max compression
+gzip compressed data, was "edri-2024.6.1.tar", last modified: Mon Jun  3 11:48:59 2024, max compression
```

## Comparing `edri-2024.4.1.tar` & `edri-2024.6.1.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.320612 edri-2024.4.1/
--rw-r--r--   0 root         (0) root         (0)     1649 2024-04-02 09:52:49.320612 edri-2024.4.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    11895 2024-03-07 10:37:30.000000 edri-2024.4.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.096617 edri-2024.4.1/edri/
--rw-rw-rw-   0 root         (0) root         (0)     2187 2024-03-13 10:35:39.000000 edri-2024.4.1/edri/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.108616 edri-2024.4.1/edri/abstract/
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/abstract/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4429 2024-03-13 10:35:39.000000 edri-2024.4.1/edri/abstract/api_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.136616 edri-2024.4.1/edri/abstract/manager/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-02 09:52:35.000000 edri-2024.4.1/edri/abstract/manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    32374 2024-03-13 10:35:39.000000 edri-2024.4.1/edri/abstract/manager/manager_base.py
--rw-rw-rw-   0 root         (0) root         (0)     7635 2024-03-13 10:35:39.000000 edri-2024.4.1/edri/abstract/manager/manager_priority_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.140616 edri-2024.4.1/edri/abstract/worker/
--rw-rw-rw-   0 root         (0) root         (0)      164 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/abstract/worker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9319 2024-04-02 09:52:35.000000 edri-2024.4.1/edri/abstract/worker/worker.py
--rw-rw-rw-   0 root         (0) root         (0)     1903 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/abstract/worker/worker_process.py
--rw-rw-rw-   0 root         (0) root         (0)     2122 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/abstract/worker/worker_thread.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.144616 edri-2024.4.1/edri/config/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-02 09:52:35.000000 edri-2024.4.1/edri/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      354 2024-03-13 10:35:39.000000 edri-2024.4.1/edri/config/constant.py
--rw-rw-rw-   0 root         (0) root         (0)     1020 2024-03-13 12:02:40.000000 edri-2024.4.1/edri/config/setting.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.152615 edri-2024.4.1/edri/dataclass/
--rw-rw-rw-   0 root         (0) root         (0)       34 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/dataclass/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.156615 edri-2024.4.1/edri/dataclass/client/
--rw-rw-rw-   0 root         (0) root         (0)       49 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/dataclass/client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      383 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/dataclass/client/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.164615 edri-2024.4.1/edri/dataclass/event/
--rw-rw-rw-   0 root         (0) root         (0)     6593 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/dataclass/event/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1921 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/dataclass/event/event.py
--rw-rw-rw-   0 root         (0) root         (0)     1212 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/dataclass/event/response.py
--rw-rw-rw-   0 root         (0) root         (0)      180 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/dataclass/queue_item.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.168615 edri-2024.4.1/edri/dataclass/switch/
--rw-rw-rw-   0 root         (0) root         (0)       35 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/dataclass/switch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      302 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/dataclass/switch/connection.py
--rw-rw-rw-   0 root         (0) root         (0)      401 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/dataclass/worker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.168615 edri-2024.4.1/edri/events/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-02 09:52:35.000000 edri-2024.4.1/edri/events/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.168615 edri-2024.4.1/edri/events/api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-02 09:52:35.000000 edri-2024.4.1/edri/events/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.176615 edri-2024.4.1/edri/events/api/client/
--rw-rw-rw-   0 root         (0) root         (0)      105 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/events/api/client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      352 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/api/client/register.py
--rw-rw-rw-   0 root         (0) root         (0)      124 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/api/client/unregister.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.184615 edri-2024.4.1/edri/events/api/group/
--rw-rw-rw-   0 root         (0) root         (0)       87 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/events/api/group/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       85 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/api/group/client.py
--rw-rw-rw-   0 root         (0) root         (0)       85 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/api/group/manage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.192615 edri-2024.4.1/edri/events/api/manage/
--rw-rw-rw-   0 root         (0) root         (0)      226 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/events/api/manage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      128 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/api/manage/list_registered.py
--rw-rw-rw-   0 root         (0) root         (0)      423 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/api/manage/register.py
--rw-rw-rw-   0 root         (0) root         (0)      129 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/api/manage/unregister.py
--rw-rw-rw-   0 root         (0) root         (0)      127 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/api/manage/unregister_all.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.192615 edri-2024.4.1/edri/events/edri/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-02 09:52:35.000000 edri-2024.4.1/edri/events/edri/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.204614 edri-2024.4.1/edri/events/edri/group/
--rw-rw-rw-   0 root         (0) root         (0)      228 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/events/edri/group/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       86 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/group/manager.py
--rw-rw-rw-   0 root         (0) root         (0)       85 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/group/router.py
--rw-rw-rw-   0 root         (0) root         (0)       88 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/group/scheduler.py
--rw-rw-rw-   0 root         (0) root         (0)       84 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/group/store.py
--rw-rw-rw-   0 root         (0) root         (0)       85 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/group/switch.py
--rw-rw-rw-   0 root         (0) root         (0)       83 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/group/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.212614 edri-2024.4.1/edri/events/edri/manager/
--rw-rw-rw-   0 root         (0) root         (0)      231 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/events/edri/manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      176 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/manager/stream_close.py
--rw-rw-rw-   0 root         (0) root         (0)      146 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/manager/stream_create.py
--rw-rw-rw-   0 root         (0) root         (0)      147 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/manager/stream_message.py
--rw-rw-rw-   0 root         (0) root         (0)      127 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/manager/worker_quit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.228614 edri-2024.4.1/edri/events/edri/router/
--rw-rw-rw-   0 root         (0) root         (0)      490 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/events/edri/router/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      214 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/router/demands.py
--rw-rw-rw-   0 root         (0) root         (0)      234 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/router/health_check.py
--rw-rw-rw-   0 root         (0) root         (0)      125 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/router/last_events.py
--rw-rw-rw-   0 root         (0) root         (0)      165 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/router/send_from.py
--rw-rw-rw-   0 root         (0) root         (0)      459 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/events/edri/router/subscribe.py
--rw-rw-rw-   0 root         (0) root         (0)      197 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/router/subscribe_connector.py
--rw-rw-rw-   0 root         (0) root         (0)      229 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/router/subscribed_all.py
--rw-rw-rw-   0 root         (0) root         (0)      192 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/router/subscribed_new.py
--rw-rw-rw-   0 root         (0) root         (0)      263 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/router/unsubscribe.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.240614 edri-2024.4.1/edri/events/edri/scheduler/
--rw-rw-rw-   0 root         (0) root         (0)      115 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/events/edri/scheduler/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/scheduler/cancel.py
--rw-rw-rw-   0 root         (0) root         (0)      369 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/events/edri/scheduler/set.py
--rw-rw-rw-   0 root         (0) root         (0)      326 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/scheduler/update.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.240614 edri-2024.4.1/edri/events/edri/store/
--rw-rw-rw-   0 root         (0) root         (0)      105 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/events/edri/store/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      256 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/store/delete.py
--rw-rw-rw-   0 root         (0) root         (0)      297 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/store/get.py
--rw-rw-rw-   0 root         (0) root         (0)      160 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/store/set.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.248613 edri-2024.4.1/edri/events/edri/switch/
--rw-rw-rw-   0 root         (0) root         (0)      109 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/events/edri/switch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      224 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/switch/demands.py
--rw-rw-rw-   0 root         (0) root         (0)      201 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/switch/last_messages.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.252613 edri-2024.4.1/edri/events/edri/test/
--rw-rw-rw-   0 root         (0) root         (0)      109 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/events/edri/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      115 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/test/ping.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/events/edri/test/ping2.py
--rw-rw-rw-   0 root         (0) root         (0)      249 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/events/edri/test/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.256613 edri-2024.4.1/edri/rest/
--rw-rw-rw-   0 root         (0) root         (0)       45 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/rest/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    25647 2024-03-13 10:35:39.000000 edri-2024.4.1/edri/rest/server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.264613 edri-2024.4.1/edri/router/
--rw-rw-rw-   0 root         (0) root         (0)      142 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/router/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5965 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/router/cache.py
--rw-rw-rw-   0 root         (0) root         (0)     6557 2024-03-11 08:54:49.000000 edri-2024.4.1/edri/router/health_checker.py
--rw-rw-rw-   0 root         (0) root         (0)    11733 2024-03-08 11:06:35.000000 edri-2024.4.1/edri/router/router.py
--rw-rw-rw-   0 root         (0) root         (0)      612 2024-03-08 11:06:35.000000 edri-2024.4.1/edri/store.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.288612 edri-2024.4.1/edri/switch/
--rw-rw-rw-   0 root         (0) root         (0)      118 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/switch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1688 2024-03-11 08:54:49.000000 edri-2024.4.1/edri/switch/forwarder.py
--rw-rw-rw-   0 root         (0) root         (0)     3269 2024-03-11 08:54:49.000000 edri-2024.4.1/edri/switch/receiver.py
--rw-rw-rw-   0 root         (0) root         (0)     1003 2024-03-11 08:54:49.000000 edri-2024.4.1/edri/switch/sender.py
--rw-rw-rw-   0 root         (0) root         (0)     2714 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/switch/switch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.304612 edri-2024.4.1/edri/utility/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-02 09:52:35.000000 edri-2024.4.1/edri/utility/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13893 2024-03-11 08:54:49.000000 edri-2024.4.1/edri/utility/api_broker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.312612 edri-2024.4.1/edri/utility/connector/
--rw-rw-rw-   0 root         (0) root         (0)       95 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/utility/connector/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10119 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/utility/connector/connector.py
--rw-rw-rw-   0 root         (0) root         (0)     3298 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/utility/connector/socket.py
--rw-rw-rw-   0 root         (0) root         (0)     1744 2024-02-21 08:23:35.000000 edri-2024.4.1/edri/utility/eta.py
--rw-rw-rw-   0 root         (0) root         (0)     2182 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/utility/function.py
--rw-rw-rw-   0 root         (0) root         (0)     8454 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/utility/scheduler.py
--rw-rw-rw-   0 root         (0) root         (0)     2247 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/utility/storage.py
--rw-rw-rw-   0 root         (0) root         (0)     3091 2024-03-11 08:54:49.000000 edri-2024.4.1/edri/utility/store.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.316612 edri-2024.4.1/edri/websocket/
--rw-rw-rw-   0 root         (0) root         (0)       40 2024-03-07 10:37:30.000000 edri-2024.4.1/edri/websocket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7001 2024-03-11 08:54:49.000000 edri-2024.4.1/edri/websocket/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.320612 edri-2024.4.1/edri.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1649 2024-04-02 09:52:49.000000 edri-2024.4.1/edri.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3303 2024-04-02 09:52:49.000000 edri-2024.4.1/edri.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 09:52:49.000000 edri-2024.4.1/edri.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2024-04-02 09:52:49.000000 edri-2024.4.1/edri.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-04-02 09:52:49.000000 edri-2024.4.1/edri.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-02 09:52:49.320612 edri-2024.4.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1841 2024-04-02 09:52:26.000000 edri-2024.4.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:52:49.320612 edri-2024.4.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1396 2024-03-07 10:37:30.000000 edri-2024.4.1/tests/test_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:48:59.549369 edri-2024.6.1/
+-rw-r--r--   0 root         (0) root         (0)     1649 2024-06-03 11:48:59.545369 edri-2024.6.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    11895 2024-03-07 10:37:30.000000 edri-2024.6.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:48:59.325373 edri-2024.6.1/edri/
+-rw-rw-rw-   0 root         (0) root         (0)     2187 2024-03-13 10:35:39.000000 edri-2024.6.1/edri/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:48:59.337373 edri-2024.6.1/edri/abstract/
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-03-07 10:37:30.000000 edri-2024.6.1/edri/abstract/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4429 2024-03-13 10:35:39.000000 edri-2024.6.1/edri/abstract/api_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:48:59.349372 edri-2024.6.1/edri/abstract/manager/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-03 11:48:45.000000 edri-2024.6.1/edri/abstract/manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    32374 2024-03-13 10:35:39.000000 edri-2024.6.1/edri/abstract/manager/manager_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     7635 2024-03-13 10:35:39.000000 edri-2024.6.1/edri/abstract/manager/manager_priority_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:48:59.357372 edri-2024.6.1/edri/abstract/worker/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2024-03-07 10:37:30.000000 edri-2024.6.1/edri/abstract/worker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9319 2024-04-02 09:52:35.000000 edri-2024.6.1/edri/abstract/worker/worker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1903 2024-03-07 10:37:30.000000 edri-2024.6.1/edri/abstract/worker/worker_process.py
+-rw-rw-rw-   0 root         (0) root         (0)     2122 2024-03-07 10:37:30.000000 edri-2024.6.1/edri/abstract/worker/worker_thread.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:48:59.361372 edri-2024.6.1/edri/config/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-03 11:48:45.000000 edri-2024.6.1/edri/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      354 2024-03-13 10:35:39.000000 edri-2024.6.1/edri/config/constant.py
+-rw-rw-rw-   0 root         (0) root         (0)     1020 2024-03-13 12:02:40.000000 edri-2024.6.1/edri/config/setting.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:48:59.381372 edri-2024.6.1/edri/dataclass/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-02-21 08:23:35.000000 edri-2024.6.1/edri/dataclass/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:48:59.385372 edri-2024.6.1/edri/dataclass/client/
+-rw-rw-rw-   0 root         (0) root         (0)       49 2024-03-07 10:37:30.000000 edri-2024.6.1/edri/dataclass/client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      383 2024-03-07 10:37:30.000000 edri-2024.6.1/edri/dataclass/client/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:48:59.393372 edri-2024.6.1/edri/dataclass/event/
+-rw-rw-rw-   0 root         (0) root         (0)     6593 2024-03-07 10:37:30.000000 edri-2024.6.1/edri/dataclass/event/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1921 2024-03-07 10:37:30.000000 edri-2024.6.1/edri/dataclass/event/event.py
+-rw-rw-rw-   0 root         (0) root         (0)     1212 2024-03-07 10:37:30.000000 edri-2024.6.1/edri/dataclass/event/response.py
+-rw-rw-rw-   0 root         (0) root         (0)      180 2024-02-21 08:23:35.000000 edri-2024.6.1/edri/dataclass/queue_item.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:48:59.397372 edri-2024.6.1/edri/dataclass/switch/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-02-21 08:23:35.000000 edri-2024.6.1/edri/dataclass/switch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      302 2024-03-07 10:37:30.000000 edri-2024.6.1/edri/dataclass/switch/connection.py
+-rw-rw-rw-   0 root         (0) root         (0)      401 2024-02-21 08:23:35.000000 edri-2024.6.1/edri/dataclass/worker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:48:59.397372 edri-2024.6.1/edri/events/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-03 11:48:45.000000 edri-2024.6.1/edri/events/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:48:59.401372 edri-2024.6.1/edri/events/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-03 11:48:45.000000 edri-2024.6.1/edri/events/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:48:59.405372 edri-2024.6.1/edri/events/api/client/
+-rw-rw-rw-   0 root         (0) root         (0)      105 2024-03-07 10:37:30.000000 edri-2024.6.1/edri/events/api/client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      352 2024-02-21 08:23:35.000000 edri-2024.6.1/edri/events/api/client/register.py
+-rw-rw-rw-   0 root         (0) root         (0)      124 2024-02-21 08:23:35.000000 edri-2024.6.1/edri/events/api/client/unregister.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:48:59.409371 edri-2024.6.1/edri/events/api/group/
+-rw-rw-rw-   0 root         (0) root         (0)       87 2024-03-07 10:37:30.000000 edri-2024.6.1/edri/events/api/group/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       85 2024-02-21 08:23:35.000000 edri-2024.6.1/edri/events/api/group/client.py
+-rw-rw-rw-   0 root         (0) root         (0)       85 2024-02-21 08:23:35.000000 edri-2024.6.1/edri/events/api/group/manage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:48:59.417371 edri-2024.6.1/edri/events/api/manage/
+-rw-rw-rw-   0 root         (0) root         (0)      226 2024-03-07 10:37:30.000000 edri-2024.6.1/edri/events/api/manage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      128 2024-02-21 08:23:35.000000 edri-2024.6.1/edri/events/api/manage/list_registered.py
+-rw-rw-rw-   0 root         (0) root         (0)      423 2024-02-21 08:23:35.000000 edri-2024.6.1/edri/events/api/manage/register.py
+-rw-rw-rw-   0 root         (0) root         (0)      129 2024-02-21 08:23:35.000000 edri-2024.6.1/edri/events/api/manage/unregister.py
+-rw-rw-rw-   0 root         (0) root         (0)      127 2024-02-21 08:23:35.000000 edri-2024.6.1/edri/events/api/manage/unregister_all.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:48:59.417371 edri-2024.6.1/edri/events/edri/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-03 11:48:45.000000 edri-2024.6.1/edri/events/edri/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:48:59.429371 edri-2024.6.1/edri/events/edri/group/
+-rw-rw-rw-   0 root         (0) root         (0)      228 2024-03-07 10:37:30.000000 edri-2024.6.1/edri/events/edri/group/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       86 2024-02-21 08:23:35.000000 edri-2024.6.1/edri/events/edri/group/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)       85 2024-02-21 08:23:35.000000 edri-2024.6.1/edri/events/edri/group/router.py
+-rw-rw-rw-   0 root         (0) root         (0)       88 2024-02-21 08:23:35.000000 edri-2024.6.1/edri/events/edri/group/scheduler.py
+-rw-rw-rw-   0 root         (0) root         (0)       84 2024-02-21 08:23:35.000000 edri-2024.6.1/edri/events/edri/group/store.py
+-rw-rw-rw-   0 root         (0) root         (0)       85 2024-02-21 08:23:35.000000 edri-2024.6.1/edri/events/edri/group/switch.py
+-rw-rw-rw-   0 root         (0) root         (0)       83 2024-02-21 08:23:35.000000 edri-2024.6.1/edri/events/edri/group/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:48:59.437371 edri-2024.6.1/edri/events/edri/manager/
+-rw-rw-rw-   0 root         (0) root         (0)      231 2024-03-07 10:37:30.000000 edri-2024.6.1/edri/events/edri/manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      176 2024-02-21 08:23:35.000000 edri-2024.6.1/edri/events/edri/manager/stream_close.py
+-rw-rw-rw-   0 root         (0) root         (0)      146 2024-02-21 08:23:35.000000 edri-2024.6.1/edri/events/edri/manager/stream_create.py
+-rw-rw-rw-   0 root         (0) root         (0)      147 2024-02-21 08:23:35.000000 edri-2024.6.1/edri/events/edri/manager/stream_message.py
+-rw-rw-rw-   0 root         (0) root         (0)      127 2024-02-21 08:23:35.000000 edri-2024.6.1/edri/events/edri/manager/worker_quit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:48:59.453371 edri-2024.6.1/edri/events/edri/router/
+-rw-rw-rw-   0 root         (0) root         (0)      490 2024-03-07 10:37:30.000000 edri-2024.6.1/edri/events/edri/router/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      214 2024-02-21 08:23:35.000000 edri-2024.6.1/edri/events/edri/router/demands.py
+-rw-rw-rw-   0 root         (0) root         (0)      234 2024-02-21 08:23:35.000000 edri-2024.6.1/edri/events/edri/router/health_check.py
+-rw-rw-rw-   0 root         (0) root         (0)      125 2024-02-21 08:23:35.000000 edri-2024.6.1/edri/events/edri/router/last_events.py
+-rw-rw-rw-   0 root         (0) root         (0)      165 2024-02-21 08:23:35.000000 edri-2024.6.1/edri/events/edri/router/send_from.py
+-rw-rw-rw-   0 root         (0) root         (0)      459 2024-03-07 10:37:30.000000 edri-2024.6.1/edri/events/edri/router/subscribe.py
+-rw-rw-rw-   0 root         (0) root         (0)      197 2024-02-21 08:23:35.000000 edri-2024.6.1/edri/events/edri/router/subscribe_connector.py
+-rw-rw-rw-   0 root         (0) root         (0)      229 2024-02-21 08:23:35.000000 edri-2024.6.1/edri/events/edri/router/subscribed_all.py
+-rw-rw-rw-   0 root         (0) root         (0)      192 2024-02-21 08:23:35.000000 edri-2024.6.1/edri/events/edri/router/subscribed_new.py
+-rw-rw-rw-   0 root         (0) root         (0)      263 2024-02-21 08:23:35.000000 edri-2024.6.1/edri/events/edri/router/unsubscribe.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:48:59.457370 edri-2024.6.1/edri/events/edri/scheduler/
+-rw-rw-rw-   0 root         (0) root         (0)      115 2024-03-07 10:37:30.000000 edri-2024.6.1/edri/events/edri/scheduler/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2024-02-21 08:23:35.000000 edri-2024.6.1/edri/events/edri/scheduler/cancel.py
+-rw-rw-rw-   0 root         (0) root         (0)      369 2024-03-07 10:37:30.000000 edri-2024.6.1/edri/events/edri/scheduler/set.py
+-rw-rw-rw-   0 root         (0) root         (0)      326 2024-02-21 08:23:35.000000 edri-2024.6.1/edri/events/edri/scheduler/update.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:48:59.461370 edri-2024.6.1/edri/events/edri/store/
+-rw-rw-rw-   0 root         (0) root         (0)      105 2024-03-07 10:37:30.000000 edri-2024.6.1/edri/events/edri/store/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      256 2024-02-21 08:23:35.000000 edri-2024.6.1/edri/events/edri/store/delete.py
+-rw-rw-rw-   0 root         (0) root         (0)      297 2024-02-21 08:23:35.000000 edri-2024.6.1/edri/events/edri/store/get.py
+-rw-rw-rw-   0 root         (0) root         (0)      160 2024-02-21 08:23:35.000000 edri-2024.6.1/edri/events/edri/store/set.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:48:59.465370 edri-2024.6.1/edri/events/edri/switch/
+-rw-rw-rw-   0 root         (0) root         (0)      109 2024-03-07 10:37:30.000000 edri-2024.6.1/edri/events/edri/switch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      224 2024-02-21 08:23:35.000000 edri-2024.6.1/edri/events/edri/switch/demands.py
+-rw-rw-rw-   0 root         (0) root         (0)      201 2024-02-21 08:23:35.000000 edri-2024.6.1/edri/events/edri/switch/last_messages.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:48:59.473370 edri-2024.6.1/edri/events/edri/test/
+-rw-rw-rw-   0 root         (0) root         (0)      109 2024-03-07 10:37:30.000000 edri-2024.6.1/edri/events/edri/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      115 2024-02-21 08:23:35.000000 edri-2024.6.1/edri/events/edri/test/ping.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2024-02-21 08:23:35.000000 edri-2024.6.1/edri/events/edri/test/ping2.py
+-rw-rw-rw-   0 root         (0) root         (0)      249 2024-03-07 10:37:30.000000 edri-2024.6.1/edri/events/edri/test/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:48:59.477370 edri-2024.6.1/edri/rest/
+-rw-rw-rw-   0 root         (0) root         (0)       45 2024-03-07 10:37:30.000000 edri-2024.6.1/edri/rest/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    25447 2024-06-03 11:48:44.000000 edri-2024.6.1/edri/rest/server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:48:59.481370 edri-2024.6.1/edri/router/
+-rw-rw-rw-   0 root         (0) root         (0)      142 2024-03-07 10:37:30.000000 edri-2024.6.1/edri/router/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5965 2024-03-07 10:37:30.000000 edri-2024.6.1/edri/router/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     6557 2024-03-11 08:54:49.000000 edri-2024.6.1/edri/router/health_checker.py
+-rw-rw-rw-   0 root         (0) root         (0)    11733 2024-03-08 11:06:35.000000 edri-2024.6.1/edri/router/router.py
+-rw-rw-rw-   0 root         (0) root         (0)      612 2024-03-08 11:06:35.000000 edri-2024.6.1/edri/store.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:48:59.505370 edri-2024.6.1/edri/switch/
+-rw-rw-rw-   0 root         (0) root         (0)      118 2024-02-21 08:23:35.000000 edri-2024.6.1/edri/switch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1688 2024-03-11 08:54:49.000000 edri-2024.6.1/edri/switch/forwarder.py
+-rw-rw-rw-   0 root         (0) root         (0)     3269 2024-03-11 08:54:49.000000 edri-2024.6.1/edri/switch/receiver.py
+-rw-rw-rw-   0 root         (0) root         (0)     1003 2024-03-11 08:54:49.000000 edri-2024.6.1/edri/switch/sender.py
+-rw-rw-rw-   0 root         (0) root         (0)     2714 2024-03-07 10:37:30.000000 edri-2024.6.1/edri/switch/switch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:48:59.525369 edri-2024.6.1/edri/utility/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-03 11:48:45.000000 edri-2024.6.1/edri/utility/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13893 2024-03-11 08:54:49.000000 edri-2024.6.1/edri/utility/api_broker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:48:59.537369 edri-2024.6.1/edri/utility/connector/
+-rw-rw-rw-   0 root         (0) root         (0)       95 2024-03-07 10:37:30.000000 edri-2024.6.1/edri/utility/connector/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10119 2024-03-07 10:37:30.000000 edri-2024.6.1/edri/utility/connector/connector.py
+-rw-rw-rw-   0 root         (0) root         (0)     3298 2024-03-07 10:37:30.000000 edri-2024.6.1/edri/utility/connector/socket.py
+-rw-rw-rw-   0 root         (0) root         (0)     1744 2024-02-21 08:23:35.000000 edri-2024.6.1/edri/utility/eta.py
+-rw-rw-rw-   0 root         (0) root         (0)     2182 2024-03-07 10:37:30.000000 edri-2024.6.1/edri/utility/function.py
+-rw-rw-rw-   0 root         (0) root         (0)     8454 2024-03-07 10:37:30.000000 edri-2024.6.1/edri/utility/scheduler.py
+-rw-rw-rw-   0 root         (0) root         (0)     2247 2024-03-07 10:37:30.000000 edri-2024.6.1/edri/utility/storage.py
+-rw-rw-rw-   0 root         (0) root         (0)     3091 2024-03-11 08:54:49.000000 edri-2024.6.1/edri/utility/store.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:48:59.541369 edri-2024.6.1/edri/websocket/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2024-03-07 10:37:30.000000 edri-2024.6.1/edri/websocket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7001 2024-03-11 08:54:49.000000 edri-2024.6.1/edri/websocket/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:48:59.545369 edri-2024.6.1/edri.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1649 2024-06-03 11:48:59.000000 edri-2024.6.1/edri.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3303 2024-06-03 11:48:59.000000 edri-2024.6.1/edri.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-03 11:48:59.000000 edri-2024.6.1/edri.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2024-06-03 11:48:59.000000 edri-2024.6.1/edri.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-06-03 11:48:59.000000 edri-2024.6.1/edri.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-06-03 11:48:59.549369 edri-2024.6.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1841 2024-06-03 11:48:34.000000 edri-2024.6.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 11:48:59.545369 edri-2024.6.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1396 2024-03-07 10:37:30.000000 edri-2024.6.1/tests/test_storage.py
```

### Comparing `edri-2024.4.1/PKG-INFO` & `edri-2024.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edri
-Version: 2024.4.1
+Version: 2024.6.1
 Summary: Event Driven Routing Infrastructure
 Author: Marek Olšan
 Author-email: marek.olsan@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `edri-2024.4.1/README.md` & `edri-2024.6.1/README.md`

 * *Files identical despite different names*

### Comparing `edri-2024.4.1/edri/__init__.py` & `edri-2024.6.1/edri/__init__.py`

 * *Files identical despite different names*

### Comparing `edri-2024.4.1/edri/abstract/api_base.py` & `edri-2024.6.1/edri/abstract/api_base.py`

 * *Files identical despite different names*

### Comparing `edri-2024.4.1/edri/abstract/manager/manager_base.py` & `edri-2024.6.1/edri/abstract/manager/manager_base.py`

 * *Files identical despite different names*

### Comparing `edri-2024.4.1/edri/abstract/manager/manager_priority_base.py` & `edri-2024.6.1/edri/abstract/manager/manager_priority_base.py`

 * *Files identical despite different names*

### Comparing `edri-2024.4.1/edri/abstract/worker/worker.py` & `edri-2024.6.1/edri/abstract/worker/worker.py`

 * *Files identical despite different names*

### Comparing `edri-2024.4.1/edri/abstract/worker/worker_process.py` & `edri-2024.6.1/edri/abstract/worker/worker_process.py`

 * *Files identical despite different names*

### Comparing `edri-2024.4.1/edri/abstract/worker/worker_thread.py` & `edri-2024.6.1/edri/abstract/worker/worker_thread.py`

 * *Files identical despite different names*

### Comparing `edri-2024.4.1/edri/config/setting.py` & `edri-2024.6.1/edri/config/setting.py`

 * *Files identical despite different names*

### Comparing `edri-2024.4.1/edri/dataclass/event/__init__.py` & `edri-2024.6.1/edri/dataclass/event/__init__.py`

 * *Files identical despite different names*

### Comparing `edri-2024.4.1/edri/dataclass/event/event.py` & `edri-2024.6.1/edri/dataclass/event/event.py`

 * *Files identical despite different names*

### Comparing `edri-2024.4.1/edri/dataclass/event/response.py` & `edri-2024.6.1/edri/dataclass/event/response.py`

 * *Files identical despite different names*

### Comparing `edri-2024.4.1/edri/rest/server.py` & `edri-2024.6.1/edri/rest/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -383,64 +383,64 @@
                         await send({
                             'type': 'http.response.body',
                             'body': b"",
                             'more_body': False
                         })
                         return
 
-                    for name, value in parameters.items():
-                        annotation = event_constructor.__annotations__.get(name, None)
-                        if not annotation:
-                            self.logger.debug("Unknown parameter %s", name)
-                            await send({
-                                'type': 'http.response.start',
-                                'status': 400,
-                                'headers': [
-                                    [b'content-type', b'text/plain'],
-                                ]
-                            })
-                            await send({
-                                'type': 'http.response.body',
-                                'body': b"",
-                                'more_body': False
-                            })
-                            return
-                        try:
-                            value = self.check_type(value, annotation)
-                        except TypeError as e:
-                            self.logger.debug("Wrong type %s for %s:%s", type(value), name, annotation, exc_info=e)
-                            await send({
-                                'type': 'http.response.start',
-                                'status': 400,
-                                'headers': [
-                                    [b'content-type', b'text/plain'],
-                                ]
-                            })
-                            await send({
-                                'type': 'http.response.body',
-                                'body': b"",
-                                'more_body': False
-                            })
-                            return
-                        except Exception as e:
-                            self.logger.debug("Unknown error during type checking", exc_info=e)
-                            await send({
-                                'type': 'http.response.start',
-                                'status': 500,
-                                'headers': [
-                                    [b'content-type', b'text/plain'],
-                                ]
-                            })
-                            await send({
-                                'type': 'http.response.body',
-                                'body': b"",
-                                'more_body': False
-                            })
-                            return
-                        parameters[name] = value
+                for name, value in parameters.items():
+                    annotation = event_constructor.__annotations__.get(name, None)
+                    if not annotation:
+                        self.logger.debug("Unknown parameter %s", name)
+                        await send({
+                            'type': 'http.response.start',
+                            'status': 400,
+                            'headers': [
+                                [b'content-type', b'text/plain'],
+                            ]
+                        })
+                        await send({
+                            'type': 'http.response.body',
+                            'body': b"",
+                            'more_body': False
+                        })
+                        return
+                    try:
+                        value = self.check_type(value, annotation)
+                    except TypeError as e:
+                        self.logger.debug("Wrong type %s for %s:%s", type(value), name, annotation, exc_info=e)
+                        await send({
+                            'type': 'http.response.start',
+                            'status': 400,
+                            'headers': [
+                                [b'content-type', b'text/plain'],
+                            ]
+                        })
+                        await send({
+                            'type': 'http.response.body',
+                            'body': b"",
+                            'more_body': False
+                        })
+                        return
+                    except Exception as e:
+                        self.logger.debug("Unknown error during type checking", exc_info=e)
+                        await send({
+                            'type': 'http.response.start',
+                            'status': 500,
+                            'headers': [
+                                [b'content-type', b'text/plain'],
+                            ]
+                        })
+                        await send({
+                            'type': 'http.response.body',
+                            'body': b"",
+                            'more_body': False
+                        })
+                        return
+                    parameters[name] = value
                 else:
                     for key, value in scope["headers"]:
                         if key == b"content-length":
                             try:
                                 size = int(value)
                             except Exception:
                                 continue
```

### Comparing `edri-2024.4.1/edri/router/cache.py` & `edri-2024.6.1/edri/router/cache.py`

 * *Files identical despite different names*

### Comparing `edri-2024.4.1/edri/router/health_checker.py` & `edri-2024.6.1/edri/router/health_checker.py`

 * *Files identical despite different names*

### Comparing `edri-2024.4.1/edri/router/router.py` & `edri-2024.6.1/edri/router/router.py`

 * *Files identical despite different names*

### Comparing `edri-2024.4.1/edri/store.py` & `edri-2024.6.1/edri/store.py`

 * *Files identical despite different names*

### Comparing `edri-2024.4.1/edri/switch/forwarder.py` & `edri-2024.6.1/edri/switch/forwarder.py`

 * *Files identical despite different names*

### Comparing `edri-2024.4.1/edri/switch/receiver.py` & `edri-2024.6.1/edri/switch/receiver.py`

 * *Files identical despite different names*

### Comparing `edri-2024.4.1/edri/switch/sender.py` & `edri-2024.6.1/edri/switch/sender.py`

 * *Files identical despite different names*

### Comparing `edri-2024.4.1/edri/switch/switch.py` & `edri-2024.6.1/edri/switch/switch.py`

 * *Files identical despite different names*

### Comparing `edri-2024.4.1/edri/utility/api_broker.py` & `edri-2024.6.1/edri/utility/api_broker.py`

 * *Files identical despite different names*

### Comparing `edri-2024.4.1/edri/utility/connector/connector.py` & `edri-2024.6.1/edri/utility/connector/connector.py`

 * *Files identical despite different names*

### Comparing `edri-2024.4.1/edri/utility/connector/socket.py` & `edri-2024.6.1/edri/utility/connector/socket.py`

 * *Files identical despite different names*

### Comparing `edri-2024.4.1/edri/utility/eta.py` & `edri-2024.6.1/edri/utility/eta.py`

 * *Files identical despite different names*

### Comparing `edri-2024.4.1/edri/utility/function.py` & `edri-2024.6.1/edri/utility/function.py`

 * *Files identical despite different names*

### Comparing `edri-2024.4.1/edri/utility/scheduler.py` & `edri-2024.6.1/edri/utility/scheduler.py`

 * *Files identical despite different names*

### Comparing `edri-2024.4.1/edri/utility/storage.py` & `edri-2024.6.1/edri/utility/storage.py`

 * *Files identical despite different names*

### Comparing `edri-2024.4.1/edri/utility/store.py` & `edri-2024.6.1/edri/utility/store.py`

 * *Files identical despite different names*

### Comparing `edri-2024.4.1/edri/websocket/api.py` & `edri-2024.6.1/edri/websocket/api.py`

 * *Files identical despite different names*

### Comparing `edri-2024.4.1/edri.egg-info/PKG-INFO` & `edri-2024.6.1/edri.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edri
-Version: 2024.4.1
+Version: 2024.6.1
 Summary: Event Driven Routing Infrastructure
 Author: Marek Olšan
 Author-email: marek.olsan@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `edri-2024.4.1/edri.egg-info/SOURCES.txt` & `edri-2024.6.1/edri.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edri-2024.4.1/setup.py` & `edri-2024.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 where events act as messages exchanged between various components to control and manage operations. Drawing parallels with TCP/IP in 
 computer networks, EDRI's **routing infrastructure** facilitates the exchange and delivery of events. Instead of IP ranges, event types (
 e.g., file uploads) are used to determine the destination of each event, ensuring efficient and targeted delivery to the appropriate 
 recipients. This approach streamlines the process of managing distributed tasks within applications."""
 
 setup(
     name='edri',
-    version='2024.04.01',
+    version='2024.06.01',
     packages=find_packages(),
     description='Event Driven Routing Infrastructure',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Marek Olšan',
     author_email='marek.olsan@gmail.com',
     install_requires=[
```

### Comparing `edri-2024.4.1/tests/test_storage.py` & `edri-2024.6.1/tests/test_storage.py`

 * *Files identical despite different names*

