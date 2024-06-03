# Comparing `tmp/bbot-1.1.9.3376rc0.tar.gz` & `tmp/bbot-1.1.9.3387rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbot-1.1.9.3376rc0.tar", max compression
+gzip compressed data, was "bbot-1.1.9.3387rc0.tar", max compression
```

## Comparing `bbot-1.1.9.3376rc0.tar` & `bbot-1.1.9.3387rc0.tar`

### file list

```diff
@@ -1,346 +1,346 @@
--rw-r--r--   0        0        0    32473 2024-06-03 11:39:19.715033 bbot-1.1.9.3376rc0/LICENSE
--rw-r--r--   0        0        0    40272 2024-06-03 11:39:19.715033 bbot-1.1.9.3376rc0/README.md
--rw-r--r--   0        0        0      211 2024-06-03 11:39:37.691229 bbot-1.1.9.3376rc0/bbot/__init__.py
--rw-r--r--   0        0        0       25 2024-06-03 11:39:19.715033 bbot-1.1.9.3376rc0/bbot/agent/__init__.py
--rw-r--r--   0        0        0     7898 2024-06-03 11:39:19.715033 bbot-1.1.9.3376rc0/bbot/agent/agent.py
--rw-r--r--   0        0        0      450 2024-06-03 11:39:19.715033 bbot-1.1.9.3376rc0/bbot/agent/messages.py
--rwxr-xr-x   0        0        0    17601 2024-06-03 11:39:19.715033 bbot-1.1.9.3376rc0/bbot/cli.py
--rw-r--r--   0        0        0       59 2024-06-03 11:39:19.715033 bbot-1.1.9.3376rc0/bbot/core/__init__.py
--rw-r--r--   0        0        0     3588 2024-06-03 11:39:19.715033 bbot-1.1.9.3376rc0/bbot/core/configurator/__init__.py
--rw-r--r--   0        0        0     9843 2024-06-03 11:39:19.715033 bbot-1.1.9.3376rc0/bbot/core/configurator/args.py
--rw-r--r--   0        0        0     5182 2024-06-03 11:39:19.715033 bbot-1.1.9.3376rc0/bbot/core/configurator/environ.py
--rw-r--r--   0        0        0     1341 2024-06-03 11:39:19.715033 bbot-1.1.9.3376rc0/bbot/core/configurator/files.py
--rw-r--r--   0        0        0      617 2024-06-03 11:39:19.715033 bbot-1.1.9.3376rc0/bbot/core/errors.py
--rw-r--r--   0        0        0       91 2024-06-03 11:39:19.715033 bbot-1.1.9.3376rc0/bbot/core/event/__init__.py
--rw-r--r--   0        0        0    46323 2024-06-03 11:39:19.715033 bbot-1.1.9.3376rc0/bbot/core/event/base.py
--rw-r--r--   0        0        0     1656 2024-06-03 11:39:19.715033 bbot-1.1.9.3376rc0/bbot/core/event/helpers.py
--rw-r--r--   0        0        0     1232 2024-06-03 11:39:19.715033 bbot-1.1.9.3376rc0/bbot/core/flags.py
--rw-r--r--   0        0        0       86 2024-06-03 11:39:19.715033 bbot-1.1.9.3376rc0/bbot/core/helpers/__init__.py
--rw-r--r--   0        0        0     3583 2024-06-03 11:39:19.715033 bbot-1.1.9.3376rc0/bbot/core/helpers/async_helpers.py
--rw-r--r--   0        0        0     1537 2024-06-03 11:39:19.715033 bbot-1.1.9.3376rc0/bbot/core/helpers/cache.py
--rw-r--r--   0        0        0     4341 2024-06-03 11:39:19.715033 bbot-1.1.9.3376rc0/bbot/core/helpers/cloud.py
--rw-r--r--   0        0        0    11950 2024-06-03 11:39:19.715033 bbot-1.1.9.3376rc0/bbot/core/helpers/command.py
--rw-r--r--   0        0        0       37 2024-06-03 11:39:19.715033 bbot-1.1.9.3376rc0/bbot/core/helpers/depsinstaller/__init__.py
--rw-r--r--   0        0        0    14117 2024-06-03 11:39:19.715033 bbot-1.1.9.3376rc0/bbot/core/helpers/depsinstaller/installer.py
--rw-r--r--   0        0        0       87 2024-06-03 11:39:19.715033 bbot-1.1.9.3376rc0/bbot/core/helpers/depsinstaller/sudo_askpass.py
--rw-r--r--   0        0        0     9199 2024-06-03 11:39:19.715033 bbot-1.1.9.3376rc0/bbot/core/helpers/diff.py
--rw-r--r--   0        0        0    47786 2024-06-03 11:39:19.715033 bbot-1.1.9.3376rc0/bbot/core/helpers/dns.py
--rw-r--r--   0        0        0     5639 2024-06-03 11:39:19.715033 bbot-1.1.9.3376rc0/bbot/core/helpers/files.py
--rw-r--r--   0        0        0     6354 2024-06-03 11:39:19.715033 bbot-1.1.9.3376rc0/bbot/core/helpers/helper.py
--rw-r--r--   0        0        0    12632 2024-06-03 11:39:19.715033 bbot-1.1.9.3376rc0/bbot/core/helpers/interactsh.py
--rw-r--r--   0        0        0     1408 2024-06-03 11:39:19.715033 bbot-1.1.9.3376rc0/bbot/core/helpers/logger.py
--rw-r--r--   0        0        0    84110 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/core/helpers/misc.py
--rw-r--r--   0        0        0    22071 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/core/helpers/modules.py
--rw-r--r--   0        0        0    10041 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/core/helpers/names_generator.py
--rw-r--r--   0        0        0     2578 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/core/helpers/ntlm.py
--rw-r--r--   0        0        0     1990 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/core/helpers/ratelimiter.py
--rw-r--r--   0        0        0     4542 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/core/helpers/regexes.py
--rw-r--r--   0        0        0     5947 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/core/helpers/url.py
--rw-r--r--   0        0        0     8781 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/core/helpers/validators.py
--rw-r--r--   0        0        0    31938 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/core/helpers/web.py
--rw-r--r--   0        0        0    19801 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/core/helpers/wordcloud.py
--rw-r--r--   0        0        0      191 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/core/logger/__init__.py
--rw-r--r--   0        0        0     8118 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/core/logger/logger.py
--rw-r--r--   0        0        0     4158 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/defaults.yml
--rw-r--r--   0        0        0      396 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/modules/__init__.py
--rw-r--r--   0        0        0     2413 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/modules/ajaxpro.py
--rw-r--r--   0        0        0     1915 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/modules/anubisdb.py
--rw-r--r--   0        0        0     1463 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/modules/azure_realm.py
--rw-r--r--   0        0        0     4782 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/modules/azure_tenant.py
--rw-r--r--   0        0        0     4237 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/modules/baddns.py
--rw-r--r--   0        0        0     1332 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/modules/baddns_zone.py
--rw-r--r--   0        0        0     3634 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/modules/badsecrets.py
--rw-r--r--   0        0        0    59062 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/modules/base.py
--rw-r--r--   0        0        0     2446 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/modules/bevigil.py
--rw-r--r--   0        0        0     1398 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/modules/binaryedge.py
--rw-r--r--   0        0        0      746 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/modules/bucket_amazon.py
--rw-r--r--   0        0        0     1111 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/modules/bucket_azure.py
--rw-r--r--   0        0        0      866 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/modules/bucket_digitalocean.py
--rw-r--r--   0        0        0     1992 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/modules/bucket_file_enum.py
--rw-r--r--   0        0        0     1443 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/modules/bucket_firebase.py
--rw-r--r--   0        0        0     2631 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/modules/bucket_google.py
--rw-r--r--   0        0        0     5010 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/modules/builtwith.py
--rw-r--r--   0        0        0     6607 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/modules/bypass403.py
--rw-r--r--   0        0        0     1287 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/modules/c99.py
--rw-r--r--   0        0        0     3470 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/modules/censys.py
--rw-r--r--   0        0        0      889 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/modules/certspotter.py
--rw-r--r--   0        0        0     1621 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/modules/chaos.py
--rw-r--r--   0        0        0     1901 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/modules/code_repository.py
--rw-r--r--   0        0        0      826 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/modules/columbus.py
--rw-r--r--   0        0        0     3366 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/modules/credshed.py
--rw-r--r--   0        0        0      428 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/modules/crobat.py
--rw-r--r--   0        0        0     1321 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/modules/crt.py
--rw-r--r--   0        0        0     5407 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/modules/deadly/dastardly.py
--rw-r--r--   0        0        0    14132 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/modules/deadly/ffuf.py
--rw-r--r--   0        0        0    17351 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/modules/deadly/nuclei.py
--rw-r--r--   0        0        0     5293 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/modules/deadly/vhost.py
--rw-r--r--   0        0        0     4020 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/modules/dehashed.py
--rw-r--r--   0        0        0     1021 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/modules/digitorus.py
--rw-r--r--   0        0        0     5384 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/modules/dnscommonsrv.py
--rw-r--r--   0        0        0     3277 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/modules/dnsdumpster.py
--rw-r--r--   0        0        0     8872 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/modules/docker_pull.py
--rw-r--r--   0        0        0     3362 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/modules/dockerhub.py
--rw-r--r--   0        0        0     9330 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/modules/dotnetnuke.py
--rw-r--r--   0        0        0      882 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/modules/emailformat.py
--rw-r--r--   0        0        0    11843 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/modules/ffuf_shortnames.py
--rw-r--r--   0        0        0     7631 2024-06-03 11:39:19.719033 bbot-1.1.9.3376rc0/bbot/modules/filedownload.py
--rw-r--r--   0        0        0     2275 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/fingerprintx.py
--rw-r--r--   0        0        0     1294 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/fullhunt.py
--rw-r--r--   0        0        0     7848 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/generic_ssrf.py
--rw-r--r--   0        0        0     1420 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/git.py
--rw-r--r--   0        0        0     2321 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/git_clone.py
--rw-r--r--   0        0        0     3246 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/github_codesearch.py
--rw-r--r--   0        0        0     8826 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/github_org.py
--rw-r--r--   0        0        0     6161 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/github_workflows.py
--rw-r--r--   0        0        0     5746 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/gitlab.py
--rw-r--r--   0        0        0    12283 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/gowitness.py
--rw-r--r--   0        0        0      981 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/hackertarget.py
--rw-r--r--   0        0        0     7257 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/host_header.py
--rw-r--r--   0        0        0     6849 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/httpx.py
--rw-r--r--   0        0        0     6075 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/hunt.py
--rw-r--r--   0        0        0     2197 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/hunterio.py
--rw-r--r--   0        0        0    13246 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/iis_shortnames.py
--rw-r--r--   0        0        0        0 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/internal/__init__.py
--rw-r--r--   0        0        0      395 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/internal/aggregate.py
--rw-r--r--   0        0        0      578 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/internal/base.py
--rw-r--r--   0        0        0    18780 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/internal/excavate.py
--rw-r--r--   0        0        0     8371 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/internal/speculate.py
--rw-r--r--   0        0        0     4475 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/internetdb.py
--rw-r--r--   0        0        0     2222 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/ip2location.py
--rw-r--r--   0        0        0     1630 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/ipneighbor.py
--rw-r--r--   0        0        0     1862 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/ipstack.py
--rw-r--r--   0        0        0     1632 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/leakix.py
--rw-r--r--   0        0        0    10907 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/masscan.py
--rw-r--r--   0        0        0    21122 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/massdns.py
--rw-r--r--   0        0        0      948 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/myssl.py
--rw-r--r--   0        0        0     2367 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/newsletters.py
--rw-r--r--   0        0        0     5597 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/nmap.py
--rw-r--r--   0        0        0     4816 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/ntlm.py
--rw-r--r--   0        0        0     5943 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/oauth.py
--rw-r--r--   0        0        0      865 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/otx.py
--rw-r--r--   0        0        0        0 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/output/__init__.py
--rw-r--r--   0        0        0    14816 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/output/asset_inventory.py
--rw-r--r--   0        0        0     3215 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/output/base.py
--rw-r--r--   0        0        0     2664 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/output/csv.py
--rw-r--r--   0        0        0      622 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/output/discord.py
--rw-r--r--   0        0        0     1076 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/output/emails.py
--rw-r--r--   0        0        0     2273 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/output/http.py
--rw-r--r--   0        0        0     1967 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/output/human.py
--rw-r--r--   0        0        0     1466 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/output/json.py
--rw-r--r--   0        0        0     2806 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/output/neo4j.py
--rw-r--r--   0        0        0      270 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/output/python.py
--rw-r--r--   0        0        0     1208 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/output/slack.py
--rw-r--r--   0        0        0     1966 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/output/splunk.py
--rw-r--r--   0        0        0     1521 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/output/subdomains.py
--rw-r--r--   0        0        0      814 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/output/teams.py
--rw-r--r--   0        0        0     3712 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/output/web_report.py
--rw-r--r--   0        0        0     2278 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/output/websocket.py
--rw-r--r--   0        0        0     1759 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/paramminer_cookies.py
--rw-r--r--   0        0        0     1766 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/paramminer_getparams.py
--rw-r--r--   0        0        0     9636 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/paramminer_headers.py
--rw-r--r--   0        0        0     1718 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/passivetotal.py
--rw-r--r--   0        0        0     1511 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/pgp.py
--rw-r--r--   0        0        0     5570 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/postman.py
--rw-r--r--   0        0        0      923 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/rapiddns.py
--rw-r--r--   0        0        0     1693 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/report/affiliates.py
--rw-r--r--   0        0        0     8551 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/report/asn.py
--rw-r--r--   0        0        0      105 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/report/base.py
--rw-r--r--   0        0        0      919 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/riddler.py
--rw-r--r--   0        0        0     2079 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/robots.py
--rw-r--r--   0        0        0     2989 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/secretsdb.py
--rw-r--r--   0        0        0     1300 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/securitytrails.py
--rw-r--r--   0        0        0      891 2024-06-03 11:39:19.723033 bbot-1.1.9.3376rc0/bbot/modules/shodan_dns.py
--rw-r--r--   0        0        0     2084 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/modules/sitedossier.py
--rw-r--r--   0        0        0     1569 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/modules/skymem.py
--rw-r--r--   0        0        0     1462 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/modules/smuggler.py
--rw-r--r--   0        0        0     2091 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/modules/social.py
--rw-r--r--   0        0        0     7903 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/modules/sslcert.py
--rw-r--r--   0        0        0     1418 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/modules/subdomaincenter.py
--rw-r--r--   0        0        0      625 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/modules/sublist3r.py
--rw-r--r--   0        0        0    17126 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/modules/telerik.py
--rw-r--r--   0        0        0     5744 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/modules/templates/bucket.py
--rw-r--r--   0        0        0     1308 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/modules/templates/github.py
--rw-r--r--   0        0        0     2436 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/modules/templates/portscanner.py
--rw-r--r--   0        0        0     1182 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/modules/templates/shodan.py
--rw-r--r--   0        0        0     6100 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/modules/templates/subdomain_enum.py
--rw-r--r--   0        0        0     3789 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/modules/templates/webhook.py
--rw-r--r--   0        0        0      754 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/modules/threatminer.py
--rw-r--r--   0        0        0     4618 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/modules/trufflehog.py
--rw-r--r--   0        0        0     4187 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/modules/url_manipulation.py
--rw-r--r--   0        0        0     3068 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/modules/urlscan.py
--rw-r--r--   0        0        0     2401 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/modules/viewdns.py
--rw-r--r--   0        0        0     1690 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/modules/virustotal.py
--rw-r--r--   0        0        0     2095 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/modules/wafw00f.py
--rw-r--r--   0        0        0     1342 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/modules/wappalyzer.py
--rw-r--r--   0        0        0     2940 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/modules/wayback.py
--rw-r--r--   0        0        0     2435 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/modules/zoomeye.py
--rw-r--r--   0        0        0       29 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/scanner/__init__.py
--rw-r--r--   0        0        0      793 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/scanner/dispatcher.py
--rw-r--r--   0        0        0    29339 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/scanner/manager.py
--rw-r--r--   0        0        0    42299 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/scanner/scanner.py
--rw-r--r--   0        0        0     2702 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/scanner/stats.py
--rw-r--r--   0        0        0    11540 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/scanner/target.py
--rwxr-xr-x   0        0        0     5889 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/scripts/docs.py
--rw-r--r--   0        0        0        0 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/test/__init__.py
--rw-r--r--   0        0        0    12010 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/test/bbot_fixtures.py
--rw-r--r--   0        0        0     4870 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/test/conftest.py
--rw-r--r--   0        0        0       31 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/test/coverage.cfg
--rwxr-xr-x   0        0        0      652 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/test/run_tests.sh
--rw-r--r--   0        0        0     1091 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/test/test.conf
--rw-r--r--   0        0        0      323 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/test/test_output.ndjson
--rw-r--r--   0        0        0        0 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/test/test_step_1/__init__.py
--rw-r--r--   0        0        0     1445 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/test/test_step_1/test__module__tests.py
--rw-r--r--   0        0        0     5523 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/test/test_step_1/test_agent.py
--rw-r--r--   0        0        0     6544 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/test/test_step_1/test_cli.py
--rw-r--r--   0        0        0     3808 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/test/test_step_1/test_cloud_helpers.py
--rw-r--r--   0        0        0     6384 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/test/test_step_1/test_command.py
--rw-r--r--   0        0        0      495 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/test/test_step_1/test_config.py
--rw-r--r--   0        0        0      722 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/test/test_step_1/test_depsinstaller.py
--rw-r--r--   0        0        0     7572 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/test/test_step_1/test_dns.py
--rw-r--r--   0        0        0       79 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/test/test_step_1/test_docs.py
--rw-r--r--   0        0        0    23553 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/test/test_step_1/test_events.py
--rw-r--r--   0        0        0      702 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/test/test_step_1/test_files.py
--rw-r--r--   0        0        0    32193 2024-06-03 11:39:19.727033 bbot-1.1.9.3376rc0/bbot/test/test_step_1/test_helpers.py
--rw-r--r--   0        0        0    16305 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_1/test_manager_deduplication.py
--rw-r--r--   0        0        0    79706 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_1/test_manager_scope_accuracy.py
--rw-r--r--   0        0        0    16943 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_1/test_modules_basic.py
--rw-r--r--   0        0        0     2657 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_1/test_python_api.py
--rw-r--r--   0        0        0    11901 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_1/test_regexes.py
--rw-r--r--   0        0        0     2870 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_1/test_scan.py
--rw-r--r--   0        0        0      706 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_1/test_scope.py
--rw-r--r--   0        0        0     2175 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_1/test_target.py
--rw-r--r--   0        0        0    13141 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_1/test_web.py
--rw-r--r--   0        0        0        0 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/__init__.py
--rw-r--r--   0        0        0        0 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/__init__.py
--rw-r--r--   0        0        0     5344 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/base.py
--rw-r--r--   0        0        0      664 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_affiliates.py
--rw-r--r--   0        0        0      473 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_aggregate.py
--rw-r--r--   0        0        0     2789 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_ajaxpro.py
--rw-r--r--   0        0        0      546 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py
--rw-r--r--   0        0        0    10606 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_asn.py
--rw-r--r--   0        0        0     3098 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py
--rw-r--r--   0        0        0     1207 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_azure_realm.py
--rw-r--r--   0        0        0     4805 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py
--rw-r--r--   0        0        0     2795 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_baddns.py
--rw-r--r--   0        0        0     2397 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_baddns_zone.py
--rw-r--r--   0        0        0     5599 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py
--rw-r--r--   0        0        0     1045 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py
--rw-r--r--   0        0        0     1101 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py
--rw-r--r--   0        0        0     3984 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_bucket_amazon.py
--rw-r--r--   0        0        0      552 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py
--rw-r--r--   0        0        0      907 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py
--rw-r--r--   0        0        0     2282 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_bucket_file_enum.py
--rw-r--r--   0        0        0      506 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_bucket_firebase.py
--rw-r--r--   0        0        0     1312 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_bucket_google.py
--rw-r--r--   0        0        0     5051 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py
--rw-r--r--   0        0        0     3551 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py
--rw-r--r--   0        0        0      982 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_c99.py
--rw-r--r--   0        0        0     3956 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_censys.py
--rw-r--r--   0        0        0      636 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py
--rw-r--r--   0        0        0      956 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_chaos.py
--rw-r--r--   0        0        0     2047 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_code_repository.py
--rw-r--r--   0        0        0      564 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py
--rw-r--r--   0        0        0     3362 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_credshed.py
--rw-r--r--   0        0        0      762 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py
--rw-r--r--   0        0        0      717 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_crt.py
--rw-r--r--   0        0        0      273 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_csv.py
--rw-r--r--   0        0        0     2321 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_dastardly.py
--rw-r--r--   0        0        0     3615 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_dehashed.py
--rw-r--r--   0        0        0     1613 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_digitorus.py
--rw-r--r--   0        0        0     1863 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_discord.py
--rw-r--r--   0        0        0      952 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py
--rw-r--r--   0        0        0    59749 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py
--rw-r--r--   0        0        0    27988 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_docker_pull.py
--rw-r--r--   0        0        0     3907 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_dockerhub.py
--rw-r--r--   0        0        0     8232 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_dotnetnuke.py
--rw-r--r--   0        0        0      461 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_emailformat.py
--rw-r--r--   0        0        0      944 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_emails.py
--rw-r--r--   0        0        0    14708 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py
--rw-r--r--   0        0        0     2955 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py
--rw-r--r--   0        0        0     7669 2024-06-03 11:39:19.731033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py
--rw-r--r--   0        0        0     2389 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_filedownload.py
--rw-r--r--   0        0        0      445 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_fingerprintx.py
--rw-r--r--   0        0        0     1946 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py
--rw-r--r--   0        0        0     2040 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py
--rw-r--r--   0        0        0     1656 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_git.py
--rw-r--r--   0        0        0    12266 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_git_clone.py
--rw-r--r--   0        0        0     3718 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_github_codesearch.py
--rw-r--r--   0        0        0    24606 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_github_org.py
--rw-r--r--   0        0        0    35521 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_github_workflows.py
--rw-r--r--   0        0        0    11579 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_gitlab.py
--rw-r--r--   0        0        0     3433 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py
--rw-r--r--   0        0        0      609 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py
--rw-r--r--   0        0        0     2702 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py
--rw-r--r--   0        0        0     2155 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_http.py
--rw-r--r--   0        0        0     4939 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py
--rw-r--r--   0        0        0      249 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_human.py
--rw-r--r--   0        0        0      665 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py
--rw-r--r--   0        0        0     4086 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py
--rw-r--r--   0        0        0     2879 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py
--rw-r--r--   0        0        0     2231 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_internetdb.py
--rw-r--r--   0        0        0     1123 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_ip2location.py
--rw-r--r--   0        0        0      604 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py
--rw-r--r--   0        0        0     2767 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py
--rw-r--r--   0        0        0     1006 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_json.py
--rw-r--r--   0        0        0     1641 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py
--rw-r--r--   0        0        0     1711 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py
--rw-r--r--   0        0        0      428 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_massdns.py
--rw-r--r--   0        0        0     1532 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py
--rw-r--r--   0        0        0     1030 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py
--rw-r--r--   0        0        0     2305 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_newsletters.py
--rw-r--r--   0        0        0     3618 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_nmap.py
--rw-r--r--   0        0        0     1116 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py
--rw-r--r--   0        0        0     5609 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py
--rw-r--r--   0        0        0     9402 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_oauth.py
--rw-r--r--   0        0        0     1160 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_otx.py
--rw-r--r--   0        0        0     2142 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py
--rw-r--r--   0        0        0    10680 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py
--rw-r--r--   0        0        0     2190 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py
--rw-r--r--   0        0        0      961 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py
--rw-r--r--   0        0        0     1609 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py
--rw-r--r--   0        0        0    14768 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_postman.py
--rw-r--r--   0        0        0      184 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_python.py
--rw-r--r--   0        0        0      750 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py
--rw-r--r--   0        0        0      747 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py
--rw-r--r--   0        0        0     1564 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_robots.py
--rw-r--r--   0        0        0      537 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py
--rw-r--r--   0        0        0      758 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py
--rw-r--r--   0        0        0      713 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py
--rw-r--r--   0        0        0     6220 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_sitedossier.py
--rw-r--r--   0        0        0     2321 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py
--rw-r--r--   0        0        0      415 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_slack.py
--rw-r--r--   0        0        0     2430 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py
--rw-r--r--   0        0        0     1700 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_social.py
--rw-r--r--   0        0        0     3121 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py
--rw-r--r--   0        0        0     1866 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_splunk.py
--rw-r--r--   0        0        0      706 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_sslcert.py
--rw-r--r--   0        0        0      610 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_subdomaincenter.py
--rw-r--r--   0        0        0     1116 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_subdomains.py
--rw-r--r--   0        0        0      611 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py
--rw-r--r--   0        0        0     1222 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_teams.py
--rw-r--r--   0        0        0     7751 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py
--rw-r--r--   0        0        0      489 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_threatminer.py
--rw-r--r--   0        0        0    62527 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_trufflehog.py
--rw-r--r--   0        0        0     1144 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py
--rw-r--r--   0        0        0     2902 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py
--rw-r--r--   0        0        0     2874 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py
--rw-r--r--   0        0        0     8726 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py
--rw-r--r--   0        0        0     3401 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py
--rw-r--r--   0        0        0     1304 2024-06-03 11:39:19.735033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py
--rw-r--r--   0        0        0      936 2024-06-03 11:39:19.739033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py
--rw-r--r--   0        0        0      548 2024-06-03 11:39:19.739033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py
--rw-r--r--   0        0        0     2026 2024-06-03 11:39:19.739033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py
--rw-r--r--   0        0        0     1009 2024-06-03 11:39:19.739033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py
--rw-r--r--   0        0        0     1979 2024-06-03 11:39:19.739033 bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py
--rw-r--r--   0        0        0     1103 2024-06-03 11:39:19.739033 bbot-1.1.9.3376rc0/bbot/test/testsslcert.pem
--rw-r--r--   0        0        0     1704 2024-06-03 11:39:19.739033 bbot-1.1.9.3376rc0/bbot/test/testsslkey.pem
--rw-r--r--   0        0        0      476 2024-06-03 11:39:19.739033 bbot-1.1.9.3376rc0/bbot/wordlists/devops_mutations.txt
--rw-r--r--   0        0        0   959424 2024-06-03 11:39:19.743033 bbot-1.1.9.3376rc0/bbot/wordlists/ffuf_shortname_candidates.txt
--rw-r--r--   0        0        0      764 2024-06-03 11:39:19.743033 bbot-1.1.9.3376rc0/bbot/wordlists/ms_on_prem_subdomains.txt
--rw-r--r--   0        0        0    32226 2024-06-03 11:39:19.743033 bbot-1.1.9.3376rc0/bbot/wordlists/nameservers.txt
--rw-r--r--   0        0        0    17458 2024-06-03 11:39:19.743033 bbot-1.1.9.3376rc0/bbot/wordlists/paramminer_headers.txt
--rw-r--r--   0        0        0    54887 2024-06-03 11:39:19.743033 bbot-1.1.9.3376rc0/bbot/wordlists/paramminer_parameters.txt
--rw-r--r--   0        0        0     6068 2024-06-03 11:39:19.743033 bbot-1.1.9.3376rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt
--rw-r--r--   0        0        0   570241 2024-06-03 11:39:19.743033 bbot-1.1.9.3376rc0/bbot/wordlists/wordninja_dns.txt.gz
--rw-r--r--   0        0        0     2663 2024-06-03 11:39:37.687229 bbot-1.1.9.3376rc0/pyproject.toml
--rw-r--r--   0        0        0    42361 1970-01-01 00:00:00.000000 bbot-1.1.9.3376rc0/PKG-INFO
+-rw-r--r--   0        0        0    32473 2024-06-03 14:07:11.908954 bbot-1.1.9.3387rc0/LICENSE
+-rw-r--r--   0        0        0    40272 2024-06-03 14:07:11.908954 bbot-1.1.9.3387rc0/README.md
+-rw-r--r--   0        0        0      211 2024-06-03 14:07:30.257282 bbot-1.1.9.3387rc0/bbot/__init__.py
+-rw-r--r--   0        0        0       25 2024-06-03 14:07:11.908954 bbot-1.1.9.3387rc0/bbot/agent/__init__.py
+-rw-r--r--   0        0        0     7898 2024-06-03 14:07:11.908954 bbot-1.1.9.3387rc0/bbot/agent/agent.py
+-rw-r--r--   0        0        0      450 2024-06-03 14:07:11.908954 bbot-1.1.9.3387rc0/bbot/agent/messages.py
+-rwxr-xr-x   0        0        0    17601 2024-06-03 14:07:11.908954 bbot-1.1.9.3387rc0/bbot/cli.py
+-rw-r--r--   0        0        0       59 2024-06-03 14:07:11.908954 bbot-1.1.9.3387rc0/bbot/core/__init__.py
+-rw-r--r--   0        0        0     3588 2024-06-03 14:07:11.908954 bbot-1.1.9.3387rc0/bbot/core/configurator/__init__.py
+-rw-r--r--   0        0        0     9843 2024-06-03 14:07:11.908954 bbot-1.1.9.3387rc0/bbot/core/configurator/args.py
+-rw-r--r--   0        0        0     5182 2024-06-03 14:07:11.908954 bbot-1.1.9.3387rc0/bbot/core/configurator/environ.py
+-rw-r--r--   0        0        0     1341 2024-06-03 14:07:11.908954 bbot-1.1.9.3387rc0/bbot/core/configurator/files.py
+-rw-r--r--   0        0        0      617 2024-06-03 14:07:11.908954 bbot-1.1.9.3387rc0/bbot/core/errors.py
+-rw-r--r--   0        0        0       91 2024-06-03 14:07:11.908954 bbot-1.1.9.3387rc0/bbot/core/event/__init__.py
+-rw-r--r--   0        0        0    46323 2024-06-03 14:07:11.908954 bbot-1.1.9.3387rc0/bbot/core/event/base.py
+-rw-r--r--   0        0        0     1656 2024-06-03 14:07:11.908954 bbot-1.1.9.3387rc0/bbot/core/event/helpers.py
+-rw-r--r--   0        0        0     1232 2024-06-03 14:07:11.912954 bbot-1.1.9.3387rc0/bbot/core/flags.py
+-rw-r--r--   0        0        0       86 2024-06-03 14:07:11.912954 bbot-1.1.9.3387rc0/bbot/core/helpers/__init__.py
+-rw-r--r--   0        0        0     3583 2024-06-03 14:07:11.912954 bbot-1.1.9.3387rc0/bbot/core/helpers/async_helpers.py
+-rw-r--r--   0        0        0     1537 2024-06-03 14:07:11.912954 bbot-1.1.9.3387rc0/bbot/core/helpers/cache.py
+-rw-r--r--   0        0        0     4341 2024-06-03 14:07:11.912954 bbot-1.1.9.3387rc0/bbot/core/helpers/cloud.py
+-rw-r--r--   0        0        0    11950 2024-06-03 14:07:11.912954 bbot-1.1.9.3387rc0/bbot/core/helpers/command.py
+-rw-r--r--   0        0        0       37 2024-06-03 14:07:11.912954 bbot-1.1.9.3387rc0/bbot/core/helpers/depsinstaller/__init__.py
+-rw-r--r--   0        0        0    14117 2024-06-03 14:07:11.912954 bbot-1.1.9.3387rc0/bbot/core/helpers/depsinstaller/installer.py
+-rw-r--r--   0        0        0       87 2024-06-03 14:07:11.912954 bbot-1.1.9.3387rc0/bbot/core/helpers/depsinstaller/sudo_askpass.py
+-rw-r--r--   0        0        0     9199 2024-06-03 14:07:11.912954 bbot-1.1.9.3387rc0/bbot/core/helpers/diff.py
+-rw-r--r--   0        0        0    47786 2024-06-03 14:07:11.912954 bbot-1.1.9.3387rc0/bbot/core/helpers/dns.py
+-rw-r--r--   0        0        0     5639 2024-06-03 14:07:11.912954 bbot-1.1.9.3387rc0/bbot/core/helpers/files.py
+-rw-r--r--   0        0        0     6354 2024-06-03 14:07:11.912954 bbot-1.1.9.3387rc0/bbot/core/helpers/helper.py
+-rw-r--r--   0        0        0    12632 2024-06-03 14:07:11.912954 bbot-1.1.9.3387rc0/bbot/core/helpers/interactsh.py
+-rw-r--r--   0        0        0     1408 2024-06-03 14:07:11.912954 bbot-1.1.9.3387rc0/bbot/core/helpers/logger.py
+-rw-r--r--   0        0        0    84110 2024-06-03 14:07:11.912954 bbot-1.1.9.3387rc0/bbot/core/helpers/misc.py
+-rw-r--r--   0        0        0    22071 2024-06-03 14:07:11.912954 bbot-1.1.9.3387rc0/bbot/core/helpers/modules.py
+-rw-r--r--   0        0        0    10041 2024-06-03 14:07:11.912954 bbot-1.1.9.3387rc0/bbot/core/helpers/names_generator.py
+-rw-r--r--   0        0        0     2578 2024-06-03 14:07:11.912954 bbot-1.1.9.3387rc0/bbot/core/helpers/ntlm.py
+-rw-r--r--   0        0        0     1990 2024-06-03 14:07:11.912954 bbot-1.1.9.3387rc0/bbot/core/helpers/ratelimiter.py
+-rw-r--r--   0        0        0     4542 2024-06-03 14:07:11.912954 bbot-1.1.9.3387rc0/bbot/core/helpers/regexes.py
+-rw-r--r--   0        0        0     5947 2024-06-03 14:07:11.912954 bbot-1.1.9.3387rc0/bbot/core/helpers/url.py
+-rw-r--r--   0        0        0     8781 2024-06-03 14:07:11.912954 bbot-1.1.9.3387rc0/bbot/core/helpers/validators.py
+-rw-r--r--   0        0        0    31938 2024-06-03 14:07:11.912954 bbot-1.1.9.3387rc0/bbot/core/helpers/web.py
+-rw-r--r--   0        0        0    19801 2024-06-03 14:07:11.912954 bbot-1.1.9.3387rc0/bbot/core/helpers/wordcloud.py
+-rw-r--r--   0        0        0      191 2024-06-03 14:07:11.912954 bbot-1.1.9.3387rc0/bbot/core/logger/__init__.py
+-rw-r--r--   0        0        0     8118 2024-06-03 14:07:11.912954 bbot-1.1.9.3387rc0/bbot/core/logger/logger.py
+-rw-r--r--   0        0        0     4158 2024-06-03 14:07:11.912954 bbot-1.1.9.3387rc0/bbot/defaults.yml
+-rw-r--r--   0        0        0      396 2024-06-03 14:07:11.912954 bbot-1.1.9.3387rc0/bbot/modules/__init__.py
+-rw-r--r--   0        0        0     2413 2024-06-03 14:07:11.912954 bbot-1.1.9.3387rc0/bbot/modules/ajaxpro.py
+-rw-r--r--   0        0        0     1915 2024-06-03 14:07:11.912954 bbot-1.1.9.3387rc0/bbot/modules/anubisdb.py
+-rw-r--r--   0        0        0     1463 2024-06-03 14:07:11.912954 bbot-1.1.9.3387rc0/bbot/modules/azure_realm.py
+-rw-r--r--   0        0        0     4782 2024-06-03 14:07:11.912954 bbot-1.1.9.3387rc0/bbot/modules/azure_tenant.py
+-rw-r--r--   0        0        0     4237 2024-06-03 14:07:11.912954 bbot-1.1.9.3387rc0/bbot/modules/baddns.py
+-rw-r--r--   0        0        0     1332 2024-06-03 14:07:11.912954 bbot-1.1.9.3387rc0/bbot/modules/baddns_zone.py
+-rw-r--r--   0        0        0     3634 2024-06-03 14:07:11.912954 bbot-1.1.9.3387rc0/bbot/modules/badsecrets.py
+-rw-r--r--   0        0        0    59062 2024-06-03 14:07:11.912954 bbot-1.1.9.3387rc0/bbot/modules/base.py
+-rw-r--r--   0        0        0     2446 2024-06-03 14:07:11.912954 bbot-1.1.9.3387rc0/bbot/modules/bevigil.py
+-rw-r--r--   0        0        0     1398 2024-06-03 14:07:11.912954 bbot-1.1.9.3387rc0/bbot/modules/binaryedge.py
+-rw-r--r--   0        0        0      746 2024-06-03 14:07:11.912954 bbot-1.1.9.3387rc0/bbot/modules/bucket_amazon.py
+-rw-r--r--   0        0        0     1111 2024-06-03 14:07:11.912954 bbot-1.1.9.3387rc0/bbot/modules/bucket_azure.py
+-rw-r--r--   0        0        0      866 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/bucket_digitalocean.py
+-rw-r--r--   0        0        0     2063 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/bucket_file_enum.py
+-rw-r--r--   0        0        0     1443 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/bucket_firebase.py
+-rw-r--r--   0        0        0     2631 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/bucket_google.py
+-rw-r--r--   0        0        0     5010 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/builtwith.py
+-rw-r--r--   0        0        0     6607 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/bypass403.py
+-rw-r--r--   0        0        0     1287 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/c99.py
+-rw-r--r--   0        0        0     3470 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/censys.py
+-rw-r--r--   0        0        0      889 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/certspotter.py
+-rw-r--r--   0        0        0     1621 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/chaos.py
+-rw-r--r--   0        0        0     1901 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/code_repository.py
+-rw-r--r--   0        0        0      826 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/columbus.py
+-rw-r--r--   0        0        0     3366 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/credshed.py
+-rw-r--r--   0        0        0      428 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/crobat.py
+-rw-r--r--   0        0        0     1321 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/crt.py
+-rw-r--r--   0        0        0     5407 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/deadly/dastardly.py
+-rw-r--r--   0        0        0    14132 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/deadly/ffuf.py
+-rw-r--r--   0        0        0    17351 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/deadly/nuclei.py
+-rw-r--r--   0        0        0     5293 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/deadly/vhost.py
+-rw-r--r--   0        0        0     4020 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/dehashed.py
+-rw-r--r--   0        0        0     1021 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/digitorus.py
+-rw-r--r--   0        0        0     5384 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/dnscommonsrv.py
+-rw-r--r--   0        0        0     3277 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/dnsdumpster.py
+-rw-r--r--   0        0        0     8872 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/docker_pull.py
+-rw-r--r--   0        0        0     3362 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/dockerhub.py
+-rw-r--r--   0        0        0     9330 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/dotnetnuke.py
+-rw-r--r--   0        0        0      882 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/emailformat.py
+-rw-r--r--   0        0        0    11843 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/ffuf_shortnames.py
+-rw-r--r--   0        0        0     8035 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/filedownload.py
+-rw-r--r--   0        0        0     2275 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/fingerprintx.py
+-rw-r--r--   0        0        0     1294 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/fullhunt.py
+-rw-r--r--   0        0        0     7848 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/generic_ssrf.py
+-rw-r--r--   0        0        0     1420 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/git.py
+-rw-r--r--   0        0        0     2321 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/git_clone.py
+-rw-r--r--   0        0        0     3246 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/github_codesearch.py
+-rw-r--r--   0        0        0     8826 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/github_org.py
+-rw-r--r--   0        0        0     6161 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/github_workflows.py
+-rw-r--r--   0        0        0     5746 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/gitlab.py
+-rw-r--r--   0        0        0    12283 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/gowitness.py
+-rw-r--r--   0        0        0      981 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/hackertarget.py
+-rw-r--r--   0        0        0     7257 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/host_header.py
+-rw-r--r--   0        0        0     6849 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/httpx.py
+-rw-r--r--   0        0        0     6075 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/hunt.py
+-rw-r--r--   0        0        0     2197 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/hunterio.py
+-rw-r--r--   0        0        0    13246 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/iis_shortnames.py
+-rw-r--r--   0        0        0        0 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/internal/__init__.py
+-rw-r--r--   0        0        0      395 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/internal/aggregate.py
+-rw-r--r--   0        0        0      578 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/internal/base.py
+-rw-r--r--   0        0        0    18780 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/internal/excavate.py
+-rw-r--r--   0        0        0     8371 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/internal/speculate.py
+-rw-r--r--   0        0        0     4475 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/internetdb.py
+-rw-r--r--   0        0        0     2222 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/ip2location.py
+-rw-r--r--   0        0        0     1630 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/ipneighbor.py
+-rw-r--r--   0        0        0     1862 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/ipstack.py
+-rw-r--r--   0        0        0     1632 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/leakix.py
+-rw-r--r--   0        0        0    10907 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/masscan.py
+-rw-r--r--   0        0        0    21122 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/massdns.py
+-rw-r--r--   0        0        0      948 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/myssl.py
+-rw-r--r--   0        0        0     2367 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/newsletters.py
+-rw-r--r--   0        0        0     5597 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/nmap.py
+-rw-r--r--   0        0        0     4816 2024-06-03 14:07:11.916955 bbot-1.1.9.3387rc0/bbot/modules/ntlm.py
+-rw-r--r--   0        0        0     5943 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/oauth.py
+-rw-r--r--   0        0        0      865 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/otx.py
+-rw-r--r--   0        0        0        0 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/output/__init__.py
+-rw-r--r--   0        0        0    14816 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/output/asset_inventory.py
+-rw-r--r--   0        0        0     3215 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/output/base.py
+-rw-r--r--   0        0        0     2664 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/output/csv.py
+-rw-r--r--   0        0        0      622 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/output/discord.py
+-rw-r--r--   0        0        0     1076 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/output/emails.py
+-rw-r--r--   0        0        0     2273 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/output/http.py
+-rw-r--r--   0        0        0     1967 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/output/human.py
+-rw-r--r--   0        0        0     1466 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/output/json.py
+-rw-r--r--   0        0        0     2806 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/output/neo4j.py
+-rw-r--r--   0        0        0      270 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/output/python.py
+-rw-r--r--   0        0        0     1208 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/output/slack.py
+-rw-r--r--   0        0        0     1966 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/output/splunk.py
+-rw-r--r--   0        0        0     1521 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/output/subdomains.py
+-rw-r--r--   0        0        0      814 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/output/teams.py
+-rw-r--r--   0        0        0     3712 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/output/web_report.py
+-rw-r--r--   0        0        0     2278 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/output/websocket.py
+-rw-r--r--   0        0        0     1759 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/paramminer_cookies.py
+-rw-r--r--   0        0        0     1766 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/paramminer_getparams.py
+-rw-r--r--   0        0        0     9636 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/paramminer_headers.py
+-rw-r--r--   0        0        0     1718 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/passivetotal.py
+-rw-r--r--   0        0        0     1511 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/pgp.py
+-rw-r--r--   0        0        0     5570 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/postman.py
+-rw-r--r--   0        0        0      923 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/rapiddns.py
+-rw-r--r--   0        0        0     1693 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/report/affiliates.py
+-rw-r--r--   0        0        0     8551 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/report/asn.py
+-rw-r--r--   0        0        0      105 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/report/base.py
+-rw-r--r--   0        0        0      919 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/riddler.py
+-rw-r--r--   0        0        0     2079 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/robots.py
+-rw-r--r--   0        0        0     2989 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/secretsdb.py
+-rw-r--r--   0        0        0     1300 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/securitytrails.py
+-rw-r--r--   0        0        0      891 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/shodan_dns.py
+-rw-r--r--   0        0        0     2084 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/sitedossier.py
+-rw-r--r--   0        0        0     1569 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/skymem.py
+-rw-r--r--   0        0        0     1462 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/smuggler.py
+-rw-r--r--   0        0        0     2091 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/social.py
+-rw-r--r--   0        0        0     7903 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/sslcert.py
+-rw-r--r--   0        0        0     1418 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/subdomaincenter.py
+-rw-r--r--   0        0        0      625 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/sublist3r.py
+-rw-r--r--   0        0        0    17126 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/telerik.py
+-rw-r--r--   0        0        0     5744 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/templates/bucket.py
+-rw-r--r--   0        0        0     1308 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/templates/github.py
+-rw-r--r--   0        0        0     2436 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/templates/portscanner.py
+-rw-r--r--   0        0        0     1182 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/templates/shodan.py
+-rw-r--r--   0        0        0     6100 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/templates/subdomain_enum.py
+-rw-r--r--   0        0        0     3789 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/templates/webhook.py
+-rw-r--r--   0        0        0      754 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/threatminer.py
+-rw-r--r--   0        0        0     4618 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/trufflehog.py
+-rw-r--r--   0        0        0     4187 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/url_manipulation.py
+-rw-r--r--   0        0        0     3068 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/urlscan.py
+-rw-r--r--   0        0        0     2401 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/viewdns.py
+-rw-r--r--   0        0        0     1690 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/virustotal.py
+-rw-r--r--   0        0        0     2095 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/wafw00f.py
+-rw-r--r--   0        0        0     1342 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/wappalyzer.py
+-rw-r--r--   0        0        0     2940 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/wayback.py
+-rw-r--r--   0        0        0     2435 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/modules/zoomeye.py
+-rw-r--r--   0        0        0       29 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/scanner/__init__.py
+-rw-r--r--   0        0        0      793 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/scanner/dispatcher.py
+-rw-r--r--   0        0        0    28681 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/scanner/manager.py
+-rw-r--r--   0        0        0    42299 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/scanner/scanner.py
+-rw-r--r--   0        0        0     2702 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/scanner/stats.py
+-rw-r--r--   0        0        0    11540 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/scanner/target.py
+-rwxr-xr-x   0        0        0     5889 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/scripts/docs.py
+-rw-r--r--   0        0        0        0 2024-06-03 14:07:11.920955 bbot-1.1.9.3387rc0/bbot/test/__init__.py
+-rw-r--r--   0        0        0    12010 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/bbot_fixtures.py
+-rw-r--r--   0        0        0     4870 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/conftest.py
+-rw-r--r--   0        0        0       31 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/coverage.cfg
+-rwxr-xr-x   0        0        0      652 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/run_tests.sh
+-rw-r--r--   0        0        0     1091 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test.conf
+-rw-r--r--   0        0        0      323 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_output.ndjson
+-rw-r--r--   0        0        0        0 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_1/__init__.py
+-rw-r--r--   0        0        0     1445 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_1/test__module__tests.py
+-rw-r--r--   0        0        0     5523 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_1/test_agent.py
+-rw-r--r--   0        0        0     6544 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_1/test_cli.py
+-rw-r--r--   0        0        0     3808 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_1/test_cloud_helpers.py
+-rw-r--r--   0        0        0     6384 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_1/test_command.py
+-rw-r--r--   0        0        0      495 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_1/test_config.py
+-rw-r--r--   0        0        0      722 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_1/test_depsinstaller.py
+-rw-r--r--   0        0        0     7572 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_1/test_dns.py
+-rw-r--r--   0        0        0       79 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_1/test_docs.py
+-rw-r--r--   0        0        0    23553 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_1/test_events.py
+-rw-r--r--   0        0        0      702 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_1/test_files.py
+-rw-r--r--   0        0        0    32193 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_1/test_helpers.py
+-rw-r--r--   0        0        0    16305 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_1/test_manager_deduplication.py
+-rw-r--r--   0        0        0    79706 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_1/test_manager_scope_accuracy.py
+-rw-r--r--   0        0        0    16943 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_1/test_modules_basic.py
+-rw-r--r--   0        0        0     2657 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_1/test_python_api.py
+-rw-r--r--   0        0        0    11901 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_1/test_regexes.py
+-rw-r--r--   0        0        0     2870 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_1/test_scan.py
+-rw-r--r--   0        0        0      706 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_1/test_scope.py
+-rw-r--r--   0        0        0     2175 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_1/test_target.py
+-rw-r--r--   0        0        0    13141 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_1/test_web.py
+-rw-r--r--   0        0        0        0 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/__init__.py
+-rw-r--r--   0        0        0     5344 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/base.py
+-rw-r--r--   0        0        0      664 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_affiliates.py
+-rw-r--r--   0        0        0      473 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_aggregate.py
+-rw-r--r--   0        0        0     2789 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_ajaxpro.py
+-rw-r--r--   0        0        0      546 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py
+-rw-r--r--   0        0        0    10606 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_asn.py
+-rw-r--r--   0        0        0     3098 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py
+-rw-r--r--   0        0        0     1207 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_azure_realm.py
+-rw-r--r--   0        0        0     4805 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py
+-rw-r--r--   0        0        0     2795 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_baddns.py
+-rw-r--r--   0        0        0     2397 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_baddns_zone.py
+-rw-r--r--   0        0        0     5599 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py
+-rw-r--r--   0        0        0     1045 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py
+-rw-r--r--   0        0        0     1101 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py
+-rw-r--r--   0        0        0     3984 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_bucket_amazon.py
+-rw-r--r--   0        0        0      552 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py
+-rw-r--r--   0        0        0      907 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py
+-rw-r--r--   0        0        0     2282 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_bucket_file_enum.py
+-rw-r--r--   0        0        0      506 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_bucket_firebase.py
+-rw-r--r--   0        0        0     1312 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_bucket_google.py
+-rw-r--r--   0        0        0     5051 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py
+-rw-r--r--   0        0        0     3551 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py
+-rw-r--r--   0        0        0      982 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_c99.py
+-rw-r--r--   0        0        0     3956 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_censys.py
+-rw-r--r--   0        0        0      636 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py
+-rw-r--r--   0        0        0      956 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_chaos.py
+-rw-r--r--   0        0        0     2047 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_code_repository.py
+-rw-r--r--   0        0        0      564 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py
+-rw-r--r--   0        0        0     3362 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_credshed.py
+-rw-r--r--   0        0        0      762 2024-06-03 14:07:11.924955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py
+-rw-r--r--   0        0        0      717 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_crt.py
+-rw-r--r--   0        0        0      273 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_csv.py
+-rw-r--r--   0        0        0     2321 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_dastardly.py
+-rw-r--r--   0        0        0     3615 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_dehashed.py
+-rw-r--r--   0        0        0     1613 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_digitorus.py
+-rw-r--r--   0        0        0     1863 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_discord.py
+-rw-r--r--   0        0        0      952 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py
+-rw-r--r--   0        0        0    59749 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py
+-rw-r--r--   0        0        0    27988 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_docker_pull.py
+-rw-r--r--   0        0        0     3907 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_dockerhub.py
+-rw-r--r--   0        0        0     8232 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_dotnetnuke.py
+-rw-r--r--   0        0        0      461 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_emailformat.py
+-rw-r--r--   0        0        0      944 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_emails.py
+-rw-r--r--   0        0        0    14708 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py
+-rw-r--r--   0        0        0     2955 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py
+-rw-r--r--   0        0        0     7669 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py
+-rw-r--r--   0        0        0     2608 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_filedownload.py
+-rw-r--r--   0        0        0      445 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_fingerprintx.py
+-rw-r--r--   0        0        0     1946 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py
+-rw-r--r--   0        0        0     2040 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py
+-rw-r--r--   0        0        0     1656 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_git.py
+-rw-r--r--   0        0        0    12266 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_git_clone.py
+-rw-r--r--   0        0        0     3718 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_github_codesearch.py
+-rw-r--r--   0        0        0    24606 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_github_org.py
+-rw-r--r--   0        0        0    35521 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_github_workflows.py
+-rw-r--r--   0        0        0    11579 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_gitlab.py
+-rw-r--r--   0        0        0     3433 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py
+-rw-r--r--   0        0        0      609 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py
+-rw-r--r--   0        0        0     2702 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py
+-rw-r--r--   0        0        0     2155 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_http.py
+-rw-r--r--   0        0        0     4939 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py
+-rw-r--r--   0        0        0      249 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_human.py
+-rw-r--r--   0        0        0      665 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py
+-rw-r--r--   0        0        0     4086 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py
+-rw-r--r--   0        0        0     2879 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py
+-rw-r--r--   0        0        0     2231 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_internetdb.py
+-rw-r--r--   0        0        0     1123 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_ip2location.py
+-rw-r--r--   0        0        0      604 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py
+-rw-r--r--   0        0        0     2767 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py
+-rw-r--r--   0        0        0     1006 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_json.py
+-rw-r--r--   0        0        0     1641 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py
+-rw-r--r--   0        0        0     1711 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py
+-rw-r--r--   0        0        0      428 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_massdns.py
+-rw-r--r--   0        0        0     1532 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py
+-rw-r--r--   0        0        0     1030 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py
+-rw-r--r--   0        0        0     2305 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_newsletters.py
+-rw-r--r--   0        0        0     3618 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_nmap.py
+-rw-r--r--   0        0        0     1116 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py
+-rw-r--r--   0        0        0     5609 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py
+-rw-r--r--   0        0        0     9402 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_oauth.py
+-rw-r--r--   0        0        0     1160 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_otx.py
+-rw-r--r--   0        0        0     2142 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py
+-rw-r--r--   0        0        0    10680 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py
+-rw-r--r--   0        0        0     2190 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py
+-rw-r--r--   0        0        0      961 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py
+-rw-r--r--   0        0        0     1609 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py
+-rw-r--r--   0        0        0    14768 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_postman.py
+-rw-r--r--   0        0        0      184 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_python.py
+-rw-r--r--   0        0        0      750 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py
+-rw-r--r--   0        0        0      747 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py
+-rw-r--r--   0        0        0     1564 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_robots.py
+-rw-r--r--   0        0        0      537 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py
+-rw-r--r--   0        0        0      758 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py
+-rw-r--r--   0        0        0      713 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py
+-rw-r--r--   0        0        0     6220 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_sitedossier.py
+-rw-r--r--   0        0        0     2321 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py
+-rw-r--r--   0        0        0      415 2024-06-03 14:07:11.928955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_slack.py
+-rw-r--r--   0        0        0     2430 2024-06-03 14:07:11.932955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py
+-rw-r--r--   0        0        0     1700 2024-06-03 14:07:11.932955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_social.py
+-rw-r--r--   0        0        0     3121 2024-06-03 14:07:11.932955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py
+-rw-r--r--   0        0        0     1866 2024-06-03 14:07:11.932955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_splunk.py
+-rw-r--r--   0        0        0      706 2024-06-03 14:07:11.932955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_sslcert.py
+-rw-r--r--   0        0        0      610 2024-06-03 14:07:11.932955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_subdomaincenter.py
+-rw-r--r--   0        0        0     1116 2024-06-03 14:07:11.932955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_subdomains.py
+-rw-r--r--   0        0        0      611 2024-06-03 14:07:11.932955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py
+-rw-r--r--   0        0        0     1222 2024-06-03 14:07:11.932955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_teams.py
+-rw-r--r--   0        0        0     7751 2024-06-03 14:07:11.932955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py
+-rw-r--r--   0        0        0      489 2024-06-03 14:07:11.932955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_threatminer.py
+-rw-r--r--   0        0        0    62527 2024-06-03 14:07:11.932955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_trufflehog.py
+-rw-r--r--   0        0        0     1144 2024-06-03 14:07:11.932955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py
+-rw-r--r--   0        0        0     2902 2024-06-03 14:07:11.932955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py
+-rw-r--r--   0        0        0     2874 2024-06-03 14:07:11.932955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py
+-rw-r--r--   0        0        0     8726 2024-06-03 14:07:11.932955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py
+-rw-r--r--   0        0        0     3401 2024-06-03 14:07:11.932955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py
+-rw-r--r--   0        0        0     1304 2024-06-03 14:07:11.932955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py
+-rw-r--r--   0        0        0      936 2024-06-03 14:07:11.932955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py
+-rw-r--r--   0        0        0      548 2024-06-03 14:07:11.932955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py
+-rw-r--r--   0        0        0     2026 2024-06-03 14:07:11.932955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py
+-rw-r--r--   0        0        0     1009 2024-06-03 14:07:11.932955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py
+-rw-r--r--   0        0        0     1979 2024-06-03 14:07:11.932955 bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py
+-rw-r--r--   0        0        0     1103 2024-06-03 14:07:11.932955 bbot-1.1.9.3387rc0/bbot/test/testsslcert.pem
+-rw-r--r--   0        0        0     1704 2024-06-03 14:07:11.932955 bbot-1.1.9.3387rc0/bbot/test/testsslkey.pem
+-rw-r--r--   0        0        0      476 2024-06-03 14:07:11.932955 bbot-1.1.9.3387rc0/bbot/wordlists/devops_mutations.txt
+-rw-r--r--   0        0        0   959424 2024-06-03 14:07:11.936955 bbot-1.1.9.3387rc0/bbot/wordlists/ffuf_shortname_candidates.txt
+-rw-r--r--   0        0        0      764 2024-06-03 14:07:11.936955 bbot-1.1.9.3387rc0/bbot/wordlists/ms_on_prem_subdomains.txt
+-rw-r--r--   0        0        0    32226 2024-06-03 14:07:11.936955 bbot-1.1.9.3387rc0/bbot/wordlists/nameservers.txt
+-rw-r--r--   0        0        0    17458 2024-06-03 14:07:11.936955 bbot-1.1.9.3387rc0/bbot/wordlists/paramminer_headers.txt
+-rw-r--r--   0        0        0    54887 2024-06-03 14:07:11.936955 bbot-1.1.9.3387rc0/bbot/wordlists/paramminer_parameters.txt
+-rw-r--r--   0        0        0     6068 2024-06-03 14:07:11.936955 bbot-1.1.9.3387rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt
+-rw-r--r--   0        0        0   570241 2024-06-03 14:07:11.940955 bbot-1.1.9.3387rc0/bbot/wordlists/wordninja_dns.txt.gz
+-rw-r--r--   0        0        0     2663 2024-06-03 14:07:30.257282 bbot-1.1.9.3387rc0/pyproject.toml
+-rw-r--r--   0        0        0    42361 1970-01-01 00:00:00.000000 bbot-1.1.9.3387rc0/PKG-INFO
```

### Comparing `bbot-1.1.9.3376rc0/LICENSE` & `bbot-1.1.9.3387rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/README.md` & `bbot-1.1.9.3387rc0/README.md`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/agent/agent.py` & `bbot-1.1.9.3387rc0/bbot/agent/agent.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/cli.py` & `bbot-1.1.9.3387rc0/bbot/cli.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/core/configurator/__init__.py` & `bbot-1.1.9.3387rc0/bbot/core/configurator/__init__.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/core/configurator/args.py` & `bbot-1.1.9.3387rc0/bbot/core/configurator/args.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/core/configurator/environ.py` & `bbot-1.1.9.3387rc0/bbot/core/configurator/environ.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/core/configurator/files.py` & `bbot-1.1.9.3387rc0/bbot/core/configurator/files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/core/errors.py` & `bbot-1.1.9.3387rc0/bbot/core/errors.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/core/event/base.py` & `bbot-1.1.9.3387rc0/bbot/core/event/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/core/event/helpers.py` & `bbot-1.1.9.3387rc0/bbot/core/event/helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/core/flags.py` & `bbot-1.1.9.3387rc0/bbot/core/flags.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/core/helpers/async_helpers.py` & `bbot-1.1.9.3387rc0/bbot/core/helpers/async_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/core/helpers/cache.py` & `bbot-1.1.9.3387rc0/bbot/core/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/core/helpers/cloud.py` & `bbot-1.1.9.3387rc0/bbot/core/helpers/cloud.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/core/helpers/command.py` & `bbot-1.1.9.3387rc0/bbot/core/helpers/command.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/core/helpers/depsinstaller/installer.py` & `bbot-1.1.9.3387rc0/bbot/core/helpers/depsinstaller/installer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/core/helpers/diff.py` & `bbot-1.1.9.3387rc0/bbot/core/helpers/diff.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/core/helpers/dns.py` & `bbot-1.1.9.3387rc0/bbot/core/helpers/dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/core/helpers/files.py` & `bbot-1.1.9.3387rc0/bbot/core/helpers/files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/core/helpers/helper.py` & `bbot-1.1.9.3387rc0/bbot/core/helpers/helper.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/core/helpers/interactsh.py` & `bbot-1.1.9.3387rc0/bbot/core/helpers/interactsh.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/core/helpers/logger.py` & `bbot-1.1.9.3387rc0/bbot/core/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/core/helpers/misc.py` & `bbot-1.1.9.3387rc0/bbot/core/helpers/misc.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/core/helpers/modules.py` & `bbot-1.1.9.3387rc0/bbot/core/helpers/modules.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/core/helpers/names_generator.py` & `bbot-1.1.9.3387rc0/bbot/core/helpers/names_generator.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/core/helpers/ntlm.py` & `bbot-1.1.9.3387rc0/bbot/core/helpers/ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/core/helpers/ratelimiter.py` & `bbot-1.1.9.3387rc0/bbot/core/helpers/ratelimiter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/core/helpers/regexes.py` & `bbot-1.1.9.3387rc0/bbot/core/helpers/regexes.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/core/helpers/url.py` & `bbot-1.1.9.3387rc0/bbot/core/helpers/url.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/core/helpers/validators.py` & `bbot-1.1.9.3387rc0/bbot/core/helpers/validators.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/core/helpers/web.py` & `bbot-1.1.9.3387rc0/bbot/core/helpers/web.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/core/helpers/wordcloud.py` & `bbot-1.1.9.3387rc0/bbot/core/helpers/wordcloud.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/core/logger/logger.py` & `bbot-1.1.9.3387rc0/bbot/core/logger/logger.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/defaults.yml` & `bbot-1.1.9.3387rc0/bbot/defaults.yml`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/ajaxpro.py` & `bbot-1.1.9.3387rc0/bbot/modules/ajaxpro.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/anubisdb.py` & `bbot-1.1.9.3387rc0/bbot/modules/anubisdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/azure_realm.py` & `bbot-1.1.9.3387rc0/bbot/modules/azure_realm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/azure_tenant.py` & `bbot-1.1.9.3387rc0/bbot/modules/azure_tenant.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/baddns.py` & `bbot-1.1.9.3387rc0/bbot/modules/baddns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/baddns_zone.py` & `bbot-1.1.9.3387rc0/bbot/modules/baddns_zone.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/badsecrets.py` & `bbot-1.1.9.3387rc0/bbot/modules/badsecrets.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/base.py` & `bbot-1.1.9.3387rc0/bbot/modules/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/bevigil.py` & `bbot-1.1.9.3387rc0/bbot/modules/bevigil.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/binaryedge.py` & `bbot-1.1.9.3387rc0/bbot/modules/binaryedge.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/bucket_amazon.py` & `bbot-1.1.9.3387rc0/bbot/modules/bucket_amazon.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/bucket_azure.py` & `bbot-1.1.9.3387rc0/bbot/modules/bucket_azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/bucket_digitalocean.py` & `bbot-1.1.9.3387rc0/bbot/modules/bucket_digitalocean.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/bucket_file_enum.py` & `bbot-1.1.9.3387rc0/bbot/modules/bucket_file_enum.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from bbot.modules.base import BaseModule
 import xml.etree.ElementTree as ET
 
 
 class bucket_file_enum(BaseModule):
     """
-    Enumerate files in a public bucket
+    Enumerate files in public storage buckets
+
+    Currently only supports AWS and DigitalOcean
     """
 
     watched_events = ["STORAGE_BUCKET"]
     produced_events = ["URL_UNVERIFIED"]
     meta = {
-        "description": "Works in conjunction with the filedownload module to download files from open storage buckets. Currently supported cloud providers: AWS",
+        "description": "Works in conjunction with the filedownload module to download files from open storage buckets. Currently supported cloud providers: AWS, DigitalOcean",
         "created_date": "2023-11-14",
         "author": "@TheTechromancer",
     }
     flags = ["passive", "safe", "cloud-enum"]
     options = {
         "file_limit": 50,
     }
```

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/bucket_firebase.py` & `bbot-1.1.9.3387rc0/bbot/modules/bucket_firebase.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/bucket_google.py` & `bbot-1.1.9.3387rc0/bbot/modules/bucket_google.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/builtwith.py` & `bbot-1.1.9.3387rc0/bbot/modules/builtwith.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/bypass403.py` & `bbot-1.1.9.3387rc0/bbot/modules/bypass403.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/c99.py` & `bbot-1.1.9.3387rc0/bbot/modules/c99.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/censys.py` & `bbot-1.1.9.3387rc0/bbot/modules/censys.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/certspotter.py` & `bbot-1.1.9.3387rc0/bbot/modules/certspotter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/chaos.py` & `bbot-1.1.9.3387rc0/bbot/modules/chaos.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/code_repository.py` & `bbot-1.1.9.3387rc0/bbot/modules/code_repository.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/columbus.py` & `bbot-1.1.9.3387rc0/bbot/modules/columbus.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/credshed.py` & `bbot-1.1.9.3387rc0/bbot/modules/credshed.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/crt.py` & `bbot-1.1.9.3387rc0/bbot/modules/crt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/deadly/dastardly.py` & `bbot-1.1.9.3387rc0/bbot/modules/deadly/dastardly.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/deadly/ffuf.py` & `bbot-1.1.9.3387rc0/bbot/modules/deadly/ffuf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/deadly/nuclei.py` & `bbot-1.1.9.3387rc0/bbot/modules/deadly/nuclei.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/deadly/vhost.py` & `bbot-1.1.9.3387rc0/bbot/modules/deadly/vhost.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/dehashed.py` & `bbot-1.1.9.3387rc0/bbot/modules/dehashed.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/digitorus.py` & `bbot-1.1.9.3387rc0/bbot/modules/digitorus.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/dnscommonsrv.py` & `bbot-1.1.9.3387rc0/bbot/modules/dnscommonsrv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/dnsdumpster.py` & `bbot-1.1.9.3387rc0/bbot/modules/dnsdumpster.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/docker_pull.py` & `bbot-1.1.9.3387rc0/bbot/modules/docker_pull.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/dockerhub.py` & `bbot-1.1.9.3387rc0/bbot/modules/dockerhub.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/dotnetnuke.py` & `bbot-1.1.9.3387rc0/bbot/modules/dotnetnuke.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/emailformat.py` & `bbot-1.1.9.3387rc0/bbot/modules/emailformat.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/ffuf_shortnames.py` & `bbot-1.1.9.3387rc0/bbot/modules/ffuf_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/filedownload.py` & `bbot-1.1.9.3387rc0/bbot/modules/filedownload.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Watch for common filetypes and download them.
 
     Capable of identifying interesting files even if the extension is not in the URL.
     E.g. if a PDF is being served at https://evilcorp.com/mypdf, it will still be downloaded and given the proper extension.
     """
 
     watched_events = ["URL_UNVERIFIED", "HTTP_RESPONSE"]
-    produced_events = []
+    produced_events = ["FILESYSTEM"]
     flags = ["active", "safe", "web-basic", "web-thorough"]
     meta = {
         "description": "Download common filetypes such as PDF, DOCX, PPTX, etc.",
         "created_date": "2023-10-11",
         "author": "@TheTechromancer",
     }
     options = {
@@ -101,15 +101,15 @@
         return True
 
     async def filter_event(self, event):
         # accept file download requests from other modules
         if "filedownload" in event.tags:
             return True
         else:
-            if event.scope_distance > 1:
+            if event.scope_distance > 0:
                 return False, f"{event} not within scope distance"
             elif self.hash_event(event) in self.urls_downloaded:
                 return False, f"Already processed {event}"
         return True
 
     def hash_event(self, event):
         if event.type == "HTTP_RESPONSE":
@@ -118,30 +118,36 @@
 
     async def handle_event(self, event):
         if event.type == "URL_UNVERIFIED":
             url_lower = event.data.lower()
             extension_matches = any(url_lower.endswith(f".{e}") for e in self.extensions)
             filedownload_requested = "filedownload" in event.tags
             if extension_matches or filedownload_requested:
-                await self.download_file(event.data)
+                await self.download_file(event.data, source_event=event)
         elif event.type == "HTTP_RESPONSE":
             headers = event.data.get("header", {})
             content_type = headers.get("content_type", "")
             if content_type:
                 url = event.data["url"]
-                await self.download_file(url, content_type=content_type)
+                await self.download_file(url, content_type=content_type, source_event=event)
 
-    async def download_file(self, url, content_type=None):
+    async def download_file(self, url, content_type=None, source_event=None):
         orig_filename, file_destination, base_url = self.make_filename(url, content_type=content_type)
         if orig_filename is None:
             return
         result = await self.helpers.download(url, warn=False, filename=file_destination, max_size=self.max_filesize)
         if result:
             self.info(f'Found "{orig_filename}" at "{base_url}", downloaded to {file_destination}')
             self.files_downloaded += 1
+            if source_event:
+                file_event = self.make_event(
+                    {"path": str(file_destination)}, "FILESYSTEM", tags=["filedownload", "file"], source=source_event
+                )
+                file_event.scope_distance = source_event.scope_distance
+                await self.emit_event(file_event)
         self.urls_downloaded.add(hash(url))
 
     def make_filename(self, url, content_type=None):
         # first, try to determine original filename
         parsed_url = self.helpers.urlparse(url)
         base_url = f"{parsed_url.scheme}://{parsed_url.netloc}"
         url_path = parsed_url.path.strip("/")
```

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/fingerprintx.py` & `bbot-1.1.9.3387rc0/bbot/modules/fingerprintx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/fullhunt.py` & `bbot-1.1.9.3387rc0/bbot/modules/fullhunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/generic_ssrf.py` & `bbot-1.1.9.3387rc0/bbot/modules/generic_ssrf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/git.py` & `bbot-1.1.9.3387rc0/bbot/modules/git.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/git_clone.py` & `bbot-1.1.9.3387rc0/bbot/modules/git_clone.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/github_codesearch.py` & `bbot-1.1.9.3387rc0/bbot/modules/github_codesearch.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/github_org.py` & `bbot-1.1.9.3387rc0/bbot/modules/github_org.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/github_workflows.py` & `bbot-1.1.9.3387rc0/bbot/modules/github_workflows.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/gitlab.py` & `bbot-1.1.9.3387rc0/bbot/modules/gitlab.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/gowitness.py` & `bbot-1.1.9.3387rc0/bbot/modules/gowitness.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/hackertarget.py` & `bbot-1.1.9.3387rc0/bbot/modules/hackertarget.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/host_header.py` & `bbot-1.1.9.3387rc0/bbot/modules/host_header.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/httpx.py` & `bbot-1.1.9.3387rc0/bbot/modules/httpx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/hunt.py` & `bbot-1.1.9.3387rc0/bbot/modules/hunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/hunterio.py` & `bbot-1.1.9.3387rc0/bbot/modules/hunterio.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/iis_shortnames.py` & `bbot-1.1.9.3387rc0/bbot/modules/iis_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/internal/base.py` & `bbot-1.1.9.3387rc0/bbot/modules/internal/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/internal/excavate.py` & `bbot-1.1.9.3387rc0/bbot/modules/internal/excavate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/internal/speculate.py` & `bbot-1.1.9.3387rc0/bbot/modules/internal/speculate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/internetdb.py` & `bbot-1.1.9.3387rc0/bbot/modules/internetdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/ip2location.py` & `bbot-1.1.9.3387rc0/bbot/modules/ip2location.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/ipneighbor.py` & `bbot-1.1.9.3387rc0/bbot/modules/ipneighbor.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/ipstack.py` & `bbot-1.1.9.3387rc0/bbot/modules/ipstack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/leakix.py` & `bbot-1.1.9.3387rc0/bbot/modules/leakix.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/masscan.py` & `bbot-1.1.9.3387rc0/bbot/modules/masscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/massdns.py` & `bbot-1.1.9.3387rc0/bbot/modules/massdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/myssl.py` & `bbot-1.1.9.3387rc0/bbot/modules/myssl.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/newsletters.py` & `bbot-1.1.9.3387rc0/bbot/modules/newsletters.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/nmap.py` & `bbot-1.1.9.3387rc0/bbot/modules/nmap.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/ntlm.py` & `bbot-1.1.9.3387rc0/bbot/modules/ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/oauth.py` & `bbot-1.1.9.3387rc0/bbot/modules/oauth.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/otx.py` & `bbot-1.1.9.3387rc0/bbot/modules/otx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/output/asset_inventory.py` & `bbot-1.1.9.3387rc0/bbot/modules/output/asset_inventory.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/output/base.py` & `bbot-1.1.9.3387rc0/bbot/modules/output/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/output/csv.py` & `bbot-1.1.9.3387rc0/bbot/modules/output/csv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/output/discord.py` & `bbot-1.1.9.3387rc0/bbot/modules/output/discord.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/output/emails.py` & `bbot-1.1.9.3387rc0/bbot/modules/output/emails.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/output/http.py` & `bbot-1.1.9.3387rc0/bbot/modules/output/http.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/output/human.py` & `bbot-1.1.9.3387rc0/bbot/modules/output/human.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/output/json.py` & `bbot-1.1.9.3387rc0/bbot/modules/output/json.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/output/neo4j.py` & `bbot-1.1.9.3387rc0/bbot/modules/output/neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/output/slack.py` & `bbot-1.1.9.3387rc0/bbot/modules/output/slack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/output/splunk.py` & `bbot-1.1.9.3387rc0/bbot/modules/output/splunk.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/output/subdomains.py` & `bbot-1.1.9.3387rc0/bbot/modules/output/subdomains.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/output/teams.py` & `bbot-1.1.9.3387rc0/bbot/modules/output/teams.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/output/web_report.py` & `bbot-1.1.9.3387rc0/bbot/modules/output/web_report.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/output/websocket.py` & `bbot-1.1.9.3387rc0/bbot/modules/output/websocket.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/paramminer_cookies.py` & `bbot-1.1.9.3387rc0/bbot/modules/paramminer_cookies.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/paramminer_getparams.py` & `bbot-1.1.9.3387rc0/bbot/modules/paramminer_getparams.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/paramminer_headers.py` & `bbot-1.1.9.3387rc0/bbot/modules/paramminer_headers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/passivetotal.py` & `bbot-1.1.9.3387rc0/bbot/modules/passivetotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/pgp.py` & `bbot-1.1.9.3387rc0/bbot/modules/pgp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/postman.py` & `bbot-1.1.9.3387rc0/bbot/modules/postman.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/rapiddns.py` & `bbot-1.1.9.3387rc0/bbot/modules/rapiddns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/report/affiliates.py` & `bbot-1.1.9.3387rc0/bbot/modules/report/affiliates.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/report/asn.py` & `bbot-1.1.9.3387rc0/bbot/modules/report/asn.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/riddler.py` & `bbot-1.1.9.3387rc0/bbot/modules/riddler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/robots.py` & `bbot-1.1.9.3387rc0/bbot/modules/robots.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/secretsdb.py` & `bbot-1.1.9.3387rc0/bbot/modules/secretsdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/securitytrails.py` & `bbot-1.1.9.3387rc0/bbot/modules/securitytrails.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/shodan_dns.py` & `bbot-1.1.9.3387rc0/bbot/modules/shodan_dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/sitedossier.py` & `bbot-1.1.9.3387rc0/bbot/modules/sitedossier.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/skymem.py` & `bbot-1.1.9.3387rc0/bbot/modules/skymem.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/smuggler.py` & `bbot-1.1.9.3387rc0/bbot/modules/smuggler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/social.py` & `bbot-1.1.9.3387rc0/bbot/modules/social.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/sslcert.py` & `bbot-1.1.9.3387rc0/bbot/modules/sslcert.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/subdomaincenter.py` & `bbot-1.1.9.3387rc0/bbot/modules/subdomaincenter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/sublist3r.py` & `bbot-1.1.9.3387rc0/bbot/modules/sublist3r.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/telerik.py` & `bbot-1.1.9.3387rc0/bbot/modules/telerik.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/templates/bucket.py` & `bbot-1.1.9.3387rc0/bbot/modules/templates/bucket.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/templates/github.py` & `bbot-1.1.9.3387rc0/bbot/modules/templates/github.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/templates/portscanner.py` & `bbot-1.1.9.3387rc0/bbot/modules/templates/portscanner.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/templates/shodan.py` & `bbot-1.1.9.3387rc0/bbot/modules/templates/shodan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/templates/subdomain_enum.py` & `bbot-1.1.9.3387rc0/bbot/modules/templates/subdomain_enum.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/templates/webhook.py` & `bbot-1.1.9.3387rc0/bbot/modules/templates/webhook.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/threatminer.py` & `bbot-1.1.9.3387rc0/bbot/modules/threatminer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/trufflehog.py` & `bbot-1.1.9.3387rc0/bbot/modules/trufflehog.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/url_manipulation.py` & `bbot-1.1.9.3387rc0/bbot/modules/url_manipulation.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/urlscan.py` & `bbot-1.1.9.3387rc0/bbot/modules/urlscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/viewdns.py` & `bbot-1.1.9.3387rc0/bbot/modules/viewdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/virustotal.py` & `bbot-1.1.9.3387rc0/bbot/modules/virustotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/wafw00f.py` & `bbot-1.1.9.3387rc0/bbot/modules/wafw00f.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/wappalyzer.py` & `bbot-1.1.9.3387rc0/bbot/modules/wappalyzer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/wayback.py` & `bbot-1.1.9.3387rc0/bbot/modules/wayback.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/modules/zoomeye.py` & `bbot-1.1.9.3387rc0/bbot/modules/zoomeye.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/scanner/dispatcher.py` & `bbot-1.1.9.3387rc0/bbot/scanner/dispatcher.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/scanner/manager.py` & `bbot-1.1.9.3387rc0/bbot/scanner/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -453,25 +453,19 @@
             try:
                 return q.get_nowait()
             except (asyncio.queues.QueueEmpty, AttributeError):
                 continue
         raise asyncio.queues.QueueEmpty()
 
     @property
-    def queued_event_types(self):
-        event_types = {}
+    def num_queued_events(self):
+        total = 0
         for q in self.incoming_queues:
-            for event, _ in q._queue:
-                event_type = getattr(event, "type", None)
-                if event_type is not None:
-                    try:
-                        event_types[event_type] += 1
-                    except KeyError:
-                        event_types[event_type] = 1
-        return event_types
+            total += len(q._queue)
+        return total
 
     def queue_event(self, event, **kwargs):
         if event:
             # nerf event's priority if it's likely not to be in scope
             if event.scope_distance > 0:
                 event_in_scope = self.scan.whitelisted(event) and not self.scan.blacklisted(event)
                 if not event_in_scope:
@@ -555,22 +549,17 @@
                 self.scan.info(f"{self.scan.name}: No events produced yet")
 
             if modules_errored:
                 self.scan.verbose(
                     f'{self.scan.name}: Modules errored: {len(modules_errored):,} ({", ".join([m for m in modules_errored])})'
                 )
 
-            queued_events_by_type = [(k, v) for k, v in self.queued_event_types.items() if v > 0]
-            if queued_events_by_type:
-                queued_events_by_type.sort(key=lambda x: x[-1], reverse=True)
-                queued_events_by_type_str = ", ".join(f"{m}: {t:,}" for m, t in queued_events_by_type)
-                num_queued_events = sum(v for k, v in queued_events_by_type)
-                self.scan.info(
-                    f"{self.scan.name}: {num_queued_events:,} events in queue ({queued_events_by_type_str})"
-                )
+            num_queued_events = self.num_queued_events
+            if num_queued_events:
+                self.scan.info(f"{self.scan.name}: {num_queued_events:,} events in queue")
             else:
                 self.scan.info(f"{self.scan.name}: No events in queue")
 
             if self.scan.log_level <= logging.DEBUG:
                 # status debugging
                 scan_active_status = []
                 scan_active_status.append(f"scan._finished_init: {self.scan._finished_init}")
```

### Comparing `bbot-1.1.9.3376rc0/bbot/scanner/scanner.py` & `bbot-1.1.9.3387rc0/bbot/scanner/scanner.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/scanner/stats.py` & `bbot-1.1.9.3387rc0/bbot/scanner/stats.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/scanner/target.py` & `bbot-1.1.9.3387rc0/bbot/scanner/target.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/scripts/docs.py` & `bbot-1.1.9.3387rc0/bbot/scripts/docs.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/bbot_fixtures.py` & `bbot-1.1.9.3387rc0/bbot/test/bbot_fixtures.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/conftest.py` & `bbot-1.1.9.3387rc0/bbot/test/conftest.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/run_tests.sh` & `bbot-1.1.9.3387rc0/bbot/test/run_tests.sh`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test.conf` & `bbot-1.1.9.3387rc0/bbot/test/test.conf`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_1/test__module__tests.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_1/test__module__tests.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_1/test_agent.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_1/test_agent.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_1/test_cli.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_1/test_cli.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_1/test_cloud_helpers.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_1/test_cloud_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_1/test_command.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_1/test_command.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_1/test_depsinstaller.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_1/test_depsinstaller.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_1/test_dns.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_1/test_dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_1/test_events.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_1/test_events.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_1/test_files.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_1/test_files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_1/test_helpers.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_1/test_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_1/test_manager_deduplication.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_1/test_manager_deduplication.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_1/test_manager_scope_accuracy.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_1/test_manager_scope_accuracy.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_1/test_modules_basic.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_1/test_modules_basic.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_1/test_python_api.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_1/test_python_api.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_1/test_regexes.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_1/test_regexes.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_1/test_scan.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_1/test_scan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_1/test_scope.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_1/test_scope.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_1/test_target.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_1/test_target.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_1/test_web.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_1/test_web.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/base.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_affiliates.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_affiliates.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_ajaxpro.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_ajaxpro.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_asn.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_asn.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_azure_realm.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_azure_realm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_baddns.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_baddns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_baddns_zone.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_baddns_zone.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_bucket_amazon.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_bucket_amazon.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_bucket_file_enum.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_bucket_file_enum.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_bucket_google.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_bucket_google.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_c99.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_c99.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_censys.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_censys.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_chaos.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_chaos.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_code_repository.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_code_repository.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_credshed.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_credshed.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_crt.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_crt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_dastardly.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_dastardly.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_dehashed.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_dehashed.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_digitorus.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_digitorus.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_discord.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_discord.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_docker_pull.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_docker_pull.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_dockerhub.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_dockerhub.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_dotnetnuke.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_dotnetnuke.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_emails.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_emails.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_filedownload.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_filedownload.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from pathlib import Path
 from .base import ModuleTestBase
 
 
 class TestFileDownload(ModuleTestBase):
     targets = ["http://127.0.0.1:8888"]
     modules_overrides = ["filedownload", "httpx", "excavate", "speculate"]
     config_overrides = {"web_spider_distance": 2, "web_spider_depth": 2}
@@ -35,26 +36,27 @@
         )
         module_test.set_expect_requests(
             dict(uri="/test2"),
             dict(response_data="<!DOCTYPE html>", headers={"Content-Type": "text/html"}),
         )
 
     def check(self, module_test, events):
+        filesystem_events = [e for e in events if e.type == "FILESYSTEM"]
         download_dir = module_test.scan.home / "filedownload"
 
         # text file
-        text_files = list(download_dir.glob("*test-file.txt"))
-        assert len(text_files) == 1, f"No text file found at {download_dir}"
-        file = text_files[0]
+        text_file_event = [e for e in filesystem_events if "test-file.txt" in e.data["path"]]
+        assert 1 == len(text_file_event), f"No text file found at {download_dir}"
+        file = Path(text_file_event[0].data["path"])
         assert file.is_file(), f"File not found at {file}"
         assert open(file).read() == "juicy stuff", f"File at {file} does not contain the correct content"
 
         # PDF file (no extension)
-        pdf_files = list(download_dir.glob("*test-pdf.pdf"))
-        assert len(pdf_files) == 1, f"No PDF file found at {download_dir}"
-        file = pdf_files[0]
+        pdf_file_event = [e for e in filesystem_events if "test-pdf.pdf" in e.data["path"]]
+        assert 1 == len(pdf_file_event), f"No PDF file found at {download_dir}"
+        file = Path(pdf_file_event[0].data["path"])
         assert file.is_file(), f"File not found at {file}"
         assert open(file).read() == self.pdf_data, f"File at {file} does not contain the correct content"
 
         # we don't want html files
         html_files = list(download_dir.glob("*.html"))
         assert len(html_files) == 0, "HTML files were erroneously downloaded"
```

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_git.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_git.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_git_clone.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_git_clone.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_github_codesearch.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_github_codesearch.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_github_org.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_github_org.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_github_workflows.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_github_workflows.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_gitlab.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_gitlab.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_http.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_http.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_internetdb.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_internetdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_ip2location.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_ip2location.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_json.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_json.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_newsletters.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_newsletters.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_nmap.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_nmap.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_oauth.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_oauth.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_otx.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_otx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_postman.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_postman.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_robots.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_robots.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_sitedossier.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_sitedossier.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_social.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_social.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_splunk.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_splunk.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_sslcert.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_sslcert.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_subdomaincenter.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_subdomaincenter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_subdomains.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_subdomains.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_teams.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_teams.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_trufflehog.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_trufflehog.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py` & `bbot-1.1.9.3387rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/testsslcert.pem` & `bbot-1.1.9.3387rc0/bbot/test/testsslcert.pem`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/test/testsslkey.pem` & `bbot-1.1.9.3387rc0/bbot/test/testsslkey.pem`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/wordlists/ffuf_shortname_candidates.txt` & `bbot-1.1.9.3387rc0/bbot/wordlists/ffuf_shortname_candidates.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/wordlists/ms_on_prem_subdomains.txt` & `bbot-1.1.9.3387rc0/bbot/wordlists/ms_on_prem_subdomains.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/wordlists/nameservers.txt` & `bbot-1.1.9.3387rc0/bbot/wordlists/nameservers.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/wordlists/paramminer_headers.txt` & `bbot-1.1.9.3387rc0/bbot/wordlists/paramminer_headers.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/wordlists/paramminer_parameters.txt` & `bbot-1.1.9.3387rc0/bbot/wordlists/paramminer_parameters.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt` & `bbot-1.1.9.3387rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/bbot/wordlists/wordninja_dns.txt.gz` & `bbot-1.1.9.3387rc0/bbot/wordlists/wordninja_dns.txt.gz`

 * *Files identical despite different names*

### Comparing `bbot-1.1.9.3376rc0/pyproject.toml` & `bbot-1.1.9.3387rc0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bbot"
-version = "v1.1.9.3376rc"
+version = "v1.1.9.3387rc"
 description = "OSINT automation for hackers."
 authors = [
     "TheTechromancer",
     "Paul Mueller",
 ]
 license = "GPL-3.0"
 readme = "README.md"
```

### Comparing `bbot-1.1.9.3376rc0/PKG-INFO` & `bbot-1.1.9.3387rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbot
-Version: 1.1.9.3376rc0
+Version: 1.1.9.3387rc0
 Summary: OSINT automation for hackers.
 Home-page: https://github.com/blacklanternsecurity/bbot
 License: GPL-3.0
 Keywords: python,cli,automation,osint,neo4j,scanner,python-library,hacking,recursion,pentesting,recon,command-line-tool,bugbounty,subdomains,security-tools,subdomain-scanner,osint-framework,attack-surface,subdomain-enumeration,osint-tool
 Author: TheTechromancer
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

