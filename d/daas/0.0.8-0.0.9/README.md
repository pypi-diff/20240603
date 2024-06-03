# Comparing `tmp/daas-0.0.8.tar.gz` & `tmp/daas-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daas-0.0.8.tar", max compression
+gzip compressed data, was "daas-0.0.9.tar", max compression
```

## Comparing `daas-0.0.8.tar` & `daas-0.0.9.tar`

### file list

```diff
@@ -1,194 +1,196 @@
--rw-r--r--   0        0        0      156 2023-03-24 13:43:43.489173 daas-0.0.8/LICENSE
--rw-r--r--   0        0        0     3715 2023-09-05 10:34:26.243077 daas-0.0.8/README.md
--rw-r--r--   0        0        0     1761 2024-01-15 03:55:03.452826 daas-0.0.8/mesh/__init__.py
--rw-r--r--   0        0        0      266 2023-03-24 13:43:43.473388 daas-0.0.8/mesh/_manylinux.py
--rw-r--r--   0        0        0      967 2023-03-24 13:43:43.155706 daas-0.0.8/mesh/asm/__init__.py
--rw-r--r--   0        0        0      572 2023-03-24 13:43:43.294565 daas-0.0.8/mesh/boost/__init__.py
--rw-r--r--   0        0        0    44616 2024-01-12 10:54:17.083583 daas-0.0.8/mesh/boost/contab.py
--rw-r--r--   0        0        0    21096 2024-01-15 08:34:55.597349 daas-0.0.8/mesh/boost/disruptor.py
--rw-r--r--   0        0        0     3526 2024-01-15 10:02:09.274196 daas-0.0.8/mesh/boost/mooter.py
--rw-r--r--   0        0        0     3748 2024-01-15 08:32:02.166777 daas-0.0.8/mesh/boost/remote.py
--rw-r--r--   0        0        0    13703 2023-03-24 13:43:43.293074 daas-0.0.8/mesh/boost/ringbuffer.py
--rw-r--r--   0        0        0     1318 2023-03-24 13:43:43.293764 daas-0.0.8/mesh/boost/runhook.py
--rw-r--r--   0        0        0     2482 2024-01-12 11:16:35.262349 daas-0.0.8/mesh/boost/scheduler.py
--rw-r--r--   0        0        0      578 2023-03-24 13:43:43.287916 daas-0.0.8/mesh/cause/__init__.py
--rw-r--r--   0        0        0     1406 2023-03-24 13:43:43.290998 daas-0.0.8/mesh/cause/errors.py
--rw-r--r--   0        0        0     4073 2024-01-10 04:34:41.900696 daas-0.0.8/mesh/cause/status.py
--rw-r--r--   0        0        0      612 2023-03-24 13:43:43.304283 daas-0.0.8/mesh/codec/__init__.py
--rw-r--r--   0        0        0      816 2023-03-24 13:43:43.310986 daas-0.0.8/mesh/codec/codec.py
--rw-r--r--   0        0        0     4043 2023-03-24 13:43:43.310310 daas-0.0.8/mesh/codec/former.py
--rw-r--r--   0        0        0     1125 2023-03-24 13:43:43.304987 daas-0.0.8/mesh/codec/jsons.py
--rw-r--r--   0        0        0      405 2023-03-24 13:43:43.311662 daas-0.0.8/mesh/codec/protobuf.py
--rw-r--r--   0        0        0    14467 2023-03-24 13:43:43.302202 daas-0.0.8/mesh/codec/tools.py
--rw-r--r--   0        0        0      414 2023-03-24 13:43:43.303706 daas-0.0.8/mesh/codec/xml.py
--rw-r--r--   0        0        0      384 2023-03-24 13:43:43.303014 daas-0.0.8/mesh/codec/yml.py
--rw-r--r--   0        0        0      445 2023-03-24 13:43:43.159643 daas-0.0.8/mesh/context/__init__.py
--rw-r--r--   0        0        0     5703 2024-01-15 06:47:36.767694 daas-0.0.8/mesh/context/context.py
--rw-r--r--   0        0        0     2321 2024-01-15 09:22:52.377368 daas-0.0.8/mesh/context/mesh.py
--rw-r--r--   0        0        0      390 2023-03-24 13:43:43.387644 daas-0.0.8/mesh/environ/__init__.py
--rw-r--r--   0        0        0     1878 2023-03-24 13:43:43.387350 daas-0.0.8/mesh/environ/cache.py
--rw-r--r--   0        0        0     7432 2024-01-15 06:52:30.746514 daas-0.0.8/mesh/environ/environ.py
--rw-r--r--   0        0        0      157 2023-03-24 13:43:43.463361 daas-0.0.8/mesh/examples/__init__.py
--rw-r--r--   0        0        0      157 2023-03-24 13:43:43.466089 daas-0.0.8/mesh/examples/consumer.py
--rw-r--r--   0        0        0      157 2023-03-24 13:43:43.461976 daas-0.0.8/mesh/examples/provider.py
--rw-r--r--   0        0        0      709 2024-01-10 04:27:23.424950 daas-0.0.8/mesh/grpx/__init__.py
--rw-r--r--   0        0        0     2728 2024-01-12 09:48:41.721135 daas-0.0.8/mesh/grpx/bindservice.py
--rw-r--r--   0        0        0     6715 2024-01-11 10:59:33.348708 daas-0.0.8/mesh/grpx/channels.py
--rw-r--r--   0        0        0     4597 2024-01-15 03:23:45.283235 daas-0.0.8/mesh/grpx/consumer.py
--rw-r--r--   0        0        0     5876 2024-01-11 11:07:24.875394 daas-0.0.8/mesh/grpx/interceptor.py
--rw-r--r--   0        0        0      352 2023-03-24 13:43:43.244419 daas-0.0.8/mesh/grpx/marshaller.py
--rw-r--r--   0        0        0     2060 2024-01-15 04:21:12.709524 daas-0.0.8/mesh/grpx/provider.py
--rw-r--r--   0        0        0     2131 2023-03-24 13:43:43.243092 daas-0.0.8/mesh/grpx/transport.py
--rw-r--r--   0        0        0      350 2023-03-24 13:43:43.392403 daas-0.0.8/mesh/http/__init__.py
--rw-r--r--   0        0        0      608 2024-01-11 03:10:46.921786 daas-0.0.8/mesh/http/consumer.py
--rw-r--r--   0        0        0      657 2024-01-15 04:20:46.252909 daas-0.0.8/mesh/http/provider.py
--rw-r--r--   0        0        0      400 2023-03-24 13:43:43.476051 daas-0.0.8/mesh/ioc/__init__.py
--rw-r--r--   0        0        0      266 2023-03-24 13:43:43.480828 daas-0.0.8/mesh/ioc/cause_handler.py
--rw-r--r--   0        0        0      398 2023-03-24 13:43:43.480160 daas-0.0.8/mesh/ioc/context.py
--rw-r--r--   0        0        0      354 2023-03-24 13:43:43.481699 daas-0.0.8/mesh/ioc/envs_processor.py
--rw-r--r--   0        0        0      627 2023-03-24 13:43:43.474868 daas-0.0.8/mesh/ioc/paas_processor.py
--rw-r--r--   0        0        0     1874 2024-01-10 04:41:46.202034 daas-0.0.8/mesh/kinds/__init__.py
--rw-r--r--   0        0        0      476 2023-03-24 13:43:43.281679 daas-0.0.8/mesh/kinds/captcha.py
--rw-r--r--   0        0        0      693 2023-03-24 13:43:43.256471 daas-0.0.8/mesh/kinds/commerce.py
--rw-r--r--   0        0        0      674 2023-03-24 13:43:43.283660 daas-0.0.8/mesh/kinds/document.py
--rw-r--r--   0        0        0     1662 2023-03-24 13:43:43.284090 daas-0.0.8/mesh/kinds/entity.py
--rw-r--r--   0        0        0     1868 2024-01-11 09:16:24.424127 daas-0.0.8/mesh/kinds/environ.py
--rw-r--r--   0        0        0     3377 2024-01-11 09:34:17.307950 daas-0.0.8/mesh/kinds/event.py
--rw-r--r--   0        0        0      406 2023-03-24 13:43:43.281251 daas-0.0.8/mesh/kinds/inbound.py
--rw-r--r--   0        0        0      489 2024-01-15 07:14:58.160839 daas-0.0.8/mesh/kinds/institution.py
--rw-r--r--   0        0        0     1569 2023-03-24 13:43:43.284989 daas-0.0.8/mesh/kinds/license.py
--rw-r--r--   0        0        0     1066 2024-01-11 11:17:07.615499 daas-0.0.8/mesh/kinds/location.py
--rw-r--r--   0        0        0     1242 2023-03-24 13:43:43.282951 daas-0.0.8/mesh/kinds/meshflag.py
--rw-r--r--   0        0        0      505 2023-03-24 13:43:43.282501 daas-0.0.8/mesh/kinds/outbound.py
--rw-r--r--   0        0        0      633 2023-03-24 13:43:43.261106 daas-0.0.8/mesh/kinds/page.py
--rw-r--r--   0        0        0      513 2023-03-24 13:43:43.286534 daas-0.0.8/mesh/kinds/paging.py
--rw-r--r--   0        0        0      405 2023-03-24 13:43:43.255157 daas-0.0.8/mesh/kinds/principal.py
--rw-r--r--   0        0        0      358 2023-03-24 13:43:43.257982 daas-0.0.8/mesh/kinds/profile.py
--rw-r--r--   0        0        0     1230 2023-03-24 13:43:43.284531 daas-0.0.8/mesh/kinds/reference.py
--rw-r--r--   0        0        0     1147 2023-03-24 13:43:43.254764 daas-0.0.8/mesh/kinds/registration.py
--rw-r--r--   0        0        0     2874 2023-03-24 13:43:43.258442 daas-0.0.8/mesh/kinds/route.py
--rw-r--r--   0        0        0      708 2023-03-24 13:43:43.286209 daas-0.0.8/mesh/kinds/script.py
--rw-r--r--   0        0        0     3223 2023-03-24 13:43:43.255808 daas-0.0.8/mesh/kinds/service.py
--rw-r--r--   0        0        0      233 2023-03-24 13:43:43.259148 daas-0.0.8/mesh/kinds/timeout.py
--rw-r--r--   0        0        0     1276 2023-03-24 13:43:43.285769 daas-0.0.8/mesh/kinds/versions.py
--rw-r--r--   0        0        0      750 2023-03-24 13:43:43.467564 daas-0.0.8/mesh/log/__init__.py
--rw-r--r--   0        0        0     2782 2024-01-11 03:23:25.363880 daas-0.0.8/mesh/log/nop.py
--rw-r--r--   0        0        0     1977 2023-03-24 13:43:43.468520 daas-0.0.8/mesh/log/types.py
--rw-r--r--   0        0        0     1334 2023-03-24 13:43:43.364011 daas-0.0.8/mesh/macro/__init__.py
--rw-r--r--   0        0        0     4161 2023-03-24 13:43:43.361003 daas-0.0.8/mesh/macro/ark.py
--rw-r--r--   0        0        0     2393 2023-03-24 13:43:43.386022 daas-0.0.8/mesh/macro/binding.py
--rw-r--r--   0        0        0      663 2023-03-24 13:43:43.365623 daas-0.0.8/mesh/macro/cause.py
--rw-r--r--   0        0        0     3878 2023-03-24 13:43:43.385415 daas-0.0.8/mesh/macro/codec.py
--rw-r--r--   0        0        0     4324 2023-03-24 13:43:43.358880 daas-0.0.8/mesh/macro/compatible.py
--rw-r--r--   0        0        0     2160 2023-03-24 13:43:43.359311 daas-0.0.8/mesh/macro/index.py
--rw-r--r--   0        0        0     2700 2024-01-11 02:42:53.874058 daas-0.0.8/mesh/macro/inspect.py
--rw-r--r--   0        0        0      452 2023-03-24 13:43:43.362645 daas-0.0.8/mesh/macro/interface.py
--rw-r--r--   0        0        0     3991 2023-03-24 13:43:43.384883 daas-0.0.8/mesh/macro/loader.py
--rw-r--r--   0        0        0     4439 2023-04-23 06:49:01.214254 daas-0.0.8/mesh/macro/mpi.py
--rw-r--r--   0        0        0     2145 2023-03-24 13:43:43.360119 daas-0.0.8/mesh/macro/mps.py
--rw-r--r--   0        0        0     7983 2024-01-12 10:02:15.550458 daas-0.0.8/mesh/macro/proxy.py
--rw-r--r--   0        0        0     1431 2023-03-24 13:43:43.386453 daas-0.0.8/mesh/macro/spi.py
--rw-r--r--   0        0        0      247 2023-03-24 13:43:43.368145 daas-0.0.8/mesh/macro/types.py
--rw-r--r--   0        0        0      220 2023-03-24 13:43:43.150120 daas-0.0.8/mesh/metrics/__init__.py
--rw-r--r--   0        0        0     6062 2023-03-24 13:43:43.149511 daas-0.0.8/mesh/metrics/collector.py
--rw-r--r--   0        0        0     2706 2023-03-24 13:43:43.153226 daas-0.0.8/mesh/metrics/scheduler.py
--rw-r--r--   0        0        0     1279 2024-01-11 09:38:04.654688 daas-0.0.8/mesh/mpc/__init__.py
--rw-r--r--   0        0        0     6762 2023-07-18 05:20:18.792244 daas-0.0.8/mesh/mpc/compiler.py
--rw-r--r--   0        0        0     1191 2024-01-10 12:26:59.216920 daas-0.0.8/mesh/mpc/consumer.py
--rw-r--r--   0        0        0     2173 2024-01-15 08:03:15.776441 daas-0.0.8/mesh/mpc/consumer_filter.py
--rw-r--r--   0        0        0     1854 2024-01-15 06:38:37.320066 daas-0.0.8/mesh/mpc/digest.py
--rw-r--r--   0        0        0     1734 2023-03-24 13:43:43.400089 daas-0.0.8/mesh/mpc/eden.py
--rw-r--r--   0        0        0     1451 2024-01-11 09:04:44.328966 daas-0.0.8/mesh/mpc/filter.py
--rw-r--r--   0        0        0     3345 2024-01-10 12:19:22.428000 daas-0.0.8/mesh/mpc/generic.py
--rw-r--r--   0        0        0      991 2024-01-11 03:38:54.655090 daas-0.0.8/mesh/mpc/inspector.py
--rw-r--r--   0        0        0     3306 2024-01-11 09:06:07.835479 daas-0.0.8/mesh/mpc/invoker.py
--rw-r--r--   0        0        0      830 2024-01-15 08:03:26.787672 daas-0.0.8/mesh/mpc/isolate_filter.py
--rw-r--r--   0        0        0    15580 2024-01-12 10:08:41.853533 daas-0.0.8/mesh/mpc/mesh_eden.py
--rw-r--r--   0        0        0      612 2024-01-12 10:11:33.381101 daas-0.0.8/mesh/mpc/provider.py
--rw-r--r--   0        0        0     1690 2024-01-15 08:02:58.718004 daas-0.0.8/mesh/mpc/provider_filter.py
--rw-r--r--   0        0        0     6524 2024-01-15 08:37:18.729447 daas-0.0.8/mesh/mpc/reference.py
--rw-r--r--   0        0        0     1256 2024-01-15 08:02:49.995226 daas-0.0.8/mesh/mpc/robust_filter.py
--rw-r--r--   0        0        0     1414 2024-01-11 03:38:28.002539 daas-0.0.8/mesh/mpc/service.py
--rw-r--r--   0        0        0     1152 2023-07-18 05:19:51.937010 daas-0.0.8/mesh/mpc/service_proxy.py
--rw-r--r--   0        0        0     4384 2024-01-15 08:37:18.707112 daas-0.0.8/mesh/mpc/stream.py
--rw-r--r--   0        0        0     3849 2024-01-15 08:37:18.715373 daas-0.0.8/mesh/mpc/transporter.py
--rw-r--r--   0        0        0     6244 2024-01-10 07:29:19.207963 daas-0.0.8/mesh/mpc/urn.py
--rw-r--r--   0        0        0     1846 2023-03-24 13:43:43.177695 daas-0.0.8/mesh/prsim/__init__.py
--rw-r--r--   0        0        0     1620 2024-01-11 08:25:41.113444 daas-0.0.8/mesh/prsim/builtin.py
--rw-r--r--   0        0        0     2645 2024-01-11 08:27:09.391977 daas-0.0.8/mesh/prsim/cache.py
--rw-r--r--   0        0        0      678 2024-01-11 08:27:25.223040 daas-0.0.8/mesh/prsim/cluster.py
--rw-r--r--   0        0        0     1300 2024-01-11 08:28:16.958879 daas-0.0.8/mesh/prsim/commerce.py
--rw-r--r--   0        0        0     7472 2024-01-15 06:38:03.427863 daas-0.0.8/mesh/prsim/context.py
--rw-r--r--   0        0        0     1620 2024-01-11 08:28:38.235421 daas-0.0.8/mesh/prsim/cryptor.py
--rw-r--r--   0        0        0     1349 2024-01-11 08:28:59.500384 daas-0.0.8/mesh/prsim/datahouse.py
--rw-r--r--   0        0        0      950 2024-01-11 08:29:35.004476 daas-0.0.8/mesh/prsim/dispatcher.py
--rw-r--r--   0        0        0      899 2024-01-11 08:29:48.933700 daas-0.0.8/mesh/prsim/endpoint.py
--rw-r--r--   0        0        0     1261 2024-01-11 08:30:06.673680 daas-0.0.8/mesh/prsim/evaluator.py
--rw-r--r--   0        0        0      855 2024-01-11 08:30:21.092401 daas-0.0.8/mesh/prsim/graphics.py
--rw-r--r--   0        0        0      736 2024-01-11 08:30:41.978620 daas-0.0.8/mesh/prsim/hodor.py
--rw-r--r--   0        0        0      778 2024-01-11 08:30:53.470319 daas-0.0.8/mesh/prsim/iostream.py
--rw-r--r--   0        0        0     1384 2024-01-11 08:31:27.233986 daas-0.0.8/mesh/prsim/kv.py
--rw-r--r--   0        0        0     1270 2024-01-11 08:31:56.821975 daas-0.0.8/mesh/prsim/licenser.py
--rw-r--r--   0        0        0     1122 2024-01-11 08:32:23.235449 daas-0.0.8/mesh/prsim/locker.py
--rw-r--r--   0        0        0     3916 2024-01-11 08:32:38.204019 daas-0.0.8/mesh/prsim/network.py
--rw-r--r--   0        0        0     2544 2024-01-11 09:37:04.803296 daas-0.0.8/mesh/prsim/publisher.py
--rw-r--r--   0        0        0     1315 2024-01-11 08:33:22.873548 daas-0.0.8/mesh/prsim/registry.py
--rw-r--r--   0        0        0     2853 2023-04-23 06:51:56.399623 daas-0.0.8/mesh/prsim/routable.py
--rw-r--r--   0        0        0      876 2024-01-12 10:08:12.301629 daas-0.0.8/mesh/prsim/runtime_hook.py
--rw-r--r--   0        0        0     2347 2024-01-11 08:33:40.253814 daas-0.0.8/mesh/prsim/scheduler.py
--rw-r--r--   0        0        0      850 2024-01-11 08:33:54.591408 daas-0.0.8/mesh/prsim/sequence.py
--rw-r--r--   0        0        0      594 2024-01-11 08:34:08.455647 daas-0.0.8/mesh/prsim/subscriber.py
--rw-r--r--   0        0        0      714 2024-01-11 08:34:16.399695 daas-0.0.8/mesh/prsim/tokenizer.py
--rw-r--r--   0        0        0     2965 2024-01-11 08:35:22.121023 daas-0.0.8/mesh/prsim/transport.py
--rw-r--r--   0        0        0      338 2023-03-24 13:43:43.313535 daas-0.0.8/mesh/runtime/__init__.py
--rw-r--r--   0        0        0      747 2023-03-24 13:43:43.317960 daas-0.0.8/mesh/runtime/container.py
--rw-r--r--   0        0        0     1554 2023-03-24 13:43:43.319630 daas-0.0.8/mesh/runtime/context.py
--rw-r--r--   0        0        0      585 2023-03-24 13:43:43.321107 daas-0.0.8/mesh/runtime/mesh_processor.py
--rw-r--r--   0        0        0      222 2023-03-24 13:43:43.326527 daas-0.0.8/mesh/schema/__init__.py
--rw-r--r--   0        0        0     1316 2023-03-24 13:43:43.344757 daas-0.0.8/mesh/system/__init__.py
--rw-r--r--   0        0        0     2195 2024-01-11 08:35:53.021769 daas-0.0.8/mesh/system/mesh_builtin.py
--rw-r--r--   0        0        0      931 2024-01-11 08:37:08.434631 daas-0.0.8/mesh/system/mesh_cache.py
--rw-r--r--   0        0        0      558 2024-01-11 08:27:46.467327 daas-0.0.8/mesh/system/mesh_cluster.py
--rw-r--r--   0        0        0      945 2024-01-11 08:37:56.749255 daas-0.0.8/mesh/system/mesh_datahouse.py
--rw-r--r--   0        0        0      531 2024-01-11 08:38:11.075150 daas-0.0.8/mesh/system/mesh_dispatcher.py
--rw-r--r--   0        0        0      427 2024-01-11 08:38:29.318977 daas-0.0.8/mesh/system/mesh_endpoint.py
--rw-r--r--   0        0        0      921 2024-01-11 08:38:58.173775 daas-0.0.8/mesh/system/mesh_evaluator.py
--rw-r--r--   0        0        0      474 2024-01-11 08:39:10.135306 daas-0.0.8/mesh/system/mesh_hodor.py
--rw-r--r--   0        0        0      782 2024-01-11 08:39:37.865970 daas-0.0.8/mesh/system/mesh_locker.py
--rw-r--r--   0        0        0     2888 2024-01-15 08:37:18.723444 daas-0.0.8/mesh/system/mesh_network.py
--rw-r--r--   0        0        0      664 2024-01-11 08:41:33.613880 daas-0.0.8/mesh/system/mesh_publisher.py
--rw-r--r--   0        0        0      898 2024-01-11 08:42:02.052058 daas-0.0.8/mesh/system/mesh_registry.py
--rw-r--r--   0        0        0      495 2024-01-15 03:43:33.934403 daas-0.0.8/mesh/system/mesh_runtime_hook.py
--rw-r--r--   0        0        0     1292 2024-01-11 08:43:10.290323 daas-0.0.8/mesh/system/mesh_scheduler.py
--rw-r--r--   0        0        0     4522 2024-01-15 08:37:18.736470 daas-0.0.8/mesh/system/mesh_transport.py
--rw-r--r--   0        0        0     2623 2023-03-24 13:43:43.223132 daas-0.0.8/mesh/test/__init__.py
--rw-r--r--   0        0        0      157 2023-03-24 13:43:43.219724 daas-0.0.8/mesh/test/boost/__init__.py
--rw-r--r--   0        0        0     8605 2023-03-24 13:43:43.220466 daas-0.0.8/mesh/test/boost/disruptor_test.py
--rw-r--r--   0        0        0     7532 2023-03-24 13:43:43.218726 daas-0.0.8/mesh/test/boost/ringbuffer_perf_test.py
--rw-r--r--   0        0        0    26327 2023-03-24 13:43:43.217943 daas-0.0.8/mesh/test/boost/ringbuffer_test.py
--rw-r--r--   0        0        0      157 2023-03-24 13:43:43.222452 daas-0.0.8/mesh/test/codec/__init__.py
--rw-r--r--   0        0        0      899 2023-03-24 13:43:43.221717 daas-0.0.8/mesh/test/codec/codec_test.py
--rw-r--r--   0        0        0      157 2023-03-24 13:43:43.216670 daas-0.0.8/mesh/test/grpx/__init__.py
--rw-r--r--   0        0        0      701 2023-03-24 13:43:43.215844 daas-0.0.8/mesh/test/grpx/grpc_test.py
--rw-r--r--   0        0        0      157 2023-03-24 13:43:43.236089 daas-0.0.8/mesh/test/ioc/__init__.py
--rw-r--r--   0        0        0      506 2023-03-24 13:43:43.235345 daas-0.0.8/mesh/test/ioc/container_test.py
--rw-r--r--   0        0        0      161 2024-01-10 04:11:17.562723 daas-0.0.8/mesh/test/load/__init__.py
--rw-r--r--   0        0        0      595 2024-01-15 02:41:07.280763 daas-0.0.8/mesh/test/load/provider.py
--rw-r--r--   0        0        0      158 2023-03-24 13:43:43.228000 daas-0.0.8/mesh/test/macro/__init__.py
--rw-r--r--   0        0        0     1954 2023-03-24 13:43:43.227335 daas-0.0.8/mesh/test/macro/macro_test.py
--rw-r--r--   0        0        0      752 2023-03-24 13:43:43.228742 daas-0.0.8/mesh/test/macro/proxy_test.py
--rw-r--r--   0        0        0      157 2023-03-24 13:43:43.207945 daas-0.0.8/mesh/test/metrics/__init__.py
--rw-r--r--   0        0        0      369 2023-03-24 13:43:43.208469 daas-0.0.8/mesh/test/metrics/collector_test.py
--rw-r--r--   0        0        0      157 2023-03-24 13:43:43.229658 daas-0.0.8/mesh/test/mpc/__init__.py
--rw-r--r--   0        0        0      887 2023-03-24 13:43:43.233327 daas-0.0.8/mesh/test/mpc/compile_test.py
--rw-r--r--   0        0        0     1338 2024-01-15 08:37:18.742836 daas-0.0.8/mesh/test/mpc/mpc_test.py
--rw-r--r--   0        0        0      408 2023-03-24 13:43:43.232010 daas-0.0.8/mesh/test/mpc/service_loader_test.py
--rw-r--r--   0        0        0      157 2023-03-24 13:43:43.209353 daas-0.0.8/mesh/test/prsim/__init__.py
--rw-r--r--   0        0        0      591 2023-03-24 13:43:43.214304 daas-0.0.8/mesh/test/prsim/network_test.py
--rw-r--r--   0        0        0      157 2023-03-24 13:43:43.237557 daas-0.0.8/mesh/test/tool/__init__.py
--rw-r--r--   0        0        0     1006 2023-03-24 13:43:43.238330 daas-0.0.8/mesh/test/tool/tool_test.py
--rw-r--r--   0        0        0     5011 2024-01-15 02:46:42.656040 daas-0.0.8/mesh/tool/__init__.py
--rw-r--r--   0        0        0     2939 2023-03-24 13:43:43.485869 daas-0.0.8/mesh/tool/snowflake.py
--rw-r--r--   0        0        0      594 2023-03-24 13:43:43.487133 daas-0.0.8/mesh/tool/versions.py
--rw-r--r--   0        0        0     1224 2024-01-21 16:18:12.092666 daas-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     4984 1970-01-01 00:00:00.000000 daas-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      156 2023-03-24 13:43:43.489173 daas-0.0.9/LICENSE
+-rw-r--r--   0        0        0     3715 2023-09-05 10:34:26.243077 daas-0.0.9/README.md
+-rw-r--r--   0        0        0     1761 2024-01-15 03:55:03.452826 daas-0.0.9/mesh/__init__.py
+-rw-r--r--   0        0        0      266 2023-03-24 13:43:43.473388 daas-0.0.9/mesh/_manylinux.py
+-rw-r--r--   0        0        0      967 2023-03-24 13:43:43.155706 daas-0.0.9/mesh/asm/__init__.py
+-rw-r--r--   0        0        0      572 2023-03-24 13:43:43.294565 daas-0.0.9/mesh/boost/__init__.py
+-rw-r--r--   0        0        0    44616 2024-01-12 10:54:17.083583 daas-0.0.9/mesh/boost/contab.py
+-rw-r--r--   0        0        0    21096 2024-01-15 08:34:55.597349 daas-0.0.9/mesh/boost/disruptor.py
+-rw-r--r--   0        0        0     3526 2024-01-15 10:02:09.274196 daas-0.0.9/mesh/boost/mooter.py
+-rw-r--r--   0        0        0     3748 2024-01-15 08:32:02.166777 daas-0.0.9/mesh/boost/remote.py
+-rw-r--r--   0        0        0    13703 2023-03-24 13:43:43.293074 daas-0.0.9/mesh/boost/ringbuffer.py
+-rw-r--r--   0        0        0     1318 2023-03-24 13:43:43.293764 daas-0.0.9/mesh/boost/runhook.py
+-rw-r--r--   0        0        0     2482 2024-01-12 11:16:35.262349 daas-0.0.9/mesh/boost/scheduler.py
+-rw-r--r--   0        0        0      578 2023-03-24 13:43:43.287916 daas-0.0.9/mesh/cause/__init__.py
+-rw-r--r--   0        0        0     1406 2023-03-24 13:43:43.290998 daas-0.0.9/mesh/cause/errors.py
+-rw-r--r--   0        0        0     4073 2024-01-10 04:34:41.900696 daas-0.0.9/mesh/cause/status.py
+-rw-r--r--   0        0        0      612 2023-03-24 13:43:43.304283 daas-0.0.9/mesh/codec/__init__.py
+-rw-r--r--   0        0        0      816 2023-03-24 13:43:43.310986 daas-0.0.9/mesh/codec/codec.py
+-rw-r--r--   0        0        0     4043 2023-03-24 13:43:43.310310 daas-0.0.9/mesh/codec/former.py
+-rw-r--r--   0        0        0     1125 2023-03-24 13:43:43.304987 daas-0.0.9/mesh/codec/jsons.py
+-rw-r--r--   0        0        0      405 2023-03-24 13:43:43.311662 daas-0.0.9/mesh/codec/protobuf.py
+-rw-r--r--   0        0        0    14467 2023-03-24 13:43:43.302202 daas-0.0.9/mesh/codec/tools.py
+-rw-r--r--   0        0        0      414 2023-03-24 13:43:43.303706 daas-0.0.9/mesh/codec/xml.py
+-rw-r--r--   0        0        0      384 2023-03-24 13:43:43.303014 daas-0.0.9/mesh/codec/yml.py
+-rw-r--r--   0        0        0      445 2023-03-24 13:43:43.159643 daas-0.0.9/mesh/context/__init__.py
+-rw-r--r--   0        0        0     5703 2024-01-15 06:47:36.767694 daas-0.0.9/mesh/context/context.py
+-rw-r--r--   0        0        0     2321 2024-01-15 09:22:52.377368 daas-0.0.9/mesh/context/mesh.py
+-rw-r--r--   0        0        0      390 2023-03-24 13:43:43.387644 daas-0.0.9/mesh/environ/__init__.py
+-rw-r--r--   0        0        0     1878 2023-03-24 13:43:43.387350 daas-0.0.9/mesh/environ/cache.py
+-rw-r--r--   0        0        0     7738 2024-01-26 04:20:03.636948 daas-0.0.9/mesh/environ/environ.py
+-rw-r--r--   0        0        0      157 2023-03-24 13:43:43.463361 daas-0.0.9/mesh/examples/__init__.py
+-rw-r--r--   0        0        0      157 2023-03-24 13:43:43.466089 daas-0.0.9/mesh/examples/consumer.py
+-rw-r--r--   0        0        0      157 2023-03-24 13:43:43.461976 daas-0.0.9/mesh/examples/provider.py
+-rw-r--r--   0        0        0      709 2024-01-10 04:27:23.424950 daas-0.0.9/mesh/grpx/__init__.py
+-rw-r--r--   0        0        0     2728 2024-01-12 09:48:41.721135 daas-0.0.9/mesh/grpx/bindservice.py
+-rw-r--r--   0        0        0     6715 2024-01-11 10:59:33.348708 daas-0.0.9/mesh/grpx/channels.py
+-rw-r--r--   0        0        0     4597 2024-01-15 03:23:45.283235 daas-0.0.9/mesh/grpx/consumer.py
+-rw-r--r--   0        0        0     5876 2024-01-11 11:07:24.875394 daas-0.0.9/mesh/grpx/interceptor.py
+-rw-r--r--   0        0        0      352 2023-03-24 13:43:43.244419 daas-0.0.9/mesh/grpx/marshaller.py
+-rw-r--r--   0        0        0     2060 2024-01-15 04:21:12.709524 daas-0.0.9/mesh/grpx/provider.py
+-rw-r--r--   0        0        0     2131 2023-03-24 13:43:43.243092 daas-0.0.9/mesh/grpx/transport.py
+-rw-r--r--   0        0        0      350 2023-03-24 13:43:43.392403 daas-0.0.9/mesh/http/__init__.py
+-rw-r--r--   0        0        0      608 2024-01-11 03:10:46.921786 daas-0.0.9/mesh/http/consumer.py
+-rw-r--r--   0        0        0      657 2024-01-15 04:20:46.252909 daas-0.0.9/mesh/http/provider.py
+-rw-r--r--   0        0        0      400 2023-03-24 13:43:43.476051 daas-0.0.9/mesh/ioc/__init__.py
+-rw-r--r--   0        0        0      266 2023-03-24 13:43:43.480828 daas-0.0.9/mesh/ioc/cause_handler.py
+-rw-r--r--   0        0        0      398 2023-03-24 13:43:43.480160 daas-0.0.9/mesh/ioc/context.py
+-rw-r--r--   0        0        0      354 2023-03-24 13:43:43.481699 daas-0.0.9/mesh/ioc/envs_processor.py
+-rw-r--r--   0        0        0      627 2023-03-24 13:43:43.474868 daas-0.0.9/mesh/ioc/paas_processor.py
+-rw-r--r--   0        0        0     1874 2024-01-10 04:41:46.202034 daas-0.0.9/mesh/kinds/__init__.py
+-rw-r--r--   0        0        0      476 2023-03-24 13:43:43.281679 daas-0.0.9/mesh/kinds/captcha.py
+-rw-r--r--   0        0        0      693 2023-03-24 13:43:43.256471 daas-0.0.9/mesh/kinds/commerce.py
+-rw-r--r--   0        0        0      674 2023-03-24 13:43:43.283660 daas-0.0.9/mesh/kinds/document.py
+-rw-r--r--   0        0        0     1662 2023-03-24 13:43:43.284090 daas-0.0.9/mesh/kinds/entity.py
+-rw-r--r--   0        0        0     1868 2024-01-11 09:16:24.424127 daas-0.0.9/mesh/kinds/environ.py
+-rw-r--r--   0        0        0     3377 2024-01-11 09:34:17.307950 daas-0.0.9/mesh/kinds/event.py
+-rw-r--r--   0        0        0      406 2023-03-24 13:43:43.281251 daas-0.0.9/mesh/kinds/inbound.py
+-rw-r--r--   0        0        0      489 2024-01-15 07:14:58.160839 daas-0.0.9/mesh/kinds/institution.py
+-rw-r--r--   0        0        0     1569 2023-03-24 13:43:43.284989 daas-0.0.9/mesh/kinds/license.py
+-rw-r--r--   0        0        0     1066 2024-01-11 11:17:07.615499 daas-0.0.9/mesh/kinds/location.py
+-rw-r--r--   0        0        0     1242 2023-03-24 13:43:43.282951 daas-0.0.9/mesh/kinds/meshflag.py
+-rw-r--r--   0        0        0      505 2023-03-24 13:43:43.282501 daas-0.0.9/mesh/kinds/outbound.py
+-rw-r--r--   0        0        0      633 2023-03-24 13:43:43.261106 daas-0.0.9/mesh/kinds/page.py
+-rw-r--r--   0        0        0      513 2023-03-24 13:43:43.286534 daas-0.0.9/mesh/kinds/paging.py
+-rw-r--r--   0        0        0      405 2023-03-24 13:43:43.255157 daas-0.0.9/mesh/kinds/principal.py
+-rw-r--r--   0        0        0      358 2023-03-24 13:43:43.257982 daas-0.0.9/mesh/kinds/profile.py
+-rw-r--r--   0        0        0     1230 2023-03-24 13:43:43.284531 daas-0.0.9/mesh/kinds/reference.py
+-rw-r--r--   0        0        0     1147 2023-03-24 13:43:43.254764 daas-0.0.9/mesh/kinds/registration.py
+-rw-r--r--   0        0        0     2874 2023-03-24 13:43:43.258442 daas-0.0.9/mesh/kinds/route.py
+-rw-r--r--   0        0        0      708 2023-03-24 13:43:43.286209 daas-0.0.9/mesh/kinds/script.py
+-rw-r--r--   0        0        0     3223 2023-03-24 13:43:43.255808 daas-0.0.9/mesh/kinds/service.py
+-rw-r--r--   0        0        0      233 2023-03-24 13:43:43.259148 daas-0.0.9/mesh/kinds/timeout.py
+-rw-r--r--   0        0        0     1276 2023-03-24 13:43:43.285769 daas-0.0.9/mesh/kinds/versions.py
+-rw-r--r--   0        0        0      750 2023-03-24 13:43:43.467564 daas-0.0.9/mesh/log/__init__.py
+-rw-r--r--   0        0        0     2782 2024-01-23 10:25:12.880088 daas-0.0.9/mesh/log/nop.py
+-rw-r--r--   0        0        0     1977 2023-03-24 13:43:43.468520 daas-0.0.9/mesh/log/types.py
+-rw-r--r--   0        0        0     1334 2023-03-24 13:43:43.364011 daas-0.0.9/mesh/macro/__init__.py
+-rw-r--r--   0        0        0     4161 2023-03-24 13:43:43.361003 daas-0.0.9/mesh/macro/ark.py
+-rw-r--r--   0        0        0     2393 2023-03-24 13:43:43.386022 daas-0.0.9/mesh/macro/binding.py
+-rw-r--r--   0        0        0      963 2024-01-23 10:59:10.865373 daas-0.0.9/mesh/macro/cause.py
+-rw-r--r--   0        0        0     4037 2024-01-23 10:54:05.961839 daas-0.0.9/mesh/macro/codec.py
+-rw-r--r--   0        0        0     4324 2023-03-24 13:43:43.358880 daas-0.0.9/mesh/macro/compatible.py
+-rw-r--r--   0        0        0     2160 2023-03-24 13:43:43.359311 daas-0.0.9/mesh/macro/index.py
+-rw-r--r--   0        0        0     2700 2024-01-11 02:42:53.874058 daas-0.0.9/mesh/macro/inspect.py
+-rw-r--r--   0        0        0      452 2023-03-24 13:43:43.362645 daas-0.0.9/mesh/macro/interface.py
+-rw-r--r--   0        0        0     3991 2023-03-24 13:43:43.384883 daas-0.0.9/mesh/macro/loader.py
+-rw-r--r--   0        0        0     4439 2023-04-23 06:49:01.214254 daas-0.0.9/mesh/macro/mpi.py
+-rw-r--r--   0        0        0     2145 2023-03-24 13:43:43.360119 daas-0.0.9/mesh/macro/mps.py
+-rw-r--r--   0        0        0     7983 2024-01-12 10:02:15.550458 daas-0.0.9/mesh/macro/proxy.py
+-rw-r--r--   0        0        0     1431 2023-03-24 13:43:43.386453 daas-0.0.9/mesh/macro/spi.py
+-rw-r--r--   0        0        0      247 2023-03-24 13:43:43.368145 daas-0.0.9/mesh/macro/types.py
+-rw-r--r--   0        0        0      220 2023-03-24 13:43:43.150120 daas-0.0.9/mesh/metrics/__init__.py
+-rw-r--r--   0        0        0     6062 2023-03-24 13:43:43.149511 daas-0.0.9/mesh/metrics/collector.py
+-rw-r--r--   0        0        0     2706 2023-03-24 13:43:43.153226 daas-0.0.9/mesh/metrics/scheduler.py
+-rw-r--r--   0        0        0     1279 2024-01-11 09:38:04.654688 daas-0.0.9/mesh/mpc/__init__.py
+-rw-r--r--   0        0        0     6762 2023-07-18 05:20:18.792244 daas-0.0.9/mesh/mpc/compiler.py
+-rw-r--r--   0        0        0     1191 2024-01-10 12:26:59.216920 daas-0.0.9/mesh/mpc/consumer.py
+-rw-r--r--   0        0        0     2173 2024-01-15 08:03:15.776441 daas-0.0.9/mesh/mpc/consumer_filter.py
+-rw-r--r--   0        0        0     1854 2024-01-15 06:38:37.320066 daas-0.0.9/mesh/mpc/digest.py
+-rw-r--r--   0        0        0     1734 2023-03-24 13:43:43.400089 daas-0.0.9/mesh/mpc/eden.py
+-rw-r--r--   0        0        0     1451 2024-01-11 09:04:44.328966 daas-0.0.9/mesh/mpc/filter.py
+-rw-r--r--   0        0        0     3345 2024-01-10 12:19:22.428000 daas-0.0.9/mesh/mpc/generic.py
+-rw-r--r--   0        0        0      991 2024-01-11 03:38:54.655090 daas-0.0.9/mesh/mpc/inspector.py
+-rw-r--r--   0        0        0     3306 2024-01-11 09:06:07.835479 daas-0.0.9/mesh/mpc/invoker.py
+-rw-r--r--   0        0        0      830 2024-01-15 08:03:26.787672 daas-0.0.9/mesh/mpc/isolate_filter.py
+-rw-r--r--   0        0        0    15580 2024-01-12 10:08:41.853533 daas-0.0.9/mesh/mpc/mesh_eden.py
+-rw-r--r--   0        0        0      612 2024-01-12 10:11:33.381101 daas-0.0.9/mesh/mpc/provider.py
+-rw-r--r--   0        0        0     1690 2024-01-15 08:02:58.718004 daas-0.0.9/mesh/mpc/provider_filter.py
+-rw-r--r--   0        0        0     6524 2024-01-15 08:37:18.729447 daas-0.0.9/mesh/mpc/reference.py
+-rw-r--r--   0        0        0     1256 2024-01-15 08:02:49.995226 daas-0.0.9/mesh/mpc/robust_filter.py
+-rw-r--r--   0        0        0     1414 2024-01-11 03:38:28.002539 daas-0.0.9/mesh/mpc/service.py
+-rw-r--r--   0        0        0     1152 2023-07-18 05:19:51.937010 daas-0.0.9/mesh/mpc/service_proxy.py
+-rw-r--r--   0        0        0     4384 2024-01-15 08:37:18.707112 daas-0.0.9/mesh/mpc/stream.py
+-rw-r--r--   0        0        0     3849 2024-01-15 08:37:18.715373 daas-0.0.9/mesh/mpc/transporter.py
+-rw-r--r--   0        0        0     6244 2024-01-10 07:29:19.207963 daas-0.0.9/mesh/mpc/urn.py
+-rw-r--r--   0        0        0     1846 2023-03-24 13:43:43.177695 daas-0.0.9/mesh/prsim/__init__.py
+-rw-r--r--   0        0        0     1620 2024-01-11 08:25:41.113444 daas-0.0.9/mesh/prsim/builtin.py
+-rw-r--r--   0        0        0     2645 2024-01-11 08:27:09.391977 daas-0.0.9/mesh/prsim/cache.py
+-rw-r--r--   0        0        0      678 2024-01-11 08:27:25.223040 daas-0.0.9/mesh/prsim/cluster.py
+-rw-r--r--   0        0        0     1300 2024-01-11 08:28:16.958879 daas-0.0.9/mesh/prsim/commerce.py
+-rw-r--r--   0        0        0     7476 2024-01-25 07:40:11.576505 daas-0.0.9/mesh/prsim/context.py
+-rw-r--r--   0        0        0     1620 2024-01-11 08:28:38.235421 daas-0.0.9/mesh/prsim/cryptor.py
+-rw-r--r--   0        0        0     1349 2024-01-11 08:28:59.500384 daas-0.0.9/mesh/prsim/datahouse.py
+-rw-r--r--   0        0        0      950 2024-01-11 08:29:35.004476 daas-0.0.9/mesh/prsim/dispatcher.py
+-rw-r--r--   0        0        0      899 2024-01-11 08:29:48.933700 daas-0.0.9/mesh/prsim/endpoint.py
+-rw-r--r--   0        0        0     1261 2024-01-11 08:30:06.673680 daas-0.0.9/mesh/prsim/evaluator.py
+-rw-r--r--   0        0        0      855 2024-01-11 08:30:21.092401 daas-0.0.9/mesh/prsim/graphics.py
+-rw-r--r--   0        0        0      736 2024-01-11 08:30:41.978620 daas-0.0.9/mesh/prsim/hodor.py
+-rw-r--r--   0        0        0      778 2024-01-11 08:30:53.470319 daas-0.0.9/mesh/prsim/iostream.py
+-rw-r--r--   0        0        0     1384 2024-01-11 08:31:27.233986 daas-0.0.9/mesh/prsim/kv.py
+-rw-r--r--   0        0        0     1270 2024-01-11 08:31:56.821975 daas-0.0.9/mesh/prsim/licenser.py
+-rw-r--r--   0        0        0     1122 2024-01-11 08:32:23.235449 daas-0.0.9/mesh/prsim/locker.py
+-rw-r--r--   0        0        0     3916 2024-01-11 08:32:38.204019 daas-0.0.9/mesh/prsim/network.py
+-rw-r--r--   0        0        0     2544 2024-01-11 09:37:04.803296 daas-0.0.9/mesh/prsim/publisher.py
+-rw-r--r--   0        0        0     1315 2024-01-11 08:33:22.873548 daas-0.0.9/mesh/prsim/registry.py
+-rw-r--r--   0        0        0     2853 2023-04-23 06:51:56.399623 daas-0.0.9/mesh/prsim/routable.py
+-rw-r--r--   0        0        0      876 2024-01-12 10:08:12.301629 daas-0.0.9/mesh/prsim/runtime_hook.py
+-rw-r--r--   0        0        0     2347 2024-01-11 08:33:40.253814 daas-0.0.9/mesh/prsim/scheduler.py
+-rw-r--r--   0        0        0      850 2024-01-11 08:33:54.591408 daas-0.0.9/mesh/prsim/sequence.py
+-rw-r--r--   0        0        0      594 2024-01-11 08:34:08.455647 daas-0.0.9/mesh/prsim/subscriber.py
+-rw-r--r--   0        0        0      714 2024-01-11 08:34:16.399695 daas-0.0.9/mesh/prsim/tokenizer.py
+-rw-r--r--   0        0        0     2965 2024-01-11 08:35:22.121023 daas-0.0.9/mesh/prsim/transport.py
+-rw-r--r--   0        0        0      338 2023-03-24 13:43:43.313535 daas-0.0.9/mesh/runtime/__init__.py
+-rw-r--r--   0        0        0      747 2023-03-24 13:43:43.317960 daas-0.0.9/mesh/runtime/container.py
+-rw-r--r--   0        0        0     1554 2023-03-24 13:43:43.319630 daas-0.0.9/mesh/runtime/context.py
+-rw-r--r--   0        0        0      585 2023-03-24 13:43:43.321107 daas-0.0.9/mesh/runtime/mesh_processor.py
+-rw-r--r--   0        0        0      222 2023-03-24 13:43:43.326527 daas-0.0.9/mesh/schema/__init__.py
+-rw-r--r--   0        0        0     1316 2023-03-24 13:43:43.344757 daas-0.0.9/mesh/system/__init__.py
+-rw-r--r--   0        0        0     2195 2024-01-11 08:35:53.021769 daas-0.0.9/mesh/system/mesh_builtin.py
+-rw-r--r--   0        0        0      931 2024-01-11 08:37:08.434631 daas-0.0.9/mesh/system/mesh_cache.py
+-rw-r--r--   0        0        0      558 2024-01-11 08:27:46.467327 daas-0.0.9/mesh/system/mesh_cluster.py
+-rw-r--r--   0        0        0      945 2024-01-11 08:37:56.749255 daas-0.0.9/mesh/system/mesh_datahouse.py
+-rw-r--r--   0        0        0      531 2024-01-11 08:38:11.075150 daas-0.0.9/mesh/system/mesh_dispatcher.py
+-rw-r--r--   0        0        0      427 2024-01-11 08:38:29.318977 daas-0.0.9/mesh/system/mesh_endpoint.py
+-rw-r--r--   0        0        0      921 2024-01-11 08:38:58.173775 daas-0.0.9/mesh/system/mesh_evaluator.py
+-rw-r--r--   0        0        0      474 2024-01-11 08:39:10.135306 daas-0.0.9/mesh/system/mesh_hodor.py
+-rw-r--r--   0        0        0      782 2024-01-11 08:39:37.865970 daas-0.0.9/mesh/system/mesh_locker.py
+-rw-r--r--   0        0        0     2888 2024-01-15 08:37:18.723444 daas-0.0.9/mesh/system/mesh_network.py
+-rw-r--r--   0        0        0      664 2024-01-11 08:41:33.613880 daas-0.0.9/mesh/system/mesh_publisher.py
+-rw-r--r--   0        0        0      898 2024-01-11 08:42:02.052058 daas-0.0.9/mesh/system/mesh_registry.py
+-rw-r--r--   0        0        0      495 2024-01-15 03:43:33.934403 daas-0.0.9/mesh/system/mesh_runtime_hook.py
+-rw-r--r--   0        0        0     1292 2024-01-11 08:43:10.290323 daas-0.0.9/mesh/system/mesh_scheduler.py
+-rw-r--r--   0        0        0     6224 2024-01-26 04:30:18.460756 daas-0.0.9/mesh/system/mesh_transport.py
+-rw-r--r--   0        0        0     2623 2023-03-24 13:43:43.223132 daas-0.0.9/mesh/test/__init__.py
+-rw-r--r--   0        0        0      157 2023-03-24 13:43:43.219724 daas-0.0.9/mesh/test/boost/__init__.py
+-rw-r--r--   0        0        0     8605 2023-03-24 13:43:43.220466 daas-0.0.9/mesh/test/boost/disruptor_test.py
+-rw-r--r--   0        0        0     7532 2023-03-24 13:43:43.218726 daas-0.0.9/mesh/test/boost/ringbuffer_perf_test.py
+-rw-r--r--   0        0        0    26327 2023-03-24 13:43:43.217943 daas-0.0.9/mesh/test/boost/ringbuffer_test.py
+-rw-r--r--   0        0        0      157 2023-03-24 13:43:43.222452 daas-0.0.9/mesh/test/codec/__init__.py
+-rw-r--r--   0        0        0     1571 2024-01-23 10:56:56.946283 daas-0.0.9/mesh/test/codec/codec_test.py
+-rw-r--r--   0        0        0      157 2023-03-24 13:43:43.216670 daas-0.0.9/mesh/test/grpx/__init__.py
+-rw-r--r--   0        0        0      701 2023-03-24 13:43:43.215844 daas-0.0.9/mesh/test/grpx/grpc_test.py
+-rw-r--r--   0        0        0      157 2023-03-24 13:43:43.236089 daas-0.0.9/mesh/test/ioc/__init__.py
+-rw-r--r--   0        0        0      506 2023-03-24 13:43:43.235345 daas-0.0.9/mesh/test/ioc/container_test.py
+-rw-r--r--   0        0        0      161 2024-01-10 04:11:17.562723 daas-0.0.9/mesh/test/load/__init__.py
+-rw-r--r--   0        0        0      595 2024-01-15 02:41:07.280763 daas-0.0.9/mesh/test/load/provider.py
+-rw-r--r--   0        0        0      158 2023-03-24 13:43:43.228000 daas-0.0.9/mesh/test/macro/__init__.py
+-rw-r--r--   0        0        0     1954 2023-03-24 13:43:43.227335 daas-0.0.9/mesh/test/macro/macro_test.py
+-rw-r--r--   0        0        0      752 2023-03-24 13:43:43.228742 daas-0.0.9/mesh/test/macro/proxy_test.py
+-rw-r--r--   0        0        0      157 2023-03-24 13:43:43.207945 daas-0.0.9/mesh/test/metrics/__init__.py
+-rw-r--r--   0        0        0      369 2023-03-24 13:43:43.208469 daas-0.0.9/mesh/test/metrics/collector_test.py
+-rw-r--r--   0        0        0      157 2023-03-24 13:43:43.229658 daas-0.0.9/mesh/test/mpc/__init__.py
+-rw-r--r--   0        0        0      887 2023-03-24 13:43:43.233327 daas-0.0.9/mesh/test/mpc/compile_test.py
+-rw-r--r--   0        0        0     1338 2024-01-15 08:37:18.742836 daas-0.0.9/mesh/test/mpc/mpc_test.py
+-rw-r--r--   0        0        0      408 2023-03-24 13:43:43.232010 daas-0.0.9/mesh/test/mpc/service_loader_test.py
+-rw-r--r--   0        0        0      157 2023-03-24 13:43:43.209353 daas-0.0.9/mesh/test/prsim/__init__.py
+-rw-r--r--   0        0        0      591 2023-03-24 13:43:43.214304 daas-0.0.9/mesh/test/prsim/network_test.py
+-rw-r--r--   0        0        0      155 2023-08-09 00:39:26.383673 daas-0.0.9/mesh/test/system/__init__.py
+-rw-r--r--   0        0        0     2306 2024-01-26 04:28:43.223744 daas-0.0.9/mesh/test/system/transport_test.py
+-rw-r--r--   0        0        0      157 2023-03-24 13:43:43.237557 daas-0.0.9/mesh/test/tool/__init__.py
+-rw-r--r--   0        0        0     1006 2023-03-24 13:43:43.238330 daas-0.0.9/mesh/test/tool/tool_test.py
+-rw-r--r--   0        0        0     5089 2024-01-26 04:19:01.193684 daas-0.0.9/mesh/tool/__init__.py
+-rw-r--r--   0        0        0     2939 2023-03-24 13:43:43.485869 daas-0.0.9/mesh/tool/snowflake.py
+-rw-r--r--   0        0        0      594 2023-03-24 13:43:43.487133 daas-0.0.9/mesh/tool/versions.py
+-rw-r--r--   0        0        0     1179 2024-03-07 03:09:39.411226 daas-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4934 1970-01-01 00:00:00.000000 daas-0.0.9/PKG-INFO
```

### Comparing `daas-0.0.8/README.md` & `daas-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/__init__.py` & `daas-0.0.9/mesh/__init__.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/asm/__init__.py` & `daas-0.0.9/mesh/asm/__init__.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/boost/__init__.py` & `daas-0.0.9/mesh/boost/__init__.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/boost/contab.py` & `daas-0.0.9/mesh/boost/contab.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/boost/disruptor.py` & `daas-0.0.9/mesh/boost/disruptor.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/boost/mooter.py` & `daas-0.0.9/mesh/boost/mooter.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/boost/remote.py` & `daas-0.0.9/mesh/boost/remote.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/boost/ringbuffer.py` & `daas-0.0.9/mesh/boost/ringbuffer.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/boost/runhook.py` & `daas-0.0.9/mesh/boost/runhook.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/boost/scheduler.py` & `daas-0.0.9/mesh/boost/scheduler.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/cause/__init__.py` & `daas-0.0.9/mesh/cause/__init__.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/cause/errors.py` & `daas-0.0.9/mesh/cause/errors.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/cause/status.py` & `daas-0.0.9/mesh/cause/status.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/codec/__init__.py` & `daas-0.0.9/mesh/codec/__init__.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/codec/codec.py` & `daas-0.0.9/mesh/codec/codec.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/codec/former.py` & `daas-0.0.9/mesh/codec/former.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/codec/jsons.py` & `daas-0.0.9/mesh/codec/jsons.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/codec/tools.py` & `daas-0.0.9/mesh/codec/tools.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/context/context.py` & `daas-0.0.9/mesh/context/context.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/context/mesh.py` & `daas-0.0.9/mesh/context/mesh.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/environ/cache.py` & `daas-0.0.9/mesh/environ/cache.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/environ/environ.py` & `daas-0.0.9/mesh/environ/environ.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,14 +113,15 @@
     __mesh_mode_keys = ['MESH_MODE', 'mesh.mode', 'mesh_mode', 'mesh-mode']
     __mesh_name_keys = ['MESH_NAME', 'mesh.name', 'mesh_name', 'mesh-name']
     __mesh_direct_keys = ['MESH_DIRECT', 'mesh.direct', 'mesh_direct', 'mesh-direct']
     __mesh_subset_keys = ['MESH_SUBSET', 'mesh.subset', 'mesh_subset', 'mesh-subset']
     __mesh_min_channels = ['MESH_GRPC_CHANNEL_RPC_MIN', 'mesh.grpc.channel.rpc.min', 'mesh_grpc_channel_rpc_min']
     __mesh_max_channels = ['MESH_GRPC_CHANNEL_RPC_MAX', 'mesh.grpc.channel.rpc.max', 'mesh_grpc_channel_rpc_max']
     __mesh_proc_keys = ['MESH_PROC', 'mesh.proc', 'mesh_proc', 'MESH.PROC']
+    __mesh_packet_size = ['mesh.packet.size', 'mesh_packet_size', 'MESH_PACKET_SIZE']
 
     @staticmethod
     def get_default_mesh_port() -> int:
         return DEFAULT_MESH_PORT
 
     def get_property(self, dft: str, keys: List[str]) -> str:
         if not keys:
@@ -139,14 +140,15 @@
         parser.add_argument("--mesh.runtime", type=str, default='', required=False)
         parser.add_argument("--mesh.enable", type=str, default='', required=False)
         parser.add_argument("--mesh.name", type=str, default='', required=False)
         parser.add_argument("--mesh.direct", type=str, default='', required=False)
         parser.add_argument("--mesh.grpc.channel.rpc.min", type=int, default=f'{os.cpu_count() * 2}', required=False)
         parser.add_argument("--mesh.grpc.channel.rpc.max", type=int, default=f'{os.cpu_count() * 2}', required=False)
         parser.add_argument("--mesh.procs", type=int, default=-1, required=False)
+        parser.add_argument("--mesh.packet.size", type=int, default=1 << 26, required=False)
         args, _ = parser.parse_known_args()
         return vars(args)
 
     @Cache
     def get_mesh_address(self) -> Addrs:
         return Addrs(self.get_property('127.0.0.1', self.__mesh_address_keys))
 
@@ -182,14 +184,18 @@
         return int(self.get_property('3', self.__mesh_min_channels))
 
     @Cache
     def get_proc(self) -> int:
         return int(self.get_property('-1', self.__mesh_proc_keys))
 
     @Cache
+    def get_packet_size(self) -> int:
+        return int(self.get_property(f"{1 << 26}", self.__mesh_packet_size))
+
+    @Cache
     def get_hostname(self) -> str:
         return socket.gethostname()
 
     @Cache
     def get_ip(self) -> str:
         s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
         s.settimeout(0)
```

### Comparing `daas-0.0.8/mesh/grpx/__init__.py` & `daas-0.0.9/mesh/grpx/__init__.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/grpx/bindservice.py` & `daas-0.0.9/mesh/grpx/bindservice.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/grpx/channels.py` & `daas-0.0.9/mesh/grpx/channels.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/grpx/consumer.py` & `daas-0.0.9/mesh/grpx/consumer.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/grpx/interceptor.py` & `daas-0.0.9/mesh/grpx/interceptor.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/grpx/provider.py` & `daas-0.0.9/mesh/grpx/provider.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/grpx/transport.py` & `daas-0.0.9/mesh/grpx/transport.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/http/consumer.py` & `daas-0.0.9/mesh/http/consumer.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/http/provider.py` & `daas-0.0.9/mesh/http/provider.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/ioc/paas_processor.py` & `daas-0.0.9/mesh/ioc/paas_processor.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/kinds/__init__.py` & `daas-0.0.9/mesh/kinds/__init__.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/kinds/commerce.py` & `daas-0.0.9/mesh/kinds/commerce.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/kinds/document.py` & `daas-0.0.9/mesh/kinds/document.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/kinds/entity.py` & `daas-0.0.9/mesh/kinds/entity.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/kinds/environ.py` & `daas-0.0.9/mesh/kinds/environ.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/kinds/event.py` & `daas-0.0.9/mesh/kinds/event.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/kinds/license.py` & `daas-0.0.9/mesh/kinds/license.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/kinds/location.py` & `daas-0.0.9/mesh/kinds/location.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/kinds/meshflag.py` & `daas-0.0.9/mesh/kinds/meshflag.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/kinds/page.py` & `daas-0.0.9/mesh/kinds/page.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/kinds/paging.py` & `daas-0.0.9/mesh/kinds/paging.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/kinds/reference.py` & `daas-0.0.9/mesh/kinds/reference.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/kinds/registration.py` & `daas-0.0.9/mesh/kinds/registration.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/kinds/route.py` & `daas-0.0.9/mesh/kinds/route.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/kinds/script.py` & `daas-0.0.9/mesh/kinds/script.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/kinds/service.py` & `daas-0.0.9/mesh/kinds/service.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/kinds/versions.py` & `daas-0.0.9/mesh/kinds/versions.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/log/__init__.py` & `daas-0.0.9/mesh/log/__init__.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/log/nop.py` & `daas-0.0.9/mesh/log/nop.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/log/types.py` & `daas-0.0.9/mesh/log/types.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/macro/__init__.py` & `daas-0.0.9/mesh/macro/__init__.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/macro/ark.py` & `daas-0.0.9/mesh/macro/ark.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/macro/binding.py` & `daas-0.0.9/mesh/macro/binding.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/macro/cause.py` & `daas-0.0.9/mesh/macro/cause.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 #
 # Copyright (c) 2000, 2099, ducesoft and/or its affiliates. All rights reserved.
 # DUCESOFT PROPRIETARY/CONFIDENTIAL. Use is subject to license terms.
 #
 #
 
 
+import traceback
+
+from mesh.cause import MeshException
+from mesh.macro.codec import serializable
 from mesh.macro.index import index
 
 
+@serializable
 class Cause:
 
     @index(0)
     def name(self) -> str:
         return ''
 
     @index(5)
@@ -24,12 +29,16 @@
 
     @index(15)
     def buff(self) -> bytes:
         return b''
 
     @staticmethod
     def of(e: BaseException) -> "Cause":
-        return Cause()
+        cause = Cause()
+        cause.name = e.__class__.__name__ if e.__class__ else str(e)
+        cause.pos = '0'
+        cause.text = traceback.format_exc()
+        return cause
 
     @staticmethod
     def of_cause(code: str, message: str, cause: "Cause") -> BaseException:
-        raise BaseException("")
+        raise MeshException(f"{code},{message},{cause.text}")
```

### Comparing `daas-0.0.8/mesh/macro/codec.py` & `daas-0.0.9/mesh/macro/codec.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 from mesh.macro.ark import T
 from mesh.macro.compatible import Compatible
 
 
 class Serializable(object):
     """ Serializable """
+    BASIC_TYPES = (int, float, str, bool, list, tuple, dict, set, type(None))
 
     def __init__(self, cls=None):
         self.cls = cls
         annotations = getattr(cls, '__annotations__') if hasattr(cls, '__annotations__') else {}
         for attr in inspect.classify_class_attrs(cls):
             if not attr.name or attr.name.startswith("_") or not attr.object or not hasattr(attr.object, 'kind'):
                 continue
@@ -26,15 +27,18 @@
         setattr(cls, 'encode', self.serialize)
         setattr(cls, '__annotations__', annotations)
 
     def serialize(self, value: Any) -> Any:
         if isinstance(value, bytes):
             return base64.b64encode(value).decode("utf-8")
 
-        if isinstance(value, (int, float)):
+        if isinstance(value, Serializable.BASIC_TYPES):
+            return value
+
+        if not hasattr(value, '__dict__'):
             return value
 
         return vars(value)
 
     def deserialize(self, instance: Any, **kwargs) -> Any:
         if kwargs is None:
             return instance
```

### Comparing `daas-0.0.8/mesh/macro/compatible.py` & `daas-0.0.9/mesh/macro/compatible.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/macro/index.py` & `daas-0.0.9/mesh/macro/index.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/macro/inspect.py` & `daas-0.0.9/mesh/macro/inspect.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/macro/loader.py` & `daas-0.0.9/mesh/macro/loader.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/macro/mpi.py` & `daas-0.0.9/mesh/macro/mpi.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/macro/mps.py` & `daas-0.0.9/mesh/macro/mps.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/macro/proxy.py` & `daas-0.0.9/mesh/macro/proxy.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/macro/spi.py` & `daas-0.0.9/mesh/macro/spi.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/metrics/collector.py` & `daas-0.0.9/mesh/metrics/collector.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/metrics/scheduler.py` & `daas-0.0.9/mesh/metrics/scheduler.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/mpc/__init__.py` & `daas-0.0.9/mesh/mpc/__init__.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/mpc/compiler.py` & `daas-0.0.9/mesh/mpc/compiler.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/mpc/consumer.py` & `daas-0.0.9/mesh/mpc/consumer.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/mpc/consumer_filter.py` & `daas-0.0.9/mesh/mpc/consumer_filter.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/mpc/digest.py` & `daas-0.0.9/mesh/mpc/digest.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/mpc/eden.py` & `daas-0.0.9/mesh/mpc/eden.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/mpc/filter.py` & `daas-0.0.9/mesh/mpc/filter.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/mpc/generic.py` & `daas-0.0.9/mesh/mpc/generic.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/mpc/inspector.py` & `daas-0.0.9/mesh/mpc/inspector.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/mpc/invoker.py` & `daas-0.0.9/mesh/mpc/invoker.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/mpc/isolate_filter.py` & `daas-0.0.9/mesh/mpc/isolate_filter.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/mpc/mesh_eden.py` & `daas-0.0.9/mesh/mpc/mesh_eden.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/mpc/provider.py` & `daas-0.0.9/mesh/mpc/provider.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/mpc/provider_filter.py` & `daas-0.0.9/mesh/mpc/provider_filter.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/mpc/reference.py` & `daas-0.0.9/mesh/mpc/reference.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/mpc/robust_filter.py` & `daas-0.0.9/mesh/mpc/robust_filter.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/mpc/service.py` & `daas-0.0.9/mesh/mpc/service.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/mpc/service_proxy.py` & `daas-0.0.9/mesh/mpc/service_proxy.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/mpc/stream.py` & `daas-0.0.9/mesh/mpc/stream.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/mpc/transporter.py` & `daas-0.0.9/mesh/mpc/transporter.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/mpc/urn.py` & `daas-0.0.9/mesh/mpc/urn.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/prsim/__init__.py` & `daas-0.0.9/mesh/prsim/__init__.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/prsim/builtin.py` & `daas-0.0.9/mesh/prsim/builtin.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/prsim/cache.py` & `daas-0.0.9/mesh/prsim/cache.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/prsim/cluster.py` & `daas-0.0.9/mesh/prsim/cluster.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/prsim/commerce.py` & `daas-0.0.9/mesh/prsim/commerce.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/prsim/context.py` & `daas-0.0.9/mesh/prsim/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -129,16 +129,16 @@
     MESH_OUTGOING_PROXY = "mesh-outgoing-proxy"
     MESH_SUBSET = "mesh-subset"
     # PTP
     MESH_VERSION = "mesh-version"
     MESH_TECH_PROVIDER_CODE = "mesh-tech-provider-code"
     MESH_TRACE_ID = "mesh-trace-id"
     MESH_TOKEN = "mesh-token"
-    MESH_FROM_NODE_ID = "mesh-from-node-id"
-    MESH_FROM_INST_ID = "mesh-from-inst-id"
+    MESH_FROM_NODE_ID = "mesh-source-node-id"
+    MESH_FROM_INST_ID = "mesh-source-inst-id"
     MESH_TARGET_NODE_ID = "mesh-target-node-id"
     MESH_TARGET_INST_ID = "mesh-target-inst-id"
     MESH_SESSION_ID = "mesh-session-id"
 
     def key(self) -> str:
         return self.value
```

### Comparing `daas-0.0.8/mesh/prsim/cryptor.py` & `daas-0.0.9/mesh/prsim/cryptor.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/prsim/datahouse.py` & `daas-0.0.9/mesh/prsim/datahouse.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/prsim/dispatcher.py` & `daas-0.0.9/mesh/prsim/dispatcher.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/prsim/endpoint.py` & `daas-0.0.9/mesh/prsim/endpoint.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/prsim/evaluator.py` & `daas-0.0.9/mesh/prsim/evaluator.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/prsim/graphics.py` & `daas-0.0.9/mesh/prsim/graphics.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/prsim/hodor.py` & `daas-0.0.9/mesh/prsim/hodor.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/prsim/iostream.py` & `daas-0.0.9/mesh/prsim/iostream.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/prsim/kv.py` & `daas-0.0.9/mesh/prsim/kv.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/prsim/licenser.py` & `daas-0.0.9/mesh/prsim/licenser.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/prsim/locker.py` & `daas-0.0.9/mesh/prsim/locker.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/prsim/network.py` & `daas-0.0.9/mesh/prsim/network.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/prsim/publisher.py` & `daas-0.0.9/mesh/prsim/publisher.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/prsim/registry.py` & `daas-0.0.9/mesh/prsim/registry.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/prsim/routable.py` & `daas-0.0.9/mesh/prsim/routable.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/prsim/runtime_hook.py` & `daas-0.0.9/mesh/prsim/runtime_hook.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/prsim/scheduler.py` & `daas-0.0.9/mesh/prsim/scheduler.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/prsim/sequence.py` & `daas-0.0.9/mesh/prsim/sequence.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/prsim/subscriber.py` & `daas-0.0.9/mesh/prsim/subscriber.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/prsim/tokenizer.py` & `daas-0.0.9/mesh/prsim/tokenizer.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/prsim/transport.py` & `daas-0.0.9/mesh/prsim/transport.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/runtime/container.py` & `daas-0.0.9/mesh/runtime/container.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/runtime/context.py` & `daas-0.0.9/mesh/runtime/context.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/runtime/mesh_processor.py` & `daas-0.0.9/mesh/runtime/mesh_processor.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/system/__init__.py` & `daas-0.0.9/mesh/system/__init__.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/system/mesh_builtin.py` & `daas-0.0.9/mesh/system/mesh_builtin.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/system/mesh_cache.py` & `daas-0.0.9/mesh/system/mesh_cache.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/system/mesh_cluster.py` & `daas-0.0.9/mesh/system/mesh_cluster.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/system/mesh_datahouse.py` & `daas-0.0.9/mesh/system/mesh_datahouse.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/system/mesh_dispatcher.py` & `daas-0.0.9/mesh/system/mesh_dispatcher.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/system/mesh_evaluator.py` & `daas-0.0.9/mesh/system/mesh_evaluator.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/system/mesh_locker.py` & `daas-0.0.9/mesh/system/mesh_locker.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/system/mesh_network.py` & `daas-0.0.9/mesh/system/mesh_network.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/system/mesh_publisher.py` & `daas-0.0.9/mesh/system/mesh_publisher.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/system/mesh_registry.py` & `daas-0.0.9/mesh/system/mesh_registry.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/system/mesh_scheduler.py` & `daas-0.0.9/mesh/system/mesh_scheduler.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/system/mesh_transport.py` & `daas-0.0.9/mesh/system/mesh_transport.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #
 # Copyright (c) 2000, 2099, ducesoft and/or its affiliates. All rights reserved.
 # DUCESOFT PROPRIETARY/CONFIDENTIAL. Use is subject to license terms.
 #
 #
-
+import math
 from typing import Dict, Any, Callable, Coroutine
 
 import mesh.log as log
 import mesh.tool as tool
 from mesh.kinds import Principal
 from mesh.macro import spi
 from mesh.mpc import ServiceProxy, Mesh
@@ -44,15 +44,16 @@
         self.sessions.clear()
 
     async def roundtrip(self, payload: bytes, metadata: Dict[str, str]) -> bytes:
         """ bid """
         pass
 
     def finalize(self, session_key: str):
-        self.sessions.__delitem__(session_key)
+        if self.sessions.__contains__(session_key):
+            self.sessions.__delitem__(session_key)
 
     @staticmethod
     def session_key(session_id: str, metadata: Dict[str, str]) -> str:
         target_node_id = Metadata.MESH_TARGET_NODE_ID.get(metadata)
         target_inst_id = Metadata.MESH_TARGET_INST_ID.get(metadata)
         return f"{session_id}.{target_node_id}.{target_inst_id}"
 
@@ -63,15 +64,15 @@
     def __init__(self, session_id: str, metadata: Dict[str, str], attachments: Dict[str, str], address: str,
                  principal: Principal, finalizer: Callable):
         self.session_id = session_id
         self.metadata = metadata
         self.attachments = attachments
         self.address = address
         self.principal = principal
-        self.session = ServiceProxy.default_proxy(Session)
+        self.session = SplitSession(ServiceProxy.default_proxy(Session))
         self.finalizer = finalizer
 
     async def with_context(self, fn: Coroutine, remote: bool, timeout: int) -> Any:
         return await Mesh.context_safe(self.context_safe(fn, remote, timeout))
 
     async def context_safe(self, fn: Any, remote: bool, timeout: int) -> Any:
         if self.attachments:
@@ -114,7 +115,46 @@
 
     async def push(self, payload: bytes, metadata: Dict[str, str], topic: str = ""):
         return await self.with_context(self.session.push(payload, metadata, topic), True, 0)
 
     async def release(self, timeout: int, topic: str = ""):
         self.finalizer()
         return await self.with_context(self.session.release(timeout, topic), False, timeout)
+
+
+class SplitSession(Session):
+
+    def __init__(self, session: Session):
+        self.session = session
+
+    async def peek(self, topic: str = "") -> bytes:
+        buff = bytes()
+        packet_size_bytes = await self.session.peek(self.split_key(topic, 0))
+        packet_size = packet_size_bytes.decode()
+        if "" == packet_size:
+            return buff
+        for idx in range(int(packet_size)):
+            buff += await self.session.peek(self.split_key(topic, idx + 1))
+        return buff
+
+    async def pop(self, timeout: int, topic: str = "") -> bytes:
+        packet_size_bytes = await self.session.pop(timeout, self.split_key(topic, 0))
+        packet_size = int(packet_size_bytes.decode())
+        buff = bytes()
+        for idx in range(packet_size):
+            buff += await self.session.pop(timeout, self.split_key(topic, idx + 1))
+        return buff
+
+    async def push(self, payload: bytes, metadata: Dict[str, str], topic: str = ""):
+        packet_length = tool.get_packet_size()
+        packet_size = math.ceil(payload.__len__() / packet_length)
+        await self.session.push(f"{packet_size}".encode(), metadata, self.split_key(topic, 0))
+        for idx in range(packet_size):
+            buff = payload[packet_length * idx:min(packet_length * (idx + 1), payload.__len__())]
+            await self.session.push(buff, metadata, self.split_key(topic, idx + 1))
+
+    async def release(self, timeout: int, topic: str = ""):
+        return await self.session.release(timeout, topic)
+
+    @staticmethod
+    def split_key(topic: str, idx: int, ) -> str:
+        return f"{topic}-mesh-split-{idx}"
```

### Comparing `daas-0.0.8/mesh/test/__init__.py` & `daas-0.0.9/mesh/test/__init__.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/test/boost/disruptor_test.py` & `daas-0.0.9/mesh/test/boost/disruptor_test.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/test/boost/ringbuffer_perf_test.py` & `daas-0.0.9/mesh/test/boost/ringbuffer_perf_test.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/test/boost/ringbuffer_test.py` & `daas-0.0.9/mesh/test/boost/ringbuffer_test.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/test/grpx/grpc_test.py` & `daas-0.0.9/mesh/test/grpx/grpc_test.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/test/load/provider.py` & `daas-0.0.9/mesh/test/load/provider.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/test/macro/macro_test.py` & `daas-0.0.9/mesh/test/macro/macro_test.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/test/macro/proxy_test.py` & `daas-0.0.9/mesh/test/macro/proxy_test.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/test/mpc/compile_test.py` & `daas-0.0.9/mesh/test/mpc/compile_test.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/test/mpc/mpc_test.py` & `daas-0.0.9/mesh/test/mpc/mpc_test.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/test/prsim/network_test.py` & `daas-0.0.9/mesh/test/prsim/network_test.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/test/tool/tool_test.py` & `daas-0.0.9/mesh/test/tool/tool_test.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/tool/__init__.py` & `daas-0.0.9/mesh/tool/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,14 +81,18 @@
     return System.environ().get_min_channels()
 
 
 def get_proc() -> int:
     return System.environ().get_proc()
 
 
+def get_packet_size() -> int:
+    return System.environ().get_packet_size()
+
+
 def required(*args: Any) -> bool:
     if not args:
         return False
 
     for arg in args:
         if arg is not None and "" != arg:
             continue
```

### Comparing `daas-0.0.8/mesh/tool/snowflake.py` & `daas-0.0.9/mesh/tool/snowflake.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/mesh/tool/versions.py` & `daas-0.0.9/mesh/tool/versions.py`

 * *Files identical despite different names*

### Comparing `daas-0.0.8/pyproject.toml` & `daas-0.0.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "daas"
-version = "0.0.8"
+version = "0.0.9"
 description = "A lightweight, distributed, relational network architecture for MPC."
 authors = ["coyzeng <coyzeng@gmail.com>"]
 maintainers = ["coyzeng <coyzeng@gmail.com>"]
 packages = [{ include = "mesh" }]
 license = "LICENSE"
 readme = "README.md"
 homepage = "https://github.com/jiumi/meio"
@@ -13,25 +13,24 @@
 keywords = ["servicemesh", "rpc", "codec", "cluster", "registry"]
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Natural Language :: English",
     "Development Status :: 5 - Production/Stable",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9"
 ]
 [tool.poetry.dependencies]
-python = "^3.7"
-protobuf = "^3.14.0"
-grpcio = "^1.43.0"
+python = "^3.8"
+protobuf = "^4.25.3"
+grpcio = "^1.62.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.0.1"
+pytest = "^8.0.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [[tool.poetry.source]]
 name = "aliyun"
```

### Comparing `daas-0.0.8/PKG-INFO` & `daas-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.1
 Name: daas
-Version: 0.0.8
+Version: 0.0.9
 Summary: A lightweight, distributed, relational network architecture for MPC.
 Home-page: https://github.com/jiumi/meio
 License: LICENSE
 Keywords: servicemesh,rpc,codec,cluster,registry
 Author: coyzeng
 Author-email: coyzeng@gmail.com
 Maintainer: coyzeng
 Maintainer-email: coyzeng@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: grpcio (>=1.43.0,<2.0.0)
-Requires-Dist: protobuf (>=3.14.0,<4.0.0)
+Requires-Dist: grpcio (>=1.62.0,<2.0.0)
+Requires-Dist: protobuf (>=4.25.3,<5.0.0)
 Project-URL: Documentation, https://github.com/jiumi/meio
 Project-URL: Repository, https://github.com/jiumi/meio
 Description-Content-Type: text/markdown
 
 # DaaS
 
 [![Build Status](https://travis-ci.org/ducesoft/babel.svg?branch=master)](https://travis-ci.org/ducesoft/babel)
```

